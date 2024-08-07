---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在 [!DNL Adobe Workfront Fusion]中建立簡單案例
description: 瞭解如何使用Adobe Workfront Fusion建立簡單的自動化案例。 自動化案例可自動化Workfront程式，包括資料操縱和轉換。 此範例將引導您完成建立情境的過程，該情境會搜尋問題然後轉換為專案。
author: Becky
hide: true
hidefromtoc: true
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '1260'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中建立基本情境

[!DNL Adobe Workfront Fusion]的角色是自動化您的程式，以便您可以專注於新任務，而不是一遍又一遍地重複相同的任務。 其運作方式是連結應用程式和服務內外的動作，以建立自動傳輸和轉換資料的情境。 您建立的案例會監視應用程式或服務中的資料，並處理該資料以提供您想要的結果。

此範例將帶您進行建立情境的過程，該情境會在Workfront中搜尋問題，並將其轉換為專案。

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## 建立實務情境

### 開始建立情境

1. 在&#x200B;**案例**&#x200B;區域中，按一下&#x200B;**建立新案例**。

   <!--To locate the Scenarios area, see navigation article-->

   情境編輯器隨即顯示，其中心包含一個空白模組。

   <!--picture?-->

1. 選取左上角的&#x200B;**[!UICONTROL 新案例]**&#x200B;預留位置名稱，然後輸入名稱。
1. 繼續[新增並設定下列第一個模組](#add-and-configure-the-first-module)。

### 新增並設定第一個模組

1. 按一下空白模組，以選擇要從中選取模組的應用程式。

   應用程式清單會顯示在模組右側。

1. 選取&#x200B;**[!DNL Adobe Workfront]**。 如果看不到，請按一下清單底部的搜尋列，輸入「Workfront」，然後在清單中出現時選取它。

   清單會變更，以顯示您能使用的所有[!DNL Workfront]模組。

1. 按一下&#x200B;**[!UICONTROL 搜尋]**&#x200B;模組。

   模組組態視窗隨即開啟。

1. 在[!UICONTROL 連線]方塊中，選取您的Workfront連線。

   如果您沒有Workfront連線，請參閱[建立與 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)的連線
1. 在[!UICONTROL 記錄型別]方塊中，選取&#x200B;**[!UICONTROL 問題]**。 這會將模組設定為僅搜尋問題。

   如果您開始輸入&quot;[!UICONTROL 問題]&quot;，可以在清單中找到&#x200B;**[!UICONTROL 問題]**。

1. 在&#x200B;**[!UICONTROL 結果集]**&#x200B;方塊中，選取&#x200B;**[!UICONTROL 第一個相符記錄]**。

   這會將模組設定為只傳回它認為符合條件的第一個記錄。
1. 在&#x200B;**[!UICONTROL 搜尋條件]**&#x200B;區域中，設定條件以傳回特定問題。

   1. 在[!UICONTROL 搜尋條件]下的第一個方塊中，選取您要納入搜尋的欄位。 在此範例中，選取&#x200B;**[!UICONTROL 名稱]**。

      如果您開始輸入「[!UICONTROL 名稱]」，可以在清單中找到&#x200B;**[!UICONTROL 名稱]**。
   1. 對於運運算元，按一下&#x200B;**存在**&#x200B;旁的下拉箭頭，並將其變更為&#x200B;[!UICONTROL **包含（不區分大小寫）**]。

      如此一來，模組便可尋找名稱中包含您所選字詞的專案，即使您並未輸入完整名稱或輸入大小寫不正確（例如全部大寫）的名稱亦然。
   1. 在[!UICONTROL 搜尋條件]下的最後一個欄位中，輸入您知道位於正在搜尋問題名稱中的字詞或片語。

1. 在&#x200B;**[!UICONTROL 輸出]**&#x200B;清單中，選取您要模組輸出的欄位。 在此範例中，請選取&#x200B;**[!UICONTROL ID]**&#x200B;和&#x200B;**[!UICONTROL Name]**&#x200B;欄位。

   >[!TIP]
   >
   >您可以使用&#x200B;**Cmd+F** （[!DNL Mac]個作業系統）或&#x200B;**Ctrl-F** （[!DNL Windows]個作業系統）來快速尋找欄位。

1. 按一下&#x200B;**[!UICONTROL 確定]**&#x200B;以儲存模組組態。

1. 以滑鼠右鍵按一下模組，按一下&#x200B;**[!UICONTROL 重新命名]**，然後輸入描述您希望模組執行的作業的名稱（例如「搜尋問題」），然後按一下&#x200B;**[!UICONTROL 確定]**。

   名稱會出現在模組正下方。 在其下方，[!DNL Workfront Fusion]包含模組所執行之動作型別的簡短說明。

   ![](assets/)

1. 繼續[新增並設定第二個模組](#add-and-configure-the-second-module)。

## 新增並設定第二個模組

1. 暫留在模組右側的部分圓圈上，然後按一下[新增其他模組]****。
1. 從應用程式清單中選取[!DNL Adobe Workfront]，然後選擇模組&#x200B;**[!UICONTROL 其他動作]**。

   其他動作模組可讓您在Workfront中執行沒有專用模組的動作。 在此範例中，此模組用於將問題轉換為專案。
1. 在「[!UICONTROL 連線]」欄位中，選取您在上一個模組中使用的相同Workfront連線。
1. 在**[!UICONTROL 記錄型別]**欄位中，選取&#x200B;**[!UICONTROL 問題]**，因為要執行的動作與問題有關。
1. 在&#x200B;**[!UICONTROL 動作]**&#x200B;欄位中，選取&#x200B;**convertToProject**。 此動作會將所選問題轉換為專案。
1. 按一下&#x200B;**[!UICONTROL ID]**&#x200B;欄位。

   畫面會隨即開啟，您可在其中選取要當作專案問題識別碼使用的專案。 面板包含任何先前模組的輸出。 由於您選取ID作為前一個模組的輸出，因此現在面板中可提供該ID。

   此面板稱為對應面板。 如需對應面板的詳細資訊，請參閱[將資訊從一個模組對應到另一個模組](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)。
1. 在對應面板中選取&#x200B;**ID**。

   ID區塊會顯示在ID欄位中。 其中顯示對應自該模組的編號，以及對應的欄位。

   ![地圖ID](assets/map-id.png)

1. （可選）在專案區段中，找出擁有者ID欄位，並在欄位中開始輸入您的名稱，然後在其出現時選取它。 這會將您設為專案的所有者，並可讓您更輕鬆地在Workfront中找到。

   >[!TIP]
   >
   >您可以使用&#x200B;**Cmd+F** （[!DNL Mac]個作業系統）或&#x200B;**Ctrl-F** （[!DNL Windows]個作業系統）來快速尋找欄位。

1. 按一下&#x200B;**[!UICONTROL 確定]**&#x200B;以儲存模組組態。

1. 以滑鼠右鍵按一下模組，按一下&#x200B;**[!UICONTROL 重新命名]**，然後輸入描述您希望模組執行之作業的名稱（例如「轉換為專案」），然後按一下&#x200B;**[!UICONTROL 確定]**。

1. 繼續[測試情境](#test-the-scenario)。

## 測試情境

在啟動情境之前，請務必執行情境至少一次，並檢視結果，以測試情境。 這有助於您瞭解資料如何流經此情境並找出任何錯誤。

對於這種情況，成功的測試將導致找到問題並將其轉換為專案。

1. 按一下案例編輯器左下角的&#x200B;**[!UICONTROL 執行一次]**。
1. 情境執行完畢後，按一下第一個模組上方的泡泡圖，即可檢視模組處理之資料束的相關資訊，包括從模組傳回的問題提取的資料。

1. 按一下第二個模組上方的執行檢測器泡泡圖，以檢視輸入（問題）和輸出（轉換的專案）。

   如需檢查泡泡中資料的詳細資訊，請參閱：

   * 如需一般資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)中的[案例執行流程。
   * 如需已處理組合的相關資訊，請參閱[案例執行、週期以及 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中的階段。

1. 在[!DNL Workfront Fusion]中，按一下左下角附近的&#x200B;**[!UICONTROL 儲存]**，以儲存您的情境進度。

   >[!IMPORTANT]
   >
   >隨時儲存並測試情境。

>[!TIP]
>
>我們建議您選擇加入每個模組相關附註的作法，但此作法相當實用。
>
>1. 以滑鼠右鍵按一下[!DNL Workfront]模組，然後按一下&#x200B;**[!UICONTROL 新增附註]**。
>1. 在顯示的附註中，輸入模組的概觀。
>
>    您可以為一個模組新增多個附註。
>
>1. 關閉&#x200B;**[!UICONTROL 附註]**&#x200B;區域。
>
>     將附註新增至情境後，情境編輯器底部的&#x200B;**[!UICONTROL 附註]**&#x200B;圖示![](assets/notes-icon-w-dot.png)上會顯示橘色點。
>
>1. 按一下&#x200B;**[!UICONTROL 附註]**&#x200B;圖示![](assets/notes-icon-w-dot.png)以檢視您的附註。
>

## 啟動情境

建立情境的最後一步是啟動情境。

由於此情境正在搜尋特定問題，因此不需要啟用它。 啟用情境會使情境依排程執行，或當應用程式中發生特定動作時執行。 啟用案例後，預設會每15分鐘執行一次。 您可以定義何時以及多久執行一次來變更此專案。

如需啟用案例的詳細資訊，請參閱[在[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)中啟用或停用案例。

如需排程的相關資訊，請參閱[在[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)中排程情境。
