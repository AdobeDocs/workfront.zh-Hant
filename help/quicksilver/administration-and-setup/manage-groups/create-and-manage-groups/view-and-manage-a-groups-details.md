---
title: 檢視及管理群組的詳細資訊
description: 您可以查看和編輯您管理的組或子組的「組詳細資訊」頁。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 1%

---

# 檢視及管理群組的詳細資訊

您可以查看和編輯您管理的組或子組的「組詳細資訊」頁。 此頁面包括：

* 群組的說明
* 業務負責人和組管理員的姓名
* 可讓您將群組及其子群組設為公用或私人的選項

   <!--
  <li>An option that allows you to deactivate or reactivate a group and its subgroups.
  DRAFTED IN FLARE:
  Make this change when Callisto adds the
  <b>Is active</b>
   option to the Details pag
  </li>
  -->

如需管理群組的其他方法，請參閱 [建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

如需如何停用或重新啟用群組的詳細資訊，請參閱 [停用或重新啟用群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

<!--
DRAFTED IN FLARE:
Delete this paragraph when Callisto adds the
<b>Is active</b>
 option to the Details pag
-->

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
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 檢視及管理群組的詳細資訊

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **群組**.

   在隨即顯示的清單中，您可以看到您管理的群組，以及這些群組擁有的任何子群組。 Adobe Workfront管理員可以查看所有群組。

1. 按一下您要編輯的頂層群組名稱。
1. 如果您想要停用或重新啟用群組，
1. 在左側功能表中，按一下 **群組詳細資料**，然後執行下列任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td> <p>您最多可以輸入512個字元。</p> <p>如果欄位空白，請按一下 <strong>新增</strong> 來輸入說明。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">活動</td> 
      <td> <p>（預設啟用）讓群組在您的Workfront執行個體中處於作用中狀態。</p> <p>在如下所示的預先輸入欄位中，當常規用戶搜索組以將其附加到對象或與其共用對象時，清單中只顯示活動組。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>若要簡化使用者的作業，您可以針對目前未使用的群組停用「作用中」選項。</p> <p>您可以使用此欄位，輕鬆地根據使用中或非使用中狀態檢視、篩選及分組群組清單。 如需在清單中使用檢視、篩選和群組的相關資訊，請參閱 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">報表元素：篩選器、檢視和群組</a>.</p> <p>如需非作用中群組的相關資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">非作用中群組的考量事項</a> 在文章中 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">刪除或停用自訂表單</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">群組協助工具</td> 
      <td> <p>(僅當查看組（而非子組）的詳細資訊時可用。) 啟用或停用選項 <strong>將此組和子組設為私有</strong>.</p> <p>對於公用群組，任何具有編輯使用者存取權的使用者（進入或退出群組）都可將群組新增至其他使用者的設定檔。 他們無法為私人群組執行此操作。</p> <p>您只能在具有多個層級之群組階層的上層父群組上編輯此選項。 父組的所有子組都會繼承其設定。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">群組關係人</td> 
      <td> 
       <ul> 
        <li><strong>群組管理員</strong>:添加或刪除具有計畫員許可證的用戶作為組的組管理員。 開始輸入使用者的名稱，然後在下拉式功能表中顯示名稱時按一下名稱。</li> 
        <li><strong>業務領導者</strong>:執行下列任一操作：
         <ul>
          <li>如果尚未為組分配業務主管，請按一下 <strong>新增</strong>，開始輸入要指派的使用者名稱，然後在出現時按一下該人的名稱。</li>
          <li>如果組已有業務主管，並且您想要更改該業務主管，請按兩下現有業務主管的名稱。 刪除名稱，開始鍵入要指派的用戶名稱，然後在出現時按一下該用戶的名稱。</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">新增自訂表格</td> 
      <td>如果您的存取層級可讓您管理自訂表單，請將自訂表單新增至群組。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">自訂表單</a>.</td> 
     </tr> 
    </tbody> 
   </table>
