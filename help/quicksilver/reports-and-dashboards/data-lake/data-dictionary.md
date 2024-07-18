---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: 資料湖資料字典
description: 此頁面包含Workfront Data Lake中資料的結構與內容相關資訊。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 81f8477dd26b828c4255c678b36d98789cd81ff8
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 5%

---

# Workfront data lake資料字典

此頁面包含Workfront Data Lake中資料的結構與內容相關資訊。

>[!NOTE]
>
>Workfront Data Lake中的資料每四小時會重新整理一次，因此最近的變更可能不會立即顯示。

## 表格型別

您可以透過多種表格型別，提供最深入的分析來檢視Workfront資料。

* **目前的資料表**

  「目前」表格所反映的資料與Workfront中的資料、每個物件及其目前狀態類似。 不過，它比Workfront內的延遲要低很多。

* **事件資料表**

  「事件」表格會追蹤Workfront中的每筆變更記錄：亦即，每次物件變更狀態時，系統都會建立記錄以顯示變更發生時間、變更人員及變更內容。 因此，此表格對時間點比較很有用。 此表格僅包含過去三年的記錄。

* **每日記錄表**

  「每日歷史記錄」表格提供「事件」表格的縮寫版本，顯示每個物件的每日狀態，而非每個個別事件發生時的狀態。 因此，此表可用於趨勢分析。

<!-- Custom table -->

## 實體關係圖

Workfront中的物件（以及您資料湖中的物件）不僅是由其個別值所定義，也是由其與其他物件的關係所定義。 下列實體關係圖表提供Workfront資料湖中物件關係的高層級對應。 您可以使用下列連結來檢視和下載圖表：

[Workfront data lake實體關係圖](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>實體關係圖表是進行中的工作，因此僅供參考，且可能會變更。

## 日期型別

有許多日期物件可提供特定事件發生時間的相關資訊。

* `DL_LOAD_TIMESTAMP`：此日期用於內部參考，並反映資料載入目前、事件或每日記錄表格的時間。 此日期不應用於資料分析，且計畫在Workfront資料湖的測試階段期間移除。
* `CALENDAR_DATE`：此日期僅出現在「每日歷史記錄」表格中。 此表格記錄了`CALENDAR_DATE`中指定的每個日期在11:59 UTC時的資料外觀。
* `BEGIN_EFFECTIVE_TIMESTAMP`：此日期同時存在於「事件」和「每日歷史記錄」表格中，且記錄記錄將記錄目前資料列中的值&#x200B;_變更為_&#x200B;的確切時間。
* `END_EFFECTIVE_TIMESTAMP`：此日期同時存在於「事件」和「每日歷史記錄」表格中，而且記錄記錄將目前資料列中的值&#x200B;_從_&#x200B;變更為其他資料列中的值的確切時間。 若要允許在`BEGIN_EFFECTIVE_TIMESTAMP`和`END_EFFECTIVE_TIMESTAMP`上的查詢之間進行，此值絕不為Null，即使沒有新值也是如此。 在記錄仍有效的情況下（亦即值未變更），`END_EFFECTIVE_TIMESTAMP`的值將為2300-01-01。

## 術語表

下表將Workfront中的物件名稱（及其在介面和API中的名稱）與其在資料湖中的對等名稱建立關聯。

<table>
<thead>
  <tr>
    <th>Workfront實體名稱</th>
    <th>介面參考</th>
    <th>API參考 | 標籤</th>
    <th>資料湖表格</th>
    <th>附註</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>指派</td>
    <td>指派</td>
    <td>指派 | 指定任務</td>
    <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>條件、優先順序、嚴重性、狀態</td>
    <td>系統 | 自訂列舉</td>
    <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
    <td>記錄型別是透過'enumClass'屬性識別。 下列是預期的型別：<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
  </tr>
  <tr>
    <td>文件</td>
    <td>文件</td>
    <td>檔案 | 檔案</td>
    <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br><br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>檔案版本</td>
    <td>文件版本</td>
    <td>DOCV | 檔案版本</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>群組</td>
    <td>群組</td>
    <td>群組 | 群組</td>
    <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>小時</td>
    <td>小時</td>
    <td>HOUR | 小時</td>
    <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>時數類型</td>
    <td>時數類型</td>
    <td>小時 | 小時型別</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>里程碑</td>
    <td>里程碑</td>
    <td>英里 | 里程碑</td>
    <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>里程碑路徑</td>
    <td>里程碑路徑</td>
    <td>MPATH | 里程碑路徑</td>
    <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>備註</td>
    <td>備註</td>
    <td>注意 | 注意</td>
    <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>Op 任務</td>
    <td>問題，請求</td>
    <td>OPTASK | 問題</td>
    <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br><br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>專案組合</td>
    <td>專案組合</td>
    <td>連線埠 | Portfolio</td>
    <td>Portfolio_CURRENT<br>PORTFOLIO_每日_歷史記錄<br>PORTFOLIO_事件<br><br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIO_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>方案</td>
    <td>方案</td>
    <td>PRGM | 計畫</td>
    <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br><br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>專案</td>
    <td>專案</td>
    <td>專案 | 專案</td>
    <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br><br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>角色</td>
    <td>職務角色</td>
    <td>角色 | 工作角色</td>
    <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>排程</td>
    <td>排程</td>
    <td>時程 | 排程</td>
    <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>任務</td>
    <td>任務</td>
    <td>任務 | 任務</td>
    <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br><br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>團隊</td>
    <td>團隊</td>
    <td>TEAMOB | 團隊</td>
    <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>時程表</td>
    <td>時程表</td>
    <td>表格 | 時間表</td>
    <td>時程表_目前<br>時程表_每日歷史記錄<br>時程表_事件</td>
    <td></td>
  </tr>
  <tr>
    <td>使用者</td>
    <td>使用者</td>
    <td>使用者 | 使用者</td>
    <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br><br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
