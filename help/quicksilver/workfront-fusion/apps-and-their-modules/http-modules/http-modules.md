---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: HTTP &gt;其他模組
description: 此 [!DNL Adobe Workfront Fusion] HTTP應用程式提供了基於超文本傳輸協定(HTTP)協定的各種通信模組。 HTTP是萬維網資料通信的基礎。 您可以使用模組來下載網頁和檔案、呼叫Webhook和API端點等。
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# HTTP >其他模組

>[!NOTE]
>
>[!UICONTROL Adobe Workfront融合] 要求 [!UICONTROL Adobe Workfront融合] 除 [!UICONTROL Adobe Workfront] 授權。

此 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] 應用程式提供基於超文本傳輸協定(HTTP)協定的各種通信模組。 HTTP是萬維網資料通信的基礎。 您可以使用模組來下載網頁和檔案、呼叫Webhook和API端點等。

模組的正確選擇取決於要訪問的資源所採用的身份驗證/授權機制。 以下是模組的範例

* 提出請求：通用模組主要用於不採用任何類型的驗證/授權的資源
* 提出基本驗證請求：適用於採用的資源 [!DNL HTTP] 基本身份驗證(BA)
* 提出OAuth 2.0請求：使用OAuth 2.0授權協定的資源
* 提出用戶端憑證驗證請求：使用需要客戶端證書的授權協定的資源。
* 提出API金鑰授權請求：用於使用API金鑰進行授權的資源。

## 要求模組

如需特定要求模組指示，請參閱下列文章：

* [[!UICONTROL HTTP] >[!UICONTROL 提出請求] 模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL 提出基本授權請求] 模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL 提出OAuth 2.0請求] 模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL 提出客戶端證書授權請求] 模組](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL 提出API金鑰授權要求]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## 其他動作模組

* [[!UICONTROL 取得檔案]](#get-a-file)
* [[!UICONTROL 解析目標URL]](#resolve-a-target-url)

### [!UICONTROL 取得檔案]

此動作模組會從指定的URL下載檔案。 下載檔案後，您可以使用案例中的其他模組進一步處理檔案（對應檔案資料）。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>輸入或對應您要下載的檔案的URL。 </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 解析目標URL]

此動作模組解析HTTP重新導向的鏈，並傳回目標URL。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>輸入或對應您要解析的URL，例如 [!DNL bit.ly] URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法] </td> 
   <td> <p>選擇您要使用[!UICONTROLHEAD]方法還是[!UICONTROLGET]方法。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 迭代器模組

### [!UICONTROL 擷取標題]

此模組會從個別套件中指定的HTTP模組傳回每個標題（名稱和值）。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模組]</td> 
   <td> <p> 選取您要擷取標題的模組。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 產生JSON網頁代號(JWT)

您可以透過內建函式產生JWT代號：

標題:

![](assets/jwt-header-350x19.png)

複製並貼上的代碼：

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

裝載：

![](assets/jwt-payload-350x17.png)

複製並貼上的代碼：

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

代號：

![](assets/jwt-token-350x15.png)

複製並貼上的代碼：

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
