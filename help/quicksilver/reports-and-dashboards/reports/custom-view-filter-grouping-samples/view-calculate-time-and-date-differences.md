---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：計算時間和日期差異'
description: 您可以計算下列 — EDIT ME之間的差異。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 0%

---

# 查看：計算時間和日期差異

>[!IMPORTANT]
>
>您無法計算Adobe Workfront中相同類型兩個不同物件之間的時間和日期差異。 例如，您無法計算兩個不同專案、工作或問題上兩個日期之間的時間和日期差異。

您可以計算下列項目之間的差異：

* 同一物件上兩個日期欄位之間的時間和日期差異
* 對象上的欄位與父對象上的其他欄位之間的時間和日期差異

>[!TIP]
>
>這些計算會顯示兩個日期之間的天數。 結果以天為單位顯示。 也會考量日期欄位的時間戳記，如果時間戳記不符，則天數之後可能會有小數。 如果任務延遲完成，則天數會顯示為負值。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 計算相同物件上兩個日期欄位之間的時間和日期差異

例如，您可以計算任務的計畫完成日期和實際完成日期之間的差值。

![](assets/view-planned-actual-completion-dates-datediff-column-350x92.png)

1. 轉到任務清單。
1. 從 **檢視** 下拉式功能表，按一下 **新建視圖**.

1. 按一下 **添加列** 並在 **顯示在此列中** 欄位，然後在清單中顯示時選取它。

1. 按一下 **添加列** 並在 **顯示在此列中** 欄位，然後在清單中顯示時加以選取。

1. 按一下 **添加列**，然後按一下 **切換到文本模式**.

1. 將滑鼠指標暫留在文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 移除您在 **文字模式** 框中，並將其替換為以下代碼：

   ```
   displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML
   ```

1. 按一下 **儲存**，然後 **保存視圖**.

## 計算對象上的欄位與父對象上的另一個欄位之間的時間和日期差異

有關對象及其父項的清單，請參閱 [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
例如，您可以計算任務的計畫完成日期與其父任務的計畫完成日期或任務所在項目之間的差值。

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-350x184.png)

1. 轉到任務清單。
1. 從 **檢視** 下拉式功能表，按一下 **新建視圖**.

1. 按一下 **添加列** 並在 **顯示在此列中** 欄位，然後在清單中顯示時加以選取。

1. 按一下 **添加列** 並在 **顯示在此列中** 欄位，然後在清單中顯示時加以選取。

1. 按一下 **添加列**，然後按一下 **切換到文本模式**.

1. 將滑鼠指標暫留在文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 移除您在 **文字模式** 框中，並將其替換為以下代碼之一：

   * 要顯示項目的計畫完成日期與任務的計畫完成日期之間的差異，請執行以下操作：

      ```
      displayname=Project Planned Completion - Task Planned Completion (Days)<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>valueformat=HTML
      ```

   * 要顯示父任務的計畫完成日期與任務的計畫完成日期之間的差異，請執行以下操作：

      ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion (Days)
      ```

1. 按一下 **儲存**，然後 **保存視圖**.
