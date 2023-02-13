---
title: 專案常見問題集
description: 專案常見問題集
author: Alina
draft: Probably
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# 專案常見問題集

以下是關於專案的常見問題。

## 在任務清單中按一下右鍵某個任務時，為什麼「在上面/下面插入任務」缺失？

### 回答

要使用插入選項，必須按編號排序任務清單。 要按數字排序列，請按一下 **#** 在左側的欄標題中 **任務名稱** 按號來調整任務。

## 實際完成日期是多少？

### 回答

實際完成日期表示完成工作的日期和時間。 如需詳細資訊，請參閱 [項目實際完成日期概覽](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## 為什麼缺少縮進/凹出按鈕？

### 回答

要使用縮進/輸出按鈕，請確保任務按任務編號排序，並且未應用分組。

## 為何無法將專案狀態變更為「完成」？

嘗試將專案標籤為完成時，系統會收到下列錯誤訊息：

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### 回答

如果您的專案中有下列任一項，則無法將專案的狀態變更為完成：

* 未完成任務或問題
* 處於待批准狀態的任務或問題

## 為何無法將專案狀態從「完成」變更為「目前」？

### 回答

如果項目將「完成模式」設定為「自動」，則完成所有任務和問題後，項目的狀態將自動變為「完成」，並且您無法將其修改為任何其他狀態。 項目的「完成模式」必須設定為「手動」，才能將完成的項目轉換為「當前」。 如需詳細資訊，請參閱 [專案狀態不會從「完成」變更為「目前」](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md).

## 雖然我擁有正確的權限，為何無法將專案新增至Portfolio?

雖然我擁有正確的權限，但Portfolio的「專案」索引標籤上仍缺少「新增專案」按鈕。

### 回答

這是由Portfolio狀態為非作用中所導致。 要更改Portfolio的狀態：

1. 按一下 **Portfolio詳細資料>概觀**.
1. 變更 **狀態** to **活動。**

1. 按一下&#x200B;**儲存**。\
   此 **新增專案** 按鈕現在應該會顯示在 **專案** 標籤。

## 資源管理員在添加到項目中時會獲得哪些訪問權？

### 回答

資源管理器會自動接收對項目的管理訪問。 從資源管理器角色中刪除用戶並不會刪除其管理共用訪問權限。

## 新增群組時，專案狀態為何變更？

### 回答

項目狀態會因為組的預設狀態而改變。 將組添加到項目時，它會將狀態清單更改為為組設定的預設狀態。

如需詳細資訊，請參閱文章 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## 預算狀態是什麼？

### 回答

預算狀態將顯示項目當前是否已添加到能力計畫員中，以及是否已完成預算計算。

以下是預算狀態：

* 未包括 — 項目未添加到能力計畫員中。
* 已包括但未計算 — 項目將添加到能力計畫員，但從預算計算中排除。
* 已包括和已計算 — 項目將添加到能力計畫員中並包含在預算計算中。

## 為什麼我無法共用我是其擁有者的專案，以及我在哪裡擁有團隊的管理權限？ 在項目的共用對話框中找不到團隊。

### 回答

Adobe Workfront管理員限制您只檢視您在的存取層級中所屬的公司、群組和團隊。 您要尋找的團隊不是您所屬的團隊之一。

![](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

如需讓使用者檢視系統中所有團隊的相關資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
