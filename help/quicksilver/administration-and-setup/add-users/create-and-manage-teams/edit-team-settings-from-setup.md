---
title: 從「設定」區域編輯團隊的設定
description: 身為Adobe Workfront管理員，您可以從「設定」區域編輯團隊的設定。 您可以向團隊添加用戶、設定團隊的佈局模板，以及在團隊完成工作項目時設定狀態的記錄方式。
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 3%

---

# 從「設定」區域編輯團隊的設定

身為Adobe Workfront管理員，您可以從「設定」區域編輯團隊的設定。 您可以向團隊添加用戶、設定團隊的佈局模板，以及在團隊完成工作項目時設定狀態的記錄方式。

如需團隊的相關資訊，請參閱 [團隊概觀](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* 群組管理員可以編輯所管理群組的團隊設定。 如需詳細資訊，請參閱 [建立和修改群組的團隊](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* 具有計畫許可證的用戶可以從「人員」區域編輯團隊的設定。 如需詳細資訊，請參閱 [編輯團隊設定](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
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

## 編輯團隊的設定

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **團隊** 中。
1. 選取團隊，然後按一下 **編輯** ![](assets/edit-icon.png).

1. 進行下列任一變更：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">團隊名稱</td> 
      <td>鍵入團隊的名稱。</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">活動 </td> 
       <td>依預設，會為新團隊和現有團隊啟用此選項。 禁用它以停用團隊。 如需詳細資訊，請參閱 <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">停用團隊</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">群組</td> 
      <td> <p>將團隊與組關聯。 開始鍵入組的名稱，然後在出現時選擇該名稱。</p> <p><b>注意</b>:將團隊分配給組或子組時，該組或子組的任何組管理員都可以管理該團隊，而不是其成員。 群組管理員可從主功能表前往「團隊」區域，然後按一下「切換團隊」箭頭 <img src="assets/switch-team-icon.png" alt="切換團隊表徵圖"> 列出分配給其管理的組的所有團隊。</p> <p>您可以將游標暫留在組上並按一下資訊表徵圖，確保正確的組與組相關聯 <img src="assets/info-icon.png"> 顯示於其旁。 此工具提示會列出群組的相關資訊，例如上方的群組階層及其管理員。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有者</td> 
      <td>選擇團隊的所有者。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">團隊成員</td> 
      <td> <p>新增和團隊成員。 開始鍵入用戶的名稱，然後在出現時選擇該名稱。 重複此過程以向團隊添加多個用戶。</p> 
      <p><b>筆尖</b>:您可以新增任意數量的使用者至團隊。 不過，我們建議您不要在一個團隊中新增過多數量，因為團隊的工作管理可能會變得太複雜。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>輸入團隊的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">配置範本</td> 
      <td> <p>開始鍵入您希望團隊使用的佈局模板的名稱，然後在出現時按一下它。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">敏捷</td> 
      <td>指定這是否為敏捷團隊。 如需敏捷團隊及如何管理其工作的相關資訊，請參閱 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">建立敏捷的團隊</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
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

1. 按一下 **儲存變更**.
