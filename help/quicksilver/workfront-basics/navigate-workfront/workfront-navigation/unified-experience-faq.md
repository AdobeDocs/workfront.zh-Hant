---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Adobe統一體驗常見問題集
description: 以下幾項功能不同： [!DNL Workfront] 和Adobe Experience Cloud，你可能有些問題 [!DNL Workfront] 例項會移轉至統一的體驗。
author: Lisa
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] 常見問題集

此 [!DNL Adobe Unified Experience] for [!DNL Workfront] 可讓您管理 [!DNL Adobe] 只需一次登入，即可將應用程式整合在一個位置。 此 [!DNL Adobe] 導航區與 [!DNL Workfront]. 有些功能不同，您可能會有一些問題 [!DNL Workfront] 例項會移轉至統一的體驗。

如需登入的相關資訊，請參閱 [!DNL Adobe Unified Experience]，請參閱 [[!DNL Adobe Unified Experience] for [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## 比較 [!DNL Adobe Unified Experience] 和 [!DNL Workfront only] 體驗

僅限使用 [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] 可以存取 [!DNL Adobe Unified Experience]. 尚未移轉的客戶將看到 [!DNL Workfront only] 體驗，無法切換 [!DNL Adobe] 應用程式。

此表格說明兩種體驗之間不同的部分功能。

| [!DNL Adobe Unified Experience] | [!DNL Workfront] 僅限體驗 |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] 主菜單] 在左側 ![主菜單](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] 主菜單] 在右側 ![主菜單](assets/main-menu-icon.png) |
| 單一登入URL可供所有使用 [!DNL Adobe Experience Cloud] 應用程式 | 登入 [!DNL Workfront] 自訂 [!DNL Workfront] URL |
| 「組織切換器」可讓您在 [!DNL Workfront] 組織與環境 | 無法使用「組織切換器」 |
| 導航包括用於 [!DNL Adobe] 產品， [!DNL Adobe] 通知、說明和您的使用者設定檔， [!DNL Workfront] 導覽列 | 導覽包含 [!DNL Workfront] 僅限導覽列 |
| 可透過 [!UICONTROL 主菜單] 上方導覽區域 | 可透過 [!UICONTROL 主菜單] 和 [!DNL Workfront] 導覽列 |

{style=&quot;table-layout:auto&quot;}

## 常見問題

**如何進一步了解 [!DNL Adobe Admin Console]?**

如需 [!DNL Admin Console]，請檢閱以下文章：

