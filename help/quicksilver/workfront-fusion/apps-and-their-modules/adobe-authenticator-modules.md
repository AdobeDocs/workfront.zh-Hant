---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Authenticator模組
description: 透過Adobe Authenticator模組，您可以使用單一連線透過API連線至任何Adobe產品。
author: Becky
feature: Workfront Fusion
exl-id: 74c943fb-37ad-4d91-8af7-9808ba69992e
source-git-commit: 443bdb5caee4b8a7ba9df95b0befff27b7aaabc2
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 1%

---

# Adobe Authenticator模組

Adobe Authenticator模組可讓您使用單一連線來連線至任何AdobeAPI。 這可讓您更輕鬆地連線到尚未擁有專用Fusion聯結器的Adobe產品。

與HTTP模組相比，您可在專用應用程式中建立連線。

若要檢視可用的AdobeAPI清單，請參閱 [ADOBEAPI](https://developer.adobe.com/apis). 您只能使用指派給您的API。

## 存取需求

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 計劃</td>
      <td>
        <p>新增：任何</p><p>或</p><p>目前： [！UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 授權</td>
      <td>
        <p>新增：標準</p><p>或</p><p>目前： [！UICONTROL計畫]，[！UICONTROL工作]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權</td>
      <td>
   <p>目前的Fusion授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版Fusion授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">產品</td>
      <td>
   <p>全新Workfront計畫：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>目前的Workfront計畫：您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td>
    </tr>
  </tbody>
</table>

## 先決條件

* 您必須擁有您希望模組連線的Adobe產品的存取權。
* 您必須擁有Adobe Developer Console的存取權。
* 您在Adobe Developer Console上必須有專案，其中包含您想要模組連線至的API。 您可以：

   * 使用API建立新專案。

     或
   * 將API新增至現有專案。

  如需在Adobe Developer Console上建立或新增API至專案的詳細資訊，請參閱 [建立專案](https://developer.adobe.com/dep/guides/dev-console/create-project/) 在Adobe檔案中。

## 建立連線

Adobe Authenticator連線會連線至Adobe Developer Console上的單一專案。 若要針對多個AdobeAPI使用相同的連線，請將API新增至相同的專案，並建立與該專案的連線。

您可以建立不同專案的個別連線，但無法使用連線來存取該連線中所指定專案以外的API。

>[!IMPORTANT]
>
>使用Adobe Authenticator聯結器，您可以選擇進行OAuth伺服器對伺服器連線，或選擇服務帳戶(JWT)連線。 Adobe已棄用JWT憑證，這些憑證將在2025年1月1日之後停止運作。 **因此，強烈建議您建立OAuth連線。**
>
>如需這些連線型別的詳細資訊，請參閱 [伺服器對伺服器驗證](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) 在Adobe檔案中

若要建立連線：

1. 在任何Adobe Authenticator模組中，按一下 **新增** ，位於連線欄位旁。
1. 填寫下列欄位：

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[！UICONTROL連線型別]</td>
        <td>
          <p>選取您要建立OAuth伺服器對伺服器連線，還是要建立服務帳戶(JWT)連線。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL連線名稱]</td>
        <td>
          <p>輸入此連線的名稱。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL使用者端ID]</td>
        <td>輸入您的 [!DNL Adobe] 使用者端ID。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL使用者端密碼]</td>
        <td>輸入您的 [!DNL Adobe] 使用者端密碼。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL範圍]</td>
        <td>如果您已選取OAuth連線，請輸入此連線所需的範圍。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL技術帳戶ID]</td>
        <td>輸入您的 [!DNL Adobe] 技術帳戶ID。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL組織ID]</td>
        <td>如果您已選取JWT連線，請輸入 [!DNL Adobe] 組織ID。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL中繼範圍]</td>
        <td>如果您已選取JWT連線，請輸入此連線所需的中繼範圍。 </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL私密金鑰]</td>
        <td>
          <p>如果您已選取JWT連線，請輸入在中建立認證時產生的私密金鑰。 [!DNL Adobe Developer Console]. </p>
          <p>若要擷取您的私密金鑰或憑證：</p>
          <ol>
            <li value="1">
              <p>按一下 <b>[！UICONTROL Extract]</b>.</p>
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
              <p>按一下 <b>[！UICONTROL儲存]</b> 以擷取檔案並返回連線設定。</p>
            </li>
          </ol>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL基底URL]</td>
        <td>您必須新增要此驗證器允許的基本URL。 稍後在情境中使用進行自訂API呼叫模組時，您將新增相對路徑至所選的URL。 在這裡輸入URL，您可以控制進行自訂API呼叫模組可以連線的專案，進而提高安全性。<p>針對您想要新增至驗證器的每個基底URL，按一下 <b>新增專案</b> 並輸入基底URL。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL驗證URL]</td>
        <td>將此項留空將使用標準Adobe IMS驗證URL <code>https://ims-na1.adobelogin.com</code>. 如果您沒有使用Adobe IMS進行驗證，請輸入用於驗證的URL。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL環境]</td>
        <td>選取您要連線到生產或非生產環境。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL型別]</td>
        <td>選取您要連線到服務帳戶還是個人帳戶。</td>
      </tr>
    </tbody>
    </table>

1. 按一下 **[!UICONTROL 繼續]** 以儲存連線並返回模組。

## 模組

### 進行自訂API呼叫

此動作模組可讓您呼叫任何AdobeAPI。

>[!TIP]
>
>您必須為要連線的API輸入整個URL。 此模組不接受相對URL。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[！UICONTROL Connection]</td>
     <td>如需建立Adobe Authenticator模組連線的指示，請參閱 <a href="#create-a-connection" class="MCXref xref" >建立連線</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL URL]</p>
      </td>
      <td>
        <p>輸入您要連線之API點的整個URL。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標頭。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion會自動新增授權標頭。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL查詢字串]  </td>
      <td>
        <p>輸入請求查詢字串。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>輸入您希望模組在一個執行週期內傳回的結果數目上限。</p>
      </td>
    </tr>
  </tbody>
</table>
