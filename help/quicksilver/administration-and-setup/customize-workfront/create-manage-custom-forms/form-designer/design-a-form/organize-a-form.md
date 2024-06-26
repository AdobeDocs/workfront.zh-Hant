---
title: 使用表單設計工具來組織和預覽表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表單設計工具來組織自訂表單。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 28961cda48ce4eec84ed272e660be6ba938be370
workflow-type: tm+mt
source-wordcount: '1285'
ht-degree: 0%

---

# 使用表單設計工具來組織和預覽表單

您可以使用表單設計工具來組織自訂表單，並預覽以確認其設定正確。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

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
   <p>新計畫：標準</p>
   <p>或</p>
   <p>目前計畫：計畫</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>管理自訂表單的存取權</p> <p>如需Workfront管理員如何授予此存取許可權的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者管理特定區域的存取權</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## 新增分割槽符號

您可以將自訂表單中的自訂欄位和Widget分組到具有標題的區段中。 這對於向將填寫表單的使用者展示有組織體驗非常有用。 此外，如果您需要限制特定使用者對特定自訂欄位和Widget的存取權，您可以將它們放置在區段中，然後僅授予這些使用者對區段的存取權。

例如，如果您需要追蹤只有系統管理員才應該能夠檢視或編輯的敏感資訊，您可以使用僅限管理員許可權建立分割槽符號，並將敏感欄位放置在該分割槽中。

您為區段選取的存取設定會直接繫結至使用者在附加自訂表單的Workfront物件上擁有的許可權。 您可以根據使用者是否有許可權檢視、貢獻或管理該物件來隱藏或顯示區段。 或者，您可以將區段設為「僅限管理員」，以便只有具有系統管理員存取層級的使用者才能存取該區段。

