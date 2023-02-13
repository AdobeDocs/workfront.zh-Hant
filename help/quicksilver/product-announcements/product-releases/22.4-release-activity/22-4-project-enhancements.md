---
title: 22.4專案增強功能
description: 22.4專案增強功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 6cd6b1433fb56b92872f0ad80bb1a700fc0854cc
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 2%

---

# 22.4專案增強功能

本頁面說明在「預覽」環境中22.4版本中進行的所有專案增強功能。 這些增強功能將於2022年10月3日當周推出。

如需22.4版所有可用變更的清單，請參閱 [22.4版本概觀](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## 前身詳細資訊現已可用

要查看任務前置任務的詳細資訊，您現在可以將滑鼠移到前置任務列中的前置任務編號上。 「詳細資訊」(Details)框顯示被引用的前置任務和項目、前置任務的計畫起始日期和終止日期，以及前置任務的前置任務和後置任務的數量。 您可以展開專案詳細資訊，以查看有關專案的詳細資訊。 跨專案前置作業會提供其他資訊。

如需詳細資訊，請參閱 [在任務清單上建立前置關係](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## 為任務或問題分配多個團隊

為了在管理任務和問題的方式上為您提供更大的靈活性，我們為一個任務或問題分配了多個團隊。 以前，只能將一個團隊指派給任務或問題。

>[!NOTE]
>
>當前在「團隊」區域的「工作負載平衡器」中不提供此功能。

如需詳細資訊，請參閱 [指派任務](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) 和 [指派問題](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## 在「編輯」和「詳細資訊」區域中為項目角色選擇智慧用戶

我們已改善從專案的「編輯」方塊和「詳細資訊」區段，將使用者新增至下列專案欄位時的顯示方式：

* 專案所有者

* 專案贊助者

* 資源管理員

現在，當您將使用者新增至「編輯」或「詳細資料」區域中的任一欄位時，除了其名稱和頭像外，其「主要角色」和電子郵件也會顯示。 這有助於區分具有類似或相同名稱的多位使用者。

如需詳細資訊，請參閱 [編輯專案](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

注意：未來發行版本中，將會使用此功能更新專案、工作和問題的其他使用者欄位。

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412390/){target=_blank}

## 計算日期欄位一律會根據協調通用時間(UTC)儲存

現在，您可以確定計算欄位中的所有日期函式都能一致運作，且為每個人產生相同的結果，無論自訂資料運算式的更新方式或使用者在全世界協作物件的位置為何。

所有計算現在都是按一個標準(協調通用時間(UTC))計算並儲存的，而不是按貴組織實例和個人用戶配置檔案設定的時區配置計算。 不過，計算會根據每位使用者在瀏覽器中設定的個別時區，以自訂形式顯示。

以前，計算中的時間設定在下列情況下會造成混淆：

* 如果某人使用表單產生器上的「更新先前的計算」來重新計算計算欄位運算式，則日期函式結果會依貴組織的UTC時區決定。

* 如果某人編輯了對象，並導致計算欄位表達式重新計算，則日期函式結果由用戶的本地時區確定。 此情境中的計算日期欄位結果也將根據UTC計算。

如需詳細資訊，請參閱 [跨時區工作](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## 自訂表單增強功能：Adobe XD和快速篩選

我們已根據您的意見導入下列增強功能，以改善您在管理自訂表單時的體驗：

* 新增Adobe XD檔案，讓自訂表單更加視覺化和資訊化。 表單附加至物件時，使用物件的使用者可以從表單內檢視XD檔案並與之互動。

   如需詳細資訊，請參閱 [在自訂表單中新增或編輯影像或其他資產介面工具集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* 使用快速篩選功能，輕鬆找出現代化自訂表單和欄位清單中的項目。 管理表單和欄位時，您也可享受更佳的外觀和風格。

   如需快速篩選的詳細資訊，請參閱 [將快速篩選器應用於清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412469/){target=_blank}

## 公開測試版 — 專案、工作和問題的全新篩選體驗

專案、任務和問題清單中的篩選已重新設計，可協助您快速建立和共用篩選器。 功能包括：

* 直覺式「測試版產生器」介面，可建立新篩選器

* 將篩選器標示為我的最愛的功能

* 篩選器堆疊（套用多個儲存的篩選器）

* 複製篩選器

* 共用篩選器

* 移除與您共用的篩選器


時間表清單和方案計畫器中也提供新的篩選體驗。

文字模式仍可供進階篩選編輯使用，系統管理員仍可透過版面範本為所有使用者指派預設篩選。

### 這個在哪裡可用？

* 項目/任務/問題清單

* 案例規劃工具

* 時程表


### 我們想要您的意見！

借由此公開測試版，使用者可以按一下意見按鈕，直接將意見提交給處理篩選體驗的團隊。 我們期待收到您和您的使用者，針對公開測試版的全新篩選體驗提供意見。 如果您的團隊想要直接與產品會面以提供額外意見，歡迎在此安排會議：https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### 接下來呢？

* 新的群組和檢視（也稱為欄）體驗

   我們將開始針對群組和檢視（也稱為欄）使用新體驗，以便與新的篩選器體驗一致，且某些強大功能與新的篩選器體驗相同。

* 在Adobe Workfront的其他區域實作新篩選器

   我們將與產品各團隊合作，在Workfront的其他領域實作新的篩選器體驗。


我們想要反覆提供價值給您，因此在新體驗和其他領域準備就緒時，我們會繼續提供。 請繼續觀看更激動人心的更新。

如需詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) 和 [在Adobe Workfront中建立或編輯篩選器](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412391/)
