---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理，子組，編輯
navigation-topic: create-and-manage-subgroups
title: 管理子組
description: 作為子組的組管理員，可以建立、移動、查看、編輯、複製、更名、導出和刪除子組。 您也可以將子組從父組中刪除，使子組成為頂級組。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 1%

---

# 管理子組

作為子組的組管理員，可以建立、移動、查看、編輯、複製、更名、導出和刪除子組。

您也可以將子組從父組中刪除，使子組成為頂級組。

如果群組上有任何群組，其管理員也可以為群組執行這些動作。 Workfront管理員（適用於任何群組）也是如此。

有關子組的詳細資訊，請參閱 [子組概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## 建立、移動、查看、編輯、複製、更名、導出或刪除子組

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

   在隨即顯示的清單中，您可以看到您管理的群組，以及這些群組擁有的任何子群組。 Adobe Workfront管理員可以查看所有群組。

1. 按一下包含要處理的子組的組的名稱。

   或

   如果要移動一個或多個子組，請按一下目標組的名稱（您將指定在以後的步驟中要移動的子組）。

1. 在左側功能表中，按一下 **子組**.

1. 執行下列任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">建立新子組</td> 
      <td> <p>如果要從正在查看的組中向下建立新子組，請按一下 <strong>添加子組</strong>.</p> <p>或者，如果要在清單中的另一個子組下建立新子組，請選擇該子組，然後按一下 <strong>新增</strong><strong>ubgroup</strong>.</p> <p>有關可用於配置子組的選項的資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">建立子組</a>.</p> <p>群組階層不能超過15個層級，但單一層級可以有不限數量的平行群組。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">移動子組 </td> 
      <td> <p>可以移動您管理的其他組下的現有子組。</p> <p>群組階層不能超過15個層級，但單一層級可以有不限數量的平行群組。</p> 
       <ol> 
        <li value="1"> <p>（可選）選擇子組，使其成為目標組。</p> <p>如果您略過此步驟，您在步驟3中選取的群組即為目標群組。</p> </li> 
        <li value="2">按一下 <strong>添加子組</strong> &gt; <strong>現有組</strong>.</li> 
        <li value="3"> <p>在 <strong>現有組</strong> 框中，開始鍵入要移動的子組的名稱。</p> <p>顯示的結果不包含目標組上方的組。</p> <p>您可以將游標移至群組上並按一下資訊圖示，以確定您正在選取正確的群組 <img src="assets/info-icon.png"> 顯示於其旁。 此工具提示會列出群組的相關資訊，例如上方的群組階層及其管理員。</p> </li> 
        <li value="4"> <p>在清單中顯示要移動的子組的名稱時，按一下它。</p> </li> 
        <li value="5"> <p>對要移到目標組的任何其他子組重複執行步驟c-d</p> </li> 
        <li value="6">按一下<strong>儲存</strong>。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">編輯子組</td> 
      <td> <p>選擇要編輯的子組，然後按一下「編輯」表徵圖 <img src="assets/edit-icon.png">.</p> <p>有關可用於配置子組的選項的資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">建立群組</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">導出一個或多個子組</td> 
      <td> 
       <ol> 
        <li value="1">選擇要導出的子組或子組。</li> 
        <li value="2">按一下「匯出」圖示 <img src="assets/export.png">，然後選取您想要的檔案格式。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">複製子組以建立新的頂級組</td> 
      <td> <p>(僅適用於Workfront管理員。) 複製子組時，它將成為父組。 所有組成員和子組都隨其複製。 組成員保留其在原始組中的任何分配。</p> <p>有關複製子組的詳細資訊，請參閱 <a href="#about-copying-a-subgroup" class="MCXref xref">關於複製子組</a> 這篇文章。</p> 
       <ol> 
        <li value="1">選擇子組，然後按一下「複製」表徵圖 <img src="assets/copy-icon.png"> 以根據選取的群組建立新的頂層群組。</li> 
        <li value="2"> <p>配置新組的設定。</p> <p>如需這些設定的說明，請參閱區段中的表格 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">複製現有組或子組以建立頂級組</a> 在文章中 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">複製現有組或子組以建立頂級組</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除子組</td> 
      <td> <p><b>重要</b>:刪除組或子組時，需要保留當前分配給它的用戶、工作項和任何子組。 為幫助您確保保留這些對象，提示要求您在以下步驟中將組的對象重新分配到另一個組。</p> 
       <ol> 
        <li value="1">選擇子組，然後按一下「刪除」表徵圖 <img src="assets/delete.png">.</li> 
        <li value="2">在 <strong>刪除組</strong> 框，開始鍵入，然後選擇要移動要刪除的組的成員、工作項和子組的組的名稱。</li> 
        <li value="3">按一下 <strong>刪除</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>管理包含子組的組時，能夠識別和篩選有關整個組及其所有子組的資料會很有幫助。 您可以使用報表或清單中的「上層父ID」欄位來執行此操作。
>
>例如，假設您管理一個大型行銷部門，而想要一份清單列出整個部門正在處理的所有專案。
>
>在Workfront中，此行銷部門由稱為「行銷」的群組表示，其中3個子群組稱為「欄位行銷」、「產品行銷」和「數位行銷」。 若要列出屬於整個行銷部門（所有4個群組）的專案，您可以使用下列篩選規則為「專案」區域建立篩選器：
>
>
```
>Group: Top Parent ID > Equal > Marketing
>```
>
>您也可以使用「上層父名稱」欄位來識別與上層群組相關聯的資料，但僅限於「檢視」中，而非「篩選器」或「群組」中。

## 從子組的父組中刪除子組，並使其成為頂級組

通過將子組從其父組中刪除，可以將其設為頂級組。

>[!TIP]
>
>如果停用下面有子組的組，這些子組也會變為非活動狀態。 如果希望其中一個活動，可以使用這些指示將其從父組中刪除，然後重新激活它。
>
>如需停用和重新啟用群組的相關指示，請參閱 [檢視及管理群組的詳細資訊](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) 和 [檢視及管理群組的詳細資訊](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) 在文章中 [檢視及管理群組的詳細資訊](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 選取您要建立頂層群組之群組的父群組，然後按一下「編輯」圖示 ![](assets/edit-icon.png).
1. 在 **編輯群組** 框，位於 **群組成員和群組管理員**，開始鍵入要建立頂級組的子組的名稱，然後在出現時按一下名稱右側的X。
1. 按一下&#x200B;**儲存**。

## 查看和管理組的子組成員

查看所管理組的首頁時，可以查看和管理組子組中的所有用戶。 如需指示，請參閱 [查看和管理子組成員](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## 關於複製子組 {#about-copying-a-subgroup}

複製子組時，請考慮以下事項。

* 如果複製的子組有其自己的子組，則這些子組將包含在複製中，其名稱的格式如下：

   ```
   Original subgroup name (Copy)
   ```

* 屬於公用組的任何子組也是公用組，因此，具有編輯用戶訪問權限的任何用戶（在組內或組外）都可以向該子組添加用戶。
