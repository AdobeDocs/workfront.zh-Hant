---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 在Adobe Workfront Fusion中鍵入脅迫
description: 本檔案說明如何 [!DNL Adobe Workfront Fusion] 會在收到預期和意外資料格式的值時採取行動。
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 1%

---

# 輸入強制 [!DNL Adobe Workfront Fusion]

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

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
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

### 輸入強制

本檔案說明如何 [!DNL Adobe Workfront Fusion] 會在收到預期和意外資料格式的值時採取行動。

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
   <td> <p>值會以未變更的方式傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>陣列 </td> 
   <td>其他 </td> 
   <td> <p>如果收到的值不是陣列型別， [!DNL Workfront Fusion] 將會建立一個陣列，第一個（也是唯一一個）元素將會是收到的值。</p> </td> 
  </tr> 
  <tr> 
   <td>布林值 </td> 
   <td>布林值 </td> 
   <td> <p>值會以未變更的方式傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>布林值 </td> 
   <td>數字 </td> 
   <td> <p>即使值為0，該值也會轉換為邏輯「是」。</p> </td> 
  </tr> 
  <tr> 
   <td>布林值 </td> 
   <td>文字 </td> 
   <td> <p>如果值等於false或值為空，則會轉換為邏輯否。 如果沒有，則會轉換為邏輯「是」。</p> </td> 
  </tr> 
  <tr> 
   <td>布林值 </td> 
   <td>其他 </td> 
   <td> <p>只要收到的值存在（不是空值），該值就會轉換為邏輯「是」。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>緩衝 </td> 
   <td> <p>只有在字碼頁如預期時，才會未變更地傳遞值。 如果程式碼頁不同， [!DNL Workfront Fusion] 會嘗試將收到的值轉換為要求的字碼頁。 如果不支援此轉換， [!DNL Workfront Fusion] 將傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>布林值 </td> 
   <td> <p>值會轉換為文字(true/false)，然後依照上述步驟轉換為二進位資料，以轉換為文字。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>日期 </td> 
   <td> <p>值會轉換為ISO 8601文字，然後依照上述轉換為文字的步驟轉換為二進位資料。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>數字 </td> 
   <td> <p>依照上述步驟將值轉換為文字，再轉換為二進位資料，以轉換為文字。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>文字 </td> 
   <td> <p>值會轉換為二進位資料，並按預期編碼。 如果未指定預期的編碼，將會使用utf8編碼。</p> </td> 
  </tr> 
  <tr> 
   <td>緩衝 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>集合 </td> 
   <td>集合 </td> 
   <td> <p>值會以未變更的方式傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>集合 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td>日期 </td> 
   <td> <p>值會以未變更的方式傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td>文字 </td> 
   <td> <p>[!DNL Workfront Fusion] 會嘗試將文字轉換為日期。 如果轉換失敗，則會傳回驗證錯誤。 日期必須包含日、月和年。 日期可能包含時間和時區。 預設時區取決於您的設定。 範例:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>日期 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>數字 </td> 
   <td>數字 </td> 
   <td> <p>值會以未變更的方式傳遞。</p> </td> 
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
   <td> <p>值會以未變更的方式傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>文字 </td> 
   <td>陣列 </td> 
   <td> <p>如果指定的陣列支援轉換為文字，則會轉換值。 如果沒有， [!DNL Workfront Fusion] 將傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>文字 </td> 
   <td>布林值 </td> 
   <td> <p>值會轉換為文字(true/false)。</p> </td> 
  </tr> 
  <tr> 
   <td>文字 </td> 
   <td>緩衝 </td> 
   <td> <p>如果為二進位資料指定了文字編碼，該值將會轉換為文字。 如果沒有， [!DNL Workfront Fusion] 將傳回驗證錯誤。</p> </td> 
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
   <td> <p>值會以未變更的方式傳遞。</p> </td> 
  </tr> 
  <tr> 
   <td>時間 </td> 
   <td>文字 </td> 
   <td> <p>[!DNL Workfront Fusion] 會嘗試將時間轉換為小時:minutes:秒數格式。 如果轉換失敗，則會傳回驗證錯誤。</p> </td> 
  </tr> 
  <tr> 
   <td>時間 </td> 
   <td>其他 </td> 
   <td> <p>[!DNL Workfront Fusion] 傳回驗證錯誤。</p> </td> 
  </tr> 
 </tbody> 
</table>
