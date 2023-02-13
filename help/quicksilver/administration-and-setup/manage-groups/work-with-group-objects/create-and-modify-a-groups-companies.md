---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 建立和修改群組的公司
description: 在「組」區域中查看管理的組時，可以查看與該組及其任何子組關聯的公司並與其合作。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# 建立和修改群組的公司

在「組」區域中查看管理的組時，可以查看與該組及其任何子組關聯的公司並與其合作。

如果群組上有任何群組，其管理員也可以為群組執行這些動作。 Workfront管理員（適用於任何群組）也是如此。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 從「組」區域查看、使用和建立組的公司

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 按一下您要建立或修改公司的群組名稱。
1. 在左側面板中，按一下 **公司** 列出與該組關聯的公司及其可能擁有的任何子組。
1. （選用）若要新增公司，請按一下 **新增公司**，然後使用下列選項設定公司。 完成後，按一下 **建立公司**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">基本資訊區段</td> 
      <td> 
       <ul> 
        <li> <p><b>公司名稱</b>:輸入公司的名稱。</p> </li> 
        <li> <p><b>活動</b>:啟用此選項後，使用者可以找到公司，並將其附加至他們建立和編輯的專案。 非活動公司無法附加至專案。 預設會啟用此選項。</p> </li> 
        <li> <p><b>這是主要公司</b>:將公司指派為您組織的主要公司。 主要公司通常代表大部分使用者所在的Workfront帳戶。</p> <p>通過修改其訪問級別，您可以限制用戶查看其他用戶：</p> 
         <ul> 
          <li>僅在其主要公司</li> 
          <li> <p>在其關聯公司和主要公司</p> <p>如需使用者存取層級內主要公司功能的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>.</p> <p>您只能有一個或沒有一個公司指定為主要公司，但不能有多個公司指定為主要公司。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>群組</b>:如果有與公司有業務往來的組，您可以在此處添加組的名稱。 這對於需要報告及管理其群組從事業務之所有公司的群組管理員非常有用。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">系統會填入 <strong>群組</strong> 欄位，以顯示您正在檢視的群組的新公司。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">如果您在存取層級有公司的管理存取權，您可以從公司中移除群組並指派不同的群組，或將公司保留為沒有群組。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">如果您沒有公司的管理存取權， <strong>群組</strong> 欄位是必填欄位，您只能選取您管理的群組或這些群組下的任何子群組。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">如需公司的管理存取權限相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">授予用戶對特定區域的管理訪問權限</a>.</p> </li> 
        <li> <p><b>公司成員</b>:新增現有使用者至公司。 通過執行此操作，您將這些用戶與此公司關聯。</p> <p>您與一個公司建立關聯的使用者數目並無限制，但一個使用者無法與多個公司建立關聯。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計費率部分</td> 
      <td> <p>您可以在公司層改寫與職務相關聯的開單費率。 有關建立職務職責以及將其與開單費率關聯的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" data-mc-variable-override="">建立和管理作業角色</a>.</p> <p>如需關於在公司層級覆寫計費率的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref" data-mc-variable-override="">在公司層改寫職務開單費率</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂Forms區段</td> 
      <td> <p>如果有您要新增至公司的欄位在Workfront中無法使用，您可以建立自訂表單，並將其與您的公司建立關聯。 您可以從下拉式功能表中選取此表單，將此表單附加至您的公司。 下拉式功能表中僅列出作用中的公司。 如需建立自訂Forms的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">建立或編輯自訂表單</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >如果您在存取層級有公司的管理存取權，您也可以按一下清單底部的新增更多公司。 這會新增一列，讓您快速設定新公司。

1. （可選）要編輯或刪除公司，請至少選擇一個公司，然後使用工具欄按鈕進行編輯 ![](assets/edit-icon.png) 或刪除 ![](assets/delete.png) 它。

   如需編輯公司的相關資訊，請參閱 [在Workfront中建立或編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) 在文章中 [建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. （可選）若要匯出公司清單，請按一下「匯出」圖示 ![](assets/export.png)，然後選取要匯出清單的檔案格式。
