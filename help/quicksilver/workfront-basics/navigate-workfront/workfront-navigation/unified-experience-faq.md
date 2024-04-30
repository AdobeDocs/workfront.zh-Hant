---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: AdobeUnified Experience常見問答
description: 幾項功能不盡相同，包括 [!DNL Workfront] 和Adobe Experience Cloud，因此您可能會有一些問題 [!DNL Workfront] 執行個體會移轉至整合式體驗。
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '1289'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] 常見問題集

此 [!DNL Adobe Unified Experience] 的 [!DNL Workfront] 可讓您管理所有 [!DNL Adobe] 應用程式於單一登入位置中。 此 [!DNL Adobe] 導覽區域與緊密整合 [!DNL Workfront]. 有些功能不盡相同，因此您可能會有疑問 [!DNL Workfront] 執行個體會移轉至整合式體驗。

如需有關如何登入 [!DNL Adobe Unified Experience]，請參閱 [[!DNL Adobe Unified Experience] 的 [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## 比較 [!DNL Adobe Unified Experience] 和 [!DNL Workfront only] 體驗

僅限使用 [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] 可以存取 [!DNL Adobe Unified Experience]. 尚未移轉的客戶將會看到 [!DNL Workfront only] 體驗，無法切換 [!DNL Adobe] 應用程式。

此表格說明兩個體驗之間的一些不同功能。

| [!DNL Adobe Unified Experience] | [!DNL Workfront] 僅限體驗 |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] 主要功能表] 在左側 ![主要功能表](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] 主要功能表] 在右側 ![主要功能表](assets/main-menu-icon.png) |
| 所有人都可使用單一登入URL [!DNL Adobe Experience Cloud] 應用計畫 | 登入 [!DNL Workfront] 與自訂 [!DNL Workfront] URL |
| 「組織切換器」可讓您在 [!DNL Workfront] 組織和環境 | 「組織切換器」無法使用 |
| 導覽包括頂層導覽區域，適用於 [!DNL Adobe] 產品， [!DNL Adobe] 通知、說明和您的使用者設定檔，以及 [!DNL Workfront] 導覽列 | 導覽功能包括 [!DNL Workfront] 僅導覽列 |
| 可透過存取說明 [!UICONTROL 主要功能表] 和頂端導覽區域 | 可透過存取說明 [!UICONTROL 主要功能表] 和 [!DNL Workfront] 導覽列 |

{style="table-layout:auto"}

## 常見問題集

### 如何判斷我使用的是Adobe Unified Experience還是Adobe Workfront？

若要判斷您的組織是否位在Adobe統一體驗，請檢查您用來存取Workfront的URL。

| URL | Adobe體驗 |
|------------|------------|
| （公司名稱）.my.workfront.com | Workfront體驗 |
| experience.adobe.com | Adobe統一體驗 |

### 我如何進一步瞭解 [!DNL Adobe Admin Console]？

如需關於的資訊， [!DNL Admin Console]，檢閱這些文章：

