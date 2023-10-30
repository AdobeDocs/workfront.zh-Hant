---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 建立和修改群組的公司
description: 當您檢視您在「群組」區域中管理的群組時，可以檢視與群組及其任何子群組相關聯的公司並與其合作。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: ab7877c048ea87180dd518c978b258d266e0f95c
workflow-type: tm+mt
source-wordcount: '755'
ht-degree: 0%

---

# 建立和修改群組的公司

當您檢視您在「群組」區域中管理的群組時，可以檢視與群組及其任何子群組相關聯的公司並與其合作。

如果您的群組之上有任何群組，其管理員也可以為您的群組執行下列動作。 Workfront管理員也是如此（適用於任何群組）。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

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
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">授予使用者完整管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要瞭解自己的計畫或授權型別，請聯絡Workfront管理員。

## 從群組區域檢視、處理和建立您群組的公司

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 按一下要為其建立或修改公司的群組名稱。
1. 在左側面板中，按一下 **公司** 列出與群組相關聯的公司及其可能擁有的任何子群組。
1. （選用）若要新增公司，請按一下 **新增公司**，然後使用下列選項設定公司。 完成後，按一下 **建立公司**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">基本資訊區段</td> 
      <td> 
       <ul> 
        <li> <p><b>公司名稱</b>：輸入公司的名稱。</p> </li> 
        <li> <p><b>已啟用</b>：啟用此選項後，使用者可以找到公司並將其附加至建立和編輯的專案。 非作用中的公司無法附加到專案。 此選項預設為啟用。</p> </li> 
        <li> <p><b>這是主要公司</b>：將公司指派為您組織的主要公司。 主要公司通常代表您大部分使用者工作所在的Workfront帳戶。</p> <p>透過修改其存取層級，您可以限制使用者檢視其他使用者：</p> 
         <ul> 
          <li>僅在其主要公司中</li> 
          <li> <p>在其關聯公司和主要公司中</p> <p>如需使用者存取層級內主要公司功能的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>.</p> <p>您只能有一個或沒有公司被指定為主要公司，但您不能有多個公司被指定為主要公司。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>群組</b>：如果存在與公司進行業務的群組，您可以在此處新增群組名稱。 這對於需要報告和管理其群組業務所在的所有公司的群組管理員非常有用。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">系統會填入 <strong>群組</strong> 欄位中適用於含有您所檢視群組的新公司。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">如果您擁有存取層級中公司的管理存取權，您可以從公司中移除群組並指派不同的群組，或離開公司而不使用群組。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">如果您沒有公司的管理存取權， <strong>群組</strong> 欄位為必填，您只能選取您管理的群組或這些群組下的任何子群組。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">如需有關對公司的管理存取權的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">授予使用者管理特定區域的存取權</a>.</p> </li> 
        <li> <p><b>公司成員</b>：將現有使用者新增至公司。 透過這樣做，您可將這些使用者與此公司建立關聯。</p> <p>您與一個公司建立關聯的使用者數量沒有限制，但一個使用者不能與多個公司建立關聯。</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">自訂Forms區段</td> 
      <td> <p>如果您想要將某些欄位新增至Workfront中不提供的公司，您可以建立自訂表格並將其與公司建立關聯。 您可以從下拉式選單中選取此表單，以將其附加至您的公司。 下拉式功能表中只會列出作用中的公司。 如需建立自訂Forms的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">建立或編輯自訂表單</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >如果您擁有存取層級中公司的管理存取權，也可以按一下清單底部的「新增更多公司」 。 這會新增一列，讓您快速設定新公司。

1. （可選）若要編輯或刪除公司，請選取至少一家公司，然後使用工具列按鈕進行編輯 ![](assets/edit-icon.png) 或刪除 ![](assets/delete.png) it.

   如需編輯公司的詳細資訊，請參閱區段 [在Workfront中建立或編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) 在文章中 [建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. （可選）若要匯出公司清單，請按一下「匯出」圖示 ![](assets/export.png)，然後選取您要用於匯出清單的檔案格式。