* [為 [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [平台管理差異([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] 概述](https://helpx.adobe.com/tw/enterprise/using/admin-console.html)

**身為客戶，我需要做什麼來促進移轉？**

將與現有客戶聯繫以安排遷移。 移轉團隊支援同事將引導客戶完成此流程，並提供相關建議 [!DNL Admin Console] 設定，並提供所需檔案的連結，讓移動盡可能簡單且輕鬆。

* [[!DNL Adobe Workfront] 支援概述](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] 資訊](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] and [!DNL Admin Console] 常見問題集](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

**您的處理方式 [!DNL Adobe Admin Console] 針對已啟用此功能的公司，以不同於 [!DNL Workfront] SSO已設定？**

[!DNL Adobe Admin Console] 可選擇包含 [!DNL Workfront]，以IMS取代SSO 所有使用者布建都會在 [!DNL Admin Console]，使用者將會看到 [!DNL Adobe] 登入畫面 [!DNL Experience Cloud] 他們將看到 [!DNL Workfront] 作為選項（如果他們有權存取）。

**這對已擁有AEM管理面板的客戶有何影響 [!DNL Adobe Assets]  — 但SSO的設定方式與[!DNL Workfront?]**

一次 [!DNL Workfront] 新增為 [!DNL Admin Console] 應用程式時，您不應為 [!DNL Workfront] 以利用您 [!DNL Adobe Assets].

**這對使用SSO設定的使用者有何影響？**

SSO是在 [!DNL Admin Console] 並由 [!DNL Workfront] 應用程式。

**是單一登入(SSO)，與我們的內部 [!DNL Active Directory] 還是IMS的選項？**

IMS取代了SSO，且功能大致相同。 所有使用者權限皆已授予，且已布建於 [!DNL Adobe Admin Console]，而使用者將看到 [!DNL Adobe] 登入畫面，可以選擇「[!UICONTROL 個人帳戶]&quot;或&quot;[!UICONTROL 公司帳戶]」登入(若 [!DNL Active Directory]，大部分都會使用公司帳戶登入)。

**對於未使用SSO的使用者， [!DNL Workfront] 登入URL是否變更？**

登入URL會變更；不過，舊的URL會重新導向至新的登入URL，因此您應重新訓練使用者前往的位置。

**我們設定的別名是否仍然有效？ [!DNL Workfront] 連結隨此移轉而變更？**

[!DNL Workfront] 重新導向/別名可用來存取首頁。

**重新導向是否會在某個時間停用？ 或者，我們是否總能在my.company.workfront.com中輸入內容？**

您將可以一律使用任何自訂URL。 按一下任何這些連結後，它會將您導向 [!DNL Workfront] 和顯示不同的URL。 但是，這樣更好 [!DNL experience] 若要登入experience.adobe.com，並將連結從內建立書籤 [!DNL Experience Cloud]. 重新導向的次數越少，延遲時間/載入時間就越少。

**到請求佇列的直接連結是否會中斷？**

所有直接連結應會重新導向至新的URL模式。 不過，如果您已將連結分發給人員，則應傳送更新以運用直接連結，並防止延遲前往預期的頁面。

**我們是否會移轉至 [!DNL Experience Cloud] 是否可針對特定使用者(並非所有使用者都使用其他Adobe產品)進行全域選取？**

整個 [!DNL Workfront] 客戶帳戶將會移轉。 無法依使用者個別執行。

**全部 [!DNL Workfront] 使用者必須透過 [!DNL Experience Cloud]? 還是只是管理員？**

是，所有使用者都會透過 [!DNL Experience Cloud]. IMS登入將取代SSO。 這是非常類似的體驗，只是不同的登入畫面。

**使用者是否必須連結 [!DNL Adobe] 帳戶 [!DNL Workfront] 帳戶（如果他們已同時擁有兩者）?**

是的，此過程會一併提供，當您的組織需要移轉至IMS時，將會提供更多詳細資訊。

**對 [!DNL Workfront] 沒有 [!DNL Adobe] 帳戶？**

未獲授權存取的使用者 [!DNL Adobe Admin Console] 進入 [!DNL Workfront] 必須建立「[!UICONTROL 個人帳戶]&quot;或 [!DNL Adobe] ID帳戶才能登入。 這會傳送電子郵件給管理員，以核准或拒絕其請求，此外還可讓管理員設定該使用者擁有的存取類型。 登入後，會前往experience.adobe.com，輸入其電子郵件地址，然後選擇 [!UICONTROL 個人帳戶]. 從那裡，他們就能 [!DNL Workfront].

**如果我們沒有 [!DNL Adobe] 產品[!DNL Workfront?]**

仍建議您的組織移轉至 [!DNL Adobe Unified Experience]. 您會收到 [!DNL Adobe] ID以及上述優點。

**我們的 [!DNL Workfront] 例項。 我們不希望他們存取 [!DNL Adobe]. 如何在主控台中限制其存取權？**

[!DNL Admin Console] 可讓管理員對使用者可存取和無法存取的項目有大量控制權。 每當外部使用者想要存取時，就需要建立 [!DNL Adobe] ID，會傳送電子郵件給管理員。 然後管理員可以接受或拒絕對產品的存取，並定義他們可以/無法存取該組織擁有之產品的權限。 然後， [!DNL Workfront] 系統管理員可以 [!UICONTROL 使用者] 區域 [!DNL Workfront] 為外部使用者提供更精細的權限。

**群組管理員可用來建立 [!DNL Workfront]. 移至 [!DNL Experience Cloud]，群組管理員仍可以建立人員嗎？**

是，您仍可透過 [!DNL Workfront]. 可將這些使用者新增至 [!DNL Experience Cloud] 自動。 您也可以在 [!DNL Admin Console] 允許他們指派 [!DNL Workfront] 至使用者。

**切換到的截止日期是多少 [!DNL Experience Cloud]?**

目前沒有移至 [!DNL Adobe Experience Cloud]. 我們與客戶合作，讓客戶在準備好行動時做出選擇。

**我們的支援團隊是否需要為此變更採取任何行動？**

如果支援團隊負責建立新使用者，則他們需要熟悉 [!DNL Admin Console] 用於建立使用者及將權限指派給Workfront的介面。 否則，您的內部支援團隊可能不會有重大變更。

**這對透過API功能進行的整合有何影響？**

現有的URL路徑將繼續可供API流量使用。 您不需要執行任何動作來更新整合中的端點。 不過，不支援透過使用者名稱和密碼直接登入 — 您必須使用API金鑰，但例外是 [!DNL Workfront Fusion] 連接器。

**那 [!DNL Creative Cloud] 使用者？ 移轉會如何影響他們？ 他們有什麼好處嗎？**

對 [!DNL Creative Cloud] 移轉至的使用者 [!DNL Adobe Unified Experience].

**是否登入 [!DNL Workfront] 行動使用者？**

[!DNL Workfront] 行動使用者不應受移轉至的影響 [!DNL Adobe Unified Experience].
