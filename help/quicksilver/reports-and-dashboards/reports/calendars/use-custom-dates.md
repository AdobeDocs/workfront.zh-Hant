---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 在行事曆報告中使用自訂日期欄位
description: 行事曆報告是一種動態報告，可提供工作的視覺化呈現。 您可以在行事曆報告中將自訂日期欄位用於任務、問題和專案。
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 1%

---

# 在行事曆報告中使用自訂日期欄位

[!UICONTROL 行事曆]報告是動態報告，提供您工作的視覺化呈現。 您可以在行事曆報告中為下列物件使用自訂日期欄位：

* 任務
* 問題
* 專案

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板和行事曆的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>管理對行事曆報告的存取權</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

1. [!DNL Workfront]執行個體中必須有自訂日期欄位和可用欄位中的值。 如果您沒有設定自訂日期的自訂表單，請依照[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)中的指示操作。
1. 將自訂表單附加至您計畫新增至行事曆的專案、任務或問題，並指定日期。 如需詳細資訊，請參閱[新增自訂表單至物件](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

## 設定專案群組

您可以選擇要在行事曆上顯示專案群組的方式。

{{step1-to-calendars}}

1. 選取您要新增一組專案的行事曆，按一下[更多]功能表，然後按一下&#x200B;**編輯**。
或
按一下&#x200B;**[!UICONTROL +新行事曆]**，輸入專案名稱，然後按一下&#x200B;**[!UICONTROL 新增進階專案]**。

   >[!NOTE]
   >
   >您必須有[!UICONTROL 編輯]存取許可權才能在存取層級中建立[!UICONTROL 報告]、[!UICONTROL 儀表板]和[!UICONTROL 行事曆]。

1. 指定下列專案：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 命名此專案群組]</strong></td>
      <td>輸入專案群組的名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 色彩]</strong></td>
      <td>選取專案群組的顏色。 所有專案都會以選取的顏色顯示在行事曆報告中。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 日期欄位]</strong></td>
      <td>選擇<strong>[!UICONTROL 自訂日期]</strong>。<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 在行事曆上，顯示]</strong></td>
      <td><p>選擇日期的顯示方式：</p>
       <ul>
        <li><strong>[!UICONTROL 單一日期]</strong>：行事曆會在單一日期顯示物件。</li>
        <li><strong>[!UICONTROL Duration] （開始至結束）</strong>：行事曆顯示物件超過天數。<br><p>注意：如果您選擇<strong>[!UICONTROL Duration]</strong>，則指定的結束日期必須晚於開始日期，否則行事曆上不會顯示該專案。</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[!UICONTROL 自訂日期]</strong></td>
      <td><p>輸入附加到您要追蹤之物件的自訂日期名稱。</p><p><strong>注意：</strong>自訂日期名稱的搜尋限製為50個結果，以避免效能問題。</td>
     </tr>
    </tbody>
   </table>

1. 繼續下一節。

### 將物件加入至專案群組

設定專案顯示方式之後，您需要將要在行事曆上看到的物件加入群組。

1. 在&#x200B;**[!UICONTROL 中，您想要新增什麼至行事曆？]**&#x200B;節，選取

   * **[!UICONTROL 任務]**
   * **[!UICONTROL 專案]**
   * **[!UICONTROL 問題]**

1. 根據您新增至行事曆的物件型別，按一下&#x200B;**[!UICONTROL 新增任務]**、**[!UICONTROL 新增專案]**、**[!UICONTROL 新增問題]**&#x200B;或&#x200B;**休假**。

1. 在下拉式功能表中，開始輸入欄位名稱，然後選取要顯示在行事曆上的物件欄位來源（例如，**[!UICONTROL 延遲工作]**）。
1. 設定行事曆分組的條件陳述式。


   若要瞭解如何設定條件，請參閱[篩選和條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   ![選取行事曆](assets/calendar-field-name.png)的物件

1. （選擇性）重複步驟1-4，為行事曆群組指定其他物件。
1. 在&#x200B;**[!UICONTROL 將任務/專案/問題標籤設定為……]**&#x200B;欄位中，選取此行事曆群組中的物件在行事曆中的標示方式。

   >[!NOTE]
   >
   >如果特定物件無法使用預設標籤選項，則會改為顯示物件名稱。 例如，選取[!UICONTROL 父系任務]標籤且沒有與物件相關聯的父系任務時，[!DNL Adobe Workfront]會顯示您在行事曆中檢視的物件名稱。

   ![設定任務標籤](assets/set-task-labels.png)
1. 按一下「**[!UICONTROL 儲存]**」。

