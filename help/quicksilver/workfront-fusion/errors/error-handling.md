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
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 錯誤處理 [!DNL Adobe Workfront Fusion]

當執行案例期間發生錯誤時，通常是因為服務因失敗而無法使用、服務以非預期資料回應，或輸入資料驗證失敗。

>[!NOTE]
>
>如果模組在方案執行期間擲回錯誤，且沒有附加至模組的錯誤處理路由，則會依照 [中的錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

通過將錯誤處理程式路由添加到模組中，可以將預設錯誤處理邏輯替換為您自己的邏輯。 [!DNL Adobe Workfront Fusion] 提供5個不同的指令，任何指令都可插入到錯誤處理程式路由的末尾。 如需詳細資訊，請參閱 [錯誤處理指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

若要將錯誤處理程式路由新增至模組（我們將稱之為模組X），請以滑鼠右鍵按一下模組，然後選取 **[!UICONTROL 添加錯誤處理程式]**:

![](assets/error-handler-route.png)

模組會顯示指令清單以及您的案例中使用的應用程式。 如果模組X是路由中的最後一個模組，則需要選擇其中一個指令。 或者，您可以繼續將一個或多個模組添加到路由中。 在此情況下， [!UICONTROL 忽略] 預設情況下，指令將應用於模組X，如果出現錯誤，將處理該路由上的後續模組。

![](assets/directives-350x426.png)

如下所示，如果執行 [!UICONTROL 建立資料夾] 模組， [!UICONTROL 忽略] 如果篩選器「Data Error Takes Place」返回一個或多個包，則指令將自動應用，並且方案將移到錯誤處理程式路由上的下一個模組。

但是，如果沒有錯誤，案例會移至 [!UICONTROL 列出資料夾模組中的所有檔案] 在常規路線上。

![](assets/if-there-is-no-error-350x234.png)

另外，為了區分錯誤處理路由和常規路由，前者由如上所示的透明圓組成。

## 處理指令時出錯

這些指示在下文中作了簡要說明。 如需詳細資訊，請參閱 [錯誤處理指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

根據方案執行是否應繼續，總共有五個指令可分為以下類別：

以下指令確保方案執行繼續：

* **[!UICONTROL 繼續]** 可讓您指定模組的替代輸出，並顯示錯誤，且情境執行狀態會標示為成功
* **[!UICONTROL 忽略]** 只會忽略錯誤，而案例執行狀態會標示為成功
* **[!UICONTROL 插播]** 將輸入儲存到未完成執行的隊列，並且方案執行狀態標籤為警告。 如需詳細資訊，請參閱 [在中檢視並解決未完成的執行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

另一方面，如果應停止執行方案，則必須使用以下指令之一：

* **[!UICONTROL 回復]** 立即停止方案執行並將其狀態標籤為錯誤
* **[!UICONTROL 提交]** 立即停止方案執行並將其狀態標示為成功

## 其他資源

* [錯誤處理指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [中的進階錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md) (包括上述Dropbox案例的設定)
