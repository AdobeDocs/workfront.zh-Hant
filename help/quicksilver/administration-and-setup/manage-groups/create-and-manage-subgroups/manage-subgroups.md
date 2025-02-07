---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理，子群組，編輯
navigation-topic: create-and-manage-subgroups
title: 管理子群組
description: 身為子群組的群組管理員，您可以建立、移動、檢視、編輯、複製、重新命名、匯出及刪除子群組。 您也可以將子群組從父群組中移除，使其成為最上層群組。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1251'
ht-degree: 1%

---

# 管理子群組

身為子群組的群組管理員，您可以建立、移動、檢視、編輯、複製、重新命名、匯出及刪除子群組。

您也可以將子群組從父群組中移除，使其成為最上層群組。

如果您的群組之上有任何群組，其管理員也可以為您的群組執行下列動作。 Workfront管理員也是如此（適用於任何群組）。

如需子群組的詳細資訊，請參閱[子群組總覽](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)。

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

## 建立、移動、檢視、編輯、複製、重新命名、匯出或刪除子群組

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

   在顯示的清單中，您可以看到您管理的群組及其擁有的任何子群組。 Adobe Workfront管理員可檢視所有群組。

1. 按一下包含您要處理之子群組的群組名稱。

   或

   如果您要移動一個或多個子群組，請按一下目的地群組的名稱（您將在後續步驟中指定要移動的子群組）。

1. 在左側功能表中，按一下&#x200B;**子群組**。

1. 執行下列任一項作業：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">建立新的子群組</td> 
      <td> <p>如果您想要從檢視的群組建立新子群組，請按一下[新增子群組] <strong> </strong>。</p> <p>或者，如果您想要在清單中另一個子群組下方建立新的子群組，請選取該子群組，然後按一下[新增s</strong><strong>子群組</strong>]。<strong></p> <p>如需您可以用來設定子群組的選項相關資訊，請參閱<a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">建立子群組</a>中的表格。</p> <p>群組階層不可超過15個層級，但單一層級可以有不限數量的平行群組。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">移動子群組 </td> 
      <td> <p>您可以將現有的子群組移至您管理的另一個群組下。</p> <p>群組階層不可超過15個層級，但單一層級可以有不限數量的平行群組。</p> 
       <ol> 
        <li value="1"> <p>（選擇性）選取一個子群組，使其成為目的地群組。</p> <p>如果您略過此步驟，您在步驟3中選取的群組就是目的地群組。</p> </li> 
        <li value="2">按一下<strong>新增子群組</strong> &gt; <strong>現有群組</strong>。</li> 
        <li value="3"> <p>在出現的<strong>現有群組</strong>方塊中，開始輸入您要移動的子群組名稱。</p> <p>顯示的結果不包含目的地群組上方的群組。</p> <p>您可以暫留在正確的群組上，並按一下旁邊顯示的資訊圖示<img src="assets/info-icon.png">，確定您選取的群組正確。 這會顯示工具提示，列出群組的相關資訊，例如群組及其管理員上方的群組階層。</p> </li> 
        <li value="4"> <p>當您看到子群組顯示在清單中時，按一下您要移動的子群組名稱。</p> </li> 
        <li value="5"> <p>針對您要移至目的地群組的任何其他子群組，重複步驟c-d</p> </li> 
        <li value="6">按一下「<strong>儲存</strong>」。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">編輯子群組</td> 
      <td> <p>選取您要編輯的子群組，然後按一下「編輯」圖示<img src="assets/edit-icon.png">。</p> <p>如需您可以用來設定子群組的選項相關資訊，請參閱<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">建立群組</a>中的表格。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">匯出一個或多個子群組</td> 
      <td> 
       <ol> 
        <li value="1">選取要匯出的子群組。</li> 
        <li value="2">按一下「匯出」圖示<img src="assets/export.png">，然後選取您想要的檔案格式。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">複製子群組以建立新的頂層群組</td> 
      <td> <p>(僅適用於Workfront管理員)。 當您複製子群組時，它會變成父群組。 所有群組成員和子群組都會隨其一起複製。 群組成員會保留其在原始群組中的任何指派。</p> <p>如需有關複製子群組的詳細資訊，請參閱本文中的<a href="#about-copying-a-subgroup" class="MCXref xref">關於複製子群組</a>。</p> 
       <ol> 
        <li value="1">選取子群組，然後按一下「複製」圖示<img src="assets/copy-icon.png">，根據選取的群組建立新的頂層群組。</li> 
        <li value="2"> <p>設定新群組的設定。</p> <p>如需這些設定的說明，請參閱<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">複製現有群組或子群組</a>中的文章<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">複製現有群組或子群組以建立最上層群組</a>一節中的表格。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除子群組</td> 
      <td> <p><b>重要</b>：當您刪除群組或子群組時，您需要保留使用者、工作專案以及目前指派給它的任何子群組。 為了協助您確定它們會被保留，出現提示時，您需要在下方步驟中將群組的物件重新指派給不同的群組。</p> 
       <ol> 
        <li value="1">選取子群組，然後按一下「刪除」圖示<img src="assets/delete.png">。</li> 
        <li value="2">在出現的<strong>刪除群組</strong>方塊中，開始輸入，然後選取您要移動所刪除群組之成員、工作專案及子群組的群組名稱。</li> 
        <li value="3">按一下<strong>刪除它們</strong>。</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>當您管理包含子群組的群組時，能夠識別和篩選有關整個群組及其所有子群組的資料會很有幫助。 您可以使用報表或清單中的「頂層父項ID」欄位來達到此目的。
