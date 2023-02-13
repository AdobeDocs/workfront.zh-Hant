---
title: SOAP API常見問題集
description: SOAP API常見問題集
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# SOAP API常見問題集

## 如何建立第一個檔案校樣？

需要3個簡單步驟：

**步驟1**:透過Post要求將檔案傳送至，將檔案上傳至Workfront校樣  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). 我們會傳回檔案雜湊 — 這非常重要！ 請注意，在此階段，您的帳戶中不會顯示任何內容，您迄今所做的只是將檔案發送給我們，但沒有告訴我們該如何處理。

**步驟2**:如果您尚未擁有工作階段ID，請使用doLogin()或getSessionID()方法取得。 使用前者使用使用者的電子郵件地址和密碼來「登入」；如果您有使用者的電子郵件地址和驗證Token，則使用後者方法。

**步驟3:** 現在是時候建立證據了。 請使用createProof()方法，並至少傳送必要欄位（目前只有5個欄位）。 請確定您將Hash參數設為「步驟1」期間傳回的檔案雜湊，因為這可讓我們決定在建立您的校樣時要使用的檔案。

如果您現在登入帳戶，便會看到校樣。

## 如何建立第一個Web快照校樣？

需要2個簡單步驟：

**步驟1**:如果您尚未擁有工作階段ID，請使用doLogin()或getSessionID()方法取得。 使用前者使用使用者的電子郵件地址和密碼來「登入」；如果您有使用者的電子郵件地址和驗證Token，則使用後者方法。

**步驟2:**現在是時候建立校樣了。 請使用createProof()方法，並至少傳送必要欄位（目前只有5個欄位）。 請確定您將雜湊參數設為&quot;web&quot;，並將SourceName參數設為您要擷取之網頁的URL。

如果您現在登入帳戶，便會看到校樣。

## 校樣和版本有何不同？

在Workfront中，校樣版本會顯示為單一校樣。 按一下Web UI中的特定版本時，會顯示該版本的詳細資料。 實際上，每個版本都是個別的證明，而網頁UI會一起顯示。

從API的角度來看，每個版本都是個別的證明，而且證明會透過其ID連結在一起。

**createProof()** 將一律建立 **版本1** 證據。 假設在範例中，針對此校樣「100」傳回的ID。

使用時 **createProofVersion()** 一律會以舊版的ID傳送。 如果我們想要建立 **版本2** 在&quot;100&quot;的證明上，我們 **傳入&quot;100&quot;作為ParentFileID** 參數。 這會告訴系統，此校樣應為集的第2版。 方法會傳回唯一的校樣ID，例如，假設這是「101」。

如果第三版，即 **版本3** 為必要，您將呼叫 **createProofVersion()** 又一次 **傳入&quot;101&quot;作為ParentFileID** 這將可確保正確建立已連結的版本清單。

## 是否需要在每次呼叫前取得新的工作階段ID?

請務必指出，每個工作階段ID本質上都是執行動作的使用者。 

您不需要在每次呼叫API前取得新的工作階段ID，且此ID將維持24小時有效。 每次您呼叫API時，到期時間都會重設。

## 什麼是證明/個人URL?

**團隊/公開**:每個校樣版本都有一個唯一的團隊（公用）URL。 如果已啟用，則會以唯讀模式開啟校樣。 您可以使用 [getProofURL()](http://api.proofhq.com/home/proofs/getproofurl) 方法。

**個人**:每個審核者和證明版本的個人URL都是唯一的。 如果校樣集包含3個版本，且審核者位於所有版本，則審核者將擁有3個不重複的個人URL。 個人URL會開啟已識別審核者的校樣版本，因此應該保持安全且不共用。 您可以呼叫 [getProofReviewers()](http://api.proofhq.com/home/proofs/getproofreviewers) 方法，然後迭代  [SOAPRecepientObject](http://api.proofhq.com/home/objects/soaprecipientobject) 並取得「proof_url」參數。

## >開啟小型校樣時如何包含自訂參數？

微校樣可讓您將校樣工具內嵌在自己的頁面中。 「referer」參數可納入微校樣中，以便在使用者按一下微校樣中的關閉按鈕時提供重新導向URL。 您可以使用逸出的「&amp;」字元來附加任何數量的自訂參數，以納入此重新導向URL。%26。

例如，微型校樣URL
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` 必須編碼為 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` 以便傳遞自訂參數。

## 如何建立Java Web服務客戶端？

[此影片](http://screencast.com/t/xsSNrqs5b) 顯示如何使用Eclipse和Workfront校樣WSDL定義來建立Java Web服務客戶端。
