---
title: 從「設定」區域建立團隊
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: 身為Adobe Workfront管理員，您可以從「設定」區域建立團隊。
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---

# 從「設定」區域建立團隊

身為Adobe Workfront管理員，您可以從「設定」區域建立團隊。 如需團隊的相關資訊，請參閱 [團隊概觀](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* 群組管理員可從「設定」區域為其管理的群組建立團隊。 如需詳細資訊，請參閱 [建立和修改群組的團隊](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* 擁有計畫許可證的用戶也可以從「人員」區域建立團隊。 如需詳細資訊，請參閱 [建立團隊](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
>


## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立團隊

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **團隊**，然後按一下 **新團隊**.

1. 在 **新團隊** 框中，指定以下資訊：

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
      <td> <p>如果要將團隊與組關聯，請開始鍵入組的名稱，然後在出現時選擇該名稱。</p> <p>您可以將游標暫留在組上並按一下資訊表徵圖，確保正確的組與組相關聯 <img src="assets/info-icon.png"> 顯示於其旁。 此工具提示會列出群組的相關資訊，例如上方的群組階層及其管理員。</p> <p><b>注意</b>:將團隊分配給組或子組時，該組或子組的任何組管理員都可以管理該團隊，而不是其成員。 群組管理員可從主功能表前往「團隊」區域，然後按一下「切換團隊」箭頭 <img src="assets/switch-team-icon.png" alt="切換團隊表徵圖"> 列出分配給其管理的組的所有團隊。</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">這是一個敏捷團隊</td> 
      <td>如果要將此新團隊配置為敏捷團隊，請選擇此項目。 如需敏捷團隊的詳細資訊，請參閱 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">建立敏捷的團隊</a>.</td> 
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

1. 按一下 **建立團隊**.

## 團隊擁有者

建立團隊時，預設情況下，您會成為團隊擁有者。

建立團隊的報表時，您可以檢視所有團隊的團隊擁有者，並在報表中加入「擁有者名稱」欄位。 (如需建立報表的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
