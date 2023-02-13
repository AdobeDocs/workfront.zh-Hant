---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Adobe Workfront聚變中的類型強制
description: 本檔案說明如何 [!DNL Adobe Workfront Fusion] 會在收到預期和非預期資料格式的值時出現行為。
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 1%

---

# 中的強制類型 [!DNL Adobe Workfront Fusion]

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

### 強制類型

本檔案說明如何 [!DNL Adobe Workfront Fusion] 會在收到預期和非預期資料格式的值時出現行為。

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>預期</th> 
   <th>已收到</th> 
   <th> <p>說明</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>陣列 </td> 
   <td>陣列 </td> 
   <td> <p>此值將不變地傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>陣列 </td> 
   <td>其他 </td> 
   <td> <p>如果接收的值不是陣列類型， [!DNL Workfront Fusion] 會建立陣列，第一個（也是唯一的）元素將會是接收的值。</p> </td> 
  </tr> 
  <tr> 
   <td>布林值 </td> 
   <td>布林值 </td> 
   <td> <p>此值將不變地傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>布林值 </td> 
   <td>數字 </td> 
   <td> <p>值會轉換為邏輯是，即使值為0亦然。</p> </td> 
  </tr> 
  <tr> 
   <td>布林值 </td> 
   <td>文字 </td> 
   <td> <p>如果值等於false或值為空，則會轉換為邏輯否。 若否，則會轉換為邏輯「是」。</p> </td> 
  </tr> 
  <tr> 
   <td>布林值 </td> 
   <td>其他 </td> 
   <td> <p>只要接收的值存在（非空值），該值就會轉換為邏輯「是」。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>緩衝 </td> 
   <td> <p>只有在程式碼頁面如預期般運作時，才會傳遞值。 如果代碼頁不同， [!DNL Workfront Fusion] 將嘗試將接收的值轉換為請求的代碼頁。 如果不支援此轉換， [!DNL Workfront Fusion] 會傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>布林值 </td> 
   <td> <p>值會轉換為文字(true/false)，然後依照上述步驟轉換為文字，轉換為二進位資料。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>日期 </td> 
   <td> <p>值會轉換為ISO 8601文字，然後依照上述轉換為文字的步驟轉換為二進位資料。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>數字 </td> 
   <td> <p>值會轉換為文字，然後依照上述步驟轉換為二進位資料，以轉換為文字。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>文字 </td> 
   <td> <p>值會轉換為二進位資料，並如預期般編碼。 如果未指定預期的編碼，則將使用utf8編碼。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>集合 </td> 
   <td>集合 </td> 
   <td> <p>此值將不變地傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>集合 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td>日期 </td> 
   <td> <p>此值將不變地傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td>文字 </td> 
   <td> <p>[!DNL Workfront Fusion] 會嘗試將文字轉換為日期。 如果轉換失敗，則會傳回驗證錯誤。 日期必須包含日、月和年。 日期可能包含時區。 預設時區是根據您的設定。 範例:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>數字 </td> 
   <td>數字 </td> 
   <td> <p>此值將不變地傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>數字 </td> 
   <td>文字 </td> 
   <td> <p>[!DNL Workfront Fusion] 會嘗試將文字轉換為數字。 如果轉換失敗，則會傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>數字 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>文字 </td> 
   <td>文字 </td> 
   <td> <p>此值將不變地傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>文字 </td> 
   <td>陣列 </td> 
   <td> <p>如果指定的陣列支援轉換為文字，則會轉換值。 如果沒有， [!DNL Workfront Fusion] 會傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>文字 </td> 
   <td>布林值 </td> 
   <td> <p>值會轉換為文字(true/false)。</p> </td> 
  </tr> 
  <tr> 
   <td>文字 </td> 
   <td>緩衝 </td> 
   <td> <p>如果為二進位資料指定了文本編碼，則值將轉換為文本。 如果沒有， [!DNL Workfront Fusion] 會傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>文字 </td> 
   <td>日期 </td> 
   <td> <p>值會轉換為ISO 8601文字。</p> </td> 
  </tr> 
  <tr> 
   <td>文字 </td> 
   <td>數字 </td> 
   <td> <p>值會轉換為文字。</p> </td> 
  </tr> 
  <tr> 
   <td>文字 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>時間 </td> 
   <td>時間 </td> 
   <td> <p>此值將不變地傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>時間 </td> 
   <td>文字 </td> 
   <td> <p>[!DNL Workfront Fusion] 會嘗試將時間轉換為小時:minutes:秒格式。 如果轉換失敗，則會傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>時間 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 傳回驗證錯誤。</p> </td> 
  </tr> 
 </tbody> 
</table>
