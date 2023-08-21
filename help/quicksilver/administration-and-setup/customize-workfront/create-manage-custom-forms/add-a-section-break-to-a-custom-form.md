---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用舊版表單產生器將分割槽符號新增至自訂表單
description: 您可以將自訂表單中的自訂欄位和Widget分組到具有標題的區段中。 這對於向將填寫表單的使用者展示有組織體驗非常有用。 此外，如果您需要限制特定使用者對特定自訂欄位和Widget的存取權，您可以將它們放置在區段中，然後僅授予這些使用者對區段的存取權。
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 44a52767-60a7-4aaa-b3b8-6b8fb7da7e72
source-git-commit: 961e0451ce9011a8a9f511d7d5da99368d22d6fb
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# 使用舊版表單產生器將分割槽符號新增至自訂表單

您可以將自訂表單中的自訂欄位和Widget分組到具有標題的區段中。 這對於向將填寫表單的使用者展示有組織體驗非常有用。 此外，如果您需要限制特定使用者對特定自訂欄位和Widget的存取權，您可以將它們放置在區段中，然後僅授予這些使用者對區段的存取權。

例如，如果您需要追蹤只有系統管理員才應該能夠檢視或編輯的敏感資訊，您可以使用僅限管理員許可權建立分割槽符號，並將敏感欄位放置在該分割槽中。

您為區段選取的存取設定會直接繫結至使用者在附加自訂表單的Workfront物件上擁有的許可權。 您可以根據使用者是否有許可權檢視、貢獻或管理該物件來隱藏或顯示區段。 或者，您可以將區段設為「僅限管理員」，以便只有具有系統管理員存取層級的使用者才能存取該區段。

如需物件許可權的相關資訊，請參閱 [物件許可權共用概觀](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

如需自訂表單中自訂欄位和Widget的相關資訊，請參閱 [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

<!--
>[!TIP]
>
>Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms and widgets added to custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).
-->

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
   <td>計劃</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>管理自訂表單的存取權</p> <p>如需Workfront管理員如何授予此存取許可權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者管理特定區域的存取權</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取層級設定，請聯絡Workfront管理員。

## 建立及設定自訂表單中區段的存取權

1. 開始建立或編輯自訂表單，如所述 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 新增自訂欄位和Widget至表單，如所述 [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. 在建立或編輯自訂表單時，請在 **新增欄位** 標籤，按一下 **分割槽符號**.

   ![](assets/click-section-break.jpg)

1. 在 **欄位設定** 標籤中，設定您想要用於區段的選項：

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
     <tr> 
      <td role="rowheader">新增邏輯</td> 
      <td>根據使用者在填寫表單時於多選自訂欄位中所做的選擇，使用顯示邏輯來指定區段是否應顯示在表單上。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">新增顯示邏輯和略過邏輯至自訂表單</a>.</td> 
     </tr> 
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
       <p>如需物件許可權的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">物件許可權共用概觀</a>.</p> 
       <p><b>附註</b>:  
       <ul> 
       <li> <p>沒有您在此指定許可權的使用者無法看到區段中的自訂欄位和Widget。 </p> <p>如果您在報表中顯示欄位值，或在文字模式報表的計算欄位中使用這些值，也會發生這種情況。</p> </li> 
       <li> <p>將多個物件型別與您的表單建立關聯，可以變更這些步驟中可用的檢視和編輯許可權。 如需詳細資訊，請參閱 <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">多個物件型別如何影響自訂表單中的分割槽符號許可權</a> 本文章內容。</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 拖曳或新增至少一個自訂欄位或Widget至新區段。

   儲存區段前必須先完成此作業。

1. 按一下 **完成**.

   >[!TIP]
   >
   >您可以按一下 **套用** 建立自訂表單時，隨時儲存變更並保持表單開啟。

1. 如果您想以其他方式繼續建置自訂表單，請繼續閱讀下列其中一篇文章：

   * [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [新增計算資料至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自訂表單中定位自訂欄位和Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [新增顯示邏輯和略過邏輯至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [預覽並完成自訂表格](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

<!--
DRAFTED IN FLARE:
<h2>Configure access for fields without section breaks</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">************This section might get added later. Team decided not to implement.</p>
<p>In a custom form, you can also control users' access to custom fields
and image widgets that are not placed inside a defined section.</p>
<ol>
<li value="1">Begin creating or editing a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Add custom fields

and widgets

to the form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md" class="MCXref xref">Add a custom field to a custom form</a>.</li>
<li value="3"> <p>While still creating or editing the custom form, open the <b>Form settings</b> tab.</p> <p>SHOW THIS </p> </li>
<li value="4"> <p>Under <b>Grant access</b>, configure the permissions that users need on an object where the custom form is attached, in order to view and edit values in fields not placed under a section break. </p> <p>If you need information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <note type="note">
<ul>
<li> <p>Users without the permissions you specify here can't see the values of the fields
and image widgets that are not placed in a defined section in the custom form. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li>
<li> <p>Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li>
</ul>
</note>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><b>Users with this access to the object can view field values</b> </td>
<td>
<ul>  
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader">Users with this access to the object can edit field values</td>
<td>
<ul>
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click Done.</p> <note type="tip">
You can click
<strong>Apply</strong> at any point while you are creating a custom form to save your changes and keep the form open.
</note> </li>
<li value="6"> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an asset widget in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position custom fields and widgets in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li>
</ul> </li>
</ol>
</div>
-->

## 多個物件型別如何影響分割槽符號許可權 {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

自訂表單分割槽符號的「有限編輯」許可權僅適用於專案、任務、問題和使用者物件型別。

在設定了「有限編輯」許可權之分割槽符號的自訂表單中，如果您將其中一個其他物件型別(Portfolio、方案、檔案、公司、記帳記錄、反複專案、費用或群組)新增到表單，系統將提示您切換到「編輯」許可權，該許可權與該物件型別和表單上的現有物件型別都相容。

>[!INFO]
>
>**範例：** 在與專案物件型別相關聯的自訂表單中，分割槽符號是以「有限編輯」許可權設定的。
>
>您將Portfolio物件型別新增至表單，這表示限制編輯許可權選項不再可用於表單中的分割槽符號。
>
>熒幕上的訊息會提示您切換到「編輯」許可權，這是與「有限編輯」最相似的選項，並與「專案」物件型別和「Portfolio」物件型別相容。
