---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 建立和修改群組的團隊
description: 在「組」區域中查看管理的組時，可以查看與該組及其任何子組關聯的團隊，並與其協作。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 3%

---

# 建立和修改群組的團隊

在「組」區域中查看管理的組時，可以查看與該組及其任何子組關聯的團隊，並與其協作。

如果群組上有任何群組，其管理員也可以為群組執行這些動作。 Workfront管理員（適用於任何群組）也是如此。

有關擁有計畫許可證的用戶如何建立團隊的資訊，請參見 [建立團隊](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

如需Workfront管理員如何建立團隊的相關資訊，請參閱 [從「設定」區域建立團隊](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

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

## 從「組」區域查看、使用和建立組的組

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 按一下您要建立或修改團隊的群組名稱。
1. 在左側面板中，按一下 **團隊** ![](assets/teams.png) 列出與該組以及該組可能擁有的任何子組的關聯團隊。

1. 執行下列任一操作：

   * **新增團隊**:按一下 **新團隊**，然後使用下列選項進行設定：
   <!-- WRITER please check table below. I stripped out wonky conditions-->

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">團隊名稱</td> 
       <td>鍵入團隊的名稱。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">群組</td> 
       <td> <p> 系統會使用您正在查看的組填充新產品組合的「組」欄位。 如果要將團隊與其他組關聯，請開始鍵入組的名稱，然後在出現時選擇該名稱。</p> <p>您可以將游標暫留在組上並按一下資訊表徵圖，確保正確的組與組相關聯 <img src="assets/info-icon.png"> 顯示於其旁。 此工具提示會列出群組的相關資訊，例如上方的群組階層及其管理員。</p> <p><b>注意</b>:將團隊分配給組或子組時，該組或子組的任何組管理員都可以管理該團隊，而不是其成員。 群組管理員可從主功能表前往「團隊」區域，然後按一下「切換團隊」箭頭 <img src="assets/switch-team-icon.png" alt="切換團隊表徵圖"> 列出分配給其管理的組的所有團隊。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">團隊成員</td> 
       <td> <p>開始鍵入要在團隊中的用戶的名稱，然後在出現在下拉清單中時選擇名稱。 重複此過程以向團隊添加多個用戶。</p> <p>您可新增至團隊的使用者數量沒有限制。 但是，我們建議不要在一個團隊中擁有過多的用戶，因為團隊的工作管理可能變得太複雜。</p> </td> 
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
       <td>將Work On It按鈕更改為Start按鈕。 當使用者按一下「開始」時，項目的狀態會自動更新。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">完成按鈕</td> 
       <td>選擇在按一下「完成」按鈕時要為項目設定的狀態。</td> 
       </tr> 
      </tbody> 
     </table>

   * **編輯團隊**:至少選擇一個團隊，按一下 **the** 編輯圖示 ![](assets/edit-icon.png)，然後使用下列選項進行設定：

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">團隊名稱</td> 
       <td>鍵入團隊的名稱。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">群組</td> 
       <td> <p>將團隊與組關聯。 開始鍵入組的名稱，然後在出現時選擇該名稱。</p> <p>您可以將游標暫留在組上並按一下資訊表徵圖，確保正確的組與組相關聯 <img src="assets/info-icon.png"> 顯示於其旁。 此工具提示會列出群組的相關資訊，例如上方的群組階層及其管理員。</p> <p><b>注意</b>:將團隊分配給組或子組時，該組或子組的任何組管理員都可以管理該團隊，而不是其成員。 群組管理員可從主功能表前往「團隊」區域，然後按一下「切換團隊」箭頭 <img src="assets/switch-team-icon.png" alt="切換團隊表徵圖"> 列出分配給其管理的組的所有團隊。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">所有者</td> 
       <td>選擇團隊的所有者。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">團隊成員</td> 
       <td> <p>新增和團隊成員。 開始鍵入用戶的名稱，然後在出現時選擇該名稱。 重複此過程以向團隊添加多個用戶。</p> <p><b>筆尖</b>:您可新增至團隊的使用者數量沒有限制。 但是，我們建議不要在一個團隊中擁有過多的用戶，因為團隊的工作管理可能變得太複雜。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">說明</td> 
       <td>輸入團隊的說明。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">配置範本</td> 
       <td> <p>開始鍵入您希望團隊使用的佈局模板的名稱，然後在出現時按一下它。</p> <p>當您指定具有此配置模板的團隊作為「首頁用戶團隊」時，此團隊中的所有用戶將在此配置模板中看到自定義項。<br>其個別配置模板設定將覆蓋主團隊配置模板的設定。 </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">敏捷</td> 
       <td>指定這是否為敏捷團隊。 如需敏捷團隊及如何管理其工作的相關資訊，請參閱 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">建立敏捷的團隊</a>.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">處理它</td> 
       <td> <p>將Work On It按鈕更改為Start按鈕。 當使用者按一下「開始」時，項目的狀態會自動更新。</p> <p>有關如何配置「開始」按鈕的詳細資訊，請參見 <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">將「Work On It（工作完成）」按鈕替換為「Start（開始）」按鈕</a>.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">完成按鈕</td> 
       <td> <p>自訂完成按鈕。 如需詳細資訊，請參閱：</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">配置任務的完成按鈕</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">設定問題的「完成」按鈕</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **刪除團隊**:至少選擇一個團隊，然後按一下「刪除」表徵圖 ![](assets/delete.png).
   * **匯出團隊清單**:按一下 **匯出** ![](assets/export.png)，然後選取要匯出清單的檔案格式。
