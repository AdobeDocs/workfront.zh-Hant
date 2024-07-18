---
title: SOAP API常見問題集
description: SOAP API常見問題集
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# SOAP API常見問題集

## 如何建立我的第一個檔案校訂？

這需要3個簡單的步驟：

**步驟1**：透過Workfront Proof要求將檔案上傳至Post  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php)。 我們將傳回檔案雜湊 — 這非常重要！ 請注意，在這個階段，您不會看到帳戶中的任何內容，您目前所做的是將檔案傳送給我們，但沒有告訴我們應如何處理。

**步驟2**：如果您還沒有工作階段ID，請使用doLogin()或getSessionID()方法取得工作階段ID。 使用前者可使用使用者的電子郵件地址和密碼「登入」，如果您有使用者的電子郵件地址和驗證Token，則使用後者方法。

**步驟3：**&#x200B;現在該建立您的校訂了。 使用createProof()方法，至少傳送必填欄位給我們（目前只有5個必填欄位）。 請確保將雜湊引數設定為「步驟1」期間傳回的檔案雜湊，因為這可讓我們決定建立校樣時要使用的檔案。

如果您現在登入您的帳戶，您將會看到證明。

## 如何建立我的第一個Web快照集校訂？

這需要2個簡單的步驟：

**步驟1**：如果您還沒有工作階段ID，請使用doLogin()或getSessionID()方法取得工作階段ID。 使用前者可使用使用者的電子郵件地址和密碼「登入」，如果您有使用者的電子郵件地址和驗證Token，則使用後者方法。

**步驟2：**現在該建立您的校訂了。 使用createProof()方法，至少傳送必填欄位給我們（目前只有5個必填欄位）。 請確定您將Hash引數設為「web」，並將SourceName引數設為您要擷取的網頁URL。

如果您現在登入您的帳戶，您將會看到證明。

## 校訂和版本之間有何差異？

在Workfront Proof中，版本會顯示為單一校訂。 按一下Web UI中的特定版本會顯示該版本的詳細資料。 實際上，每個版本都是獨立的校訂，Web UI會顯示在一起。

從API的觀點來看，每個版本都是個別的校訂，校訂透過其ID連結在一起。

**createProof()**&#x200B;將一律建立&#x200B;**版本1**&#x200B;的校訂。 舉例來說，我們假設針對此校訂傳回的ID「100」。

使用&#x200B;**createProofVersion()**&#x200B;時，一律會傳送先前版本的ID。 如果要在校訂&quot;100&quot;上建立&#x200B;**版本2**，我們&#x200B;**傳入&quot;100&quot;給ParentFileID**&#x200B;引數。 這會告訴系統，此校訂應該是集合的第2版。 此方法將傳回不重複校訂ID，例如，假設這是「101」。

如果需要第三版本，即&#x200B;**版本3**，您將再次呼叫&#x200B;**createProofVersion()**，這次為ParentFileID **傳入「101」，以確保正確建立連結的版本清單。**

## 我需要在每次呼叫前取得新的工作階段ID嗎？

請務必注意，每個工作階段ID基本上都是執行動作的使用者。 

您不需要在每次呼叫API前取得新的工作階段ID，其24小時內將維持有效。 每次呼叫API時，到期時間都會重設。

## 什麼是校訂/個人URL？

**團隊/公用**：每個校訂版本都有唯一的團隊（公用） URL。 如果啟用，它將以唯讀模式開啟校訂。 您可以使用[getProofURL()](https://api.proofhq.com/home/proofs/getproofurl.html)方法取得團隊URL。

**個人**：每個檢閱者和校訂版本的個人URL都是唯一的。 如果校訂集包含3個版本，而稽核者位於所有版本，則稽核者將有3個不重複的個人URL。 個人URL會開啟校訂版本，其中檢閱者已識別，因此應妥善儲存且不分享。 呼叫[getProofReviewers()](https://api.proofhq.com/home/proofs/getproofreviewers.html)方法，然後反複處理每個方法，即可取得個人網址  [SOAPRecepientObject](https://api.proofhq.com/home/objects/soaprecipientobject.html)並取得引數&quot;proof_url&quot;。

## >如何在開啟迷你校樣時包含自訂引數？

迷你校訂可讓您將校訂工具嵌入到您自己的頁面中。 「referer」引數可包含在小型校訂中，以便在使用者點按小型校訂的關閉按鈕時提供重新導向URL。 您可以使用逸出的&#39;&amp;&#39;字元（例如%26）附加任意數目的自訂引數，以包含在此重新導向URL中。

例如，miniproof URL
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=`必須編碼為 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=`以便傳遞自訂引數。

## 如何建立Java Web服務使用者端？

[此影片](https://screencast.com/t/xsSNrqs5b)說明如何使用Eclipse和Workfront Proof WSDL定義來建立Java Web Service使用者端。

