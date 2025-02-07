---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 建立和修改群組的團隊
description: 當您在「群組」區域中檢視您管理的群組時，您可以檢視與群組及其任何子群組相關聯的專案團隊並與其合作。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 3%

---

# 建立和修改群組的團隊

當您在「群組」區域中檢視您管理的群組時，您可以檢視與群組及其任何子群組相關聯的專案團隊並與其合作。

如果您的群組之上有任何群組，其管理員也可以為您的群組執行下列動作。 Workfront管理員也是如此（適用於任何群組）。

如需有關如何擁有計畫授權的使用者建立團隊的資訊，請參閱[建立團隊](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)。

如需Workfront管理員如何建立團隊的詳細資訊，請參閱[從設定區域建立團隊](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td> <p>規劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">群組管理員</a>和<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">授與使用者完整管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要瞭解您擁有的計畫或授權型別，請連絡您的Workfront管理員。

+++

## 從群組區域檢視、處理和建立群組的團隊

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

1. 按一下要為其建立或修改專案團隊的群組名稱。
1. 在左側面板中，按一下&#x200B;**團隊** ![團隊](assets/teams.png)，列出與群組及其可能擁有的任何子群組相關聯的團隊。

1. 執行下列任一項作業：

   * **新增團隊**：按一下&#x200B;**新增團隊**，然後使用下列選項進行設定：

   <!-- WRITER please check table below. I stripped out wonky conditions-->

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">團隊名稱</td> 
       <td>輸入團隊的名稱。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">群組</td> 
       <td> <p> 系統會用您正在檢視的群組來填入新專案團隊的「群組」欄位。 如果要將專案團隊與不同的群組相關聯，請開始輸入群組的名稱，然後在其出現時選取名稱。</p> <p>您可以暫留在正確的群組上，並按一下旁邊顯示的資訊圖示<img src="assets/info-icon.png">，確定您要將正確的群組與團隊建立關聯。 這會顯示工具提示，列出群組的相關資訊，例如群組及其管理員上方的群組階層。</p> <p><b>注意</b>：將團隊指派給群組或子群組時，該群組或子群組的任何群組管理員都可以管理團隊，而無需成為其成員。 群組管理員可以從主功能表前往團隊區域，然後按一下「切換團隊」箭頭<img src="assets/switch-team-icon.png" alt="切換群組圖示">以列出指派給其管理群組的所有團隊。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">團隊成員</td> 
       <td> <p>開始輸入要加入團隊的使用者名稱，然後在出現於下拉式清單中的時選取名稱。 重複此程式，將多位使用者新增至團隊。</p> <p>您可以新增到團隊的使用者數量沒有限制。 但是，我們建議一個團隊中的使用者數量不要過多，因為團隊的工作管理可能會變得太複雜。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">說明</td> 
       <td>輸入團隊的說明。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">行事曆</td> 
       <td>選擇針對此團隊顯示的行事曆標籤。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">處理它</td> 
       <td>將處理它按鈕變更為開始按鈕。 當使用者按一下開始，專案的狀態會自動更新。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">完成按鈕</td> 
       <td>按一下「完成」按鈕時，選取您要為專案設定的狀態。</td> 
       </tr> 
      </tbody> 
     </table>

   * **編輯團隊**：請至少選取一個團隊，按一下&#x200B;****「編輯」圖示![「編輯」圖示](assets/edit-icon.png)，然後使用下列選項進行設定：

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">團隊名稱</td> 
       <td>輸入團隊的名稱。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">群組</td> 
       <td> <p>將團隊與群組建立關聯。 開始輸入群組的名稱，然後在其出現時選取名稱。</p> <p>您可以暫留在正確的群組上，並按一下旁邊顯示的資訊圖示<img src="assets/info-icon.png">，確定您要將正確的群組與團隊建立關聯。 這會顯示工具提示，列出群組的相關資訊，例如群組及其管理員上方的群組階層。</p> <p><b>注意</b>：將團隊指派給群組或子群組時，該群組或子群組的任何群組管理員都可以管理團隊，而無需成為其成員。 群組管理員可以從主功能表前往團隊區域，然後按一下「切換團隊」箭頭<img src="assets/switch-team-icon.png" alt="切換群組圖示">以列出指派給其管理群組的所有團隊。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">所有者</td> 
       <td>選取團隊的擁有者。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">團隊成員</td> 
       <td> <p>新增和團隊成員。 開始輸入使用者的名稱，然後在其出現時選取名稱。 重複此程式，將多位使用者新增至團隊。</p> <p><b>秘訣</b>：您可以新增至團隊的使用者數目沒有限制。 但是，我們建議一個團隊中的使用者數量不要過多，因為團隊的工作管理可能會變得太複雜。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">說明</td> 
       <td>輸入團隊的說明。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">版面配置範本</td> 
       <td> <p>開始輸入您希望團隊使用的版面配置範本名稱，然後在其出現時按一下它。</p> <p>當您指定具有此配置範本的專案團隊作為使用者的主專案團隊時，此專案團隊中的所有使用者都會看到此配置範本中的自訂。<br>他們的個別配置範本設定將覆寫主團隊配置範本的設定。 </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">敏捷</td> 
       <td>指定這是否為敏捷團隊。 有關敏捷團隊以及如何管理其工作的資訊，請參閱<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">建立敏捷團隊</a>。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">處理它</td> 
       <td> <p>將處理它按鈕變更為開始按鈕。 當使用者按一下開始，專案的狀態會自動更新。</p> <p>如需如何設定[開始]按鈕的詳細資訊，請參閱<a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">以[開始]按鈕取代[處理它]按鈕</a>。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">完成按鈕</td> 
       <td> <p>自訂完成按鈕。 如需詳細資訊，請參閱：</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">設定任務的[完成]按鈕</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">設定問題的完成按鈕</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **刪除團隊**：請至少選取一個團隊，然後按一下「刪除」圖示![「刪除」圖示](assets/delete.png)。
   * **匯出團隊清單**：按一下&#x200B;**匯出** ![匯出圖示](assets/export.png)，然後選取您要用於匯出清單的檔案格式。
