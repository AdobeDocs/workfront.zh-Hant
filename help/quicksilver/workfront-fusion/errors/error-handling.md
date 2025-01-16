---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在 [!DNL Adobe Workfront Fusion]中處理錯誤
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中處理錯誤

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [新增錯誤處理](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/error-handling.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

當在執行案例期間發生錯誤時，通常是因為服務因失敗而無法使用、服務以非預期的資料回應，或輸入資料的驗證失敗。

如果模組在案例執行期間擲回錯誤，並且沒有附加到模組的錯誤處理路由，則會執行預設錯誤處理邏輯，如[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)中處理錯誤中所述。

透過將錯誤處理常式路由新增至模組，您可以將預設的錯誤處理邏輯取代為您自己的邏輯。 [!DNL Adobe Workfront Fusion]提供五種不同的指令，可在錯誤處理常式路由的結尾插入。

如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)中錯誤處理的[指示。

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

## 錯誤處理常式路由

若要將錯誤處理常式路由新增至模組：

1. 用滑鼠右鍵按一下模組並選取&#x200B;**[!UICONTROL 新增錯誤處理常式]**：

   ![](assets/error-handler-route.png)

   此模組會顯示指令清單，以及在您的情境中使用的應用程式。

1. 如果您新增錯誤處理常式的模組是路由的最後一個模組，請選取其中一個指令。

   或

   新增一或多個模組至錯誤處理常式路由。

   如果您將更多模組加入路由，預設會套用[!UICONTROL Ignore]指示詞，並在發生錯誤時，處理該路由上的後續模組。


>[!INFO]
>
>在此範例中，如果在執行[!UICONTROL 建立資料夾]模組時發生錯誤，將會自動套用[!UICONTROL Ignore]指示詞，而案例將會移至錯誤處理常式路由上的下一個模組。
>
>但是，如果沒有錯誤，則案例會移至一般路由上的[!UICONTROL 列出資料夾模組]中的所有檔案。
>
>![](assets/if-there-is-no-error-350x234.png)

請注意，錯誤處理常式路由是由透明圓組成，而一般路由是由實心圓組成。

## 處理指示時發生錯誤

這些指示詞會簡要說明如下。 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)中錯誤處理的[指示。

根據案例執行是否應該繼續，共有五個指令可以分組為下列類別。

下列指令可確保案例執行繼續進行：

* **[!UICONTROL 繼續]**：可讓您指定發生錯誤的模組替代輸出。 案例執行狀態會標籤為成功
* **[!UICONTROL 忽略]**：忽略錯誤。 案例執行狀態會標籤為成功
* **[!UICONTROL 中斷]**：將輸入儲存到未完成執行的佇列。 案例執行狀態會標示為警告。 如需詳細資訊，請參閱[檢視並解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中未完成的執行。

如果發生錯誤時，案例執行應該停止，請使用以下指令之一：

* **[!UICONTROL 回覆]**：立即停止案例執行並標示其狀態為錯誤
* **[!UICONTROL 認可]**：立即停止案例執行並將其狀態標籤為成功

如需錯誤處理的詳細資訊，請參閱：

* [在 [!DNL Adobe Workfront Fusion]中處理錯誤的指示](../../workfront-fusion/errors/directives-for-error-handling.md)
* 在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)中處理[進階錯誤