* [準備 [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [平台式管理差異([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] 概述](https://helpx.adobe.com/tw/enterprise/using/admin-console.html)

### 身為客戶，我需要做什麼來促進移轉？

將會聯絡現有客戶以排程移轉。 移轉團隊支援同事將引導客戶進行此程式，並提供建議 [!DNL Admin Console] 設定，並提供所需檔案的連結，讓移動儘可能簡單輕鬆。

* [[!DNL Adobe Workfront] 支援概述](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] 資訊](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] 和 [!DNL Admin Console] 常見問題集](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### 您的處理方式 [!DNL Adobe Admin Console] 適用於已對Federated ID啟用此功能的公司 [!DNL Workfront] 已設定SSO？

[!DNL Adobe Admin Console] 可選擇包含 [!DNL Workfront]，以IMS取代SSO。 所有使用者布建作業都會在 [!DNL Admin Console]，使用者將看到 [!DNL Adobe] 登入畫面以存取 [!DNL Experience Cloud] 他們將看到的位置 [!DNL Workfront] 作為選項（如果授予他們存取權）。

### 這對已擁有AEM管理面板的客戶有何影響 [!DNL Adobe Assets]  — 但SSO的設定方式與 [!DNL Workfront?]

一次 [!DNL Workfront] 新增為 [!DNL Admin Console] 應用程式，您就不必為下列專案執行任何其他操作 [!DNL Workfront] 以利用您擁有的現有SSO設定 [!DNL Adobe Assets].

### 這對使用SSO設定的專案有何影響？

SSO設定於 [!DNL Admin Console] 並繼承自 [!DNL Workfront] 應用程式。

### SSO與我們的內部 [!DNL Active Directory] 仍舊是IMS的選項嗎？

IMS是SSO的替代品，其功能大致相同。 所有使用者許可權皆會在中授與及布建 [!DNL Adobe Admin Console]，使用者將看到 [!DNL Adobe] 登入畫面，可從中選擇&quot;[!UICONTROL 個人帳戶]「或」[!UICONTROL 公司帳戶]」以登入(如果已 [!DNL Active Directory]，大部分使用者會使用公司帳戶登入)。

### 對於未使用SSO的使用者，會 [!DNL Workfront] 登入URL變更？

登入URL將會變更，但舊的URL將會重新導向至新的登入URL，因此您應該重新訓練使用者前往何處。

### 我們設定的別名是否仍然有效，或是 [!DNL Workfront] 連結會隨著此移轉而變更？

[!DNL Workfront] 重新導向/別名可用於存取首頁。

### 重新導向是否將會停用？ 或者，我們永遠都可以輸入my.company.workfront.com嗎？

您一律可以使用任何自訂URL。 按一下這些連結中的任何一個，系統就會將您導向至 [!DNL Workfront] 和顯示不同的URL。 不過，這樣會更好 [!DNL experience] 以登入experience.adobe.com，並將中的連結加入書籤 [!DNL Experience Cloud]. 減少重新導向等於減少延遲時間/載入時間。

### 要求佇列的直接連結會中斷嗎？

所有直接連結都應重新導向至新的URL模式。 不過，如果您已將連結分送給人員，則應傳送更新以運用直接連結，並防止延遲進入預期頁面。

### 我們會移轉至 [!DNL Experience Cloud] 全球或我們可以為特定使用者選取(並非所有使用者都使用其他Adobe產品)？

整個 [!DNL Workfront] 將會移轉客戶帳戶。 無法逐個使用者完成。

### 全部將 [!DNL Workfront] 使用者必須透過登入 [!DNL Experience Cloud]？ 還是僅管理員？

是，所有使用者都將透過以下方式登入： [!DNL Experience Cloud]. IMS登入將會取代SSO。 這是非常類似的體驗，只是不同的登入畫面。

### 使用者必須連結其 [!DNL Adobe] 帳戶至其 [!DNL Workfront] 帳戶（如果他們已經同時擁有兩者）？

是的，有一個程式，當您的組織需要移至IMS時，將會提供更多詳細資料。

### 會發生什麼事 [!DNL Workfront] 沒有 [!DNL Adobe] 帳戶？

未獲授權存取許可權的使用者 [!DNL Adobe Admin Console] 以進入 [!DNL Workfront] 必須建立「」[!UICONTROL 個人帳戶]「或 [!DNL Adobe] 能夠登入的ID帳戶。 這會傳送電子郵件給管理員，要求核准或拒絕其要求，並且可讓管理員設定該使用者具有的存取權型別。 登入時，他們會前往experience.adobe.com，輸入電子郵件地址，然後選擇 [!UICONTROL 個人帳戶]. 接著，他們便能存取 [!DNL Workfront].

### 如果我們沒有任何 [!DNL Adobe] 產品（...除外） [!DNL Workfront?]

仍建議貴組織移轉至 [!DNL Adobe Unified Experience]. 您將會收到 [!DNL Adobe] ID以及上方列出的優點。

### 我們已將外部使用者包含在 [!DNL Workfront] 執行個體。 我們不希望他們能存取包含在 [!DNL Adobe]. 我們如何限制使用者在主控台中的存取權？

[!DNL Admin Console] 可讓管理員充分控制使用者可以及無法存取的專案。 每當外部使用者想要存取時，他們都需要建立 [!DNL Adobe] ID，會傳送電子郵件給管理員。 然後，管理員可以接受或拒絕對產品的存取權，並定義他們可以/無法存取該組織所擁有之產品的內容。 然後 [!DNL Workfront] 系統管理員可以前往 [!UICONTROL 使用者] 區域 [!DNL Workfront] 為外部使用者提供更精細的許可權。

### 群組管理員是用來在中建立人員 [!DNL Workfront]. 隨著移至 [!DNL Experience Cloud]，群組管理員仍能夠建立人員嗎？

可以，使用者仍可透過以下方式建立： [!DNL Workfront]. 這些使用者可新增至 [!DNL Experience Cloud] 自動。 您也可以在下列位置將您的群組管理員設定為產品擁有者： [!DNL Admin Console] 以允許他們指派 [!DNL Workfront] 至使用者。

### 切換至的截止日期為 [!DNL Experience Cloud]？

目前沒有移至的截止日期 [!DNL Adobe Experience Cloud]. 我們正在與客戶合作，讓他們選擇何時準備好進行遷移。

### 我們的支援團隊需要為此變更執行任何操作嗎？

如果支援團隊負責建立新使用者，則他們必須熟悉 [!DNL Admin Console] 用來建立使用者及將權利指派給Workfront的介面。 否則，您的內部支援團隊可能不會發生重大變更。

### 這對透過API函式進行的整合有何影響？

現有的URL路徑將可繼續用於API流量。 您不需要執行任何動作，即可更新整合中的端點。 但是，不支援透過使用者名稱和密碼直接登入 — 您必須使用API金鑰，例外情況為 [!DNL Workfront Fusion] 聯結器。

### 那又如何 [!DNL Creative Cloud] 使用者？ 移轉對它們有何影響？ 這對他們是否有任何好處？

沒有影響 [!DNL Creative Cloud] 移轉至「 」的使用者 [!DNL Adobe Unified Experience].

### 登入次數會變更為 [!DNL Workfront] 行動使用者？

[!DNL Workfront] 行動使用者不應受移轉至「 」的影響 [!DNL Adobe Unified Experience].
