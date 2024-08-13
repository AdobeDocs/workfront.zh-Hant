---
title: 從設定區域建立團隊
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: 作為Adobe Workfront管理員，您可以從設定區域建立團隊。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 4%

---

# 從設定區域建立團隊

作為Adobe Workfront管理員，您可以從設定區域建立團隊。 如需有關團隊的資訊，請參閱[團隊概觀](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md)。

>[!NOTE]
>
>* 群組管理員可以從「設定」區域為所管理的群組建立群組。 如需詳細資訊，請參閱[建立和修改群組的團隊](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)。
>* 擁有「計畫」授權的使用者也可以從「人員」區域建立團隊。 如需詳細資訊，請參閱[建立團隊](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)。
>

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
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 建立團隊

{{step-1-to-setup}}

1. 按一下&#x200B;**團隊**，然後按一下&#x200B;**新增團隊**。

1. 在顯示的&#x200B;**新團隊**&#x200B;方塊中，指定下列資訊：

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
      <td> <p>如果要將專案團隊與群組相關聯，請開始輸入群組的名稱，然後在其出現時選取名稱。</p> <p>您可以暫留在正確的群組上，並按一下旁邊顯示的資訊圖示<img src="assets/info-icon.png">，確定您要將正確的群組與團隊建立關聯。 這會顯示工具提示，列出群組的相關資訊，例如群組及其管理員上方的群組階層。</p> <p><b>注意</b>：將團隊指派給群組或子群組時，該群組或子群組的任何群組管理員都可以管理團隊，而無需成為其成員。 群組管理員可以從主功能表前往團隊區域，然後按一下「切換團隊」箭頭<img src="assets/switch-team-icon.png" alt="切換群組圖示">以列出指派給其管理群組的所有團隊。</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">這是一個敏捷團隊</td> 
      <td>如果您想要將此新團隊設定為敏捷團隊，請選取此專案。 如需敏捷團隊的詳細資訊，請參閱<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">建立敏捷團隊</a>。</td> 
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

1. 按一下&#x200B;**建立團隊**。

## 團隊擁有者

建立團隊時，預設會成為團隊擁有者。

當您建立專案團隊的報告時，可以檢視所有專案團隊的專案團隊擁有者，並在報告中包含「擁有者名稱」欄位。 （如需建立報告的詳細資訊，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。）
