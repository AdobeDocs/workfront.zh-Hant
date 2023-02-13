---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1預覽1和2
description: 本頁介紹R1.1和R1.2版本在預覽環境中可用的所有更改。 本頁面的功能已於2017年1月19日在「預覽」環境中使用。
author: Luke
feature: Product Announcements
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 2%

---

# R1預覽1和2

本頁介紹R1.1和R1.2版本在預覽環境中可用的所有更改。 本頁面的功能已於2017年1月19日在「預覽」環境中使用。

有關在R1中進行的所有更改的清單，請參見 [R1發行活動概觀](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## 從資源回收筒還原項目、任務和問題 

Workfront管理員現在可以還原過去30天內已刪除的專案、任務和問題。 與項目、任務或問題相關的所有資訊都將被還原，包括文檔和自定義資料。

也提供新選項，可針對已刪除的專案、任務或問題，設定記錄的時數有何變化。 如需詳細資訊，請參閱 [配置對象被刪除和還原時對時間的影響](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

如需在Workfront中還原物件的詳細資訊，請參閱 [還原已刪除的項](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

如需如何檢視最近還原之專案、工作和問題的相關資訊，請參閱 [查看已還原的項](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## 核准圖表顯示先前、目前和未來核准步驟的視覺表示

現在，當專案、任務或問題上有待核準時，會顯示圖表。 核准圖表顯示核准程式中（待審）的目前步驟，也可讓您快速檢視先前和未來的核准步驟，而不需導覽至「核准」標籤。

在此更改之前，有關批准步驟的資訊僅顯示在項目、任務或問題的「批准」頁簽上，而且它只顯示在清單視圖中，而不顯示在圖表視圖中。 （此資訊仍可供使用，在「核准」標籤中未變更。）

在專案上，核准資訊會顯示在專案標題旁的標題中。 在任務和問題上，核准資訊會顯示在右側面板中。

如需詳細資訊，請參閱 [核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md) in  [核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## 配置待更新的待批准對象

當項目、任務或問題等待批准時，您現在可以配置用戶是否可以：

* 編輯待批准的項目、任務或問題的自定義表單。\
   如需如何在待核準時設定要編輯的專案、工作和問題的相關資訊，請參閱 [配置全局批准設定](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* 將問題新增至待核准的專案。\
   如需如何設定專案，讓使用者在專案待核準時新增問題的相關資訊，請參閱 [配置系統範圍的項目首選項](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 編輯項目中待批准的任務和問題。\
   如需如何設定專案，讓使用者在專案待核準時編輯工作和問題的相關資訊，請參閱 [配置系統範圍的項目首選項](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

在此更改之前，無法編輯待批准的項目、任務和問題；此外，無法將問題添加到待批准的項目中，以及無法在待批准的項目中編輯任務和問題。

## 將版面範本指派給群組

您現在可以將版面範本指派給群組。

在此變更前，您可以將版面範本指派給使用者、團隊和工作角色。 為組分配佈局模板時，佈局模板分配優先順序中的排名最低。 

如需詳細資訊，請參閱建立和管理版面範本。

## 大量編輯使用者通知的變更

編輯使用者電子郵件通知設定的功能已大量變更。 當您選擇多個用戶以編輯其通知電子郵件設定時，只有您正在更新的特定通知才會更改所有選定用戶。 所有選取的使用者（即使他們與使用者不同），所有未變更的電子郵件通知設定都維持不變。 

在此更改之前，您選擇的電子郵件通知設定已保存，而在您保存更改時，已取消選擇所有其他未更改的通知設定。 

如需詳細資訊，請參閱以下主題中的「大量修改使用者通知設定」： [啟用或停用您自己的事件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## 更新數封電子郵件通知的外觀

以下電子郵件通知的外觀已使用新的UI更新：

* 問題分配
* 提交日期更改
* 我所在的一個專案變為使用中專案
* 對利害關係方的批准決定
* 任務從屬項的前置任務完成
* 待批准（項目、任務、問題）
* 項目、任務、問題的狀態更改

請記得更新與您的帳戶相關聯的電子郵件地址，以便測試此功能，因為「預覽沙箱」會清除所有使用者的電子郵件地址。    如需電子郵件通知的詳細資訊，請參閱 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## 適用於數個通知區域的新電子郵件摘要選項

已新增「每日摘要」選項的下列通知區域：

* 我所執行專案的相關資訊
* 關於我贊助的專案資訊
* 核准資訊
* 關於指派給我的工作資訊
* 溝通

如需詳細資訊，請參閱 [Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md).  請記得更新與您的帳戶相關聯的電子郵件地址，以便測試此功能，因為「預覽沙箱」會清除所有使用者的電子郵件地址。 

## 將群組設為公用

將群組設為公用時，您現在可以將該群組新增至使用者，而不需成為群組擁有者。 您必須有使用者管理存取權，才能編輯使用者。

如需將群組公開的詳細資訊，請參閱 [建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) 區段 [建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## 在行動應用程式中共用物件的URL 

您現在可以在Workfront行動應用程式上共用下列物件的URL:

* 專案
* 任務
* 問題
* 時程表
* 文件

您可以在下列應用程式中共用物件的URL:

* 文字訊息
* 電子郵件
* 儲存驅動器（例如iCloud驅動器）
* 另一個已安裝的應用程式(例如Notes、Facebook)
* 您可以將物件的連結複製到剪貼簿，之後再貼到任何其他應用程式中。 

## 設定中的內容相關說明

「設定」功能表下的所有區域都已更新為區域右上角的「說明」圖示。 此圖示提供該區域相關說明網站文章的連結。 「設定」區域內的某些區段也已以「說明」圖示更新。 

## 添加更精確的費用率

現在，您可以在建立費用類型時添加更準確的費用率。 費用率在小數後最多可包含4個字元（例如1.0375）。 這表示使用此比率的任何欄位都可更精確。

在此變更前，費用率最多只能包含小數後的2個字元（例如1.03）。

有關建立費用率的詳細資訊，請參閱 [建立自定義支出類型](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## R1預覽1和2版網路研討會錄音

此網路研討會由Workfront發行整備團隊於2017年1月19日主持。 此網路研討會主要討論2017年的版本變更，涵蓋可在預覽中測試的新功能。
