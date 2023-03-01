---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在中執行報表 [!DNL Workfront Proof]
description: Workfront Proof可讓您檢視報表，以追蹤團隊的工作進度和效率。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# 在中執行報表 [!DNL Workfront Proof]


>[!IMPORTANT]
>
>* <span class="previe">中不再提供報表功能 [!DNL Workfront Proof]. 報表標籤仍會顯示，但資料不準確。</span>
> 
>* 本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).


Workfront Proof可讓您檢視報表，以追蹤團隊的工作進度和效率。

您可以輕鬆檢視中建立的校樣數 [!DNL Workfront Proof] 帳戶、每個校樣關聯的版本數、週轉時間等。

## 必要條件

報表是否可用取決於您的 [!DNL Workfront Proof] 帳戶和使用者權限層級。

* [帳戶必要條件](#account-prerequisites)
* [使用者必要條件](#user-prerequisites)

### 帳戶必要條件 {#account-prerequisites}

報表資訊僅適用於Premium計畫。

### 使用者必要條件 {#user-prerequisites}

報表資訊僅適用於擁有帳戶上所有校樣的完整存取權的使用者(亦即至少具有 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md))。

在此面板中，您可以

* 控制顯示資料的時間範圍
* 分析量度隨時間的變更
* 將滑鼠暫留在所選時間點上，以檢查其詳細資訊
* 檢查在所選時間範圍內建立的校樣總數
* 檢查完成的校樣集中包含的平均版本數

## 檢視報表 {#viewing-reports}

1. 前往 **[!UICONTROL 控制面板]** 頁面。
1. 按一下 **[!UICONTROL 報表]** 標籤。\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. 在 **[!UICONTROL 時間範圍]** 下拉式功能表，選取您要顯示過去24小時、7天、30天、90天或自訂時段內所建立之校樣的相關資訊。\
   如果您選取自訂時段，請選取開始和結束日期，然後按一下 **[!UICONTROL 套用]**.\
   系統會針對您選取的時段顯示下列資訊：\
   **已建立校樣：** 在所選時段內建立的校樣數。\
   **每個校樣的版本：** 在所選時段內，所有已完成校樣（已核准或已核准且有變更）的每個校樣的平均版本數。\
   **轉過身來：** 從建立第一個版本到決定最終版本的平均時間。\
   **首次活動時間：** 從建立校樣到校樣上第一個活動的平均時間。\
   **延遲校樣：** 至少有一個版本在所選時段內延遲的已完成校樣（已核准或已核准且有變更）的平均百分比。\
   **評論和答復：** 在所選時段內對所有校樣發表的意見和回覆的平均數量。

1. （選用）選取或取消選取 **[!UICONTROL 顯示最小 — 最大範圍]** 選項，以判斷圖形中是否顯示最小值和最大值。\
   選取此選項時，在記錄的最小值和最大值之間顯示藍色底紋。

1. （選用）您可以篩選顯示的資料，如 [篩選報表](#filtering-reports).

## 篩選報表 {#filtering-reports}

依預設，報表中顯示的資料包含 [!DNL Workfront Proof] 系統。 您可以使用篩選條件來僅顯示與您的需求相關的資訊。

若要篩選報表資訊：

1. 前往 **[!UICONTROL 控制面板]** 頁面。
1. 按一下 **[!UICONTROL 報表]** 標籤。\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. 執行報表，如 [檢視報表](#viewing-reports).
1. 按一下 **[!UICONTROL 篩選]**.

1. 在頁面左側，從下列篩選選項中選取：\
   **[!UICONTROL 校樣類型]:** 選取要納入報表的校樣類型。\
   **[!UICONTROL 決策]:** 選取選項，以判斷是否只進行包含特定決策的校樣。\
   **[!UICONTROL 收件者]:** 選取個別使用者，以檢視與所選使用者共用之校樣相關的資訊。\
   **[!UICONTROL 校樣擁有者]:** 選取個別使用者，以檢視與所選使用者擁有之校樣相關的資訊。\
   **[!UICONTROL 證明建立者]:** 選取個別使用者，以檢視與所選使用者建立之校樣相關的資訊。\
   **[!UICONTROL 帳戶]:** 選取您要納入報表的帳戶。

1. 按一下 **[!UICONTROL 套用]**.
1. （選用）選取或取消選取 **[!UICONTROL 顯示最小 — 最大範圍]** 選項，以判斷圖形中是否顯示最小值和最大值。\
   選取此選項時，在記錄的最小值和最大值之間顯示藍色底紋。

## 列印報表

1. 前往 **[!UICONTROL 控制面板]** 頁面。
1. 按一下 **[!UICONTROL 報表]** ，然後按一下 **[!UICONTROL 列印]**.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. 從可用的各種打印選項中選擇。\
   列印選項會依您使用的瀏覽器和瀏覽器版本而有所不同。
