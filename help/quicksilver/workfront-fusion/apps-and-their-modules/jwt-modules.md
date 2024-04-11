---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: jwt模組
description: 此 [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] 應用程式會提供根據所提供演演算法建立JWT權杖的模組。
author: Becky
feature: Workfront Fusion
source-git-commit: d4f6f5d4919120e37fb94a23ac834a3896019584
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# [!UICONTROL JWT] 模組

此 [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] 應用程式會提供根據所提供演演算法建立JWT權杖的模組。

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
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 工作自動化與整合]，請參閱[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## JWT模組及其欄位

### 產生JWT

此模組會根據選取的演演算法產生JWT。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL演演算法]</td> 
   <td> <p>選取您要用來產生JWT的演演算法。</p> <ul>
   <li><b>HS256</b>：使用SHA-256雜湊演演算法的HMAC</li>
   <li><b>HS384</b>：使用SHA-384雜湊演演算法的HMAC</li>
   <li><b>HS512</b>：使用SHA-512雜湊演演算法的HMAC</li>
   <li><b>RS256</b>：使用SHA-256雜湊演演算法的RSASSA-PKCS1-v1_5</li>
   <li><b>RS384</b>：使用SHA-384雜湊演演算法的RSASSA-PKCS1-v1_5</li>
   <li><b>RS512</b>：使用SHA-512雜湊演演算法的RSASSA-PKCS1-v1_5</li>
   <li><b>PS256</b>：使用SHA-256雜湊演演算法的RSASSA-PSS （僅限節點^6.12.0或&gt;=8.0.0）</li>
   <li><b>PS384</b>：使用SHA-384雜湊演演算法的RSASSA-PSS （僅限節點^6.12.0或&gt;=8.0.0）</li>
   <li><b>PS512</b>：使用SHA-512雜湊演演算法的RSASSA-PSS （僅限節點^6.12.0或&gt;=8.0.0）</li>
   <li><b>ES256</b>：使用P-256曲線和SHA-256雜湊演演算法的ECDSA</li>
   <li><b>ES384</b>：使用P-384曲線和SHA-384雜湊演演算法的ECDSA</li>
   <li><b>ES512</b>：使用P-521曲線和SHA-512雜湊演演算法的ECDSA</li>
   </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL裝載] </td> 
   <td> <p>針對您要新增的每個裝載專案，按一下 <b>新增專案</b> 並輸入專案的索引鍵和值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Options] </td> 
   <td> <p>對於每個要新增的選項專案，按一下 <b>新增專案</b> 並輸入專案的索引鍵和值。</p> <p>下列鍵可供使用：
   <ul>
   <li><b>演演算法</b>：（預設值： RS256）</li>
   <li><b>expiresIn</b>：以秒或描述時間範圍的字串表示（例如2天、10小時、7天）。 數值會解譯為秒數。 如果您使用字串，請務必提供時間單位（天、小時等），否則預設會使用毫秒單位（120等於120毫秒）。</li>
   <li><b>notBefore</b>：以秒或描述時間範圍的字串表示（例如2天、10小時、7天）。 數值會解譯為秒數。 如果您使用字串，請務必提供時間單位（天、小時等），否則預設會使用毫秒單位（120等於120毫秒）。
</li>
   <li><b>對象</b></li>
   <li><b>簽發者</b></li>
   <li><b>jwtid</b></li>
   <li><b>主旨</b></li>
   <li><b>noTimestamp</b></li>
   <li><b>頁首</b></li>
   <li><b>keyid</b></li>
   <li><b>mutatePayload</b>：如果 <code>true</code>，sign函式會直接修改裝載物件。 如果在宣告套用至裝載後、但在裝載編碼為Token之前，您需要該裝載的原始參考，這個功能會很好用。</li>
   <li><b>allowInsecureKeySizes</b>：如果 <code>true</code>，可讓模數低於2048的私密金鑰用於RSA。</li>
   <li><b>allowInvalidAsymmetricKeyType</b>：如果 <code>true</code>，允許不符合指定演演算法的非對稱金鑰。 此選項僅供回溯相容性使用，應避免使用。</li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

