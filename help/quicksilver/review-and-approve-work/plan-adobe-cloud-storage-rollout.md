---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: 規劃您的Adobe雲端儲存空間轉出
description: 選擇Adobe雲端儲存空間對使用者的顯示方式，透過單一群組進行試點，並安排工作順序，讓稽核者、核准者和專案所有者不會有任何意外。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
exl-id: b4413742-c250-4110-9097-6d38842355a4
source-git-commit: 2b5d95ed0a5c72062700bf026a18b8301e4be421
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 0%

---
# 規劃您的Adobe雲端儲存空間轉出

您可以決定Adobe雲端儲存空間如何及何時抵達您的使用者。 在Workfront管理員將Adobe雲端儲存空間設定為設定區域中的預設儲存空間選項之前，不會有任何變更，因此您有時間在團隊中工作之前測試體驗並準備團隊。

本文會介紹您可以選擇的轉出設定、如何使用單一群組進行試驗，以及建議的工作順序。

## 選擇Adobe雲端儲存空間的推出方式

有兩個設定，您可以將其中一個套用至整個組織或特定的Workfront群組。 依預設，在Adobe雲端儲存空間上建立的每個專案都會使用統一核准和Frame.io檢視器。

如需逐步指示，請參閱[為您的組織啟用Adobe雲端儲存空間](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

### 設定選項

* **僅限Adobe雲端儲存空間**：新專案預設使用Adobe雲端儲存空間。 使用者無法建立舊版專案。
* **Adobe雲端儲存空間與舊版Workfront儲存空間**：使用者建立專案時，他們會選擇Adobe雲端儲存空間（標示為「新專案」）與舊版Workfront儲存空間（標示為「舊版儲存空間」）。 在設定區域中選取&#x200B;**允許使用者選取儲存提供者**&#x200B;核取方塊，即可啟用此選項。

>[!TIP]
>
>若要先將Adobe雲端儲存空間放在較小型的團隊前，請將任一設定套用至單一Workfront群組。 這可讓您在更廣泛地推出之前，先執行目標明確的試行方案。 我們建議從控制步調的群組層級推出開始，然後在試驗群組驗證體驗後，展開至整個組織。

現有物件會保留建立它們的儲存模型。 變更預設儲存偏好設定不會變更任何現有物件。

安裝程式中的![儲存偏好設定](assets/storage-preference-groups.png)

## 規劃您的轉出

每個Workfront環境都不同。 在您將Adobe雲端儲存空間設定為您的使用者預設之前，請先花點時間規劃組織的成功轉出情況。 以下建議並非完整的檢查清單，而是您自己計畫的起點。

### 挑選試行方案群組

群組範圍的轉出可讓您先將Adobe雲端儲存空間放在較小團隊的前面、收集意見並在更廣的轉出之前進行調整。 選擇其工作模式具有足夠代表性的群組，以便及早顯示您想要瞭解的問題。

<!--
>[!IMPORTANT]
>
>Only members of the pilot group can convert an Adobe cloud storage object, such as a request or a task, into a project. Users outside the group, including Workfront administrators, see the error "User is not eligible for this operation."
-->

### 上線前測試

Adobe雲端儲存空間可在Workfront沙箱環境中使用，因此您可以在生產之前驗證大部分體驗。 Frame.io檢視器無法在沙箱中使用，因此您可以與試驗群組一起驗證生產環境中的完整檢閱和核准體驗。 如需詳細資訊，請參閱[為您的組織啟用Adobe雲端儲存空間](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

### 將變更傳達給一般使用者

檢閱者、核准者和專案所有者所看到的最大變更是新的「檔案」區域和Frame.io檢視器，它們可支援Adobe雲端儲存體專案的檢閱和核准。 規劃您將如何推出這些產品，讓使用者瞭解在遇到第一個Adobe雲端儲存空間專案時會有什麼期望。 [開始進行統一檢閱和核准](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)文章是面向使用者的材料的實用起點。

### 檢閱您的許可權和控管

在Adobe雲端儲存空間專案中，「管理」和「貢獻」都會對應至Frame.io中的「編輯與共用」，其中包含外部共用。 在將團隊帶入Adobe雲端儲存空間之前，請先檢閱您的共用模式，並決定這是否符合您的治理模式。 如需詳細資訊，請參閱[Adobe雲端儲存空間上的不同之處](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-permissions-mapping)。

### 稽核範本和命名

Adobe雲端儲存空間會強制實施嚴格的命名規則，而Workfront會自動重新命名與其衝突的物件。 如果您從範本建立專案，請檢閱這些範本，使其產生的名稱和結構符合規則。 如需詳細資訊，請參閱[Adobe雲端儲存空間上的不同之處](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-naming-rules)。

### 圍繞Workfront Fusion進行規劃

現有的校訂型Fusion案例會繼續用於舊版專案，但不會自動用於Adobe雲端儲存空間專案。 將依賴這些情境的團隊帶入Adobe雲端儲存空間之前，請將每個情境分類為「編輯」、「重建」或「淘汰」。 如需詳細資訊，請參閱[更新Workfront Fusion的整合稽核與核准案例](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)。

### 規劃報告變更

統一的核准工作流程資料和報告會出現在畫布儀表板中。 舊版核准報告不會自動延續，因此在您的試行方案團隊需要之前，請設定替代儀表板。 如需詳細資訊，請參閱[建立報告儀表板以供檢閱和核准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)。

## 建議的順序

使用此順序作為範本，根據您的環境進行調整：

1. 在沙箱中測試體驗，並在生產環境中與試點群組測試體驗。
2. 分類並更新您的Fusion情境，並建置您的畫布儀表板報表。
3. 稽核您的範本並檢閱您的許可權和共用模型。
4. 將變更傳達給將使用該變更的稽核者、核准者和專案所有者。
5. 將Adobe雲端儲存空間設為試行方案的群組的預設值，然後在試行方案驗證體驗後，展開至更多群組或整個組織。
