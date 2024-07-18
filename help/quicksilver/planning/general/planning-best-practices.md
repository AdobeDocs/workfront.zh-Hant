---
title: 「Adobe Workfront規劃最佳實務」
description: 身為行銷營運領導者，您可以使用Adobe Workfront Planning來組織所有團隊在行銷生命週期中的工作。 這些是我們從Workfront Planning開始建議的一些最佳實務。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d1da3ee59b074dec3e161cf1e0134aba39ad90a4
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%

---


# Adobe Workfront規劃最佳作法

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

身為行銷營運領導者，您可以使用Adobe Workfront Planning來組織所有團隊在行銷生命週期中的工作。

本文記錄了一些開始使用Workfront Planning時建議的最佳實務。

## 什麼是Workfront規劃？

Workfront規劃模組是三個相異但連結的Workfront功能之一，這些功能共同建立行銷記錄系統。 這三項功能包括：

* **規劃**： Workfront規劃中包含的新進階功能。

* **工作流程**：您目前在Workfront中使用的合作工作管理功能（專案管理、資源管理等）

* **自動化與整合**：由Workfront Fusion支援的全面整合與自動化功能。

Workfront Planning是高度可自訂的。 如需Workfront Planning術語和關鍵概念的詳細資訊，請參閱[Adobe Workfront Planning概觀](/help/quicksilver/planning/general/planning-overview.md)。

## 設定Workfront Planning前須回答的問題

熟悉Workfront Planning術語和架構後，您就可以開始設定新環境。

當您設定Planning時，可能會問自己以下問題：

* **我是否要將工作區用於較大的組織群組？ 或者我應該鼓勵人們設定個人的？**

  您可能會發現兩者都有很好的用途。 工作區可能會變得難以管理，且您的工作流程可能太分散，因此我們建議您不要使用太多工作區。

  >[!TIP]
  >
  >    在一個Workfront例項中可以有1,000個工作區。

* **我應該在每個工作區中建立哪些自訂記錄型別？**

  記錄型別類似於Workfront的物件型別。 考慮您的工作流程，並決定哪些記錄型別（工作物件、人員物件、分類法等） 每個工作流程可能需要。

  如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)

* **我要如何建立我的記錄？ 是否有外部清單或試算表已經包含我需要新增至Planning的記錄，可供我使用？ 會視需要逐步新增記錄嗎？ 還是會使用Fusion或自訂API整合來匯入它們？**

  如需詳細資訊，請參閱：

   * [建立記錄](/help/quicksilver/planning/records/create-records.md)
   * [Adobe Workfront規劃模組](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-planning-modules.md)

* **我需要為記錄建立哪些欄位？**

  如需詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

* **我需要哪些Workfront或AEM Assets物件型別連線到Workfront Planning記錄型別，才能顯示相依性並為我的組織建立順暢的工作流程？**

  如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)

* **我需要講述行銷活動故事的行銷日曆和檢視表為何？ 我可以將這些檢視提供給哪些利害關係人進行緊密的協同合作？**

  如需詳細資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。


## Workfront規劃最佳作法

本節列出設定Workfront Planning時的幾項注意事項和最佳作法准則。

指南會根據您設定的物件或區域進行組織。

### 工作區

#### 有的工作區有無

* 針對組織層級工作區的最低體積進行設計

  例如，嘗試為所有行銷活動建立單一Workspace

* 請定期組織您的工作區。 您可能會發現您可以修改現有的一個，而不是從頭開始建立一個新的。

* 如果團隊有完全不同的操作動作，請務必為其建立新的Workspace。

  「產品開發」工作區應與「行銷」工作區不同

* 不要為每一件小事都建立唯一的工作區。 將工作區想像成一個記錄系統，可以讓整個組織受益，讓每個人都可以對應工作流程和共同作業，而不是一個用於追蹤個人請求的私人空間。

* 請勿為組織內的每個專案團隊或程式建立唯一的Workspace。

  行銷組織應儘量只維護一個工作區，以維持可見度，並允許資料在全球規劃層級累計。

  請避免為遵循類似流程的團隊建立類似或重複的工作區（例如EMEA行銷與APAC行銷），尤其是這些團隊可能會進行向上彙整至共同策略行銷活動的工作區。

#### 我應如何使用工作區區段？

* 建立區段和標籤區段，協助您的使用者瞭解您如何組織您的營運生命週期。

  例如，您可以建立名為「核心記錄」的區段，放置行銷活動、戰術和交付專案。

* 將「讚」的記錄型別群組在一起。

  您可以建立名為「地理位置」的區段，其中包含記錄型別，例如：地區、國家/地區和城市。

#### 我該如何管理工作區許可權？

* 請勿將存取許可權製為選定的受信任人員群組，以免這些人員意外刪除記錄型別，或建立不必要的記錄型別和欄位。

  >[!TIP]
  >
  >在測試版計畫期間，我們發現許多客戶都想要將「管理」存取權授與群組管理員。

* 請將Planning區域新增至擁有Standard授權之使用者的版面配置範本。

* 允許擁有Standard授權的使用者建立個人工作區。 這為他們提供了安全的空間來學習該工具並熟悉它。 這不會干擾其他人的體驗，並可能改善使用者的個人生產力。

  >[!TIP]
  >
  >    建議他們不要分享其個人工作區作為最佳實務。


### 記錄類型

#### 單一或多重選取欄位與連結的記錄型別

* 如果物件將用於多個其他記錄型別，請建立新的記錄型別

  例如，行銷活動可能連線至多個Target對象，而策略可能連線至單一Target對象。

* 如果物件需要儲存可能在查詢中有用的其他中繼資料值，請建立新的記錄型別。

  例如，通道記錄型別（例如「電子郵件」）可能會以原生中繼資料或獨立「交付專案」記錄型別的連線形式，儲存支援交付專案的清單。

* 如果您儲存的資料只需要限定為單一記錄型別，請勿新增記錄型別。 請改用選取欄位。

  例如，行銷活動記錄型別可能有一個稱為行銷活動大小的單一選取欄位，只有在直接與特定行銷活動相關聯時才相關。

#### 如何為我的記錄型別加上標籤？

請建立並標示代表單一建構或名詞的記錄型別，例如「促銷活動」

:no_entry_sign:請勿建立較適合作為檢視層顯示的記錄型別 — 例如，「行事曆」對於記錄型別而言是不好的選擇，因為它不是記錄型別本身，而是記錄的檢視。

### 我應該建立多少階層圖層？

檢視

...

工作流程

...

### 欄位管理

主要欄位

請使用唯一的主要欄位值，以便在建立連線時更輕鬆地尋找和「挑選」這些記錄。

建立連線時，使用者將依照主要欄位中的值進行搜尋，如果它們不是唯一的，使用者將無法知道應該選擇哪一個。

避免使用非唯一值作為主要欄位，因為使用連線選擇器選單時，這可能會讓必須在主要欄位上搜尋的使用者感到困惑。



從克里斯·奧尼爾：

另一個不要思考的領域是（或不是）最能運用Planning的使用案例。 例如，我們今天所討論的資源管理。



Alina的筆記：

ExL的「最佳實務」文章範例： https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/planning/sites-stores-store-views

來自Lauren S.現場整備的其他資訊： https://fieldreadiness-adobe.highspot.com/spots/5fd14ae8b7b7390523f57346