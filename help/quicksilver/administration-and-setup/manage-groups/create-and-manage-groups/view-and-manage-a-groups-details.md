---
title: 檢視及管理群組的詳細資訊
description: 您可以檢視並編輯您管理的群組或子群組的「群組詳細資訊」頁面。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 1%

---

# 檢視及管理群組的詳細資訊

您可以檢視並編輯您管理的群組或子群組的「群組詳細資訊」頁面。 此頁面包含：

* 群組的說明
* 業務主管和群組管理員的姓名
* 可讓您將群組及其子群組設為公開或私用的選項

如需管理群組的其他方法相關資訊，請參閱[建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)。

如需如何停用或重新啟用群組的詳細資訊，請參閱[停用或重新啟用群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr>
  <tr> 
   <td>存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視及管理群組的詳細資訊

{{step-1-to-setup}}

1. 按一下&#x200B;**群組**。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下您要編輯的最上層群組的名稱。
1. 如果您想要停用或重新啟用群組，
1. 在左側功能表中，按一下&#x200B;**群組詳細資料**，然後執行下列任一項作業：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td> <p>最多可輸入512個字元。</p> <p>如果欄位空白，請按一下[新增] <strong> </strong>輸入說明。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">為作用中</td> 
      <td> <p>（預設為啟用）在您的Workfront執行個體中啟用群組。</p> <p>在類似下面所示的預先輸入欄位中，當一般使用者搜尋群組以將其附加至物件或與其共用物件時，清單中只會顯示作用中的群組。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>若要簡化使用者的這項作業，您可以停用目前未使用之群組的[作用中]選項。</p> <p>您可以使用此欄位，根據作用中或非作用中狀態輕鬆檢視、篩選及分組群組清單。 如需有關在清單中使用檢視、篩選和群組的資訊，請參閱<a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">報告元素：篩選器、檢視和群組</a>。</p> <p>如需非作用中群組的相關資訊，請參閱文章<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">刪除或停用自訂表單</a>中的<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">非作用中群組的考量事項</a>一節。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">群組協助工具</td> 
      <td> <p>(只有在檢視群組（而非子群組）的「詳細資訊」時才可用。) 啟用或停用選項<strong>將此群組和子群組設為私人</strong>。</p> <p>對於公用群組，任何擁有編輯使用者存取許可權的使用者（在群組內或群組外），都可以將該群組新增到其他使用者的設定檔中。 他們無法為私人群組執行此操作。</p> <p>您只能在具有多個層級的群組階層中的頂層父群組上編輯此選項。 父群組的所有子群組都會繼承其設定。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">群組關係人</td> 
      <td> 
       <ul> 
        <li><strong>群組管理員</strong>：新增或移除具有Planner授權的使用者，作為群組的群組管理員。 開始輸入使用者的名稱，然後在名稱出現在下拉式選單中時按一下該名稱。</li> 
        <li><strong>業務領導者</strong>：執行下列任一項作業：
         <ul>
          <li>如果您尚未指派群組的業務領導者，請按一下[新增] <strong></strong>，開始輸入您要指派的使用者名稱，然後在人員出現時按一下該人員的名稱。</li>
          <li>如果群組已經有「業務領導者」且您想要變更它，請連按兩下現有「業務領導者」的名稱。 刪除名稱，開始輸入您要指派的使用者名稱，然後在人員出現時按一下該人員的名稱。</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">新增自訂表格</td> 
      <td>如果您的存取層級可讓您管理自訂表格，請新增自訂表格至群組。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">自訂表格</a>。</td> 
     </tr> 
    </tbody> 
   </table>
