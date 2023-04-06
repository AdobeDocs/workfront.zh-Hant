---
title: 使用表單設計工具組織和預覽表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表單設計器組織自訂表單。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 使用表單設計工具組織和預覽表單

您可以使用表單設計工具組織自訂表單。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>
   <p>當前計畫：標準</p>
   <p>或</p>
   <p>舊計畫：計畫</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>管理對自訂表單的存取</p> <p>如需Workfront管理員如何授予此存取權的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## 新增區段插播

您可以將自訂表單中的自訂欄位和Widget分組為具有標題的區段。 這對於向將填寫表單的使用者呈現有條理的體驗非常有用。 此外，如果您需要限制特定使用者對特定自訂欄位和Widget的存取權，您可以將它們放在區段中，然後僅將區段的存取權授予這些使用者。

例如，如果您需要追蹤只有系統管理員才能檢視或編輯的敏感資訊，您可以使用「僅管理員」權限建立分區符號，並將敏感欄位放在該區段中。

您為區段選取的存取設定會直接系結至使用者在自訂表單附加位置的Workfront物件上的權限。 您可以根據使用者是否有檢視、貢獻或管理該物件的存取權，來隱藏或顯示區段。 或者，您可以將區段設為「僅管理員」，讓只有具有系統管理員存取權限的使用者才能存取。

有關對象權限的資訊，請參見 [對象共用權限概述](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

如需自訂表單中自訂欄位和小工具的相關資訊，請參閱 [設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### 為自訂表單中的區段建立和設定存取權

1. 開始建立或編輯自訂表單和新增欄位，如 [設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 按一下 **區段分隔** 並將其拖曳至畫布上的所需位置。

1. 在右側面板中，設定您要區段的選項：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入要在區段上方顯示的描述性標籤。 您隨時都可以變更標籤。</p> <p><b>重要</b>:請避免在此標籤中使用特殊字元。 報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>如果您想要向使用者說明區段的用途，請輸入文字。 這會顯示在自訂表單上區段的標籤下方。</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>授予存取權</p> </td> 
      <td> <p> 選取使用者對自訂表單附加所在物件所需的權限，以檢視此區段並編輯其欄位值。 
       <p>下列權限可在 <b>具有物件存取權的使用者可檢視欄位值</b>:</p> 
         <ul>  
          <li><p><b>有限編輯</b>:（只有對象是項目、任務、問題或用戶時才可用）:</p> 
          <p>如果物件是專案、任務或問題，可讓使用者貢獻物件。</p>
          <p>允許用戶編輯配置檔案或擁有對象的配置檔案權限（如果對象是用戶）。</p></li> 
          <li><b>編輯</b>:管理物件的權限 </li> 
          <li><b>僅限管理員</b>:系統管理員訪問級別</li> 
         </ul> </li> 
        <p>下列權限可在 <b>對對象具有此訪問權限的用戶可以編輯欄位值</b>: </p> 
         <ul> 
          <li> <p><b>有限編輯</b>:（只有對象是項目、任務、問題或用戶時才可用）:</p> 
           <p>如果物件是專案、任務或問題，此權限可讓使用者貢獻該物件</p>
          <p>如果對象是用戶，則此權限允許用戶編輯配置檔案或擁有該對象的配置檔案權限。</p> 
          <li><b>編輯</b>:管理物件的權限 </li> 
          <li><b>僅限管理員</b>:系統管理員訪問級別</li> 
         </ul> </li> 
       </ul> 
       <p>有關對象權限的資訊，請參見 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">對象共用權限概述</a>.</p> 
       <p><b>附註</b>:  
       <ul> 
       <li> <p>沒有您在此處指定權限的使用者看不到區段中的自訂欄位和Widget。 </p> <p>如果在報表中顯示欄位值，或在文字模式報表中的計算欄位中使用這些值，也會是正確的。</p> </li> 
       <li> <p>將多個對象類型與表單關聯可以更改這些步驟中可用的查看和編輯權限。 如需詳細資訊，請參閱 <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">多種對象類型如何影響自定義表單中的分節符權限</a> 這篇文章。</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 將至少一個自訂欄位或介面工具集拖曳或新增至新區段。 儲存區段之前，此為必要項目。

1. 按一下 **完成**.

   >[!TIP]
   >
   >您可以按一下 **套用** 在您建立自訂表單時隨時儲存變更並保持表單開啟。

### 多種對象類型如何影響分節符權限 {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

自訂表單區段分段的「有限編輯」權限僅適用於「專案」、「任務」、「問題」和「使用者」物件類型。

在配置了「有限編輯」權限的帶分區符的自定義表單中，如果向表單中添加其他對象類型(Portfolio、程式、文檔、公司、帳單記錄、小版本、費用或組)，將提示您切換到「編輯」權限，該權限與該對象類型和表單上的現有對象類型都相容。

>[!INFO]
>
>**範例：** 在與「項目」對象類型關聯的自定義窗體中，分區符將配置為「有限編輯」權限。
>
>將Portfolio對象類型添加到窗體中，這表示窗體中的分區分隔符不再提供「有限編輯」權限選項。
>
>螢幕上的消息提示您切換到「編輯」權限，該權限是與「項目」對象類型和「Portfolio」對象類型相容的最低權限級別。


## 在自訂表單中放置自訂欄位和小工具


1. 開始建立或編輯自訂表單，如 [設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 若要將自訂欄位和介面工具集放置在同一列，請將一個欄位拖曳到另一個欄位，直到它們之間出現一行。

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* 您可以使用 **預覽** 按鈕，了解自訂欄位和介面工具集在表單中的顯示方式。
>* 自訂欄位和Widget在表單中不一定會以相同的方式顯示，視使用者檢視時可用的螢幕空間大小而定。 例如，如果水準空間有限，一列欄位中的第三個欄位可能會換行到下一列欄位。


1. （可選）若要將自訂欄位或介面工具集置於另一個欄位或介面工具集之上或之下，請將其拖曳至上方或下方，直到項目之間出現水準藍線為止。

1. 若要儲存變更，請按一下 **套用**

   或

   按一下 **儲存並關閉**.

## 預覽自訂表單

1. 開始建立或編輯自訂表單和新增欄位，如 [設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 按一下 **預覽** 在左上角，查看使用表單時的外觀，然後按一下 **結束預覽** 返回編輯表單。