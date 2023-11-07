---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: 篩選事件訂閱訊息
description: 篩選事件訂閱訊息
author: Becky
feature: Workfront API
role: Developer
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# 篩選事件訂閱訊息

您可以建立中介處理元件，協助您僅篩選及處理業務所需的事件訂閱訊息。

若要瞭解事件訂閱，請參閱 [事件訂閱API](../../wf-api/general/event-subs-api.md).

## 篩選事件訊息

本節包含篩選的程式碼片段，您可實施這些程式碼片段來減少事件訂閱訊息的負載。  為了協助顯示各種語言語法的差異，這些片段說明了使用下列語言撰寫的相同篩選器集：

您可以在下列位置檢視篩選範例： [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples)，您可在此檢視每種語言的語法差異，以及與AWS SDK互動的方式。這些範例會撰寫為AWS Lambdas，這是運用中介篩選與處理元件的常見方法。

下列程式碼片段幾近可供部署使用，可當作協助您撰寫自己的更複雜篩選器及處理元件的起點。

### Java

以下Java範例說明如何根據專案的群組ID篩選專案裝載，如中所示 [ProjectGroupFiltering.java：](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. 建立您要尋找的群組ID，並將其建立為靜態常數。

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   在此範例中，handleRequest方法(這是AWS Lambda標準方法名稱)會以Map型別作為其第一個引數（即事件訂閱訊息內容）。\
   第二個引數是目前Lambda Proxy要求的前後關聯。\
   Context物件用於取得Lambda記錄器，後者用於將訊息寫入CloudWatchLogs。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. 叫用handleRequest方法時，取得事件訂閱訊息的「newState」屬性，代表已更新的資源狀態。

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   若要瞭解newState格式，請參閱 [事件訂閱的傳出訊息格式](../../wf-api/api/message-format-event-subs.md).

3. 從訊息中剖析「newState」對應後，請確定物件的群組ID符合您在步驟1中識別的群組ID。

4. （視條件而定）如果ID **不要** 比對，拖放訊息以傳回空白回應。

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
   >傳回空白的成功回應至關重要。 200層級回應以外的任何專案都視為傳送失敗。

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

   AWS SDK可用來叫用另一個Lambda，後者負責將篩選後的訊息傳遞至我們想要的端點。

   將傳遞訊息的責任傳遞給另一個Lambda的目的是避免來自事件訂閱服務的傳遞請求逾時。 目前，傳遞允許的逾時設定為5秒。 如果篩選所需時間超過設定，您可以處理請求，但事件訂閱服務將會逾時，並進入重試回圈，直到在逾時期間內收到200層級的回應為止。

   若要進一步瞭解管理訊息傳送，請參閱 [改善訊息傳送，同時容納逾時](#improving-message-delivery-while-accommodating-timeouts).

### Python

Java和Python範例的主要差異在於，在Java範例中，會收到事件訂閱訊息作為第一個引數，而在Python範例中，第一個引數是Lambda Proxy「event」，其包含事件訂閱訊息以及AWS Lambda Proxy請求的資訊。

以下Python範例說明如何根據專案的群組ID篩選專案裝載，如中所示  [projectGroupFiltering.py：](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. 建立您要尋找的群組ID，並將其建立為靜態常數。

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   第一個引數是Lambda Proxy「事件」，其中包含事件訂閱訊息和一些需要剖析的其他資訊。\
   第二個引數是目前Lambda Proxy要求的前後關聯。\
   在此範例中，Context物件用於取得Lambda記錄器，後者用於將訊息寫入CloudWatchLogs。

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. 從事件剖析訊息。

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. 取得事件訂閱訊息的「newState」屬性。\
   newState屬性代表資源的更新狀態。

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   若要瞭解newState格式，請參閱 [事件訂閱的傳出訊息格式](../../wf-api/api/message-format-event-subs.md).

1. 從訊息中剖析「newState」對應後，請確定物件的群組ID符合您在步驟1中識別的群組ID。

1. （條件式）如果ID不相符，請拖放訊息以傳回空白回應。

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
   >傳回空白的成功回應至關重要。 200層級回應以外的任何專案都視為傳送失敗。

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

   AWS SDK可用來叫用另一個Lambda，後者負責將篩選後的訊息傳遞至我們想要的端點。

   將傳遞訊息的責任傳遞給另一個Lambda的目的是避免來自事件訂閱服務的傳遞請求逾時。 目前，傳送逾時設定為五秒。 如果篩選所需時間超過設定，您可以處理請求，但事件訂閱服務將會逾時，並進入重試回圈，直到在逾時期間內收到200層級的回應為止。


### Node.js

專案群組ID篩選的Node.js範例讀取類似Java和Python範例。 和Python範例一樣，第一個引數是Lambda代理事件，第二個引數是Lambda內容。

以下Node.js範例顯示如何根據專案的群組ID篩選專案裝載，如中所示  [projectGroupFiltering.js：](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. 建立您要尋找的群組ID，並將其建立為靜態常數。

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   第一個引數是Lambda Proxy「事件」，其中包含事件訂閱訊息和一些需要剖析的其他資訊。\
   第二個引數是目前Lambda Proxy要求的前後關聯。\
   在此範例中，Context物件用於取得Lambda記錄器，後者用於將訊息寫入CloudWatchLogs。

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. 從事件剖析訊息。

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. 從事件訂閱訊息的「newState」屬性取得projectGroupID，然後將其與您在步驟1中識別的群組的群組ID配對。

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   若要瞭解newState格式，請參閱 [事件訂閱的傳出訊息格式](../../wf-api/api/message-format-event-subs.md).

4. （條件式）如果ID不相符，請拖放訊息以傳回空白回應。\
   下列範例顯示相符的群組ID：

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
   >傳回空白的成功回應至關重要。 200層級回應以外的任何專案都視為傳送失敗。

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

   AWS SDK可用來叫用另一個Lambda，後者負責將篩選後的訊息傳遞至我們想要的端點。\
   將傳遞訊息的責任傳遞給另一個Lambda的目的是避免來自事件訂閱服務的傳遞請求逾時。 目前，傳送逾時設定為五秒。 如果篩選所需時間超過設定，您可以處理請求，但事件訂閱服務將會逾時，並進入重試回圈，直到在逾時期間內收到200層級的回應為止。\
   若要瞭解如何管理訊息傳送，請參閱 [改善訊息傳送，同時容納逾時](#improving-message-delivery-while-accommodating-timeouts).

## 改善訊息傳送，同時容納逾時

事件訂閱服務的嚴格逾時為 **五秒** 用於所有傳送請求。 如果訊息的傳送超過允許的時間，「事件訂閱」服務會開始該訊息的重試週期。

例如，您建立的專案群組ID篩選器，類似於中的其中一個範例 [篩選事件訊息](#filtering-event-messages) 而且您可以包含資料庫查詢，以判斷是否需要該訊息。 資料庫查詢以及所需處理和Lambda冷啟動所需的時間可能會超過五秒，導致「事件訂閱」服務重新嘗試傳遞訊息。

若要避免重試，可將程式耗時的部分與負責判斷訊息是否是要處理和傳送的邏輯分開。 如此一來，您便可接受訊息，並將200層級的回應傳回至事件訂閱服務，同時以非同步方式繼續在背景處理或篩選訊息（請參閱中的步驟5） [Java](#java) 例如)。


即使您的處理或篩選未超過五秒逾時，將訊息篩選或處理的第一個接觸點與使用者端的其他處理或傳送步驟分開，仍然有好處。 如此一來，從「事件訂閱」服務將訊息移交至目的地對雙方的時間和效能的影響就會降到最低。

若要深入瞭解重試機制，請參閱 [事件訂閱重試次數](../../wf-api/api/event-sub-retries.md).

## 在無雲架構中實作託管篩選器

如果您無法運用雲端架構來篩選事件訂閱專案，您仍可使用下列範例： [篩選事件訊息](#filtering-event-messages) 作為如何實作您自己的託管篩選器或處理元件的藍圖。

### 調整獨立服務的篩選範例

在無雲環境中使用篩選範例之前，請先執行下列動作：

* 省略範例的Lambda特定片段，例如Context引數。

* 變更範例中其他Lambda的引動過程，對您託管的其他篩選器或處理元件提出額外的非同步HTTP請求。

* 若提及Python和Node.js範例，請以Java範例中顯示的第一個裝載引數取代第一個事件引數。 請參閱中的步驟1 [Java](#java).

* 使用網頁式API部署篩選器或處理器。

### 防止遺漏事件訂閱訊息

有時，在無雲架構中，負責接收事件訂閱訊息的服務可能無法連線。 在這種情況下，訊息可能會超過重試限制並遺失，且無法擷取訊息中的資訊。

我們建議您在服務啟動期間，實作查詢，以詢問可能包含在未接訊息中的所有資源的最新狀態。 如下列範例所示，您可以使用篩選條件來查詢符合該條件的資源，然後處理其目前狀態。

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v15.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
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

透過查詢資源，您可以確保您的整合系統擁有最新版本的資源。

### 在傳遞訊息中實作非同步處理

此頁面中的所有範例： [篩選事件訊息](#filtering-event-messages) 區段會將經篩選的訊息傳遞至另一個AWS Lambda。 這麼做可避免傳送請求超過五秒逾時，這是由發出請求的事件訂閱服務所強制執行。

在無雲架構中，您可能需要實作非同步處理機制，類似AWS SDK允許對其他AWS Lambda進行非同步呼叫的方式。 大部分的現代程式設計語言都有處理非同步處理的協力廠商或核心程式庫，可讓您運用範例中實作的非同步處理風格。
