---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 在行事曆報告中使用自訂日期欄位
description: 行事曆報告是一種動態報告，可提供工作的視覺化呈現。 您可以在行事曆報告中將自訂日期欄位用於任務、問題和專案。
author: Lisa
feature: Reports and Dashboards
exl-id: 40cc8628-7641-41ce-b8e5-7f5ed5ad36c7
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 1%

---

# 在行事曆報告中使用自訂日期欄位

A [!UICONTROL 行事曆] 報告是動態報告，提供工作的視覺化呈現。 您可以在行事曆報告中為下列物件使用自訂日期欄位：

* 任務
* 問題
* 專案

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>[！UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>[！UICONTROL Edit]對[！UICONTROL報告]、[！UICONTROL儀表板]和[！UICONTROL行事曆的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>[！UICONTROL Manage]對行事曆報表的存取權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

1. 您必須有自訂日期欄位，而且欄位內的值可在 [!DNL Workfront] 執行個體。 如果您未設定包含自訂日期的自訂表單，請遵循以下前兩個區段中的指示 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 將自訂表單附加至您計畫新增至行事曆的專案、任務或問題，並指定日期。 如需詳細資訊，請參閱 [新增自訂表單至物件](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 設定專案群組

您可以選擇要在行事曆上顯示專案群組的方式。

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 行事曆]**.

1. 選取您要新增一組專案的行事曆。\
   或\
   按一下 **[!UICONTROL +新增行事曆]** 並輸入行事曆名稱。

   >[!NOTE]
   >
   >您必須擁有 [!UICONTROL 編輯] 存取目標 [!UICONTROL 報表]， [!UICONTROL 儀表板]、和 [!UICONTROL 行事曆] 建立行事曆報告的存取層級。

1. 在左側，按一下 **[!UICONTROL 新增至行事曆]**，然後按一下 **[!UICONTROL 新增進階專案]**.

1. 指定下列專案：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL命名此專案群組]</strong></td>
      <td>輸入專案群組的名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL色彩]</strong></td>
      <td>選取專案群組的顏色。 所有專案都會以選取的顏色顯示在行事曆報告中。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL日期欄位]</strong></td>
      <td>選擇 <strong>[！UICONTROL自訂日期]</strong>.<br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL在行事曆上，顯示]</strong></td>
      <td><p>選擇日期的顯示方式：</p>
       <ul>
        <li><strong>[！UICONTROL單一日期]</strong>：行事曆會在單一日期顯示物件。</li>
        <li><strong>[！UICONTROL Duration] （開始至結束）</strong>：行事曆會持續顯示物件。<br><p>附註：如果您選擇 <strong>[！UICONTROL持續時間]</strong>，指定的結束日期必須晚於開始日期，否則行事曆不會顯示專案。</p></li>
       </ul></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader"><strong>[！UICONTROL自訂日期]</strong></td>
      <td><p>輸入附加到您要追蹤之物件的自訂日期名稱。</p><p><strong>注意：</strong> 自訂日期名稱的搜尋限製為50個結果，以避免效能問題。</td>
     </tr>
    </tbody>
   </table>

1. 繼續下一節。

## 將物件加入至專案群組

設定專案顯示方式之後，您需要將要在行事曆上看到的物件加入群組。

1. 在 **[!UICONTROL 您要新增什麼至行事曆？]** 區段，選取

   * **[!UICONTROL 任務]**
   * **[!UICONTROL 專案]**
   * **[!UICONTROL 問題]**

1. 按一下 **[!UICONTROL 新增任務]**， **[!UICONTROL 新增專案]**，或 **[!UICONTROL 新增問題]**，視您新增至行事曆的物件型別而定。\
   ![選取行事曆的物件](assets/field-name.png)

1. 在下拉式功能表中，開始輸入欄位名稱，然後選取要顯示在行事曆上的物件欄位來源(例如， **[!UICONTROL 延遲任務]**)。
1. 設定行事曆分組的條件陳述式。

   ![條件陳述式](assets/condition-statement-calendar.png)

   若要瞭解如何設定條件，請參閱 [篩選和條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. （選擇性）重複步驟1-4，為行事曆群組指定其他物件。
1. 在 **[!UICONTROL 將任務/專案/問題標籤設定為……]** 欄位，選取此行事曆群組中的物件在行事曆中的標示方式。

   >[!NOTE]
   >
   >如果特定物件無法使用預設標籤選項，則會改為顯示物件名稱。 例如，當 [!UICONTROL 父系任務] 標籤已選取，且沒有與物件關聯的父系任務， [!DNL Adobe Workfront] 顯示您在行事曆中檢視的物件名稱。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。
