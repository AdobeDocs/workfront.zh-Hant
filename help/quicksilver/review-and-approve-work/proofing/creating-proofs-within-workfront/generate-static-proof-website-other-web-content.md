---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 為網站或其他網路內容建立靜態校樣
description: 您可以為網頁內容產生新的靜態校樣或現有靜態校樣的新版本。 網路內容可以包括諸如具有流視頻、HTML動畫或互動式橫幅的廣告，但它將被切成多個螢幕截圖，以便進行靜態校樣。
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# 為網站或其他網路內容建立靜態校樣

您可以為網頁內容產生新的靜態校樣或現有靜態校樣的新版本。 網路內容可以包括諸如具有流視頻、HTML動畫或互動式橫幅的廣告，但它將被切成多個螢幕截圖，以便進行靜態校樣。

為網站或其他網路內容建立靜態校樣時，請考量下列事項：

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Select或Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>管理員或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 為網站或其他網路內容建立靜態校樣

若要建立靜態校樣，網站必須可公開存取（而非防火牆後），或貴組織的允許清單必須包含Workfront網域。 Workfront無法將受密碼保護的網站擷取為靜態校樣。

>[!TIP]
>
>對於需要授權和受密碼保護的內部頁面，建議進行互動式校對，而非靜態校對。 如需詳細資訊，請參閱 [互動式內容校樣概觀](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. 前往您要建立新網站校樣或現有網站的新版本的專案、工作或問題。
1. 按一下 **檔案** 中。
1. （條件性）如果要建立新校樣，請按一下 **新增**，然後按一下 **校樣** 中。
1. （條件性）如果您要建立現有校樣的新版本：

   1. 將滑鼠移至您要建立新版本的URL校樣上，然後按一下其周圍淺藍色背景中的，以選取它。

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. 按一下 **新增** > **版本** > **校樣**.

1. 在 **新增檔案** 區域，然後按 **輸入**.

   URL會顯示在您輸入該URL的方塊下方。

   ![](assets/url-name-appears-below-350x142.png)

1. 按一下您新增的URL。

   隨即顯示設定網站校樣的選項。

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. （選用）如果您想要將校樣名稱從網站URL變更為其他名稱，請輸入 **校樣名稱。**
1. 請確定 **擷取螢幕擷圖** ，並使用下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>螢幕截圖解析度</strong> </td> 
      <td> <p>審核者檢視校樣時，可調整內容的解析度，讓他們看到內容在各種大小的裝置（例如手機、平板電腦和顯示器）上的顯示方式。</p> <p>如果您選取多個解析度，則會針對您選取的每個解析度建立個別的校樣。</p> <p>注意：當審閱者對校樣發表評論時，評論包括顯示評論發表時間的解析度，以便其他審閱者知道與評論相關聯的解析度。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>尋找子頁面</strong> </td> 
      <td> <p>擷取網站的子頁面及其主要頁面。 您可以按一下「全部選取」以包含所有頁面，或只按一下您要包含的特定頁面。 加號和減號按鈕可讓您展開和關閉網站中的子頁面區域。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >您無法更改您建立的校樣的任何後續版本的Capture螢幕截圖設定。

1. 按一下 **完成**.

   如果您在步驟8中選取了多個螢幕擷取解析度，清單會包含一組各解析度的螢幕擷取畫面。 您可以以個別校樣產生這些螢幕擷取畫面，或將它們合併成單一校樣（請參閱中的）。 建議您合併這些範本，尤其是當您要建立靜態網站校樣時。

   >[!NOTE]
   >
   >如果您要將新版本新增至現有的URL校樣，在原始校樣或舊版上設定的任何選項都會保留在此版本中。

1. 按一下 **建立校樣** 建立簡單校樣，而不需進行審核程式。\
   或\
   繼續操作，方法是配置高級校樣：

   * [使用基本工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自動化工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
