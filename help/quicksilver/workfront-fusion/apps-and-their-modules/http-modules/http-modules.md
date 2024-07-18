---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: HTTP &amp；gt；其他模組
description: ' [!DNL Adobe Workfront Fusion] HTTP應用程式提供各種模組，用於以超文字傳輸通訊協定(HTTP)通訊協定為基礎的通訊。 HTTP是全球資訊網資料通訊的基礎。 您可以使用模組下載網頁和檔案、呼叫Webhook和API端點等。'
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 45540ccc3b9fca98f8aaae86ac4d6574a067a6e4
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# HTTP >其他模組

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion]除了[!UICONTROL Adobe Workfront]授權外，還需要[!UICONTROL Adobe Workfront Fusion]授權。

[!DNL Adobe Workfront Fusion] [!UICONTROL HTTP]應用程式提供各種模組，以根據超文字傳輸通訊協定(HTTP)通訊協定進行通訊。 HTTP是全球資訊網資料通訊的基礎。 您可以使用模組下載網頁和檔案、呼叫Webhook和API端點等。

模組的正確選擇取決於您要存取的資源所使用的驗證/授權機制。 以下是模組的範例

* 提出請求：通用模組主要用於不使用任何型別的驗證/授權的資源
* 提出基本驗證要求：針對採用[!DNL HTTP]基本驗證(BA)的資源
* 提出OAuth 2.0請求：針對採用OAuth 2.0授權通訊協定的資源
* 提出使用者端憑證驗證請求：針對採用需要使用者端憑證之授權通訊協定的資源。
* 發出API金鑰授權請求：針對採用API金鑰授權的資源。

>[!NOTE]
>
>如果您要連線至目前沒有專用聯結器的Adobe產品，建議您使用Adobe Authenticator模組。
>
>如需詳細資訊，請參閱[Adobe Authenticator模組](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md)。

## 請求模組

如需特定請求模組指示，請參閱下列文章：

* [[!UICONTROL HTTP] >[!UICONTROL 提出要求]模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL 發出基本授權要求]模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL 發出OAuth 2.0請求]模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL 發出使用者端憑證授權要求]模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL 發出API金鑰授權要求]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## 其他動作模組

* [[!UICONTROL 取得檔案]](#get-a-file)
* [[!UICONTROL 解析目標URL]](#resolve-a-target-url)

### [!UICONTROL 取得檔案]

此動作模組會從指定的URL下載檔案。 下載檔案後，您可以使用情境中的其他模組進一步處理檔案（對應檔案資料）。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL] </td> 
   <td> <p>輸入或對應您要下載之檔案的URL。 </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 解析目標URL]

此動作模組會解析HTTP重新導向鏈結並傳回目標URL。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL] </td> 
   <td> <p>輸入或對應您要解析的URL，例如[!DNL bit.ly] URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法] </td> 
   <td> <p>選取您要使用[！UICONTROLHEAD]方法或[！UICONTROLGET]方法。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 疊代器模組

### [!UICONTROL 擷取標頭]

此模組會以個別的套件組合，從指定的HTTP模組傳回每個標題（名稱和值）。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source模組]</td> 
   <td> <p> 選取您要從中擷取標題的模組。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 產生JSON Web權杖(JWT)

您可使用內建函式產生JWT權杖：

頁首：

![](assets/jwt-header-350x19.png)

複製貼上的程式碼(&amp;P)：

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

裝載：

![](assets/jwt-payload-350x17.png)

複製貼上的程式碼(&amp;P)：

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Token：

![](assets/jwt-token-350x15.png)

複製貼上的程式碼(&amp;P)：

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
