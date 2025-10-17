---
title: 從設定區域編輯團隊的設定
description: 作為Adobe Workfront管理員，您可以從設定區域編輯團隊設定。 您可以將使用者新增至專案團隊、設定專案團隊的版面配置範本，以及設定當專案團隊完成工作專案時如何記錄狀態。
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 4%

---

# 從設定區域編輯團隊的設定

作為Adobe Workfront管理員，您可以從設定區域編輯團隊設定。 您可以將使用者新增至專案團隊、設定專案團隊的版面配置範本，以及設定當專案團隊完成工作專案時如何記錄狀態。

如需有關團隊的資訊，請參閱[團隊概觀](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md)。

>[!NOTE]
>
>* 群組管理員可以編輯團隊對其所管理之群組的設定。 如需詳細資訊，請參閱[建立和修改群組的團隊](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)。
>* 擁有Standard或Plan授權的使用者可以從團隊區域編輯團隊的設定。 如需詳細資訊，請參閱[編輯團隊設定](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)。

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
   <td>[！UICONTROL系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 編輯團隊的設定

{{step-1-to-setup}}

1. 按一下左側面板中的&#x200B;**團隊**。
1. 選取團隊，然後按一下&#x200B;**編輯** ![編輯圖示](assets/edit-icon.png)。

1. 進行下列任一變更：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">團隊名稱</td> 
      <td>輸入團隊的名稱。</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">為作用中 </td> 
       <td>依預設，新團隊和現有團隊都會啟用此選項。 停用它以停用團隊。 如需詳細資訊，請參閱<a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">停用團隊</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">群組</td> 
      <td> <p>將團隊與群組建立關聯。 開始輸入群組的名稱，然後在其出現時選取名稱。</p> <p><b>注意</b>：將團隊指派給群組或子群組時，該群組或子群組的任何群組管理員都可以管理團隊，而無需成為其成員。 群組管理員可以從主功能表前往團隊區域，然後按一下「切換團隊」箭頭<img src="assets/switch-team-icon.png" alt="切換群組圖示">以列出指派給其管理群組的所有團隊。</p> <p>您可以暫留在正確的群組上，並按一下旁邊顯示的資訊圖示<img src="assets/info-icon.png">，確定您要將正確的群組與團隊建立關聯。 這會顯示工具提示，列出群組的相關資訊，例如群組及其管理員上方的群組階層。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有者</td> 
      <td>選取團隊的擁有者。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">團隊成員</td> 
      <td> <p>新增和團隊成員。 開始輸入使用者的名稱，然後在其出現時選取名稱。 重複此程式，將多位使用者新增至團隊。</p> 
      <p><b>秘訣</b>：您可以新增任意數目的使用者至團隊。 不過，我們建議您不要在一個團隊中新增過多數字，因為團隊的工作管理可能變得過於複雜。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>輸入團隊的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">版面配置範本</td> 
      <td> <p>開始輸入您希望團隊使用的版面配置範本名稱，然後在其出現時按一下它。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">敏捷</td> 
      <td>指定這是否為敏捷團隊。 有關敏捷團隊以及如何管理其工作的資訊，請參閱<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">建立敏捷團隊</a>。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
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

1. 按一下「**儲存變更**」。
