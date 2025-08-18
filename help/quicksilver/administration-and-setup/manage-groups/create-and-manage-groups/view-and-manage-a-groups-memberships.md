---
user-type: administrator
product-area: system-administration;user-management
keywords: 新增，使用者，群組，新增，其他，指派，管理員，移除，使用者，檢視，角色，成員，匯出，成員資格，資料
navigation-topic: create-and-manage-groups
title: 檢視和管理群組的成員資格
description: 身為Adobe Workfront管理員，您可以檢視、新增、移除、匯出、啟用和停用您管理之任何群組的成員。 您也可以編輯其設定檔、將更新新增至其設定檔，並將他們指派為群組的其他群組管理員。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: 2096cfa0fd4d0e7eeb85dbf00668dc1dd7fb1d99
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 1%

---

# 檢視和管理群組的成員資格

身為Adobe Workfront管理員，您可以檢視、新增、移除、匯出、啟用和停用您管理之任何群組的成員。 您也可以編輯其設定檔、將更新新增至其設定檔，並將他們指派為群組的其他群組管理員。

如果您的群組之上有任何群組，其管理員也可以為您的群組執行下列動作。 Workfront管理員也是如此（適用於任何群組）。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視和管理群組的成員資格

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組**。

   在顯示的清單中，Workfront管理員可檢視所有群組和子群組。 群組管理員只能看到他們管理的群組和子群組。

1. 按一下要編輯的群組名稱。
1. 在出現的頁面上，在左側功能表中選取&#x200B;**群組成員**&#x200B;時，執行下列任一動作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新增使用者至群組</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">按一下<strong>新增成員</strong> <img src="assets/add-icon-plus-in-circle.png">，開始輸入使用者的名稱，然後在其出現時選取它。</li> 
        <li value="2"> <p>對您要新增的任何其他使用者重複此步驟。</p> <p>如果您決定不新增該使用者，可以按一下名稱右側的X。</p> </li> 
        <li value="3">完成時，按一下<strong>完成</strong>。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">從群組移除使用者</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">選取一或多個使用者名稱，然後按一下[移除成員]。<strong></strong><img src="assets/remove-icon---x-in-circle.png"></li> 
        <li value="2"> <p>在顯示的警告訊息中，按一下<strong>移除</strong>。</p> <p>您可以按一下<strong>搜尋清單中的人員和群組</strong>，在方塊中輸入其名稱，然後在名稱出現時按一下該名稱，來尋找您要從清單中移除的使用者。</p> <p><b>附註</b>：  
          <ul> 
           <li>如果此群組是您要移除之使用者的「主群組」，您必須先在使用者設定檔中指派另一個主群組。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">主群組總覽</a>和<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>。</li> 
           <li>如果群組只有一個群組管理員，而您需要從群組中移除該管理員，則需要先將另一個群組管理員指派給該群組。</li> 
           <li>使用者可以個別屬於子群組以及父群組。 當您從子群組中移除某人時，該人員會保留在父群組的一部分。 同樣地，當您從父群組中移除這些物件時，它們仍將是子群組的一部分。 如果您不想讓使用者擁有父群組的允許存取權，則必須將使用者從子群組和父群組中移除（如果兩者分別列在兩個位置）。</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">編輯使用者的設定檔資訊</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">選取一或多個使用者名稱，然後按一下<strong>編輯</strong> <img src="assets/edit-icon.png">。</li> 
        <li value="2"> <p>變更使用者的設定檔資訊。</p> <p>如需您可以進行之變更的相關資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">匯出使用者成員資格資料</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">選取一或多個使用者名稱，然後按一下[匯出]。<strong></strong> <img src="assets/export.png">。</li> 
        <li value="2"> <p>將資料匯出為PDF、Excel或Tab分隔檔案。</p> <p>如需匯出資料的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">匯出資料</a>。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">檢視和編輯成員的群組角色</td> 
      <td> <p><strong>群組角色</strong>欄列出每個成員的角色。 作為群組管理員，您可以連按兩下成員的角色來進行變更。</p> <p>對於不是群組管理員的群組成員，此欄不可編輯。</p> <p>群組管理員一律位於清單頂端。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">傳送註解給群組成員</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">請至少選取一個群組成員，然後按一下工具列中的<strong>傳送更新給使用者</strong>。</li> 
        <li value="2"><p>輸入您要傳送給使用者的註解，以及使用者設定檔的更新區域。</p>
        <p>如需詳細資訊，請參閱<a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">傳送直接訊息給其他使用者</a>。</p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在Workfront中啟動使用者</td> 
      <td>選取一或多個非作用中的使用者，然後按一下[啟用使用者]，在Workfront中啟用這些使用者。<strong></strong> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在Workfront中停用使用者</td> 
      <td>選取一或多個使用中的使用者，然後按一下[停用使用者]，在Workfront中停用使用者<strong>。</strong><img src="assets/deactivate-user.png"></td> 
     </tr> 
     <tr> 
      <td role="rowheader">依欄排序</td> 
      <td>按一下欄標題，依該欄中的內容排序清單。</td> 
     </tr> 
    </tbody> 
   </table>
