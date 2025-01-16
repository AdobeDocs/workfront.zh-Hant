---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion]中的HTTP要求方法'
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的HTTP要求方法

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [HTTP要求方法](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/http-request-methods.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

當您在模組中設定API呼叫時，您需要填寫HTTP要求方法的欄位。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## HTTP方法

使用下列其中一個HTTP方法。

* **[!UICONTROL GET]**：根據您的引數從網頁伺服器擷取資料。 [!UICONTROL GET]要求指定資源的表示法，並在成功時收到包含所要求內容的[!UICONTROL 200 OK]回應訊息。
* **[!UICONTROL POST]**：根據您的引數傳送資料至網頁伺服器。 [!UICONTROL POST]要求包含上傳檔案之類的動作。 多個[!UICONTROL POST]可能會產生與單一[!UICONTROL POST]不同的結果，因此對於無意中傳送多個[!UICONTROL POST]請小心。如果[!UICONTROL POST]成功，您會收到[!UICONTROL 200 OK]回應訊息。
* **[!UICONTROL PUT]**：根據您的引數傳送資料至網頁伺服器的位置。 [!UICONTROL PUT]要求包含上傳檔案之類的動作。 [!UICONTROL PUT]與[!UICONTROL POST]之間的差異在於PUT為等冪，這表示單一成功[!UICONTROL PUT]的結果與許多相同的[!UICONTROL PUT]相同。如果PUT成功，您會收到200回應訊息（通常是201或204）。
* **[!UICONTROL PATCH]**： （某些API呼叫模組無法使用）根據您的引數，將部分修改套用至網頁伺服器上的資源。 [!UICONTROL PATCH]不是等冪，這表示多個[!UICONTROL PATCH]的結果可能會產生非預期的後果。 如果[!UICONTROL PATCH]成功，您將會收到200回應訊息（通常是204）。
* **[!UICONTROL DELETE]**：根據您的引數（如果資源存在），從網頁伺服器刪除指定的資源。 如果[!UICONTROL DELETE]成功，您會收到「200確定」回應訊息。
