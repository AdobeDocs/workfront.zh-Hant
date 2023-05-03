---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 錯誤處理 [!DNL Adobe Workfront Fusion]
description: 當執行案例期間發生錯誤時，通常是因為服務因失敗而無法使用、服務以非預期資料回應，或輸入資料驗證失敗。
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: e936bbd2837e4aec67d4136b8efcccb6f8454a89
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# 錯誤處理 [!DNL Adobe Workfront Fusion]

當執行案例期間發生錯誤時，通常是因為服務因失敗而無法使用、服務以非預期資料回應，或輸入資料驗證失敗。

如果模組在方案執行期間擲回錯誤，且沒有附加到模組的錯誤處理路由，則會執行預設錯誤處理邏輯，如 [中的錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

通過將錯誤處理程式路由添加到模組中，可以將預設錯誤處理邏輯替換為您自己的邏輯。 [!DNL Adobe Workfront Fusion] 提供五個不同的指令，可插入到錯誤處理程式路由的末尾。

如需詳細資訊，請參閱 [錯誤處理指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 錯誤處理程式路由

向模組添加錯誤處理程式路由：

1. 以滑鼠右鍵按一下模組，然後選取 **[!UICONTROL 添加錯誤處理程式]**:

   ![](assets/error-handler-route.png)

   模組會顯示指令清單以及您的案例中使用的應用程式。

1. 如果向添加錯誤處理程式的模組是路由中的最後一個模組，請選擇其中一個指令。

   或

   向錯誤處理程式路由添加一個或多個模組。

   如果向路由添加更多模組，則 [!UICONTROL 忽略] 預設會套用指令，而如果發生錯誤，則會處理該路由上的後續模組。


>[!INFO]
>
>在此範例中，如果執行 [!UICONTROL 建立資料夾] 模組， [!UICONTROL 忽略] 指令將自動應用，並且方案將移至錯誤處理程式路由上的下一個模組。
>
>但是，如果沒有錯誤，案例會移至 [!UICONTROL 列出資料夾模組中的所有檔案] 在常規路線上。
>
>![](assets/if-there-is-no-error-350x234.png)

請注意，錯誤處理路由由透明圓組成，而常規路由由實心圓組成。

## 處理指令時出錯

這些指示在下文中作了簡要說明。 如需詳細資訊，請參閱 [錯誤處理指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

根據方案執行是否應繼續，總共有五個指令可分為以下類別。

以下指令確保方案執行繼續：

* **[!UICONTROL 繼續]**:可讓您指定有錯誤的模組替代輸出。 方案執行狀態會標示為成功
* **[!UICONTROL 忽略]**:會忽略錯誤。 方案執行狀態會標示為成功
* **[!UICONTROL 插播]**:將輸入儲存到未完成執行的隊列。 方案執行狀態標籤為警告。 如需詳細資訊，請參閱 [在中檢視並解決未完成的執行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

如果發生錯誤時應停止執行方案，請使用以下指令之一：

* **[!UICONTROL 回復]**:立即停止方案執行並將其狀態標籤為錯誤
* **[!UICONTROL 提交]**:立即停止方案執行並將其狀態標示為成功

有關錯誤處理的詳細資訊，請參閱：

* [錯誤處理指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [中的進階錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)