---
title: 22.4專案增強功能
description: 22.4專案增強功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 2%

---

# 22.4專案增強功能

本頁說明22.4版對預覽環境所做的所有專案增強功能。 這些增強功能將在2022年10月3日當週提供。

如需22.4版本可用的所有變更清單，請參閱[22.4版本總覽](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md)。

## 前置任務詳細資料已可供參考

若要檢視任務前置任務的詳細資訊，您現在可以將滑鼠游標停留在「前置任務」欄中的前置任務編號上。 詳細資訊方塊會顯示被參考的前置任務與專案、前置任務的計劃開始與結束日期，以及前置任務的前置任務與後置任務的數目。 您可以展開專案詳細資料以檢視有關專案的更多資訊。 其他資訊包含在跨專案前置任務中。

如需詳細資訊，請參閱[在工作清單](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md)上建立前置任務關係。

## 將多個團隊指派到一個任務或問題

為了讓您在管理任務和問題的方式上有更大的彈性，我們讓您將多個團隊指派到一個任務或問題成為可能。 以前，只能將一個團隊指派給一個任務或問題。

>[!NOTE]
>
>團隊區域的工作負載平衡器目前不提供此功能。

如需詳細資訊，請參閱[指派任務](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md)和[指派問題](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md)。

## 在「編輯」和「詳細資訊」區域中，為專案角色選取智慧使用者

當您將使用者從專案的編輯方塊和詳細資訊區段新增到以下專案欄位時，我們改進了使用者的顯示方式：

* 專案所有者

* 專案贊助者

* 資源管理員

現在，當您在「編輯」或「詳細資訊」區域中新增使用者至這些欄位時，除了他們的名稱和顯示圖片之外，也會顯示其主要角色和電子郵件。 這有助於區分具有類似或相同名稱的多位使用者。

如需詳細資訊，請參閱[編輯專案](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)。

注意：專案、任務和問題的其他使用者欄位將在未來版本中使用此功能進行更新。

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412390/){target=_blank}

## 計算的日期欄位一律根據世界協調時間(UTC)儲存

現在，您可以確定計算欄位中的所有日期函式都一致運作，並為所有人產生相同的結果，無論自訂資料運算式如何更新，或使用者在世界各地合作處理物件的位置如何。

所有計算現在都是透過一種標準(國際標準時間(UTC))計算並儲存，而不是透過針對您組織的執行個體和您個別使用者設定檔設定的時區組態進行計算並儲存。 不過，計算會根據每位使用者在瀏覽器中設定的個別時區，以自訂表單顯示。

先前，計算中的時間設定在下列情況中有所不同時，會產生混淆：

* 如果有人在表單產生器上使用「更新之前的計算」重新計算已計算的欄位運算式，日期函式結果由您組織的UTC時區決定。

* 如果有人編輯了物件且導致計算欄位運算式重新計算，則日期函式結果由使用者的當地時區決定。 此情境中的計算日期欄位結果也將根據UTC進行計算。

如需詳細資訊，請參閱[跨時區工作](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)。

## 自訂表單增強功能：Adobe XD和快速篩選

根據您的意見反應，我們已推出下列增強功能，以改善您管理自訂表單的體驗：

* 新增Adobe XD檔案，讓自訂表單更視覺化，並提供更多資訊。 當表單附加到物件時，使用物件的使用者可以從表單內檢視XD檔案並與其互動。


* 使用快速篩選器輕鬆找出現代化自訂表單和欄位清單中的專案。 管理表單和欄位時，也能享受改善的外觀和感覺。

  如需快速篩選的詳細資訊，請參閱[將快速篩選套用至清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md)。

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412469/){target=_blank}

## 公開Beta — 專案、任務和問題的新篩選器體驗

專案、任務和問題清單中的篩選已重新設計，以幫助您快速建立和共用篩選。 功能包括：

* 直覺式的「測試版產生器」介面可建立新篩選器

* 將篩選器標示為我的最愛

* 篩選器棧疊（套用多個已儲存的篩選器）

* 複製篩選器

* 共用篩選器

* 移除與您共用的篩選器


新篩選器體驗也可在時程表清單和「情境規劃工具」中取得。

文字模式仍可用於進階篩選器編輯，系統管理員仍可透過版面配置範本為所有使用者指派預設篩選器。

### 這在哪裡可用？

* 專案/任務/問題清單

* 情境規劃工具

* 時程表


### 我們需要您的意見反應！

有了此公共Beta，使用者可以按一下意見按鈕，直接將意見提交至處理篩選器體驗的團隊。 我們期待您和您的使用者能分享公開測試版中新的篩選器體驗。 如果您的團隊想要直接與產品會面以提供其他意見反應，歡迎在這裡排程會議： https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### 接下來呢？

* 新的群組和檢視（也稱為欄）體驗

  我們將開始設計新的分組和檢視體驗（也稱為欄），以便與新的篩選器體驗一致，並具有一些與新的篩選器體驗相同的強大功能。

* 在Adobe Workfront的其他區域中實作新篩選器

  我們將與整個產品的團隊合作，在Workfront中的其他區域實施新的篩選器體驗。


我們希望以反複的方式為您提供價值，因此我們會在新體驗和其他區域準備就緒時繼續提供價值。 請繼續關注更令人興奮的更新消息。

如需詳細資訊，請參閱[篩選器總覽](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)和[在Adobe Workfront中建立或編輯篩選器](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md)。

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412391/)
