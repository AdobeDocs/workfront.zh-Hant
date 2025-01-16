---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在 [!DNL Adobe Workfront Fusion]中處理錯誤的指示
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 12%

---

# [!DNL Adobe Workfront Fusion]中錯誤處理的指示

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* 錯誤處理的[指示](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/errors/directives-for-error-handling.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

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

## 錯誤處理的指示

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>復原</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>案例執行立即停止，並且在所有模組上啟動<a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">回覆</a>階段，以嘗試將所有模組回復到其初始狀態。 後續的模組並未進行處理。</p> <p>除非有少數錯誤型別，否則在「案例」設定下指定的連續錯誤數後，就會停用案例。 如需詳細資訊，請參閱<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">連續錯誤數</a>。</p> <p>情境執行狀態標記為「錯誤」。</p> <p>注意：如果沒有將錯誤處理常式路由附加到模組，並且未勾選[！UICONTROL案例設定]下的<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[！UICONTROL允許儲存不完整的執行]</a>設定，則此為預設行為。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>認可</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>案例執行會立即停止，且所有模組上的認可階段都會開始。 後續的模組並未進行處理。</p> <p>會忽略所有未處理的組合。</p> <p>案例執行狀態會標示為「成功」。 如需有關認可階段的資訊，請參閱文章<a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Adobe Workfront Fusion中的案例執行、週期和階段</a>中的<a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">認可</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>繼續</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>指定替代輸出並提供給發生錯誤的模組。</p> <p>接著處理後續的模組。</p> <p>情境執行狀態標記為「成功」。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>忽略</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>忽略錯誤，而且不處理後續的模組。</p> <p>若有未處理的套件，情境執行將按正常情況繼續。</p> <p>情境執行狀態標記為「成功」。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>中斷</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>情境執行的狀態儲存在未完成執行作業的佇列中，而錯誤可以手動解決。如需詳細資訊，請參閱<a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">在Adobe Workfront Fusion中檢視並解決不完整的執行</a>。 </p> <p>不過，也有一些例外。 如需詳細資訊，請參閱文章<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Adobe Workfront Fusion中的案例設定面板</a>中的<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">允許儲存不完整的執行</a>。</p> <p>後續的模組並未進行處理。</p> <p>若有未處理的套件，情境執行將按正常情況繼續。</p> <p>停用[！UICONTROL自動完成執行]選項時，案例執行狀態會標示為「警告」。</p> <p>如需進一步資訊，請參閱下方的<a href="#break" class="MCXref xref">[！UICONTROL Break]</a>區段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>重試</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>在某些情況下，當失敗的原因有可能隨著時間推移而過去時，重新執行幾次失敗模組會很有用。</p> <p>Workfront Fusion目前不提供Retry指示詞，不過可採取數個因應措施來模擬其功能。 如需詳細資訊，請參閱<a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">在Adobe Workfront Fusion中重試錯誤處理</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 目前錯誤處理指示不能用於錯誤處理路由之外。
>
>   如需詳細資訊，請參閱Adobe Workfront Fusion ](../../workfront-fusion/errors/error-handling.md)中文章[錯誤處理中的[錯誤處理常式路由](../../workfront-fusion/errors/error-handling.md#error)。
>* [!DNL Workfront Fusion]目前不提供Throw模組，該模組可讓您輕鬆有條件地產生（擲回）錯誤，不過可採用因應措施來模擬其功能。
>
>   如需詳細資訊，請參閱文章[在Adobe Workfront Fusion中處理擲回錯誤](../../workfront-fusion/errors/throw.md)中的[Throw](../../workfront-fusion/errors/throw.md#workaround-for-throw)因應措施。

## 中斷 {#break}

當錯誤由[!DNL Break]指示詞處理時，會在「未完成執行」資料夾中建立記錄。 此記錄會儲存案例執行的狀態，以及先前模組的資料。 記錄會參考引發錯誤的模組，並包含模組收到哪些資料作為輸入的資訊。 對於導致錯誤的每個資料束，都會建立個別記錄。

如需詳細資訊，請參閱[在Adobe Workfront Fusion中檢視並解決不完整的執行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)。

### 解決由Break指示詞造成的錯誤

您可以手動解決錯誤，方法是更新情境（如果需要）並執行一次該情境。

您也可以設定情境，透過重新執行情境來自動處理不完整的執行。 若要設定模組以處理未完成的執行：

1. 在Break模組內，啟用&#x200B;[!UICONTROL **自動完成執行**]&#x200B;選項。
1. 在&#x200B;**嘗試次數**&#x200B;欄位中，輸入或對應您希望模組重試執行的嘗試次數上限

   此數字必須介於1到100之間。
1. 在&#x200B;**嘗試間隔**&#x200B;欄位中，輸入或對應每次重試之間的分鐘數。

啟用此選項後，當發生錯誤時，會擷取不完整的執行（在[!UICONTROL 嘗試間隔]欄位中指定的時間之後）並使用原始輸入資料執行。 這將重複執行，直到模組執行完成且沒有錯誤，或直到達到指定的嘗試次數。

>[!NOTE]
>
>如果初始重試嘗試失敗，重試間隔會每隔一次嘗試以指數方式增加。


當「自動完成執行」開啟時，案例執行會標籤為「成功」，因為Break錯誤處理常式的自動重試正在自動處理問題。 在此情況下，使用者不會收到有關失敗執行的電子郵件。

當「自動完成執行」關閉時，此執行會標示為「警告」。

在「不完整的執行」下儲存的執行有一些例外，並且由於某些錯誤型別，不可能自動重試案例執行。

如需詳細資訊，請參閱文章[Adobe Workfront Fusion中的案例設定面板](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[允許儲存不完整的執行](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow)。

如需詳細資訊，請參閱[Adobe Workfront Fusion中的進階錯誤處理](../../workfront-fusion/errors/advanced-error-handling.md)。
