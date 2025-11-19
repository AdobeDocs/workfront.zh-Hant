---
product-area: reports and dashboards
navigation-topic: data-connect
title: 在Data Connect中使用監控資料重新整理檢視
description: 透過Data Connect，Workfront管理員可存取最近重新整理期間對Data Lake日期進行之最近更新的詳細記錄。
author: Jenny
feature: Reports and Dashboards
source-git-commit: 1bcb64fbcdf2cb8b40cb50e5a7d4f5768f3a712f
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 2%

---

# 在Data Connect中使用監控資料重新整理檢視

「監控資料重新整理」檢視會顯示最近重新整理期間對資料湖日期所做的最新更新。 每次成功完成資料載入後，此檢視的資料都會更新。

由於資料量大且彙總複雜，「監督資料重新整理」檢視只會顯示過去2週內更新的物件檢視。 如果此檢視中缺少特定記錄型別，很可能是因為該時間範圍內缺少活動。

>[!NOTE]
>
>此檢視會顯示應用程式和重新整理活動所提供的資料詳細集合，而非顯示重新整理活動歷程記錄的每日歷史記錄或事件檢視。 若要取得歷史重新整理活動詳細資料，您可以利用<code>DL_LOAD_TIMESTAMP</code> 日期物件。

## 監控資料重新整理檢視欄

「監督資料重新整理」檢視資料欄包含下列資訊：

<table>
    <tr>
        <td><b>欄名稱</b></td>
        <td><b>類型</b></td>
        <td><b>說明</b></td>
    </tr>
    <tr>
        <td>物件型別</td>
        <td>Varchar
        </td>
        <td> 
      與傳送至資料湖的Workfront記錄相關聯的物件型別。 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>日期</td>
        <td>
   顯示在OBJ_TYPE欄中的物件型別上次成功重新整理資料的日期。 </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 顯示在OBJ_TYPE欄中的物件型別，其最近一次資料重新整理的日期和時間。  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ </td>
        <td>
       顯示在OBJ_TYPE欄中的物件型別，其最近一次資料重新整理的日期和時間。 </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>數字</td>
        <td>
     物件型別自上次資料重新整理以來經過的時間（分鐘）。 </td>
    </tr>
            <tr>
        <td>已建立 </td>
        <td>數字 </td>
        <td>在物件型別的前次和最新資料重新整理之間擷取的CREATE記錄事件計數。  </td>
    </tr>
                <tr>
        <td>已更新</td>
        <td>數字 </td>
        <td>在物件型別的前次和最新資料重新整理之間擷取的UPDATE記錄事件計數。</td>
    </tr>
                <tr>
        <td>已刪除</td>
        <td>數字 </td>
        <td>在物件型別之前和最新資料重新整理之間擷取的DELETE記錄事件計數。 </td>
    </tr>
                <tr>
        <td>總計</td>
        <td>數字 </td>
        <td>物件型別之前和最近資料重新整理之間的事件總數計數。 
        <br> 
        <br><b>注意</b>：這與受CREATE、UPDATE或DELETE事件影響的記錄總數不同，因為相同的記錄可能會在重新整理的間隔內多次CREATE和UPDATE。  </td>
    </tr>
   </table>

