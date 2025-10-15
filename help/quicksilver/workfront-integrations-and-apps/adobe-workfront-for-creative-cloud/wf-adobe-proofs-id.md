---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: 從InDesign上傳校樣
description: 您可以將圖片展示板上傳為檔案，以快速檢閱和核准，或直接儲存至Adobe Workfront。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: ee3dc446-6886-4285-a942-4f44f5c0ac31
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# 從[!DNL InDesign]上傳校樣

您可以將藝術版面板直接上傳到[!DNL Adobe Workfront]作為校訂，以進行徹底的檢閱和核准。

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
   <td>[！UICONTROL Manager]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>編輯[！UICONTROL檔案]的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


+++

## 先決條件

* 您必須先安裝[!DNL Adobe Workfront for design and video]外掛程式，才能從[!DNL InDesign]上傳校樣。

  如需指示，請參閱[安裝 [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md)。

## 上傳基本校訂

1. 按一下右上角的&#x200B;**[!UICONTROL 功能表]**&#x200B;圖示，然後選取&#x200B;**[!UICONTROL 工作清單]**。 您也可以使用功能表導覽至父物件。

   ![返回工作清單](assets/go-back-to-work-list-350x314.png)

1. 前往您要上傳校樣的工作專案。
1. 按一下導覽列中的&#x200B;**[!UICONTROL 檔案]**&#x200B;圖示![檔案圖示](assets/documents.png)。
1. 按一下外掛程式底部附近的&#x200B;**[!UICONTROL 新增檔案]**。
1. 啟用&#x200B;**[!UICONTROL 建立校訂]**&#x200B;切換。
1. （選擇性）在&#x200B;**[!UICONTROL 校訂名稱]**&#x200B;文字方塊中輸入校訂的名稱。
1. 在&#x200B;**[!UICONTROL 校訂核准]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 基本]**。
1. （選用）新增核准者。
1. （選擇性）在&#x200B;**[!UICONTROL 更新]**&#x200B;區域輸入註解。

   ![新增註解](assets/add-comment.png)

1. 從下拉式功能表中選擇&#x200B;**[!UICONTROL 資產型別]**。

1. （選擇性）選取&#x200B;**[!UICONTROL 新增外部檔案]**&#x200B;以從您的電腦新增檔案。
1. 按一下&#x200B;**[!UICONTROL 上傳]**，然後根據上述選擇的資產型別設定任何需要的匯出選項。

   外掛程式![中的](assets/plugin-files-350x307.png)檔案\
   檔案會顯示在外掛程式與案頭應用程式的[!UICONTROL 檔案]區域中。


## 上傳自動證明

1. 按一下右上角的&#x200B;**[!UICONTROL 功能表]**&#x200B;圖示，然後選取&#x200B;**[!UICONTROL 工作清單]**。 您也可以使用功能表導覽至父物件。

   ![返回工作清單](assets/go-back-to-work-list-350x314.png)

1. 前往您要上傳校樣的工作專案。
1. 按一下導覽列中的&#x200B;**[!UICONTROL 檔案]**&#x200B;圖示![檔案圖示](assets/documents.png)。

1. 按一下外掛程式底部附近的&#x200B;**[!UICONTROL 新增檔案]**。
1. 啟用&#x200B;**[!UICONTROL 建立校訂]**&#x200B;切換。
1. （選擇性）在&#x200B;**[!UICONTROL 校訂名稱]**&#x200B;文字方塊中輸入校訂的名稱。
1. 在&#x200B;**[!UICONTROL 校訂核准]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 自動化]**。
1. （選擇性）在&#x200B;**[!UICONTROL 工作流程範本]**&#x200B;方塊中，輸入校訂工作流程範本的名稱。

{{adjust-proof-settings}}

>[!NOTE]
>
> 如果工作流程範本中有任何空白的必填欄位，自動校樣設定會自動開啟，並且您需填入這些欄位才能上傳校樣。


1. （選擇性）在&#x200B;**[!UICONTROL 更新]**&#x200B;區域輸入註解。

   ![新增評論自動核准](assets/add-comment-automated-approval.png)

1. 從下拉式功能表中選擇&#x200B;**[!UICONTROL 資產型別]**。
1. （選擇性）選取&#x200B;**[!UICONTROL 新增外部檔案]**&#x200B;以從您的電腦新增檔案。
1. 按一下&#x200B;**[!UICONTROL 上傳]**，然後根據上述選擇的資產型別設定任何需要的匯出選項。
檔案會顯示在外掛程式與案頭應用程式的[!UICONTROL 檔案]區域中。

## 上傳新的校訂版本

您可以上傳新版本的校訂。 外掛程式會記住先前版本上設定的校訂工作流程，但您可以視需要變更此設定。

1. 按一下右上角的&#x200B;**[!UICONTROL 功能表]**&#x200B;圖示，然後選取&#x200B;**[!UICONTROL 工作清單]**。 您也可以使用功能表導覽至父物件。

   ![返回工作清單](assets/go-back-to-work-list-350x314.png)

1. 前往上載檔案所需的工作專案。
1. 按一下導覽列中的&#x200B;**[!UICONTROL 檔案]**&#x200B;圖示![檔案圖示](assets/documents.png)。

1. 按一下外掛程式底部附近的&#x200B;**[!UICONTROL 新版本]**。
1. 啟用&#x200B;**[!UICONTROL 建立校訂]**&#x200B;切換。

1. 在&#x200B;*[!UICONTROL *校訂核准]**區段中，選擇&#x200B;**[!UICONTROL 基本]**&#x200B;或&#x200B;**[!UICONTROL 自動化]**。

1. 根據您在步驟7中選取的核准型別，新增&#x200B;**[!UICONTROL 檢閱者]**&#x200B;或&#x200B;**[!UICONTROL 工作流程範本]**。

1. （選擇性）在&#x200B;**[!UICONTROL 更新]**&#x200B;區域輸入註解。
1. 從下拉式功能表中選擇&#x200B;**[!UICONTROL 資產型別]**。
1. 按一下&#x200B;**[!UICONTROL 上傳]**，然後根據上述選擇的資產型別設定任何需要的匯出選項。
檔案會顯示在外掛程式與案頭應用程式的[!UICONTROL 檔案]區域中。
