---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: 將XD工作區域作為校訂上傳至Workfront
description: 您可以將工作區域作為校訂直接上傳到Adobe Workfront以進行徹底的檢閱和核准。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 0%

---

# 將[!DNL XD]個工作區域上傳為校訂到[!DNL Workfront]

您可以將工作區域作為校訂直接上傳到[!DNL Adobe Workfront]，以進行徹底的檢閱和核准。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 封裝</td> 
   <td>任何 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>標準</p> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他產品</td> 
   <td>除了[!DNL Adobe Creative Cloud]授權之外，您還必須有[!DNL Workfront]授權。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣權限設定檔 </td> 
   <td>[!UICONTROL Manager]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>編輯[!UICONTROL 檔案]的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


+++

## 先決條件

* 您必須先安裝[!DNL Adobe Workfront for XD]外掛程式，才能在[!DNL Adobe XD]中上傳校樣。

  如需指示，請參閱[安裝 [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md)。

## 上傳靜態校樣

1. 按一下右上角的&#x200B;**[!UICONTROL 功能表]**&#x200B;圖示，然後選取&#x200B;**[!UICONTROL 工作清單]**。 您也可以使用功能表導覽至父物件。

   ![功能表圖示](assets/menu-350x440.png)

1. 前往您要上傳靜態校樣的工作專案。
1. 按一下導覽列中的&#x200B;**[!UICONTROL 檔案]**&#x200B;圖示![檔案圖示](assets/documents.png)。

1. 按一下外掛程式底部附近的&#x200B;**[!UICONTROL 新增檔案]**。
1. 選取您要上載的工作區域。

   >[!TIP]
   >
   >* 工作區域將依照其選取的順序出現在校樣中。 第一個選取的工作區域將是校訂中的第一個頁面，以此類推。
   >* 若要快速選取多個工作區域，請按一下滑鼠，並將滑鼠拖曳到您想要的工作區域上。 這不允許您控制校樣中工作區域的順序。

1. 啟用&#x200B;**[!UICONTROL 建立校訂]**。

1. 為校訂命名。

1. 選擇您想要的校訂核准型別：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]： </td> 
      <td> <p>基本核准流程是臨時性的，可以根據需要包含不同的稽核者： </p> 
       <ul> 
        <li> <p>（選擇性）在方塊中新增<strong>核准者</strong>。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 自動化]</td> 
      <td> <p>自動核准流程由管理員預先建立，並包括特定稽核者和階段。 如需詳細資訊，請參閱<a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動化工作流程總覽</a>。</p> 
       <ul> 
        <li> <p>從下拉式選單中選擇[!UICONTROL 工作流程範本]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. （選擇性）在&#x200B;**[!UICONTROL 更新]**&#x200B;區域輸入註解。

   在XD中![校訂核准](assets/proof-approvals-xd-350x396.png)

1. 從&#x200B;**[!UICONTROL 資產型別]**&#x200B;下拉式功能表中選擇匯出格式。


1. （選擇性）如果您選取PDF作為資產型別，且已選取多個工作區域，請選擇您要將工作區域匯出為&#x200B;**[!UICONTROL 單一PDF檔案]s**&#x200B;或&#x200B;**M[!UICONTROL 多個PDF檔案]**。

1. （選用）為PDF命名。

   ![PDF選項](assets/pdf-options.png)

1. 按一下&#x200B;**[!UICONTROL 上傳]**。\
   檔案會顯示在外掛程式與案頭應用程式的[!UICONTROL 檔案]區域中。

## 上傳互動式校樣 {#upload-an-interactive-proof}

您可以使用[!DNL Workfront for Adobe]外掛程式，為您的工作區域建立互動式校樣。 此程式分為兩個步驟。 首先您需要建立互動式連結，然後您需要將校樣上傳到工作專案。

### 為您的工作區域建立互動式連結  {#create-an-interactive-link-for-your-art-board}

1. 開啟工作畫板，然後按一下畫面左上方區域中的&#x200B;**[!UICONTROL 共用]**。
1. 指定連結設定：

   1. 為連結命名。
   1. 選擇檢視設定。
   1. 在&#x200B;**[!UICONTROL 連結存取]**&#x200B;區段中，確定已選取&#x200B;**[!UICONTROL 擁有此連結的任何人]**。

      您必須啟用這類存取權才能產生互動式校樣。

   1. 按一下&#x200B;**[!UICONTROL 建立連結]**。

1. 按一下回到畫面左上方區域中的&#x200B;**[!UICONTROL 設計]**。 繼續前往下方的[上傳互動式校訂](#upload-an-interactive-proof)區段。

   >[!NOTE]
   >
   >您可能需要重新開啟畫面左下角的外掛程式面板。

### 上傳互動式校樣

