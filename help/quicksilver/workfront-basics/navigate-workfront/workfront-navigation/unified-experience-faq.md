---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Adobe Unified Experience常見問題集
description: ' [!DNL Workfront] 和Adobe Experience Cloud的一些功能不同，當您將 [!DNL Workfront] 執行個體移轉至統一體驗時，可能會有一些問題。'
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1385'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience]常見問題集

[!DNL Workfront]的[!DNL Adobe Unified Experience]可讓您透過單一登入在一個位置管理所有[!DNL Adobe]應用程式。 [!DNL Adobe]導覽區域與[!DNL Workfront]緊密整合。 有些功能不同，當您將[!DNL Workfront]執行個體移轉至統一體驗時，可能會有一些問題。

如需有關如何登入[!DNL Adobe Unified Experience]的資訊，請參閱 [!DNL Workfront][&#128279;](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)的[!DNL Adobe Unified Experience] 。

## [!DNL Adobe Unified Experience]與[!DNL Workfront only]體驗的比較

只有使用[!DNL Adobe Business Platform] / [!DNL Adobe Admin Console]的客戶才能存取[!DNL Adobe Unified Experience]。 尚未移轉的客戶將會看到[!DNL Workfront only]體驗，無法在[!DNL Adobe]個應用程式之間切換。

此表格說明兩個體驗之間的一些不同功能。

| [!DNL Adobe Unified Experience] | 僅[!DNL Workfront]體驗 |
| ---- | ----|
| [!UICONTROL [!DNL Workfront]主功能表]位於左側![主功能表](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront]主功能表]位於右側![主功能表](assets/main-menu-icon.png) |
| 所有[!DNL Adobe Experience Cloud]應用程式都可以使用單一登入URL | 使用自訂[!DNL Workfront] URL登入[!DNL Workfront] |
| 「組織切換器」可讓您在[!DNL Workfront]組織和環境之間移動 | 「組織切換器」無法使用 |
| 導覽除了包含[!DNL Workfront]導覽列之外，還包含[!DNL Adobe]產品、[!DNL Adobe]通知、說明和您的使用者設定檔的頂層導覽區域 | 導覽僅包含[!DNL Workfront]導覽列 |
| 可透過[!UICONTROL 主功能表]和頂端導覽區域存取說明 | 可透過[!UICONTROL 主功能表]與[!DNL Workfront]導覽列存取說明 |
| 校訂檢視器會在新標籤中開啟 | 校訂檢視器會在Workfront中開啟 |
| 用來存取Workfront的URL為`experience.adobe.com` | 用來存取Workfront的URL為`(CompanyName).my.workfront.com` |
| 日期格式（例如YYYY/MM/DD）是以Unified Experience語言設定為基礎。 如果使用者尚未更新其語言設定，則會使用`en-US`設定。 | 日期格式（例如YYYY/MM/DD）是根據瀏覽器偏好設定 |

{style="table-layout:auto"}

## 常見問題集

### 如何判斷我使用的是Adobe Unified Experience還是Adobe Workfront？

若要判斷您的組織是否位在Adobe統一體驗上，請檢查您用來存取Workfront的URL。

| URL | Adobe體驗 |
|------------|------------|
| （公司名稱）.my.workfront.com | Workfront體驗 |
| experience.adobe.com | Adobe Unified Experience |

### 如何進一步瞭解[!DNL Adobe Admin Console]？

如需[!DNL Admin Console]的相關資訊，請檢閱下列文章：

