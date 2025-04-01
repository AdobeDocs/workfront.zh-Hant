---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目標中編輯目標
description: 您可以從任何時段和任何狀態編輯現有目標。
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

# 在Adobe Workfront目標中編輯目標

<!--Audited for P&P only: 4/2025-->

您可以從任何時段和任何狀態編輯現有目標。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> 
   <p>對於新計畫和授權結構：
  <ul><li>Ultimate計畫 </li></ul>
   </p>
<p>對於目前的計畫與授權結構： 
<ul><li> A Pro或更高版本 </li>
  <li>除了Adobe Workfront授權之外，還有Workfront目標授權。</li></ul></p>
   </td>  
  </tr>
 <tr>
 <tr>
 <td role="rowheader">Adobe Workfront授權*</td>
 <td>
 <p>新授權：投稿人或以上版本</p>
 或
 <p>目前授權：要求或以上</p> <p>如需詳細資訊，請參閱<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權總覽</a>。</p> </td>
 </tr>
 <tr>
 <td role="rowheader">產品*</td>
 <td>
  <p> 新產品需求：Workfront</p>
 <p>或</p>
  <p>目前產品需求：除了Workfront授權之外，您必須購買Adobe Workfront Goals的授權。 </p> <p>如需詳細資訊，請參閱<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">存取層級</td>
 <td> <p>編輯目標的存取權</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">物件許可權</td>
 <td>
  <div>
  <p>檢視目標或更高許可權以檢視它</p>
  <p>管理目標的許可權以編輯它</p>
  <p>如需共用目標的相關資訊，請參閱<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>。 </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「目標」區域。 </p>  
</td>
  </tr>
</tbody>
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 編輯目標的相關考量事項

* 您無法編輯狀態為「已關閉」的目標。
* 您可以從任何時段編輯目標。

  您可以編輯過去目標的下列資訊：

   * 姓名
   * 時段
   * 狀態

     >[!TIP]
     >
     >如果目標為「已關閉」，重新開啟它將會重新計算進度完成百分比。 您無法編輯已關閉的目標。

   * 說明
   * 結果和活動

## 編輯目標

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Edit**.

   ![Edit goal](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

1. 按一下&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**目標**。\
   隨即顯示目標清單。
1. 按一下目標。\
   目標頁面隨即顯示。

   ![目標頁面](assets/goal-page-unshimmed.png)

1. 執行下列任一項作業來編輯目標的資訊：
   * 按一下目標標題中顯示的欄位以進行更新。 並非標題中的所有欄位都可以編輯。
   * 按一下目標名稱右側的&#x200B;**更多圖示** ![更多圖示](assets/more-icon.png)，然後按一下&#x200B;**編輯**。
   * 按一下左側面板中的&#x200B;**目標詳細資料**，然後按一下右上角的&#x200B;**編輯圖示** ![編輯圖示](assets/edit-icon.png)，然後按一下&#x200B;**全部編輯**。 開始更新「目標詳細資料」區段中的欄位。

     >[!IMPORTANT]
     >
     >並非以上區域顯示的所有欄位都可以編輯。 Workfront會計算某些欄位，且這些欄位為唯讀。

1. （視條件而定）根據您在上一步驟中所選取的專案，更新以下有關目標的資訊：

   * 更新目標標題中的下列資訊，然後按Enter儲存變更：
      * **目標名稱**：按一下目標的名稱，然後開始輸入新名稱。
      * **擁有者**：按一下擁有者的名稱，然後開始輸入使用者、團隊、群組或您公司的名稱，然後在清單中顯示時選取該名稱。 一個目標只能有一個擁有者。
   * 在[編輯目標]方塊中更新下列資訊，然後按一下[儲存] ****：
      * **目標名稱**
      * **期間**：按一下以更新目標的期間\
        或\
        選取&#x200B;**啟用自訂日期**&#x200B;以指定目標的&#x200B;**開始**&#x200B;和&#x200B;**結束日期**&#x200B;的日期。

        >[!TIP]
        >
        >取消選取&#x200B;**啟用自訂日期**&#x200B;以返回目標的原始時段。

      * **目標所有者**
      * **描述**：新增或更新目標的相關資訊。
   * 更新或檢閱「目標詳細資料」區段中的資訊。 如需詳細資訊，請參閱Adobe Workfront目標](../goal-management/update-goals-in-goal-details-panel.md)中「目標詳細資料」一節的[更新目標。

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. （選用）按一下左側面板中的&#x200B;**進度指示器**，將結果、活動或專案新增至目標。 新增進度指示器可確保您可以追蹤目標的進度。
如需詳細資訊，請參閱下列文章：
   * [將活動新增至Adobe Workfront目標中的目標](../results-and-activities/add-activities-to-goals.md)
   * [將結果新增至Adobe Workfront目標中的目標](../results-and-activities/add-results-to-goals.md)。
   * [在Adobe Workfront目標中新增專案](../results-and-activities/connect-projects-to-goals-overview.md)。

</div>
