---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: 將XD畫板上傳為校樣至Workfront
description: 您可以將畫板作為校樣直接上傳至Adobe Workfront，以進行徹底的審核和核准。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: d0afdfc7be9177f6ff45dcc247253faa9dc57967
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 上傳 [!DNL XD] 將畫板作為校樣 [!DNL Workfront]

您可以將畫板作為校樣直接上傳至 [!DNL Adobe Workfront] 進行徹底的審查和批准。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>當前計畫：[!UICONTROL Pro]或更高版本</p> <p>或</p> <p>舊計畫：[!UICONTROL Premium]</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>當前計畫：[!UICONTROL工作]或[!UICONTROL校樣]</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您必須有 [!DNL Adobe Creative Cloud] 除了 [!DNL Workfront] 授權。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>[!UICONTROL Manager]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>編輯對[!UICONTROL文檔]的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請連絡您的 [!DNL Workfront] 或 [!DNL Workfront Proof] 管理員。

## 必要條件

* 您必須安裝 [!DNL Adobe Workfront for XD] 外掛程式，您才能在中上傳校樣 [!DNL Adobe XD].

   如需指示，請參閱 [安裝 [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## 上傳靜態校樣

1. 按一下 **[!UICONTROL 功能表]** 圖示，然後選取 **[!UICONTROL 工作清單]**. 您也可以使用功能表導覽至上層物件。

   ![](assets/menu-350x440.png)

1. 前往您要上傳靜態校樣的工作項目。
1. 按一下 **[!UICONTROL 檔案]** 圖示 ![](assets/documents.png) 的下一頁。

1. 按一下 **[!UICONTROL 新檔案]** 在外掛程式底部附近。
1. 選取您要上傳的畫板。

   >[!TIP]
   >
   >要選擇多個畫板，請按一下並將滑鼠拖動到所需畫板上。

1. 啟用 **[!UICONTROL 建立校樣]**.

1. 為校樣命名。

1. 選擇所需的校樣批准類型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>基本的核准程式是隨選的，可視需要包含不同的審核者： </p> 
       <ul> 
        <li> <p>（可選）新增 <strong>批准者</strong> 框中。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>管理員預先建立自動化的核准程式，並包含特定的審核者和階段。 如需詳細資訊，請參閱 <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動化工作流程概觀</a>.</p> 
       <ul> 
        <li> <p>從下拉菜單中選擇[!UICONTROL工作流模板]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. （選用）在 **[!UICONTROL 更新]** 的上界。

   ![](assets/proof-approvals-xd-350x396.png)

1. 從 **[!UICONTROL 資產類型]** 下拉式功能表。


1. （可選）如果您選取「PDF」作為資產類型，並選取了多個畫板，請選擇您是否要將畫板匯出為 **[!UICONTROL 單一PDF檔案]s** 或 **M[!UICONTROL 多個PDF檔案]**.

1. （選用）為PDF命名。

   ![](assets/pdf-options.png)

1. 按一下 **[!UICONTROL 上傳]**.\
   文檔將出現在 [!UICONTROL 檔案] 區域。

## 上傳互動式校樣 {#upload-an-interactive-proof}

您可以使用 [!DNL Workfront for Adobe] 外掛程式。 這是兩步驟的程式。 首先，您需要建立互動式連結，然後需要將校樣上傳至工作項目。

### 為畫板建立互動式連結  {#create-an-interactive-link-for-your-art-board}

1. 開啟畫板，然後按一下 **[!UICONTROL 共用]** 在畫面的左上角。
1. 指定連結設定：

   1. 為連結命名。
   1. 選擇視圖設定。
   1. 在 **[!UICONTROL 連結存取]** 小節，確保 **[!UICONTROL 任何具有此連結的人]** 中所有規則的URL。

      您必須啟用此類型的存取，才能產生互動式校樣。

   1. 按一下 **[!UICONTROL 建立連結]**.

1. 按一下返回 **[!UICONTROL 設計]** 在畫面的左上角。 繼續 [上傳互動式校樣](#upload-an-interactive-proof) 一節。

   >[!NOTE]
   >
   >您可能需要在畫面左下角重新開啟外掛程式面板。

### 上傳互動式校樣

1. 按一下 **[!UICONTROL 功能表]** 圖示，然後選取 **[!UICONTROL 工作清單]**. 您也可以使用功能表導覽至上層物件。

   ![](assets/menu-350x440.png)

1. 前往您要上傳互動式校樣的工作項目。
1. 按一下 **[!UICONTROL 檔案]** 圖示 ![](assets/documents.png) 的下一頁。

1. 按一下 **[!UICONTROL 新檔案]** 在外掛程式底部附近。
1. 啟用 **[!UICONTROL 建立校樣]**.

1. 選擇所需的校樣批准類型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>基本的核准程式是隨選的，可視需要包含不同的審核者： </p> 
       <ul> 
        <li> <p>（可選）新增 <strong>批准者</strong> 框中。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>管理員預先建立自動化的核准程式，並包含特定的審核者和階段。 如需詳細資訊，請參閱 <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動化工作流程概觀</a>.</p> 
       <ul> 
        <li> <p>從下拉菜單中選擇[!UICONTROL工作流模板]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. （選用）在 **[!UICONTROL 更新]** 的上界。

   ![](assets/proof-approvals-xd-350x396.png)

1. 在 **[!UICONTROL 資產類型]** 下拉式選單中，選取您剛在 **共用連結** 標籤。 如需詳細資訊，請參閱 [為畫板建立互動式連結](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. 按一下 **[!UICONTROL 上傳]**.

   文檔將出現在 [!UICONTROL 檔案] 區域。

   >[!IMPORTANT]
   >
   >使用者必須擁有 [!UICONTROL 案頭校對檢視器] 來檢閱和核准互動式校樣。 如需詳細資訊，[請安裝[!UICONTROL 桌面校訂檢視器]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md)。

## 上傳新校樣版本

您可以上傳新版校樣。 外掛程式會記住先前版本上設定的校對工作流程，但您可視需要加以變更。

1. 按一下 **[!UICONTROL 功能表]** 圖示，然後選取 **[!UICONTROL 工作清單]**. 您也可以使用功能表導覽至上層物件。

   ![](assets/menu-350x440.png)

1. 轉至要將文檔上載到的工作項。
1. 按一下 **[!UICONTROL 檔案]** 圖示 ![](assets/documents.png)的下一頁。

1. 按一下 **[!UICONTROL 新版本]** 在外掛程式底部附近。
1. 啟用 **[!UICONTROL 建立校樣]**.
1. 選取您要上傳的畫板。

   >[!NOTE]
   >
   >如果要上傳.svg、.png或.jpg的新版本，則只能上傳一個畫板。

1. 選擇所需的校樣批准類型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]: </td> 
      <td> <p>基本的核准程式是隨選的，可視需要包含不同的審核者： </p> 
       <ul> 
        <li> <p>（可選）新增 <strong>批准者</strong> 框中。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automated]</td> 
      <td> <p>管理員預先建立自動化的核准程式，並包含特定的審核者和階段。 如需詳細資訊，請參閱 <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動化工作流程概觀</a>.</p> 
       <ul> 
        <li> <p>從下拉菜單中選擇[!UICONTROL工作流模板]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. 從 **[!UICONTROL 資產類型]** 下拉式功能表。

   ![](assets/create-a-proof-xd-350x202.png)

1. （選用）在 **[!UICONTROL 更新]** 的上界。

   ![](assets/proof-approvals-xd-350x396.png)

1. （可選）如果您選取「PDF」作為資產類型，並選取了多個畫板，請選擇您是否要將畫板匯出為 **[!UICONTROL 單一PDF檔案]s** 或 **M[!UICONTROL 多個PDF檔案]**.

1. （選用）為PDF命名。

   ![](assets/pdf-options.png)

1. 按一下 **[!UICONTROL 上傳]**.\
   文檔將出現在 [!UICONTROL 檔案] 區域。
