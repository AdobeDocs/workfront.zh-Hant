---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 還原已刪除的項
description: 如果您是Workfront管理員，則可以還原Adobe Workfront中的專案、任務、問題、檔案和範本（如果這些項目在過去30天內被刪除）。 30天後，這些項目會永久刪除且無法還原。 還原對象時，其所有子對象和欄位也將還原。 例如，如果還原項目，則項目中的所有任務、問題、文檔、小時、附註、分配和自定義資料也會還原。items
feature: System Setup and Administration
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 1fb283df7090173d8f4dd36b9474ced10c8d30d1
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 1%

---

# 還原已刪除的項

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

如果您是Workfront管理員，則可以還原Adobe Workfront中的專案、任務、問題、檔案和範本（如果這些項目在過去30天內被刪除）。 30天後，這些項目會永久刪除且無法還原。

還原對象時，其所有子對象和欄位也將還原。 例如，如果還原項目，則項目中的所有任務、問題、文檔、小時、附註、分配和自定義資料也會還原。

組管理員還可以為他們管理的組還原這些對象。

>[!IMPORTANT]
>
>* 如果刪除報表、控制面板、使用者、群組、團隊或小版本，則無法還原。
>* 在組中，當組管理員以外的其他人直接將文檔上載到對象的「文檔」區域時，只有Workfront管理員才能還原該文檔。
>
>* 如果移動任務或問題，並選擇不移動附加到任務或問題的文檔，則這些文檔將被刪除並放在資源回收筒中30天。 管理員可以還原它們，並將它們重新附加到移動的任務或問題。 如果自移動任務或問題後已刪除該任務或問題，則將在恢復任務或問題的管理員的用戶頁的「文檔」區域中恢復這些文檔。


## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請聯絡您的Workfront管理員。

## 恢復項目、任務或問題時恢復的資訊

恢復項目、任務或問題時，將同時恢復以下相關資訊：

* 「更新」區域中的備注和回覆
* 核准
* 指派
* 自訂表單
* 隊列設定
* 業務案例，包括計分卡、目標和風險
* 專案團隊
* 日期
* 問題
* 任務
* 子任務
* 狀態
* 財務資訊:

   * 帳單記錄
   * 計費率
   * 費用

* 時間表資訊：

   * 前置任務
   * 任務約束
   * 持續時間類型

* 基準線

   恢復其父項項目或任務時會恢復任務基線，但恢復單獨刪除的任務時不會恢復。

* 小時（和小時ID）

   小時數是否還原到已刪除的項目，取決於在配置工時單和小時數首選項時選擇的設定。 如需詳細資訊，請參閱 [配置對象被刪除和還原時對時間的影響](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* 項目的URL

   還原後，項目的URL會維持不變。 如果人們已為項目建立瀏覽器書籤，則它們仍然有效。

* 存取與權限

   在項目被刪除前有權訪問的用戶將在項目恢復後重新獲得訪問權。

* 檔案（包括證明檔案）

   在恢復文檔和文檔版本時，請考慮以下事項：

   * 單獨刪除的文檔可以單獨還原。

      在恢復父項時，刪除的文檔及其父項項目、任務或問題將被恢復，但無法單獨恢復它們。

   * 恢復文檔時，將恢復文檔或文檔校樣的所有版本。\
      無法恢復單獨刪除的文檔或文檔校樣的單個版本。

## 恢復項目、任務或問題時未恢復的資訊

恢復項目、任務或問題時，將不會同時恢復以下相關資訊：

* 按贊次數
* 簽署
* 請求佇列中的接收電子郵件地址
* 我的最愛

   在刪除之前添加到收藏夾菜單的項目、任務或問題在還原後不會再出現在收藏夾菜單中。

* 解析對象

   解決物件是已轉換的問題，並以選項設定 **保留原始問題，並將其解決辦法與此聯繫起來** &lt;**專案** 或 **任務)**>。 如果刪除父項項目或任務，則不再將問題標識為解決對象，因為不再有將其連接到項目或任務的連結。 如果還原父項，則不會還原連結。

   有關Workfront管理員或群組管理員在轉換時如何配置問題以符合解決物件的詳細資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) 和 [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   如需轉換問題的詳細資訊，請參閱 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

## 還原項目

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **回收筒** > **最近刪除**.
1. 按一下 **專案**, **工作**, **問題**，或 **檔案** 頁簽，具體取決於要還原的項目類型。

   項目會依 **刪除日期** 欄。

1. 選擇最多10個要還原的項。

   如果刪除子任務，該任務將顯示在清單中。

   如果刪除父任務，則清單中只顯示父任務。 但是，恢復父任務時，所有子任務都會恢復。

1. 按一下 **還原** 將所選項目還原到其原始位置。
1. （可選）若要快速檢視已還原的項目，請遵循 [查看已還原的項](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   如需還原項目後會發生的詳細資訊，請參閱 [還原項目後會發生什麼事](#what-happens-after-you-restore-items) 這篇文章。

## 還原項目後會發生什麼事 {#what-happens-after-you-restore-items}

* 還原任務和子任務時，它們會按刪除前的順序顯示。

   但是，如果在刪除任務時其他任務的順序發生更改，則任務可能會還原到任務或子任務清單的底部。

* 還原項目後：

   * 會顯示訊息，讓您知道您是否成功。

      您也會收到電子郵件通知。 如果您還原了多個項目，電子郵件會列出這些項目。

   * 備注會顯示在項目、任務或問題的「更新」區域中以及父對象的「更新」區域中。

      恢復文檔時不會發生此情況。

## 還原的校樣

目前，當某人還原有校樣的檔案時，校樣的「校樣活動」頁面可能會顯示貴組織例項所列第一個作用中Workfront管理員的名稱（依設定檔ID的順序），而非還原校樣的實際人員。
