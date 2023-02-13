---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 中的HTTP要求方法 [!DNL Adobe Workfront Fusion]
description: 在模組中設定API呼叫時，您需要填入HTTP要求方法的欄位。
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# 中的HTTP要求方法 [!DNL Adobe Workfront Fusion]

在模組中設定API呼叫時，您需要填入HTTP要求方法的欄位。

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

## HTTP方法

使用下列其中一種HTTP方法。

* **[!UICONTROL GET]**:根據您的參數從Web伺服器擷取資料。 [!UICONTROL GET] 請求指定資源的表示，並接收 [!UICONTROL 200 OK] 如果成功，則使用請求的內容回應訊息。
* **[!UICONTROL POST]**:根據您的參數將資料傳送至Web伺服器。 [!UICONTROL POST] 請求包括上傳檔案之類的動作。 多個 [!UICONTROL POST]可能會導致與單一 [!UICONTROL POST]，因此請謹慎避免無意傳送多個 [!UICONTROL POST]s.若 [!UICONTROL POST] 成功時，您會收到 [!UICONTROL 200 OK] 回應訊息。
* **[!UICONTROL PUT]**:根據您的參數將資料傳送至Web伺服器中的位置。 [!UICONTROL PUT] 請求包括上傳檔案之類的動作。 區別於 [!UICONTROL PUT] 和 [!UICONTROL POST] 是PUT是等冪，表示單一成功的結果 [!UICONTROL PUT] 與許多相同 [!UICONTROL PUT]s.如果PUT成功，您會收到200回應訊息（通常為201或204）。
* **[!UICONTROL PATCH]**:（某些API呼叫模組無法使用）根據您的參數，將部分修改套用至Web伺服器上的資源。 [!UICONTROL PATCH] 不是等冪，表示多個的結果 [!UICONTROL PATCH]可能會產生意想不到的後果。 若 [!UICONTROL PATCH] 成功時，您會收到200則回應訊息（通常為204）。
* **[!UICONTROL DELETE]**:根據參數（如果存在資源）從Web伺服器刪除指定的資源。 若 [!UICONTROL DELETE] 成功時，您會收到200 OK回應訊息。
