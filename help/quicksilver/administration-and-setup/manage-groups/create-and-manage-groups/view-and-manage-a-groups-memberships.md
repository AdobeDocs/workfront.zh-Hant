---
user-type: administrator
product-area: system-administration;user-management
keywords: 添加，用戶，組，添加，其他，分配，管理員，刪除，用戶，視圖，角色，成員，導出，成員，資料
navigation-topic: create-and-manage-groups
title: 查看和管理組成員資格
description: 身為Adobe Workfront管理員，您可以檢視、新增、移除、匯出、啟用和停用您管理之任何群組的成員。 您也可以編輯其設定檔、新增更新至其設定檔，並將其指派為群組的其他群組管理員。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# 查看和管理組成員資格

身為Adobe Workfront管理員，您可以檢視、新增、移除、匯出、啟用和停用您管理之任何群組的成員。 您也可以編輯其設定檔、新增更新至其設定檔，並將其指派為群組的其他群組管理員。

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
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 查看和管理組成員資格

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組**.

   在顯示的清單中，Workfront管理員可以查看所有群組和子群組。 群組管理員只能查看其管理的群組和子群組。

1. 按一下您要編輯的群組名稱。
1. 顯示的頁面上，使用 **群組成員** 在左側功能表中選取，執行下列任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新增使用者至群組</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">按一下 <strong>添加成員</strong> <img src="assets/add-icon-plus-in-circle.png">，開始輸入使用者名稱，然後在出現時選取名稱。</li> 
        <li value="2"> <p>對您要新增的任何其他使用者重複執行此操作。</p> <p>如果您決定不新增該使用者，可以按一下名稱右側的X。</p> </li> 
        <li value="3">按一下 <strong>完成</strong> 時，才能執行此操作。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">從群組中移除使用者</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">選取一或多個使用者名稱，然後按一下 <strong>刪除成員</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>按一下 <strong>移除</strong> 顯示的警告訊息中。</p> <p>您可以按一下 <strong>在清單中搜尋人員和群組</strong>，在方塊中輸入其名稱，然後在出現名稱時按一下名稱。</p> <p><b>附註</b>:  
          <ul> 
           <li>如果此群組是您要移除之使用者的首頁群組，您必須先在使用者的設定檔中指派另一個首頁群組。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">首頁群組概觀</a> 和 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>.</li> 
           <li>如果組只有一個組管理員，而您需要從組中刪除他/她，則需要先為組分配另一個組管理員。</li> 
           <li>使用者可個別屬於子群組以及父群組。 從子組中刪除某個人時，這些人仍是父組的一部分。 同樣地，從父組中刪除它們時，它們仍是子組的一部分。 如果您不希望用戶具有父組的訪問權限，則必須同時從子組和父組中刪除該用戶（如果這兩個用戶分別列在兩個位置）。</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">編輯使用者的設定檔資訊</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">選取一或多個使用者名稱，然後按一下 <strong>編輯</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>變更使用者的設定檔資訊。</p> <p>如需您可進行的變更，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">匯出使用者成員資格資料</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">選取一或多個使用者名稱，然後按一下 <strong>匯出</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>將資料匯出為PDF、Excel或定位點分隔檔案。</p> <p>如需匯出資料的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">匯出資料</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">查看和編輯成員的組角色</td> 
      <td> <p>此 <strong>群組角色</strong> 列列出每個成員的角色。 作為組管理員，可以按兩下某個成員的角色以更改它。</p> <p>對於非群組管理員的群組成員，此欄不可編輯。</p> <p>群組管理員一律位於清單頂端。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將評論發送給組成員</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">選取一或多個使用者名稱，然後按一下 <strong>更新</strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">鍵入注釋。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在Workfront中啟用使用者</td> 
      <td>選取一或多個非作用中使用者，然後按一下 <strong>啟動使用者</strong> 在Workfront中啟用。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在Workfront中停用使用者</td> 
      <td>選取一或多個作用中使用者，然後按一下 <strong>停用使用者</strong><img src="assets/deactivate-user.png"> 在Workfront停用。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">按列排序</td> 
      <td>按一下欄的標題，依該欄的內容排序清單。</td> 
     </tr> 
    </tbody> 
   </table>
