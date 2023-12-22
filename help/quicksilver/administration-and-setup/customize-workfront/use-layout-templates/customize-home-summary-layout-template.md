---
title: 使用版面配置範本自訂首頁和摘要
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 您可以使用版面配置範本來設定當使用者按一下首頁和摘要中的任務或問題時會看到的內容。 您使用下列步驟進行的每個設定都會以相同方式影響「首頁」區域和「摘要」面板。 這些自訂不適用於「檔案摘要」面板。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: abaabf12d63ea1e279d14ad8467ac239e6c211b1
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 2%

---

# 使用版面配置範本自訂首頁和摘要

您可以使用版面配置範本來設定當使用者按一下首頁和摘要中的任務或問題時會看到的內容。 您使用下列步驟進行的每個設定都會以相同方式影響「首頁」區域和「摘要」面板。 這些自訂不適用於「檔案摘要」面板。

您可以設定：

* 詳細資訊區域中針對任務或問題顯示哪些欄位，以及按照什麼順序
* 所選任務或問題的更新、記錄時間、附加檔案和時間戳記是否顯示

您也可以自訂當使用者按一下指派給他們的專案核准、檔案核准或檔案版本核準時，使用者在「首頁」區域中看到的欄位。

如需有關「首頁」區域的資訊，請參閱 [使用首頁區域](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). 如需「摘要」面板的相關資訊，請參閱 [摘要概觀](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

如需有關建立版面配置範本的資訊，請參閱 [建立及管理版面範本](../use-layout-templates/create-and-manage-layout-templates.md).

如需有關群組版面配置範本的資訊，請參閱 [建立和修改群組的版面配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

配置版面範本後，您必須將其指派給使用者，才能讓其他人看到您所做的變更。 如需有關指派配置範本給使用者的資訊，請參閱 [將使用者指派至版面配置範本](../use-layout-templates/assign-users-to-layout-template.md).

## 存取需求

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
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。
若要為群組執行這些動作，您必須是該群組的管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用版面配置範本自訂首頁和摘要

1. 開始使用版面範本，如所述 [建立及管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. 按一下向下箭頭 ![](assets/dropdown-arrow.png) 在 **自訂使用者看到的內容**，然後按一下 **首頁和摘要**.

1. 在左側顯示的清單中，按一下物件型別(**任務**， **問題**， **專案**， **檔案**，或 **檔案版本**)中選取要自訂的「首頁」和「摘要」。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">任務</td> 
      <td> <p>在首頁中，此設定的組態會影響使用者按一下任務時任務右側的區域。 此外，在任務清單中，它會影響當使用者選擇任務，然後按一下「開啟摘要」圖示時顯示在頁面右側的「摘要」面板 <img src="assets/summary-panel-icon.png">.</p> <p>例如，您可以決定當使用者在首頁中選擇任務時，使用者在詳細資訊區域中會看到哪些欄位：</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>當他們在摘要中選取任務時：</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">問題</td> 
      <td> <p>在首頁中，您對此設定的設定會影響使用者點按問題右側的區域。</p> <p>在問題清單中，此設定會影響當使用者選擇問題，然後按一下「開啟摘要」圖示時顯示在頁面右側的「摘要」面板 <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">專案</td> 
      <td>在首頁中，當使用者按一下指派給他們的專案核準時，此設定的設定會影響核准右側的區域。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">文件</td> 
      <td>在首頁中，當使用者按一下指派給他們的檔案核準時，您對此設定的設定會影響核准右側的區域。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">文件版本</td> 
      <td>在首頁中，當使用者按一下指派給他們用於特定檔案版本的核準時，您對此設定的設定會影響核准右側的區域。</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >如果未指派任務，則指派給版面配置範本的使用者將不會在「摘要」中看到欄位自訂。

1. （視條件而定）如果您在上一步中按一下任務或問題，請選取您要自訂的任務或問題類別。

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. （視條件而定）如果 **設定主要動作按鈕** 下拉式選單出現(如果您選取 **任務** 或 **問題** 在左側的清單中)，按一下主要動作(**完成** 或 **狀態**)可供使用者在首頁區域及摘要面板中檢視任務或問題時使用。

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. 新增 ![](assets/add-item-plus-in-circle-blue.png) 或隱藏 ![](assets/close-or-hide---x.png) 所選物件型別的欄位。

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. 重複步驟3-6以自訂任何其他物件型別的「首頁」區域和「摘要」面板。
1. 按一下 **全域設定**，然後在首頁和摘要中啟用或停用與Adobe Workfront物件相關的下列任何選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">顯示工作的更新</td> 
      <td>在首頁或摘要中顯示對所選任務或問題所做的任何更新。 這包括系統更新和使用者所做的更新。 使用者仍然可以篩選掉系統更新，如中所述 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">啟用或停用系統更新</a> 在 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">針對工作記錄時間</td> 
      <td>當選取任務或問題時，顯示「針對工作記錄時間」選項，可讓使用者直接從「首頁」和「摘要」區域記錄工作專案的時間。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">檢視與工作相關的檔案</td> 
      <td>選擇任務或問題時在「首頁」和「摘要」中顯示「檔案」區域，列出附加到任務或問題的任何檔案。 使用者可以按一下檔案，在預覽視窗中檢視檔案。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隱藏時間戳記</td> 
      <td>在「首頁」和「摘要」中隱藏下列日期欄位的時間戳記：
       <ul>
        <li>規劃完成日期</li>
        <li>認可日期</li>
        <li>提交日期</li>
       </ul><p><b>注意</b>：啟用此選項後，過期的工作專案只會根據日期（而非時間）移至「首頁工作清單」的「延遲」分組。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下 **儲存**.

如需版面配置範本的詳細資訊，請參閱 [建立及管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
