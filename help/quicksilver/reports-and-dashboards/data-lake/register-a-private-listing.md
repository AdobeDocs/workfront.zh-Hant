---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: 註冊Workfront Data Connect私人清單
description: 註冊Snowflake私人清單，直接與貴組織的Snowflake帳戶共用您的Workfront Data Connect資料。
author: Courtney
feature: Reports and Dashboards
exl-id:
last-update: 2026-09-15T00:00:00.000Z
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ed31fce397f9e99e7049d4f55eaca94f43dfcf5c
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 1%
---
# 註冊Workfront Data Connect私人清單

您可以註冊私人清單，直接與組織的Snowflake帳戶共用您的Workfront Data Connect資料。 此連線方法使用Snowflake的私人清單功能，在不公開資料的情況下在組織之間安全地共用資料，並且跨地區和託管平台運作。

當您想要將Workfront資料與企業資料倉儲中的其他資料結合時，私人清單會很有用。 由於資料位於您自己的Snowflake帳戶中，因此您可以連同其他資料一起查詢。

## 存取權要求

+++ 展開以檢視存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

您還需要具有接受清單和建立資料庫許可權的Snowflake帳戶，以及Workfront Data Connect權益。

## 什麼是私人上市共用

私人清單可讓您存取下列專案：

* Workfront物件超過100個資料檢視。 如需每個檢視的說明，請參閱[Workfront Data Connect資料字典](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md)。
* `*_event`個資料檢視，其中包含傳遞至Data Connect資料管道的每個變更交易。
* 可擴充資料物件的自訂資料值。 如需範例，請參閱[Workfront Data Connect查詢範例](/help/quicksilver/reports-and-dashboards/data-lake/basic-query-examples.md)中的自訂資料查詢範例。

## 與Reader帳戶連線的差異

私人清單與讀取器帳戶連線共用不同的檢視集，而資料到達時程表不同。 請記住下列差異：

* 私人上市僅分享`*_event`檢視。 `*_current`和`*_daily_history`檢視可透過讀取器帳戶使用，但無法透過私人清單使用。 您可以在自己的Snowflake帳戶中建立這些帳戶。 如需詳細資訊，請參閱本文中的[設定目前和每日歷程記錄檢視](#set-up-current-and-daily-history-views)。
* 私人清單可能不包括讀者帳戶提供的每個檢視。 未共用的檢視範例包括Workfront Planning物件、`MONITORING_DATA_REFRESHES`、`BOOKINGS`和`CLASSIFIER`。 此清單並非詳盡無遺。
* Data Connect每4小時會載入變更事件。 由於私人清單需要額外的復寫步驟才能呈現資料，因此預計資料到達所需時間會比透過讀取器帳戶多大約1小時。
* 資料復寫在01:01、05:01、09:01、13:01、17:01和21:01 UTC執行。 資料通常可在每次執行後約10分鐘內取得。
* `MONITORING_DATA_REFRESHES`和`JOB_HISTORY`檢視不會反映資料透過私人清單變為可用的時間。 雖然`JOB_HISTORY`檢視是透過私人清單共用，但建議您透過讀者帳戶讀取檢視，以便更快速地識別失敗的工作。

## 註冊私人清單

若要註冊私人清單，請先收集您的Snowflake帳戶詳細資料，然後將清單新增至Workfront。

### 收集您的Snowflake帳戶詳細資料

Workfront會使用您的Snowflake帳戶詳細資料，將清單鎖定至您的帳戶。 收集下列詳細資訊：

* 帳戶定位器
* 帳戶URL
* 帳戶組織
* 帳戶名稱

這些值均可從Snowflake中的「帳戶詳細資料」強制回應視窗取得。

若要尋找您的帳戶詳細資料，請執行下列步驟：

1. 登入您的Snowflake帳戶時，請按一下左下角的使用者功能表。

1. 在功能表的&#x200B;**帳戶**&#x200B;區段中選取您的帳戶。

1. 按一下帳戶的&#x200B;**檢視帳戶詳細資料**。

1. 記錄以上列出的每個值。

同時決定您要透過存取連結Workfront資料的資料庫名稱。 當您註冊清單時，請輸入此名稱。

### 在Workfront中新增私人清單

您可透過Adobe Workfront介面註冊私人清單。

>[!IMPORTANT]
>
>您只能為每個帳戶儲位建立一個私人清單。

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**設定**。

1. 在左側面板中，按一下&#x200B;**系統** > **資料連線**。

1. 按一下「**Snowflake連線**」標籤。

1. 按一下&#x200B;**新增私人清單**。

1. 使用您收集的帳戶詳細資料填寫表單，包括您偏好的資料庫名稱。

1. 按一下&#x200B;**新增私人清單**。

### 連線至Snowflake中的清單

在您的Snowflake帳戶中，建立與私人清單的連線，以作為外部資料來源。 然後，您可以連同其他資料一起查詢您的Workfront資料。

## 設定目前與每日歷史記錄檢視

讀取器帳戶連線會為每個物件表格提供三個資料檢視：

* **目前** — 資料目前存在於來源應用程式中的低延遲表示。
* **每日歷程記錄** — 代表每天晚上11:59 UTC的資料。
* **事件** — 每個變更交易都會傳遞至Data Connect資料管道。

私人上市只會共用事件檢視。 本節提供SQL，讓您在自己的帳戶中建置「目前」、「每日歷史記錄」和「事件」檢視。

清單中包含的所有事件檢視都具有以下檢視邏輯所需的欄位。 這些範例假設您已在目標Snowflake帳戶中建立您所選擇的新資料庫和結構描述，且這些範例使用`projects_event`檢視。 在每個範例中，將`<listing_db>`和`<listing_schema>`取代為您自己的值。

>[!TIP]
>
>我們建議您使用您用於分析的欄清單來取代`select *`。 如果您使用`select *`，且稍後會將欄新增至清單的事件檢視，則必須重新建立檢視以啟用新欄。

### 目前檢視

物件的「目前」檢視是儲存在「資料連線」中的最後一個變更事件記錄。 如果最後一個記錄處於已刪除狀態，該記錄會從「目前」檢視中省略。 所有事件檢視都有相同的結構。

```sql
create or replace view projects_current copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event
where end_effective_timestamp = '2300-01-01'::timestamp_ntz
 and nvl(deleted, 0) != 1;
```

目前檢視中不需要`deleted`和`end_effective_timestamp`資料行。 檢視會將資料篩選為單一值，如果刪除記錄，則會完全移除記錄。

### 每日歷史記錄檢視

「每日歷史記錄」檢視會識別指定日期的23:59:59處於作用中狀態的變更事件記錄，因此您可以分析記錄狀態在一段時間內的趨勢。 下列範例提供每個行事曆日期結尾的專案記錄狀態。

```sql
create or replace view projects_daily_history copy grants
as
select d.calendardate as
 , p.*
from <listing_db>.<listing_schema>.calendar_dates d
join <listing_db>.<listing_schema>.projects_event p
 on p.begin_effective_timestamp <= d.calendareodtimestamp
and d.calendareodtimestamp < p.end_effective_timestamp
where d.calendareodtimestamp < current_date() - 1
 and nvl(deleted, 0) != 1;
```

### 事件檢視

為保持一致性，建議您從清單資料庫建立事件檢視的復本，並將其置於與目前和每日歷史記錄檢視相同的結構描述中。

```sql
create or replace view projects_event copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event;
```