* [準備 [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [平台式管理差異([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] 總覽](https://helpx.adobe.com/tw/enterprise/using/admin-console.html)

### 身為客戶，我需要做什麼來促進移轉？

將會聯絡現有客戶以排程移轉。 移轉團隊支援同事將引導客戶完成程式、建議[!DNL Admin Console]設定，並提供必要的檔案連結，讓移轉過程儘可能簡單且輕鬆自在。

* [[!DNL Adobe Workfront] 支援概述](https://experienceleague.adobe.com/zh-hant/docs/customer-one/using/workfront/overview)
* [[!DNL Workfront Admin Console] 資訊](https://experienceleague.adobe.com/zh-hant/docs/customer-one/using/workfront/landing)
* [[!DNL Adobe Business Platform] 和 [!DNL Admin Console] 常見問題集](https://experienceleague.adobe.com/zh-hant/docs/customer-one/using/workfront/faq)

### 對於已為Federated ID啟用此功能與已設定[!DNL Workfront] SSO不同功能的公司，您如何處理[!DNL Adobe Admin Console]？

[!DNL Adobe Admin Console]可選擇包含[!DNL Workfront]，將SSO取代為IMS。 所有使用者布建作業都會在[!DNL Admin Console]中進行，且使用者會看到[!DNL Adobe]登入畫面以存取[!DNL Experience Cloud]，並在其中看到[!DNL Workfront]選項（如果使用者被授予存取權）。

### 這對已擁有[!DNL Adobe Assets]的AEM管理面板的客戶有何影響 — 但SSO的設定與[!DNL Workfront?]不同

將[!DNL Workfront]新增為[!DNL Admin Console]應用程式後，您就不必再為[!DNL Workfront]執行任何其他動作，即可使用您為[!DNL Adobe Assets]設定的現有SSO設定。

### 這對使用SSO設定的專案有何影響？

SSO是在[!DNL Admin Console]中設定，並由[!DNL Workfront]應用程式繼承。

### 我們的內部[!DNL Active Directory]的SSO是否仍會是IMS的選項？

IMS是SSO的替代品，其功能大致相同。 所有使用者許可權皆已在[!DNL Adobe Admin Console]中授與及布建，且使用者會看到[!DNL Adobe]登入畫面，使用者可在其中選擇&quot;[!UICONTROL 個人帳戶]&quot;或&quot;[!UICONTROL 公司帳戶]&quot;登入（如果您有[!DNL Active Directory]，則大部分使用者會使用公司帳戶登入）。

### 對於未使用SSO的使用者，[!DNL Workfront]登入URL是否會變更？

登入URL將會變更，但舊的URL將會重新導向至新的登入URL，因此您應該重新訓練使用者前往何處。

### 我們設定的別名是否仍有效，或[!DNL Workfront]個連結是否會隨著此移轉而變更？

有[!DNL Workfront]個重新導向/別名可存取首頁。

### 重新導向是否將會停用？ 或者，我們永遠都可以輸入my.company.workfront.com嗎？

您一律可以使用任何自訂URL。 按一下這些連結中的任何一個，它都會將您導向至[!DNL Workfront]並顯示不同的URL。 不過，最好是[!DNL experience]登入experience.adobe.com，並將連結從[!DNL Experience Cloud]內加入書籤。 減少重新導向等於減少延遲時間/載入時間。

### 要求佇列的直接連結會中斷嗎？

所有直接連結都應重新導向至新的URL模式。 不過，如果您已將連結分送給人員，則應傳送更新以運用直接連結，並防止延遲進入預期頁面。

### 我們會在全域移轉至[!DNL Experience Cloud]嗎？還是可以為某些使用者(並非所有使用者都使用其他Adobe產品)進行選擇？

將移轉整個[!DNL Workfront]客戶帳戶。 無法逐個使用者完成。

### 所有[!DNL Workfront]使用者都必須透過[!DNL Experience Cloud]登入嗎？ 還是僅管理員？

是，所有使用者將透過[!DNL Experience Cloud]登入。 IMS登入將會取代SSO。 這是非常類似的體驗，只是不同的登入畫面。

### 如果使用者已經同時擁有其[!DNL Adobe]帳戶和[!DNL Workfront]帳戶，使用者必須將其帳戶連結到這兩個帳戶嗎？

是的，有一個程式，當您的組織需要移至IMS時，將會提供更多詳細資料。

### 沒有[!DNL Adobe]帳戶的[!DNL Workfront]使用者會發生什麼事？

尚未在[!DNL Adobe Admin Console]中取得存取許可權以登入[!DNL Workfront]的使用者必須建立「[!UICONTROL 個人帳戶]」或[!DNL Adobe] ID帳戶才能登入。 這會傳送電子郵件給管理員，要求核准或拒絕其要求，並且可讓管理員設定該使用者具有的存取權型別。 登入時，會前往experience.adobe.com，輸入電子郵件地址，然後選擇[!UICONTROL 個人帳戶]。 他們可從此處存取[!DNL Workfront]。

### 如果我們沒有[!DNL Workfront?]以外的任何[!DNL Adobe]產品，該怎麼辦

仍建議您的組織移轉至[!DNL Adobe Unified Experience]。 您將會收到[!DNL Adobe] ID以及上方列出的優點。

### 我們的[!DNL Workfront]執行個體中包含外部使用者。 我們不希望他們能存取[!DNL Adobe]中包含的任何其他產品。 我們如何限制使用者在主控台中的存取權？

[!DNL Admin Console]可讓管理員充分控制使用者可以和無法存取的專案。 當外部使用者想要存取時，他們需要建立[!DNL Adobe] ID，這會傳送電子郵件給管理員。 然後，管理員可以接受或拒絕對產品的存取權，並定義他們可以/無法存取該組織所擁有之產品的內容。 然後，[!DNL Workfront]系統管理員可以進入[!DNL Workfront]的[!UICONTROL 使用者]區域，為外部使用者提供更細微的許可權。

### 群組管理員是用來在[!DNL Workfront]中建立人員。 移至[!DNL Experience Cloud]後，群組管理員是否仍可建立人員？

可以，仍可透過[!DNL Workfront]建立使用者。 這些使用者可以自動新增到[!DNL Experience Cloud]。 您也可以在[!DNL Admin Console]中將群組管理員設定為產品擁有者，讓他們將[!DNL Workfront]指派給使用者。

### 切換至[!DNL Experience Cloud]的截止日期為何？

目前沒有移至[!DNL Adobe Experience Cloud]的期限。 我們正在與客戶合作，讓他們選擇何時準備好進行遷移。

### 我們的支援團隊需要為此變更執行任何操作嗎？

如果支援團隊負責建立新使用者，則他們必須熟悉用來建立使用者及將權益指派給Workfront的[!DNL Admin Console]介面。 否則，您的內部支援團隊可能不會發生重大變更。

### 這對透過API函式進行的整合有何影響？

現有的URL路徑將可繼續用於API流量。 您不需要執行任何動作，即可更新整合中的端點。 但是，不支援透過使用者名稱和密碼直接登入 — 您必須使用API金鑰，但[!DNL Workfront Fusion]聯結器除外。

### [!DNL Creative Cloud]位使用者呢？ 移轉對它們有何影響？ 這對他們是否有任何好處？

移轉至[!DNL Adobe Unified Experience]對[!DNL Creative Cloud]個使用者沒有影響。

### [!DNL Workfront]個行動使用者的登入是否會變更？

移轉至[!DNL Adobe Unified Experience]時，不應影響[!DNL Workfront]行動使用者。

### JumpSeat無法搭配[!DNL Adobe Unified Experience]使用，我該如何解決這個問題？

JumpSeat可與[!DNL Adobe Unified Experience]搭配使用，但需要設定更新。 使用JumpSeat管理面板，將應用程式URL從`workfront.com`變更為以`.workfront.adobe.com`結尾
