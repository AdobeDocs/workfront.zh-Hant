---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 中用於錯誤處理的指令 [!DNL Adobe Workfront Fusion]
description: 本文說明可用於錯誤處理的指令。 [!DNL Adobe Workfront Fusion] 情境。
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# 中用於錯誤處理的指令 [!DNL Adobe Workfront Fusion]

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

## 用於錯誤處理的指令

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>復原</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>案例執行會立即停止並 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">復原</a> 階段會在所有模組上啟動，以嘗試將所有模組還原成其初始狀態。 後續模組不會進行處理。</p> <p>除了一些錯誤型別，在「案例」設定下指定的連續錯誤數後，就會停用案例。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">連續錯誤數</a>.</p> <p>案例執行狀態會標示為「錯誤」。</p> <p>注意：如果沒有錯誤處理常式路由附加到模組和 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[！UICONTROL允許儲存不完整的執行]</a> 不會核取[！UICONTROL案例設定]底下的設定。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>認可</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>案例執行會立即停止，且所有模組上的認可階段都會開始。 後續模組不會進行處理。</p> <p>會忽略所有未處理的組合。</p> <p>案例執行狀態會標示為「成功」。 如需認可階段的相關資訊，請參閱 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">認可</a> 在文章中 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Adobe Workfront Fusion中的案例執行、週期和階段</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>繼續</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>會指定替代輸出，並提供給發生錯誤的模組。</p> <p>後續模組會進行處理。</p> <p>案例執行狀態會標示為「成功」。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>忽略</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>會忽略錯誤，且不會處理後續模組。</p> <p>如果有未處理的組合，情境執行會正常繼續。</p> <p>案例執行狀態會標示為「成功」。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>中斷</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>情境執行的狀態會儲存在未完成執行的佇列中，而錯誤可以手動解決。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">在Adobe Workfront Fusion中檢視和解決未完成的執行</a>. </p> <p>不過，也有一些例外。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">允許儲存未完成的執行</a> 在文章中 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Adobe Workfront Fusion中的案例設定面板</a>.</p> <p>後續模組不會進行處理。</p> <p>如果有未處理的組合，情境執行會正常繼續。</p> <p>停用[！UICONTROL自動完成執行]選項時，案例執行狀態會標示為「警告」。</p> <p>請參閱 <a href="#break" class="MCXref xref">[！UICONTROL分頁符號]</a> 區段以取得進一步資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>重試</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>在某些情況下，當失敗的原因可能隨著時間推移而過去時，重新執行幾次失敗模組會很有用。</p> <p>Workfront Fusion目前不提供Retry指令，不過可採取數個因應措施來模擬其功能。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">在Adobe Workfront Fusion中重試錯誤處理</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 目前，錯誤處理指示詞不能用於錯誤處理路由之外。
>
>   如需詳細資訊，請參閱 [錯誤處理常式路由](../../workfront-fusion/errors/error-handling.md#error) 在文章中 [Adobe Workfront Fusion中的錯誤處理](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] 目前不提供Throw模組，該模組可讓您根據條件輕鬆地產生（擲回）錯誤，不過您可以利用因應措施模擬其功能。
>
>   如需詳細資訊，請參閱 [擲回的因應措施](../../workfront-fusion/errors/throw.md#workaround-for-throw) 在文章中 [在Adobe Workfront Fusion中處理擲回錯誤](../../workfront-fusion/errors/throw.md).

## 中斷 {#break}

當錯誤由 [!DNL Break] 指示詞，即會在未完成執行資料夾中建立記錄。 此記錄會儲存案例執行的狀態，以及先前模組的資料。 記錄會參考產生錯誤的模組，並包含模組收到哪些資料作為輸入的資訊。 對於導致錯誤的每個資料組合，都會建立個別記錄。

如需詳細資訊，請參閱 [在Adobe Workfront Fusion中檢視和解決未完成的執行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### 解決Break指示詞造成的錯誤

您可以手動解決錯誤，方法是更新情境（如有需要）並執行一次。

您也可以設定情境，透過重新執行情境來自動處理不完整的執行。 若要設定模組以處理未完成的執行：

1. 在Break模組內，啟用 [!UICONTROL **自動完成執行**] 選項。
1. 在 **嘗試次數** 欄位，輸入或對應您希望模組重試執行的嘗試次數上限

   此數字必須介於1到100之間。
1. 在 **嘗試間隔** 欄位，輸入或對應每次重試之間的分鐘數。

啟用此選項後，當發生錯誤時，會擷取不完整的執行(在 [!UICONTROL 嘗試間隔] 欄位)並使用原始輸入資料執行。 這將重複執行，直到模組執行完成且沒有錯誤，或直到達到指定的嘗試次數。

>[!NOTE]
>
>如果初始重試嘗試失敗，重試間隔會每隔一次嘗試以指數方式增加。


當「自動完成執行」開啟時，案例執行會標籤為「成功」，因為Break錯誤處理常式的自動重試會自動處理問題。 在此情況下，使用者不會收到有關失敗執行的電子郵件。

當「自動完成執行」關閉時，該執行會標示為「警告」。

執行儲存在「未完成執行」下有一些例外，並且由於一些錯誤型別，無法自動重試情景執行。

如需詳細資訊，請參閱 [允許儲存未完成的執行](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) 在文章中 [Adobe Workfront Fusion中的案例設定面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

如需詳細資訊，請參閱 [Adobe Workfront Fusion中的進階錯誤處理](../../workfront-fusion/errors/advanced-error-handling.md).
