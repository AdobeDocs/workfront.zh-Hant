---
product-area: reports and dashboards
navigation-topic: data-connect
title: 在Data Connect中使用工作歷史記錄檢視
description: 透過Data Connect，Workfront管理員可以存取「工作歷史記錄」檢視中每個資料重新整理工作的詳細記錄。
author: Jenny
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
source-git-commit: 79e8b2b1dd3b7374173c2a930abdf8a0bca2cda6
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# 在Data Connect中使用工作歷史記錄檢視

在「工作歷史記錄」檢視中，Workfront管理員可存取每個資料重新整理工作的詳細記錄。 這些記錄為工作提供寶貴的insight，讓您的資料保持最新，並協助您建立理想的時間範圍，說明何時執行流程並重新整理業務視覺效果。

![工作記錄檢視](assets/job-history-tab.png)

「工作歷史記錄」檢視資料欄包含下列資訊：

* **OBJECT_NAME**：顯示與工作關聯的物件名稱。
* **SCHEDULED_TIME**：顯示工作的開始時間。
* **COMPLETED_TIME**：顯示工作的完成時間。
* **LATEST_FLAG**：指出工作是否為最近重新整理的一部分。
* **狀態**：顯示工作的狀態。 如需詳細資訊，請參閱本文中的下列章節： [可用的工作狀態](#available-job-statuses)。
* **LAST_UPDATED**：作業的上次更新時間戳記。

>[!NOTE]
>
>「工作歷史記錄」檢視包含排程工作前72小時的詳細資訊。


## 可用的工作狀態

每個Data Connect工作都會指派一個狀態，指出其是否成功、已略過或失敗。

<table>
    <tr>
        <td><b>工作狀態</b></td>
        <td><b>定義</b></td>
    </tr>
    <tr>
        <td>成功</td>
        <td>該作業已成功處理每個可用的更新，並且該記錄型別的所有更新現在都反映在資料湖中。</td>
    </tr>
    <tr>
        <td>已略過</td>
        <td>已略過此工作，因為佇列中沒有任何記錄型別要處理的更新。</td>
    </tr>
    <tr>
        <td>失敗</td>
        <td>工作無法執行。 在這些情況下，佇列中的資料可能未提交至資料湖。 系統會在該記錄型別的下一個排程工作中處理佇列中保留的記錄。 </td>
    </tr>
   </table>


## 有關工作執行和記錄行為的考量事項

Snowflake使用工作排程器最佳化工具，該工具可能會影響工作執行的處理方式以及在「工作歷史記錄」檢視中的記錄方式。 此記錄行為會因是否有資料可處理而有所不同。

例如，如果沒有任何新列可處理指定的物件，則可能會出現下列其中一種結果：

* **工作執行並標示為「已略過」**： Snowflake偵測到沒有要處理的列、執行工作，並在資料表中將其記錄為「已略過」狀態。

* **工作未執行**： Snowflake判定沒有要處理的列、不執行工作，並在資料表中將其記錄為「已略過」狀態。

  >[!NOTE]
  >
  >在第二個未執行工作的案例中，該物件的最新記錄可能會反映與預期排程不相符的時間戳記。

換言之，即使未處理任何資料列，工作仍可視為已執行，且視該特定工作之工作排程器的行為而定，可能會記錄也可能不記錄。