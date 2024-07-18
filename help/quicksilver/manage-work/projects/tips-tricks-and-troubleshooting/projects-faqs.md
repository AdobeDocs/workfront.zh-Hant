---
title: 專案常見問題集
description: 專案常見問題集
author: Alina
draft: Probably
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 1%

---

# 專案常見問題集

以下是有關專案的常見問題集。

## 為什麼我以滑鼠右鍵按一下任務清單中的任務時，遺失以上/以下插入任務？

### 解答

若要使用插入選項，工作清單必須依數字排序。 若要依數字排序欄，請按一下&#x200B;**工作名稱**&#x200B;左邊欄標題中的&#x200B;**#**，依數字重新排序工作。

## 實際完成日期為何？

### 解答

實際完成日期代表完成工作的日期和時間。 如需詳細資訊，請參閱[專案實際完成日期的總覽](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md)。

## 為何遺失縮排/凸排按鈕？

### 解答

若要使用「縮排/凸排」按鈕，請確定作業是按作業編號排序，且沒有套用群組。

## 為何無法將專案狀態變更為完成？

當我嘗試將我的專案標籤為完成時，收到以下錯誤訊息：

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### 解答

如果您的專案符合下列任何條件，您無法將專案狀態變更為完成：

* 未完成的任務或問題
* 處於未決核准狀態的任務或問題

## 為何無法將專案狀態從完成變更為目前？

### 解答

如果專案的「完成模式」設定為「自動」，當所有任務和問題完成時，專案狀態會自動變成「完成」，您無法將其修改為任何其他狀態。 專案的完成模式必須設定為手動，才能將完成的專案轉換為目前。 如需詳細資訊，請參閱[專案狀態不會從完成變更為目前](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md)。

## 為什麼我無法將專案新增至Portfolio，雖然我有執行此作業的正確許可權？

雖然我有正確的許可權，但Portfolio的「專案」索引標籤上缺少「新增專案」按鈕。

### 解答

這是因為Portfolio狀態為非使用中所致。 若要變更Portfolio的狀態：

1. 按一下&#x200B;**Portfolio詳細資料>概觀**。
1. 將&#x200B;**狀態**&#x200B;變更為&#x200B;**作用中。**

1. 按一下「**儲存**」。\
   **新增專案**&#x200B;按鈕現在應會顯示在&#x200B;**專案**&#x200B;索引標籤上。

## 資源管理員在新增至專案時會獲得什麼存取權？

### 解答

資源管理員會自動獲得專案的管理存取權。 從資源管理員角色中移除使用者並不會移除其管理共用存取權。

## 為什麼當我新增群組時專案狀態會變更？

### 解答

由於「群組」的預設狀態，專案狀態會變更。 將群組新增至專案時，專案會將狀態清單變更為為該群組設定的預設狀態。

如需詳細資訊，請參閱文章[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

## 什麼是預算狀態？

### 解答

預算狀態將顯示專案目前是否新增到能力規劃工具，以及預算計算是否已完成。

預算狀態如下：

* 未包含 — 專案未新增到Capacity Planner。
* 包含但未計算 — 專案已新增至「能力規劃工具」，但已從預算計算中排除。
* 包含與計算 — 專案會新增至Capacity Planner並包含在預算計算中。

## 為什麼我無法與團隊共用我是其擁有者且在其中具有「管理」許可權的專案？ 我在專案的共用對話方塊中找不到專案團隊。

### 解答

Adobe Workfront管理員限制您只能檢視您存取層級中所屬的公司、群組和團隊。 您尋找的團隊不是您所屬的團隊之一。

![](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

如需讓使用者檢視系統中所有團隊的詳細資訊，請參閱[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。
