---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: 篩選事件訂閱訊息
description: 篩選事件訂閱訊息
author: John
feature: Workfront API
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# 篩選事件訂閱訊息

您可以建立中介處理元件，協助您只篩選及處理您的業務所需的事件訂閱訊息。

若要了解事件訂閱，請參閱 [事件訂閱API](../../wf-api/general/event-subs-api.md).

## 篩選事件訊息

本節包含篩選的程式碼片段，您可以實作這些片段，以減少事件訂閱訊息的負載。  為了幫助顯示各種語言語法的差異，這些片段說明了以下列語言編寫的一組相同的篩選器：

您可以在 [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples)，您可以在其中查看每種語言的語法差異，以及與AWS SDK互動的方式。這些範例撰寫為AWS Lambdas，這是採用中繼篩選及處理元件的常見方法。

下列程式碼片段幾乎可用於部署，可作為您編寫自己、更複雜的篩選器和處理元件的起點。

### Java

下列Java範例說明如何根據專案的群組ID來篩選專案裝載，如 [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. 建立您要尋找的群組ID，並將其建立為靜態常數。

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   在此示例中，handleRequest方法(一種AWS Lambda標準方法名稱)將映射類型作為其第一個參數，即事件訂閱消息內容。\
   它所採用的第二個參數是當前Lambda代理請求的上下文。\
   Context對象用於獲取Lambda記錄器，該記錄器用於向CloudWatchLogs寫入消息。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. 調用handleRequest方法時，獲取事件訂閱消息的「newState」屬性，該屬性表示資源的更新狀態。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   若要了解newState格式，請參閱 [事件訂閱的傳出訊息格式](../../wf-api/api/message-format-event-subs.md).

3. 從訊息剖析「newState」對應後，請確定物件的群組ID符合您在步驟1中識別的群組ID。

4. （視條件而定）若 **不** 相符，請放置訊息以傳回空回應。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);    
    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
      }
    return "";
   }
   ```

   >[!NOTE]
   >
   >傳回空的成功回應至關重要。 除200層級回應以外的任何項目，都視為傳送失敗。

5. 處理訊息。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");
   
        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
      }
    ... 
   }
   ```

   AWS SDK可用來叫用另一個Lambda，其負責將篩選後的訊息傳送至所需的端點。

   傳遞消息到另一個Lambda的責任的目的是避免來自事件訂閱服務的傳送請求超時。 目前，允許的傳送逾時設為5秒。 如果篩選器所花費的時間超過設定允許的時間，您可以處理請求，但事件訂閱服務會逾時並陷入重試回圈，直到在逾時期間內收到200層級的回應為止。

   若要進一步了解管理訊息傳送，請參閱 [改善訊息傳送，同時容納逾時](#improving-message-delivery-while-accommodating-timeouts).

### Python

Java和Python示例之間的主要區別是，在Java示例中，事件訂閱消息作為第一個參數被接收，在Python示例中，第一個參數是Lambda代理「event」，它包含事件訂閱消息以及有關AWS Lambda代理請求的資訊。

以下Python示例說明如何根據項目的組ID篩選項目負載，如下所示：  [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. 建立您要尋找的群組ID，並將其建立為靜態常數。

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   第一個參數是Lambda代理「事件」，它包含事件訂閱消息和需要分析的一些附加資訊。\
   第二個參數是當前Lambda代理請求的上下文。\
   在此示例中，上下文對象用於獲取Lambda記錄器，該記錄器用於向CloudWatchLogs寫入消息。

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. 從事件中剖析訊息。

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. 取得事件訂閱訊息的「newState」屬性。\
   newState屬性表示資源的更新狀態。

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   若要了解newState格式，請參閱 [事件訂閱的傳出訊息格式](../../wf-api/api/message-format-event-subs.md).

1. 從訊息剖析「newState」對應後，請確定物件的群組ID符合您在步驟1中識別的群組ID。

1. （條件性）如果ID不相符，請放置訊息以傳回空回應。

   ```
   if new_state['groupID'] == DESIRED_GROUP_ID:
      # Process the message
      print('matched group ID')
      process_message(event_subscription_message)
   
   return {
   'statusCode': 200
   ```

   >[!NOTE]
   >
   >傳回空的成功回應至關重要。 除200層級回應以外的任何項目，都視為傳送失敗。

1. 處理訊息。

   ```
   def process_message(event_subscription_message):
      aws_lambda.invoke(
         FunctionName='forwardMessageOntoMyEndpoint',
         InvocationType='Event',
         LogType='None',
         Payload=event_subscription_message
      )
   ```

   AWS SDK可用來叫用另一個Lambda，其負責將篩選後的訊息傳送至所需的端點。

   傳遞消息到另一個Lambda的責任的目的是避免來自事件訂閱服務的傳送請求超時。 目前，傳送的逾時已設為5秒。 如果篩選器所花費的時間超過設定允許的時間，您可以處理請求，但事件訂閱服務會逾時並陷入重試回圈，直到在逾時期間內收到200層級的回應為止。


### Node.js

專案群組ID篩選的Node.js範例讀取方式與Java和Python範例類似。 與Python示例一樣，第一個參數是Lambda代理事件，第二個參數是Lambda上下文。

下列Node.js範例說明如何根據專案的群組ID來篩選專案裝載，如  [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. 建立您要尋找的群組ID，並將其建立為靜態常數。

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   第一個參數是Lambda代理「事件」，它包含事件訂閱消息和需要分析的一些附加資訊。\
   第二個參數是當前Lambda代理請求的上下文。\
   在此示例中，上下文對象用於獲取Lambda記錄器，該記錄器用於向CloudWatchLogs寫入消息。

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. 從事件中剖析訊息。

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. 從事件訂閱訊息的「newState」屬性取得projectGroupID，然後與您在步驟1中識別之群組的群組ID比對。

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   若要了解newState格式，請參閱 [事件訂閱的傳出訊息格式](../../wf-api/api/message-format-event-subs.md).

4. （條件性）如果ID不相符，請放置訊息以傳回空回應。\
   下列範例顯示相符的群組ID:

   ```
   if (projectGroupId === DESIRED_GROUP_ID) {
      // Process the message
      console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
      forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
   } else {
      endLambdaRequest(context);
   }
   ```

   >[!NOTE]
   >
   >傳回空的成功回應至關重要。 除200層級回應以外的任何項目，都視為傳送失敗。

5. 處理訊息。

   ```
   function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
      let lambdaParams = {
         FunctionName: 'forwardMessageOntoMyEndpoint',
         InvocationType: 'Event',
         LogType: 'None',
         Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
      };
   
      lambda.invoke(lambdaParams, function (err, data) {
         if (err) {
            console.error(err, err.stack);
         } else {
            console.log('data = ' + data);
         }
         endLambdaRequest(context);
      });
   }
   ```

   AWS SDK可用來叫用另一個Lambda，其負責將篩選後的訊息傳送至所需的端點。\
   傳遞消息到另一個Lambda的責任的目的是避免來自事件訂閱服務的傳送請求超時。 目前，傳送的逾時已設為5秒。 如果篩選器所花費的時間超過設定允許的時間，您可以處理請求，但事件訂閱服務會逾時並陷入重試回圈，直到在逾時期間內收到200層級的回應為止。\
   若要了解如何管理訊息傳送，請參閱 [改善訊息傳送，同時容納逾時](#improving-message-delivery-while-accommodating-timeouts).

## 改善訊息傳送，同時容納逾時

事件訂閱服務的逾時限制為 **五秒** 適用於所有傳送請求。 如果郵件的傳送超過允許的時間，事件訂閱服務就會開始該郵件的重試週期。

例如，您建立了類似於 [篩選事件訊息](#filtering-event-messages) 並且您包含資料庫查閱，以判斷是否需要該訊息。 資料庫查找以及所需處理和Lambda冷啟動所需的時間可能需要超過五秒，導致事件訂閱服務重試傳遞消息。

您可以將流程中耗時的部分與負責確定報文是否要處理和傳送的邏輯分開，以避免重試。 如此一來，您就可以接受訊息，並傳回200層級的回應給事件訂閱服務，同時以非同步方式繼續在背景處理或篩選訊息(請參閱 [Java](#java) 例如)。


即使您的處理或篩選未超過五秒逾時，將訊息篩選或處理的第一接觸點與用戶端的其他處理或傳送步驟分開，仍然是有利的。 這樣，從事件訂閱服務向目的地的消息的切換對雙方的時間和效能影響最小。

若要進一步了解重試機制，請參閱 [事件訂閱重試次數](../../wf-api/api/event-sub-retries.md).

## 在無雲架構中實作托管篩選器

如果您無法運用雲架構進行事件訂閱篩選，您仍可以在 [篩選事件訊息](#filtering-event-messages) 作為如何實作您自己的托管篩選器或處理元件的藍圖。

### 調整獨立服務的篩選範例

在無雲環境中使用篩選範例之前，請執行下列操作：

* 忽略示例的Lambda特定部分，如Context參數。

* 將範例中其他Lambda的叫用變更為對您托管的其他篩選器或處理元件發出其他非同步HTTP要求。

* 如果引用Python和Node.js示例，請用Java示例中顯示的第一個裝載參數替換第一個事件參數。 請參閱 [Java](#java).

* 使用網頁型API部署篩選器或處理器。

### 防止遺漏事件訂閱訊息

有時，在無雲架構中，負責接收事件訂閱訊息的服務可能無法連線。 在這種情況下，郵件可能超過重試限制並丟失，無法檢索郵件中的資訊。

建議您在服務啟動期間實作查詢，詢問所有可能包含在遺漏訊息中的資源的最新狀態。 如下列範例所示，您可以使用篩選條件來查詢符合該條件的資源，然後處理其目前狀態。

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v9.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;
    try 
    {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
      } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}
```

透過查詢資源，您可確保整合系統擁有最新版本的資源。

### 在傳送訊息時實作非同步處理

中的所有範例 [篩選事件訊息](#filtering-event-messages) 小節將過濾的消息傳送到另一個AWS Lambda的責任。 這麼做是為了避免超過傳送請求中的五秒逾時，而傳送請求是由發出請求的事件訂閱服務強制執行。

在無雲架構中，您可能需要實作非同步處理機制，類似於AWS SDK允許非同步呼叫其他AWS Lambdas的方式。 大部分的現代化程式設計語言都有可處理非同步處理的第三方或核心程式庫，可讓您運用範例中實作的非同步處理樣式。