>
>例如，假設您管理一個大型行銷部門，並且想要一個包含整個部門正在處理之所有專案的清單。
>
>在Workfront中，此行銷部門由稱為行銷的群組表示，有3個稱為現場行銷、產品行銷和數位行銷的子群組。 若要列出屬於整個行銷部門（全部4個群組）的專案，您可以使用以下篩選規則為專案區域建立篩選：
>
>`Group: Top Parent ID > Equal > Marketing`
>
>您也可以使用「頂層父項名稱」欄位來識別與頂層群組相關聯的資料，但僅限於在「檢視」中，而不適用於「篩選器」或「群組」。

## 從子群組的父群組中移除子群組，並將其設為最上層群組

您可以將子群組從父群組中移除，使其成為最上層群組。

>[!TIP]
>
>當您停用下有子群組的群組時，這些子群組也會變成非使用中。 如果您希望其中一個處於作用中狀態，可以使用這些指示將其從父群組中移除，然後重新啟用它。
>
>如需停用及重新啟用群組的說明，請參閱文章[檢視及管理群組詳細資料](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)中的[檢視及管理群組詳細資料](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view)及[檢視及管理群組詳細資料](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive)小節。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

1. 選取您要建立最上層群組的父群組，然後按一下「編輯」圖示![「編輯」圖示](assets/edit-icon.png)。
1. 在出現的&#x200B;**編輯群組**&#x200B;方塊中，在&#x200B;**群組成員和群組管理員**&#x200B;下方，開始輸入您要建立最上層群組的子群組名稱，然後在其名稱右側按一下X。
1. 按一下「**儲存**」。

## 檢視和管理群組的子群組成員

當您檢視所管理群組的首頁時，可以檢視和管理群組子群組中的所有使用者。 如需指示，請參閱[檢視和管理子群組成員](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md)。

## 關於複製子群組 {#about-copying-a-subgroup}

複製子群組時，請考量下列事項。

* 如果您複製的子群組有自己的子群組，它們會包含在複製中，其名稱的格式如下：

  `Original subgroup name (Copy)`

* 屬於公用群組的任何子群組也是公用的，因此任何具有編輯 — 使用者存取權的使用者（在群組內或群組外）都可以將使用者新增至子群組。
