---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: 將XD工作區域作為檔案上傳到Workfront
description: 您可以將工作區域上傳為檔案，以快速檢閱和核准，或直接儲存至Adobe Workfront。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: bf47ae15d2972e8ee11f76741f8e5c676d79e626
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---


# 將[!DNL XD]工作區域上傳為檔案至[!DNL Workfront]

您可以將工作區域上傳為檔案，以進行快速檢閱和核准，或僅儲存於[!DNL Adobe Workfront]。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">產品</td> 
   <td>除了[!DNL Workfront]授權之外，您還必須有[!DNL Adobe Creative Cloud]授權。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯[！UICONTROL檔案]的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>[！UICONTROL檢視]存取您要上傳檔案之物件的更高版本。</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 先決條件

* 您必須先安裝[!DNL Adobe Workfront for XD]外掛程式，才能將XD圖案面板作為檔案上傳到Workfront。

如需指示，請參閱[安裝 [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md)。

## 新增檔案

1. 按一下右上角的&#x200B;**[!UICONTROL 功能表]**&#x200B;圖示，然後選取&#x200B;**[!UICONTROL 工作清單]**。 您也可以使用功能表導覽至父物件。

   ![](assets/menu-350x440.png)

1. 移至您要上傳檔案的工作專案。
1. 按一下導覽列中的&#x200B;**[!UICONTROL 檔案]**&#x200B;圖示![](assets/documents.png)。

1. 按一下外掛程式底部附近的&#x200B;**[!UICONTROL 新增檔案]**。
1. 選取您要上載的工作區域。

   >[!TIP]
   >
   >若要選取多個工作區域，請按一下滑鼠，並將滑鼠拖曳到您想要的工作區域上。
1. （選擇性）在&#x200B;**[!UICONTROL 更新]**&#x200B;區域輸入註解。
1. 從下拉式功能表中選擇&#x200B;**[!UICONTROL 資產型別]**：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[！UICONTROL匯出格式]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>工作區域會以PNG形式上傳至[!DNL Workfront]中工作專案的[！UICONTROL檔案]索引標籤。 </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>工作區域會以JPG形式上傳至[!DNL Workfront]中工作專案的[！UICONTROL檔案]索引標籤。 <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>工作區域會以SVG形式上傳至[!DNL Workfront]中的工作專案[！UICONTROL檔案]索引標籤。 </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>若要將選取的工作區域上傳為<strong>單一PDF檔案</strong>或<strong>多個PDF檔案</strong>，請選擇此選項。 工作區域會以PDF形式上傳至[!DNL Workfront]中的工作專案[！UICONTROL檔案]索引標籤。</td>
     </tr>
    </tbody>
   </table>


1. 按一下&#x200B;**[!UICONTROL 上傳]**。\
   檔案會顯示在外掛程式與案頭應用程式的[!UICONTROL 檔案]區域中。

## 新增新版本

1. 按一下右上角的&#x200B;**[!UICONTROL 功能表]**&#x200B;圖示，然後選取&#x200B;**[!UICONTROL 工作清單]**。 您也可以使用功能表導覽至父物件。

   ![](assets/menu-350x440.png)

1. 移至您要上傳檔案的工作專案。
1. 按一下導覽列中的&#x200B;**[!UICONTROL 檔案]**&#x200B;圖示![](assets/documents.png)。

1. 按一下要新增新版本的檔案。
1. 按一下外掛程式底部附近的&#x200B;**[!UICONTROL 新版本]**。
1. 選取您要上載的工作區域。

   >[!NOTE]
   >
   >如果您想要上傳新版的SVG、PNG或JPG，則只能上傳一個工作畫板。

1. （選擇性）在&#x200B;**[!UICONTROL 更新]**&#x200B;區域輸入註解。

1. 從下拉式功能表中選擇&#x200B;**[!UICONTROL 資產型別]**：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">匯出格式</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>工作區域會以PNG形式上傳至[!DNL Workfront]中工作專案的[！UICONTROL檔案]索引標籤。 </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>工作區域會以JPG形式上傳至[!DNL Workfront]中工作專案的[！UICONTROL檔案]索引標籤。 <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>工作區域會以SVG形式上傳至[!DNL Workfront]中的工作專案[！UICONTROL檔案]索引標籤。 </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>工作區域會以PDF形式上傳至[!DNL Workfront]中的工作專案[！UICONTROL檔案]索引標籤。</p>
      <p><strong>附註</strong>：您只能為新檔案版本上傳一個工作畫板。</p>
      </td>
     </tr>
    </tbody>
   </table>

1. 按一下&#x200B;**[!UICONTROL 上傳]**。\
   檔案會顯示在外掛程式與案頭應用程式的[!UICONTROL 檔案]區域中。