1. 按一下右上角的&#x200B;**[!UICONTROL 功能表]**&#x200B;圖示，然後選取&#x200B;**[!UICONTROL 工作清單]**。 您也可以使用功能表導覽至父物件。

   ![功能表圖示](assets/menu-350x440.png)

1. 前往您要上傳互動式校樣的工作專案。
1. 按一下導覽列中的&#x200B;**[!UICONTROL 檔案]**&#x200B;圖示![檔案圖示](assets/documents.png)。

1. 按一下外掛程式底部附近的&#x200B;**[!UICONTROL 新增檔案]**。
1. 啟用&#x200B;**[!UICONTROL 建立校訂]**。

1. 選擇您想要的校訂核准型別：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]： </td> 
      <td> <p>基本核准流程是臨時性的，可以根據需要包含不同的稽核者： </p> 
       <ul> 
        <li> <p>（選擇性）在方塊中新增<strong>核准者</strong>。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 自動化]</td> 
      <td> <p>自動核准流程由管理員預先建立，並包括特定稽核者和階段。 如需詳細資訊，請參閱<a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動化工作流程總覽</a>。</p> 
       <ul> 
        <li> <p>從下拉式選單中選擇[!UICONTROL 工作流程範本]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. （選擇性）在&#x200B;**[!UICONTROL 更新]**&#x200B;區域輸入註解。

   在XD中![校訂核准](assets/proof-approvals-xd-350x396.png)

1. 在&#x200B;**[!UICONTROL 資產型別]**&#x200B;下拉式功能表中，選擇您剛才在&#x200B;**共用連結**&#x200B;標籤下建立的連結。 如需詳細資訊，請參閱[為您的工作區域建立互動式連結](#create-an-interactive-link-for-your-artboard)。\
   在XDS![中](assets/shared-links-xd-350x870.png)個共用連結

1. 按一下&#x200B;**[!UICONTROL 上傳]**。

   檔案會顯示在外掛程式與案頭應用程式的[!UICONTROL 檔案]區域中。

   >[!IMPORTANT]
   >
   >使用者必須擁有[!UICONTROL 案頭校訂檢視器]的存取權，才能檢閱及核准互動式校訂。 如需詳細資訊，請參閱[安裝[!UICONTROL 案頭校訂檢視器]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md)。

## 上傳新的校訂版本

您可以上傳新版本的校訂。 外掛程式會記住先前版本上設定的校訂工作流程，但您可以視需要變更此設定。

1. 按一下右上角的&#x200B;**[!UICONTROL 功能表]**&#x200B;圖示，然後選取&#x200B;**[!UICONTROL 工作清單]**。 您也可以使用功能表導覽至父物件。

   ![功能表圖示](assets/menu-350x440.png)

1. 前往上載檔案所需的工作專案。
1. 按一下導覽列中的&#x200B;**[!UICONTROL 檔案]**&#x200B;圖示![檔案圖示](assets/documents.png)。

1. 按一下外掛程式底部附近的&#x200B;**[!UICONTROL 新版本]**。
1. 啟用&#x200B;**[!UICONTROL 建立校訂]**。
1. 選取您要上載的工作區域。

   >[!NOTE]
   >
   >如果您想要上傳.svg、.png或.jpg的新版本，只能上傳一個工作畫板。

1. 選擇您想要的校訂核准型別：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic]： </td> 
      <td> <p>基本核准流程是臨時性的，可以根據需要包含不同的稽核者： </p> 
       <ul> 
        <li> <p>（選擇性）在方塊中新增<strong>核准者</strong>。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 自動化]</td> 
      <td> <p>自動核准流程由管理員預先建立，並包括特定稽核者和階段。 如需詳細資訊，請參閱<a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動化工作流程總覽</a>。</p> 
       <ul> 
        <li> <p>從下拉式選單中選擇[!UICONTROL 工作流程範本]。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. 從&#x200B;**[!UICONTROL 資產型別]**&#x200B;下拉式功能表中選擇匯出格式。

   ![在XD中建立校訂](assets/create-a-proof-xd-350x202.png)

1. （選擇性）在&#x200B;**[!UICONTROL 更新]**&#x200B;區域輸入註解。

   在XD中![校訂核准](assets/proof-approvals-xd-350x396.png)

1. （選擇性）如果您選取PDF作為資產型別，且已選取多個工作區域，請選擇您要將工作區域匯出為&#x200B;**[!UICONTROL 單一PDF檔案]s**&#x200B;或&#x200B;**M[!UICONTROL 多個PDF檔案]**。

1. （選用）為PDF命名。

   PDF選項

1. 按一下&#x200B;**[!UICONTROL 上傳]**。\
   檔案會顯示在外掛程式與案頭應用程式的[!UICONTROL 檔案]區域中。
