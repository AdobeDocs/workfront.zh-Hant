---
title: 使用版面範本自訂首頁和摘要
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 您可以使用配置模板配置用戶在首頁和摘要中按一下任務或問題時看到的內容。 您使用下列步驟進行的每個配置都會以相同的方式影響「首頁」區域和「摘要」面板。 這些自定義項不適用於「文檔摘要」面板。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 2%

---

# 使用版面範本自訂首頁和摘要

您可以使用配置模板配置用戶在首頁和摘要中按一下任務或問題時看到的內容。 您使用下列步驟進行的每個配置都會以相同的方式影響「首頁」區域和「摘要」面板。 這些自定義項不適用於「文檔摘要」面板。

您可以設定：

* 在「詳細資訊」區域中會針對任務或問題顯示哪些欄位，以及順序
* 是否顯示選定任務或問題的更新、記錄時間、附加文檔和時間戳

當用戶按一下分配給他們的項目批准、文檔批准或文檔版本批准時，您還可以自定義用戶在「首頁」區域中看到的欄位。

有關「首頁」區域的資訊，請參閱 [使用首頁區域](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). 有關「摘要」面板的資訊，請參閱 [摘要概觀](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

如需群組版面範本的相關資訊，請參閱 [建立和修改群組的版面範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td> <p>要在系統級別執行這些步驟，需要系統管理員訪問級別。
要為組執行這些操作，您必須是該組的經理。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用版面範本自訂首頁和摘要

1. 開始使用版面範本，如 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. 按一下向下箭頭 ![](assets/dropdown-arrow.png) 在 **自訂使用者看見的項目**，然後按一下 **首頁和摘要**.

1. 在左側顯示的清單中，按一下物件類型(**工作**, **問題**, **專案**, **檔案**，或 **文檔版本**)，以便在首頁和摘要中自訂。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">任務</td> 
      <td> <p>在「首頁」中，用戶按一下任務時，此設定的配置會影響任務右側的區域。 而且，在任務清單中，它會影響當用戶選擇任務，然後按一下「開啟摘要」表徵圖時顯示在頁面右側的「摘要」面板 <img src="assets/summary-panel-icon.png">.</p> <p>例如，當使用者在「首頁」中選取任務時，您可以決定使用者在「詳細資訊」區域中看到的欄位：</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>當他們在「摘要」中選擇任務時：</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">問題</td> 
      <td> <p>在「首頁」中，使用者點按問題時，此設定的設定會影響問題右側的區域。</p> <p>在問題清單中，此設定會影響「摘要」面板，當使用者選取問題，然後按一下「開啟摘要」圖示時，該面板會顯示在頁面右側 <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">專案</td> 
      <td>在「首頁」中，當用戶按一下分配給他們的項目批准時，您對此設定的配置會影響批准右側的區域。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">文件</td> 
      <td>在「首頁」中，當用戶按一下分配給他們的文檔批准時，您為此設定的配置會影響批准右側的區域。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">文件版本</td> 
      <td>在「首頁」中，當用戶按一下為特定版本的文檔分配給他們的批准時，您針對此設定的配置會影響批准右側的區域。</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >如果未分配任務，則分配給佈局模板的用戶將不會在「摘要」中看到欄位自定義。

1. （條件性）如果您按一下上一步中的「任務」或「問題」，請選取要自訂的任務或問題類別。

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. （條件性）若 **設定主要動作按鈕** 下拉式功能表(若您選取 **工作** 或 **問題** 在左側的清單中)，按一下主要動作(**完成** 或 **狀態**)，讓使用者檢視工作或問題時，可在首頁區域和摘要面板中使用。

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. 新增 ![](assets/add-item-plus-in-circle-blue.png) 或隱藏 ![](assets/close-or-hide---x.png) 欄位。

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. 重複步驟3-6，對任何其他對象類型自定義「首頁」區域和「摘要」面板。
1. 按一下 **全域設定**，靠近左下角，然後啟用或停用「首頁」和「摘要」中與Adobe Workfront物件相關的下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">顯示工作的更新</td> 
      <td>在「首頁」或「摘要」中顯示對選定任務或問題所做的任何更新。 這包括使用者進行的系統更新和更新。 用戶仍可以篩選系統更新，如 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">啟用或禁用系統更新</a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">針對工作記錄時間</td> 
      <td>選擇任務或問題時顯示「根據工作記錄時間」選項，允許用戶直接從「首頁」和「摘要」區域登錄工作項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">查看與工作關聯的文檔</td> 
      <td>選擇任務或問題時，在「首頁」和「摘要」中顯示「文檔」區域，列出附加到任務或問題的任何文檔。 用戶可以按一下文檔，在預覽窗口中查看它們。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隱藏時間戳記</td> 
      <td>隱藏「首頁」和「摘要」中以下日期欄位的時間戳記：
       <ul>
        <li>計畫完成日期</li>
        <li>認可日期</li>
        <li><p>提交日期</p></li>
       </ul><p><b>注意</b>:啟用此選項後，過期的工作項將僅根據日期而非時間移到「主工作清單」中的「延遲」分組。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 繼續自訂配置範本。

   或

   如果您已完成自訂，請按一下 **儲存**.

如需版面範本的詳細資訊，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
