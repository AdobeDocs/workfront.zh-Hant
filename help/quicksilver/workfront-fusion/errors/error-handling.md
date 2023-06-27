---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 中的錯誤處理 [!DNL Adobe Workfront Fusion]
description: 當在執行案例期間發生錯誤時，通常是因為服務因失敗而無法使用、服務以非預期的資料回應，或輸入資料的驗證失敗。
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 中的錯誤處理 [!DNL Adobe Workfront Fusion]

當在執行案例期間發生錯誤時，通常是因為服務因失敗而無法使用、服務以非預期的資料回應，或輸入資料的驗證失敗。

如果模組在情景執行期間擲回錯誤，並且沒有附加到模組的錯誤處理路由，則會執行預設錯誤處理邏輯，如中所述 [中的處理錯誤 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

藉由將錯誤處理常式路由新增至模組，您可以將預設的錯誤處理邏輯取代為您自己的邏輯。 [!DNL Adobe Workfront Fusion] 提供五個不同的指令，可在錯誤處理常式路由的結尾插入。

如需詳細資訊，請參閱 [中用於錯誤處理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## 錯誤處理常式路由

若要將錯誤處理常式路由新增至模組：

1. 以滑鼠右鍵按一下模組，然後選取 **[!UICONTROL 新增錯誤處理常式]**：

   ![](assets/error-handler-route.png)

   此模組會顯示指令清單，以及在您的情境中使用的應用程式。

1. 如果您新增錯誤處理常式的模組是路由中的最後一個模組，請選取其中一個指令。

   或

   新增一或多個模組至錯誤處理常式路由。

   如果您在路由中新增更多模組， [!UICONTROL 忽略] 指令會依預設套用，並在發生錯誤時，處理該路由上的後續模組。


>[!INFO]
>
>在此範例中，如果在執行 [!UICONTROL 建立資料夾] 模組， [!UICONTROL 忽略] 指示詞將會自動套用，而案例將會移至錯誤處理常式路由上的下一個模組。
>
>不過，如果沒有錯誤，情境會移至 [!UICONTROL 列出資料夾模組中的所有檔案] 在一般路線上。
>
>![](assets/if-there-is-no-error-350x234.png)

請注意，錯誤處理常式繞線是由透明圓圈所組成，而一般繞線是由實心圓圈所組成。

## 處理指示詞時發生錯誤

這些指示詞會簡短說明如下。 如需詳細資訊，請參閱 [中用於錯誤處理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

根據案例執行是否應該繼續，總共有五個指令可以分組為以下類別。

下列指示詞可確保案例執行持續進行：

* **[!UICONTROL 繼續]**：可讓您為出現錯誤的模組指定替代輸出。 案例執行狀態會標籤為成功
* **[!UICONTROL 忽略]**：忽略錯誤。 案例執行狀態會標籤為成功
* **[!UICONTROL 中斷]**：將輸入儲存到未完成執行的佇列。 情境執行狀態會標示為警告。 如需詳細資訊，請參閱 [在中檢視和解決未完成的執行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

如果發生錯誤時，案例執行應該停止，請使用以下指令之一：

* **[!UICONTROL 復原]**：立即停止情景執行並將其狀態標籤為錯誤
* **[!UICONTROL 認可]**：立即停止情景執行並將其狀態標籤為成功

如需錯誤處理的詳細資訊，請參閱：

* [中用於錯誤處理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [中的進階錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)