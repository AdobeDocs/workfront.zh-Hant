---
title: 建立或自訂問題嚴重程度
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 您的使用者可使用嚴重程度來定義問題的嚴重程度。 您可以自訂Adobe Workfront中現有的五種預設嚴重程度，或為使用者建立新的嚴重程度。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 5c80dca8a9f7dd5a693db9bf22738602da8b521b
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 4%

---

# 建立或自訂問題嚴重程度

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

您的使用者可使用嚴重程度來定義問題的嚴重程度。 您可以自訂Adobe Workfront中現有的五種預設嚴重程度，或為使用者建立新的嚴重程度。

>[!NOTE]
>
>任務和專案沒有嚴重性。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>系統管理員</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++ 

## 內建問題嚴重程度

Workfront有五個內建問題嚴重性：

* 輕微
* 導致混淆
* 有因應措施的錯誤
* 無因應措施的錯誤
* 致命錯誤

您可以針對這些嚴重程度編輯下列專案：

* 姓名
* 顏色

  如果您依問題嚴重程度將結果分組，嚴重程度的顏色會保留在圖表報告中。 如需圖表報表的資訊，請參閱[新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

* 預設嚴重程度

  如需預設嚴重程度的詳細資訊，請參閱本文中的[建立或編輯問題嚴重程度](#create-or-edit-an-issue-severity)。

* 說明
* Workfront中是否隱藏嚴重程度

  如需隱藏嚴重程度的詳細資訊，請參閱本文中的[建立或編輯問題嚴重程度](#create-or-edit-an-issue-severity)。

* 刪除嚴重程度

  執行此操作時，必須選取替代嚴重程度。

## 建立或編輯問題嚴重程度 {#create-or-edit-an-issue-severity}

身為Workfront管理員，您可以根據使用者的需求建立和編輯問題嚴重程度。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**專案偏好設定** > **嚴重程度**。

1. 如果您正在建立新的嚴重程度，請按一下表格底部的&#x200B;**新增列**。
1. 針對新嚴重性設定下列選項，或編輯現有嚴重性的選項：

   * **嚴重程度名稱**：輸入嚴重程度的名稱。
   * **重要性**：增加或減少嚴重程度的嚴重性等級，最初由Workfront指派。

     每個嚴重程度的重要性數字必須是唯一的。 最高數字對應於嚴重性的最高層級。

     儲存嚴重程度後，就無法編輯此數字。

   * **色彩**：選擇嚴重程度的色彩。

     當您依問題嚴重程度將結果分組時，會在圖表報告中使用嚴重程度的顏色。 如需圖表報表的資訊，請參閱[新增圖表至報表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

   * **預設嚴重程度**：選取您要Workfront自動套用至所有新建立問題的嚴重程度。

     在Workfront中，**輕微**&#x200B;是問題的預設嚴重程度。

     您無法設定隱藏嚴重程度的預設值。

     預設嚴重程度以圖示![預設嚴重程度圖示](assets/default-icon.png)表示。 若要選擇新的預設值，請執行下列任一項作業：

      * 選取嚴重度名稱旁的核取方塊，並在熒幕底部的動作列中選取&#x200B;**設定預設值**。
      * 將滑鼠停留在嚴重度名稱上，然後按一下出現的&#x200B;**更多**&#x200B;功能表。 然後，選取&#x200B;**設定預設值**。

        新的預設嚴重程度會以圖示標示。

   * **描述**：輸入嚴重程度的描述，以說明其功能。
   * **隱藏選擇**：選取&#x200B;**是**&#x200B;以隱藏不再需要的嚴重程度。

     隱藏的嚴重程度不會在Workfront的任何位置顯示，因此使用者無法針對其問題選擇它。

     >[!IMPORTANT]
     >
     >建議您隱藏嚴重性，不要刪除您不想再使用的嚴重性。 如此一來，您就可以保留物件上所有已使用嚴重度完成的歷史資料，同時防止人們日後使用嚴重度。

1. （可選）以您想要的順序拖放嚴重性，以變更其清單順序。

   這會變更問題顯示的順序。 它不會變更&#x200B;**重要性**&#x200B;數字。

1. 按一下「**儲存**」。

如需處理問題時如何使用嚴重程度的詳細資訊，請參閱[更新問題嚴重程度](../../../manage-work/issues/issue-information/update-issue-severity.md)。