如需物件許可權的相關資訊，請參閱 [物件許可權共用概觀](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

如需自訂表單中自訂欄位和Widget的相關資訊，請參閱 [設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### 建立及設定自訂表單中區段的存取權

1. 開始建立或編輯自訂表單並新增欄位，如中所述 [設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 按一下 **分割槽符號** 並將其拖曳至畫布上所需的位置。

1. 在右側面板中，設定您要用於區段的選項：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">標籤</td> 
      <td> <p>（必要）輸入描述性標籤以顯示於區段上方。 您可以隨時變更標籤。</p> <p><b>重要</b>：請避免在此標籤中使用特殊字元。 它們在報表中無法正確顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>如果要向使用者說明此區段的用途，請鍵入文字。 這會顯示在自訂表單上區段的標籤下方。</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>授予存取權</p> </td> 
      <td> <p> 選取使用者在已附加自訂表單的物件上所需的許可權，以便檢視此區段並編輯其欄位值。 
       <p>下列許可權位於 <b>具有物件存取許可權的使用者可以檢視欄位值</b>：</p> 
         <ul>
          <li><strong>檢視</strong>：檢視物件的許可權</li>
          <li><p><b>有限的編輯</b>：（僅當物件為專案、任務、問題或使用者時可用）：</p> 
          <p>允許使用者為專案、任務或問題的物件貢獻內容。</p>
          <p>如果物件為使用者，則允許使用者編輯設定檔或擁有該物件的設定檔許可權。</p></li> 
          <li><b>編輯</b>：管理物件的許可權 </li> 
          <li><b>僅限管理員</b>：系統管理員存取層級</li> 
         </ul> </li> 
        <p>下列許可權位於 <b>具有物件存取許可權的使用者可以編輯欄位值</b>： </p> 
         <ul> 
          <li> <p><b>有限的編輯</b>：（僅當物件為專案、任務、問題或使用者時可用）：</p> 
           <p>如果物件是專案、任務或問題，則此許可權可讓使用者為物件貢獻內容</p>
          <p>如果物件是使用者，則此許可權可讓使用者編輯設定檔或擁有物件的設定檔許可權。</p> 
          <li><b>編輯</b>：管理物件的許可權 </li> 
          <li><b>僅限管理員</b>：系統管理員存取層級</li> 
         </ul> </li> 
       </ul> 
       <p>如需物件許可權的相關資訊，請參閱 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">物件許可權共用概觀</a>.</p> 
       <p><b>注意</b>：  
       <ul> 
       <li> <p>沒有您在此指定許可權的使用者無法看到區段中的自訂欄位和Widget。 </p> <p>如果您在報表中顯示欄位值，或在文字模式報表的計算欄位中使用這些值，也會發生這種情況。</p> </li> 
       <li><p>針對請求/問題自訂表單：如果需要檢視存取權才能檢視分割槽符號中的欄位，但需要管理員存取權才能編輯欄位，則非管理員在填寫表單時將看不到分割槽及其所有欄位。 建立請求後，擁有檢視存取許可權的使用者即可檢視區段中的欄位。</p></li>
       <li> <p>將多個物件型別與您的表單建立關聯，可以變更這些步驟中可用的檢視和編輯許可權。 如需詳細資訊，請參閱 <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">多個物件型別如何影響自訂表單中的分割槽符號許可權</a> 本文章內容。</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>新增邏輯</p></td> 
      <td><p>根據使用者在填寫表單時於多選自訂欄位中所做的選擇，使用顯示邏輯來指定區段是否應顯示在表單上。</p><p><strong>注意：</strong> 如果分割槽符號下的所有個別欄位已套用顯示邏輯，並且它們都因該邏輯而隱藏，則整個分割槽將在自訂表單上隱藏。 即使顯示邏輯未套用至分割槽符號，也會發生這種情況。</p><p>如需詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref">使用表單設計工具新增顯示邏輯和略過邏輯</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 拖曳或新增至少一個自訂欄位或Widget至新區段。 儲存區段前必須先完成此作業。

1. 按一下 **完成**.

   >[!TIP]
   >
   >您可以按一下 **套用** 建立自訂表單時，隨時儲存變更並保持表單開啟。

### 多個物件型別如何影響分割槽符號許可權 {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

自訂表單分割槽符號的「有限編輯」許可權僅適用於專案、任務、問題和使用者物件型別。

在設定了「有限編輯」許可權之分割槽符號的自訂表單中，如果您將其中一個其他物件型別(Portfolio、方案、檔案、公司、記帳記錄、反複專案、費用或群組)新增到表單，系統將提示您切換到「編輯」許可權，該許可權與該物件型別和表單上的現有物件型別都相容。

>[!INFO]
>
>**範例：** 在與專案物件型別相關聯的自訂表單中，分割槽符號是以「有限編輯」許可權設定的。
>
>您將Portfolio物件型別新增至表單，這表示限制編輯許可權選項不再可用於表單中的分割槽符號。
>
>熒幕上的訊息會提示您切換到「編輯」許可權，這是與Project物件型別和Portfolio物件型別相容的最低許可權等級。


## 在自訂表單中定位自訂欄位和Widget


1. 開始建立或編輯自訂表單，如所述 [設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 若要將自訂欄位和Widget放置在同一列，請將其中一個拖曳到另一個旁邊，直到它們之間出現線條為止。

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* 您可以使用 **預覽** 按鈕來瞭解自訂欄位和Widget在表單中的顯示方式。
>* 自訂欄位和Widget不一定會在表單中以相同的方式顯示，取決於使用者檢視時可用的熒幕空間。 例如，如果水準間距受限，欄位列中的第三個欄位可能會換成下一列欄位。

1. （可選）若要將自訂欄位或Widget置於另一個欄位之上或之下，請將其拖曳至另一個欄位之上或之下，直到專案之間出現水準藍色線為止。

1. 若要儲存變更，請按一下 **套用**

   或

   按一下 **儲存並關閉**.

## 預覽自訂表單

1. 開始建立或編輯自訂表單並新增欄位，如中所述 [設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 按一下 **預覽** ，檢視表單使用時的外觀，然後按一下 **結束預覽** 以返回編輯表單。

