---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Forms模組
description: 使用 [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Forms] 帳戶的 [!DNL Adobe Experience Manager Forms] 聯結器，建立、上傳和更新資產，以及複製或行動資料夾和資產。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 107d81f7-ca41-4d76-a6dd-e579886dc2ad
source-git-commit: 6c7d22bea669586c56acfc23d328d7cc815b04be
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# [!DNL Adobe Experience Manager Forms]模組

使用[!DNL Adobe Workfront Fusion]的[!DNL Adobe Experience Manager Forms]聯結器，您可以建立webhook以根據[!DNL Adobe Experience Manager Forms]帳戶中的事件啟動案例。

您可以在[!DNL Adobe Experience Manager Forms]內設定表單，以將表單提交內容傳送至此webhook。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

* 您必須有[!DNL Adobe Experience Manager Forms]帳戶才能使用此模組。

## 建立與Adobe Experience Manager Forms的連線

若要為您的[!DNL Adobe Experience Manager Forms]模組建立連線：

1. 按一下[連線]方塊旁的&#x200B;**[!UICONTROL 新增]**。

1. 填寫下列欄位：

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[！UICONTROL連線名稱]</td>
        <td>
          <p>輸入此連線的名稱。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL環境]</td>
        <td>
          <p>選取此連線是連線至生產或非生產環境。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL型別]</td>
        <td>
          <p>選取此帳戶是服務帳戶還是個人帳戶。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL執行個體URL，不含尾隨斜線]</td>
        <td>
          <p>輸入您用來存取帳戶的URL，不含最後一個斜線。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL IMS端點]</td>
        <td>
          <p><code>https://ims-na1.adobelogin.com</code></p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL使用者端ID]</td>
        <td>輸入您的[!DNL Adobe]使用者端識別碼。 這可以在[!DNL Adobe Developer Console]的[！UICONTROL認證詳細資料]區段中找到。
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL使用者端密碼]</td>
        <td>輸入您的[!DNL Adobe]使用者端密碼。 這可以在[!DNL Adobe Developer Console]的[！UICONTROL認證詳細資料]區段中找到。
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL組織ID]</td>
        <td>輸入您的[!DNL Adobe]組織識別碼。 這可以在[!DNL Adobe Developer Console]的[！UICONTROL認證詳細資料]區段中找到。
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL技術帳戶ID]</td>
        <td>輸入您的[!DNL Adobe]技術帳戶ID。 這可以在[!DNL Adobe Developer Console]的[！UICONTROL認證詳細資料]區段中找到。
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL中繼範圍]</td>
        <td>輸入任何適當的中繼範圍       </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL私密金鑰]</td>
        <td>
          <p>輸入在[!DNL Adobe Developer Console]中建立認證時產生的私密金鑰。 </p>
          <p>若要擷取您的私密金鑰或憑證：</p>
          <ol>
            <li value="1">
              <p>按一下<b>[！UICONTROL Extract]</b>。</p>
            </li>
            <li value="2">
              <p>選取要解壓縮的檔案型別。</p>
            </li>
            <li value="3">
              <p>選取包含私密金鑰或憑證的檔案。</p>
            </li>
            <li value="4">
              <p>輸入檔案的密碼。</p>
            </li>
            <li value="5">
              <p>按一下<b>[！UICONTROL儲存]</b>以擷取檔案並返回連線設定。</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以儲存連線並返回模組。

## Adobe Experience Manager Forms模組及其欄位

目前Adobe Experience Manager Forms聯結器中只有一個模組。

### 關注表單事件

此即時觸發器(webhook)可讓您在Adobe Experience Manager表單上發生提交動作時開始案例。

>[!IMPORTANT]
>
>此模組也需要Adobe Experience Manager中的設定。 設定此webhook後，您必須開啟Adobe Experience Manager並設定表單，以將提交內容傳送至webhook。
>
><!--For instructions on the required form configuration, see insert url here-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook名稱]</td> 
   <td> <p>輸入webhook的名稱</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Adobe Experience Manager]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/apps-and-their-modules/aem-forms-modules.md#create-a-connection-to-adobe-experience-manager-forms" class="MCXref xref">建立與[!DNL Adobe Experience Manager Forms]</a>的連線</p> </td> 
  </tr>

模組會建立webhook並提供webhook位址，您可以在[!DNL Adobe Experience Manager Forms]中輸入此位址至表單提交對話方塊。
