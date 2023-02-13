---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: 將XD畫板上傳為檔案至Workfront
description: 您可以上傳畫板作為檔案，以快速檢閱和核准，或僅儲存在Adobe Workfront中。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: bf47ae15d2972e8ee11f76741f8e5c676d79e626
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---


# 上傳 [!DNL XD] 將畫板作為文檔 [!DNL Workfront]

您可以上傳畫板作為檔案，以快速檢閱和核准，或僅儲存在 [!DNL Adobe Workfront].

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>您必須有 [!DNL Adobe Creative Cloud] 除了 [!DNL Workfront] 授權。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對[!UICONTROL文檔]的訪問</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>[!UICONTROL View]或更高版本訪問要上載文檔的對象。</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

* 您必須安裝 [!DNL Adobe Workfront for XD] 外掛程式，您才能將XD藝術展示板上傳為檔案至Workfront。

如需指示，請參閱 [安裝 [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## 添加新文檔

1. 按一下 **[!UICONTROL 功能表]** 圖示，然後選取 **[!UICONTROL 工作清單]**. 您也可以使用功能表導覽至上層物件。

   ![](assets/menu-350x440.png)

1. 轉到要上載文檔的工作項。
1. 按一下 **[!UICONTROL 檔案]** 圖示 ![](assets/documents.png) 的下一頁。

1. 按一下 **[!UICONTROL 新檔案]** 在外掛程式底部附近。
1. 選取您要上傳的畫板。

   >[!TIP]
   >
   >要選擇多個畫板，請按一下並將滑鼠拖動到所需畫板上。
1. （選用）在 **[!UICONTROL 更新]** 的上界。
1. 選擇 **[!UICONTROL 資產類型]** 從下拉式功能表：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL導出格式]</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>畫板會上傳為PNG，並顯示在 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>畫板將作為JPG上載到 [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>畫板會上傳為工作項目的[!UICONTROL Documents]標籤的SVG，位於 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>選擇是否要將所選畫板上傳為 <strong>單一PDF檔案</strong> 或 <strong>多個PDF檔案</strong>. 畫板會以PDF形式上傳至下列位置的工作項目的[!UICONTROL Documents]索引標籤： [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. 按一下 **[!UICONTROL 上傳]**.\
   文檔將出現在 [!UICONTROL 檔案] 區域。

## 新增版本

1. 按一下 **[!UICONTROL 功能表]** 圖示，然後選取 **[!UICONTROL 工作清單]**. 您也可以使用功能表導覽至上層物件。

   ![](assets/menu-350x440.png)

1. 轉到要上載文檔的工作項。
1. 按一下 **[!UICONTROL 檔案]** 圖示 ![](assets/documents.png)的下一頁。

1. 按一下要向中添加新版本的文檔。
1. 按一下 **[!UICONTROL 新版本]** 在外掛程式底部附近。
1. 選取您要上傳的畫板。

   >[!NOTE]
   >
   >如果要上傳新版本的SVG、PNG或JPG，則只能上傳一個畫板。

1. （選用）在 **[!UICONTROL 更新]** 的上界。

1. 選擇 **[!UICONTROL 資產類型]** 從下拉式功能表：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">匯出格式</td>
     </tr>
     <tr>
      <td role="rowheader">PNG</td>
      <td>畫板會以PNG的形式上傳至下列位置中的工作項目的[!UICONTROL Documents]索引標籤 [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>畫板會以JPG形式上傳至下列位置的工作項目的[!UICONTROL Documents]索引標籤： [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>畫板會以SVG形式上傳至下列位置的工作項目的[!UICONTROL Documents]索引標籤： [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>畫板將作為PDF上載到 [!DNL Workfront].</p>
      <p><strong>附註</strong>:您只能為新文檔版本上傳一個畫板。</p>
      </td>
     </tr>
    </tbody>
   </table>

1. 按一下 **[!UICONTROL 上傳]**.\
   文檔將出現在 [!UICONTROL 檔案] 區域。
