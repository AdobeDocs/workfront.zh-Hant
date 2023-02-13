---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 檢視及管理群組最近刪除的項目
description: 在「組」區域中查看管理的組時，可以查看、篩選、還原和導出其最近刪除的工作項、文檔和模板。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 1%

---

# 檢視及管理群組最近刪除的項目

在「組」區域中查看管理的組時，可以通過以下方式查看和處理最近刪除的項目、任務、問題、文檔和模板：

* 檢視、篩選及分組最近刪除的項目清單
* 還原您選擇的最近刪除的項目
* 導出最近刪除的項的清單

如果群組上有任何群組，其管理員也可以為群組執行這些動作。 Workfront管理員（適用於任何群組）也是如此。

如需已刪除項目的詳細資訊，請參閱 [管理已刪除的項目](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>已刪除的項目必須與組或其任何子組相關聯。 </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 檢視及管理群組最近刪除的項目

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 按一下群組的名稱。
1. 在左側面板中，按一下 **最近刪除**.
1. 開啟下列其中一個標籤，您可以在其中檢視及管理群組最近刪除的項目：

   * 專案
   * 任務
   * 問題
   * 文件
   * 範本

   每個頁簽都列出屬於當前組或其子組、且在過去30天內被刪除的相應對象類型的項。

   >[!NOTE]
   >
   >如果某人刪除了項目，則其所有單獨任務、問題和文檔都將隨其刪除。 「任務」、「問題」、「文檔」或「模板」頁簽上不會單獨顯示這些內容。 但是，還原項目也會將所有這些子對象還原到項目中。
   >
   >
   >如果某人單獨刪除了任務、問題、文檔或模板，則可以在相應的頁簽上查看和管理它。

1. 執行下列任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>還原對象</p> </td> 
      <td> <p>選取最多10個物件，然後按一下 <strong>還原</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>導出頁簽上的整個對象清單</p> </td> 
      <td> <p>按一下 <strong>匯出</strong>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>更改清單中資訊的顯示</p> </td> 
      <td> <p>在清單上方的右上角，使用 <strong>篩選</strong> 以根據您提供的條件定義顯示的內容。 使用 <strong>檢視</strong> 定義要以列顯示的欄位。 使用 <strong>分組</strong> 將項目分組為類別。</p> </td> 
     </tr> 
    </tbody> 
   </table>
