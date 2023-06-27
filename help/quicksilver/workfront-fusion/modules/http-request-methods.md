---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 中的HTTP要求方法 [!DNL Adobe Workfront Fusion]
description: 當您在模組中設定API呼叫時，您需要填寫HTTP要求方法的欄位。
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# 中的HTTP要求方法 [!DNL Adobe Workfront Fusion]

當您在模組中設定API呼叫時，您需要填寫HTTP要求方法的欄位。

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

## HTTP方法

使用下列HTTP方法之一。

* **[!UICONTROL GET]**：根據您的引數從網頁伺服器擷取資料。 [!UICONTROL GET] 要求指定資源的表示法，並接收 [!UICONTROL 200 OK] 包含請求內容的回應訊息（如果成功）。
* **[!UICONTROL POST]**：根據您的引數傳送資料至網頁伺服器。 [!UICONTROL POST] 請求包括上傳檔案等動作。 多個 [!UICONTROL POST]s可能會造成與單一結果不同的結果 [!UICONTROL POST]，因此請小心不要無意間傳送多筆資料 [!UICONTROL POST]s.若為 [!UICONTROL POST] 成功，您會收到 [!UICONTROL 200 OK] 回應訊息。
* **[!UICONTROL PUT]**：根據您的引數傳送資料至網頁伺服器中的位置。 [!UICONTROL PUT] 請求包括上傳檔案等動作。 兩者之間的差異 [!UICONTROL PUT] 和 [!UICONTROL POST] 該PUT為等冪，表示單一成功的結果 [!UICONTROL PUT] 與許多相同專案相同 [!UICONTROL PUT]s.如果PUT成功，您會收到200回應訊息（通常是201或204）。
* **[!UICONTROL PATCH]**：（對部分API呼叫模組不可用）根據您的引數將部分修改套用至網頁伺服器上的資源。 [!UICONTROL PATCH] 不是等冪的，這表示多個字元的結果 [!UICONTROL PATCH]可能會產生非預期的結果。 若為 [!UICONTROL PATCH] 成功，您會收到200則回應訊息（通常為204）。
* **[!UICONTROL DELETE]**：根據您的引數（如果資源存在），從Web伺服器刪除指定的資源。 若為 [!UICONTROL DELETE] 成功，您會收到「200確定」回應訊息。
