---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 在日曆報表中使用計畫日期
description: 日曆報表是動態報表，可提供您作品的視覺表示。 您可以在日曆報表中使用「計畫日期」欄位來處理任務、問題和項目。
author: Lisa
feature: Reports and Dashboards
exl-id: 27bf6f03-2f6b-4556-a715-75c4a21bfbbb
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 2%

---

# 使用 [!UICONTROL 計畫日期] 在日曆報表中

日曆報表是動態報表，可提供您作品的視覺表示。 您可以使用 [!UICONTROL 計畫日期] 日曆報表中的欄位，以了解下列對象：

* 任務
* 問題
* 專案

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>[!UICONTROL編輯]對[!UICONTROL報表]、[!UICONTROL控制面板]和[!UICONTROL日曆]的訪問</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>[!UICONTROL管理]對日曆報表的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 設定項目群組

您可以選擇要在日曆上顯示項目群組的方式。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 日曆]**.

1. 選擇要添加新項目組的日曆。\
   或\
   按一下 **[!UICONTROL +新日曆]** 並輸入日曆名稱。

   >[!NOTE]
   >
   >您必須在存取層級中擁有「編輯」存取權，才能建立日曆報表。

1. 在左側，按一下 **[!UICONTROL 添加到日曆]**，然後按一下 **[!UICONTROL 新增進階項目]**.

1. 指定下列項目：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL為這組項目命名]</strong></td>
      <td>輸入項目群組的名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL顏色]</strong></td>
      <td>選取項目群組的顏色。 所有項目都會以日曆報表上選取的顏色顯示。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL日期欄位]</strong></td>
      <td><p>選擇 <strong>[!UICONTROL計畫日期]</strong>. 如需計畫日期的詳細資訊，請參閱 </p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-start-date.md" class="MCXref xref">項目計劃開始日期概覽</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">任務計畫起始日期概覽</a></li>
        <li><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任務計畫完成日期概覽</a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">設定項目計畫完成日期</a><br></li>
       </ul></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>在行事曆上，顯示</strong></td>
      <td><p>選擇要如何顯示日期：</p>
       <ul>
        <li><strong>[!UICONTROL僅開始日期]</strong>:日曆會在單一日期顯示物件。</li>
        <li><strong>[!UICONTROL僅結束日期]</strong>:日曆會在單一日期顯示物件。</li>
        <li><strong>[!UICONTROL持續時間]（從開始到結束）</strong>:日曆會在數天內顯示物件。</li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL切換到實際日期（若有）]</strong></td>
      <td><p>日曆會自動切換為實際日期（若有）。 <br>選擇 <strong>[!UICONTROL是]</strong> 或 <strong>[!UICONTROL否]</strong> 切換為實際日期（若有）。 如需實際日期的詳細資訊，請參閱</p>
       <ul>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">項目實際起始日期概覽 </a></li>
        <li><a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">項目實際完成日期概覽 </a></li>
       </ul></td>
     </tr>
    </tbody>
   </table>

1. 繼續下一節。

## 向項組添加對象

設定項目顯示方式後，您需要將要在日曆上查看的對象添加到分組中。

1. 在 **[!UICONTROL 要將什麼添加到日曆中？]** 部分，選擇

   * **[!UICONTROL 任務]**
   * **[!UICONTROL 專案]**
   * **[!UICONTROL 問題]**

1. 按一下 **[!UICONTROL 添加任務]**, **[!UICONTROL 新增專案]**，或 **[!UICONTROL 新增問題]**，視您要新增至日曆的物件類型而定。\
   ![為日曆選擇對象](assets/field-name.png)

1. 在下拉式功能表中，開始輸入欄位名稱，然後選取您要在日曆上顯示之物件的欄位來源(例如 **[!UICONTROL 延遲任務]**)。
1. 設定日曆分組的條件語句。

   ![條件陳述式](assets/condition-statement-calendar.png)

   若要了解設定條件，請參閱 [篩選條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. （可選）重複步驟1-4，為日曆分組指定其他對象。
1. 在 **[!UICONTROL 將任務/項目/問題標籤設定為……]** 欄位中，選擇此日曆分組中的對象在日曆中的標籤方式。

   >[!NOTE]
   >
   >如果預設標籤選項不適用於特定對象，則會改為顯示對象名稱。 例如，當 [!UICONTROL 父任務] 標籤已選中，並且沒有與對象關聯的父任務， [!DNL Adobe Workfront] 顯示您在日曆中查看的對象名稱。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。
