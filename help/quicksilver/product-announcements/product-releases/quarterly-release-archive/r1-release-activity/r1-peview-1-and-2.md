---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1預覽1和2
description: 本頁說明R1.1和R1.2版本在「預覽」環境中可用的所有變更。 此頁面的功能已於2017年1月19日在預覽環境中推出。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 2%

---

# R1預覽1和2

本頁說明R1.1和R1.2版本在「預覽」環境中可用的所有變更。 此頁面的功能已於2017年1月19日在預覽環境中推出。

如需R1中所有變更的清單，請參閱[R1發行活動概覽](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md)。 

## 從資源回收筒還原專案、任務和問題 

Workfront管理員現在可以還原過去30天內刪除的專案、任務和問題。 與專案、任務或問題相關的所有資訊都會還原，包括檔案和自訂資料。

新選項也可用於設定針對已刪除專案、任務或問題記錄的小時數。 如需詳細資訊，請參閱[設定刪除和還原物件時數的影響](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md)。

如需有關在Workfront中還原物件的詳細資訊，請參閱[還原已刪除的專案](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

有關如何檢視最近還原的專案、任務和問題的資訊，請參閱[檢視還原的專案](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md)。

## 核准圖表顯示先前、目前和未來核准步驟的視覺化表示法

現在，當專案、任務或問題的核准擱置時，會顯示圖表。 核准圖表會顯示核准流程中的目前步驟（擱置中），也可讓您快速檢視之前和未來的核准步驟，而不需導覽至「核准」標籤。

在此變更之前，有關核准步驟的資訊僅在專案、任務或問題的核准索引標籤上可用，並且僅在清單檢視中顯示，而不是圖表檢視。 （此資訊仍然可用，且在核准索引標籤中未變更。）

在專案中，核准資訊會顯示在專案標題旁的標題中。 關於任務和問題，核准資訊會顯示在右側面板中。

如需詳細資訊，請參閱[核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)  [核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)。

## 設定待核准要更新的物件

當專案、任務或問題處於未決核準時，您現在可以設定使用者是否可以：

* 編輯待核准專案、任務或問題的自訂表單。\
  如需在等待核準時如何設定要編輯的專案、任務和問題的相關資訊，請參閱[設定全域核准設定](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* 將問題新增至擱置核准的專案。\
  如需如何設定專案以允許使用者在專案未決核準時新增問題的相關資訊，請參閱[設定全系統的專案偏好設定](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

* 編輯擱置核准專案中的任務和問題。\
  如需如何設定專案，讓使用者在專案未決核準時編輯任務和問題的相關資訊，請參閱[設定全系統的專案偏好設定](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

在此變更之前，無法編輯未決核准的專案、任務和問題；此外，問題無法新增到未決核准的專案，並且任務和問題無法在未決核准的專案中進行編輯。

## 將版面配置範本指派給群組

您現在可以將配置範本指派給群組。

在此變更之前，您可以將版面配置範本指派給使用者、團隊和職位角色。 將版面配置範本指派給群組，其排版配置範本指派優先順序排名最低。 

如需詳細資訊，請參閱建立和管理版面範本。

## 變更大量編輯使用者通知

大量編輯使用者電子郵件通知設定的功能已變更。 當您選取多位使用者來編輯其通知電子郵件設定時，只有您正在更新的特定通知會針對所有選取的使用者而變更。 對於所有選取的使用者，所有未變更的電子郵件通知設定都會維持相同，即使這些使用者之間有所差異。 

在此變更之前，您選取的電子郵件通知設定已儲存，當您儲存變更時，所有其他未變更的通知設定都已取消選取。 

如需詳細資訊，請參閱[修改您自己的電子郵件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)中的[大量修改使用者通知設定]。

## 更新數個電子郵件通知的外觀

以下電子郵件通知的外觀與操作方式已更新為新的UI：

* 問題指派
* 認可日期變更
* 我參與的一個專案變更為啟用中
* 相關各方的核准決定
* 前置任務完成到任務依存性
* 未決核准（專案、任務、問題）
* 專案、任務、問題的狀態變更

請記得更新與您的帳戶關聯的電子郵件地址，以便能夠測試此功能，因為預覽沙箱會清除所有使用者的電子郵件地址。    如需電子郵件通知的詳細資訊，請參閱[Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)。  

## 多個通知區域的新電子郵件摘要選項

下列通知區域已新增「每日摘要」選項：

* 關於我所在的專案資訊
* 我贊助的專案的相關資訊
* 核准資訊
* 指派給我的工作的相關資訊
* 通訊

如需詳細資訊，請參閱[Adobe Workfront通知](../../../../workfront-basics/using-notifications/wf-notifications.md)。  請記得更新與您的帳戶關聯的電子郵件地址，以便能夠測試此功能，因為預覽沙箱會清除所有使用者的電子郵件地址。 

## 將群組設為公開

將群組設為公開時，您現在可以將該群組新增至使用者，而無需成為群組擁有者。 您必須具有使用者管理存取權才能編輯使用者。

如需將群組設為公開的相關資訊，請參閱[建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的[建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public)區段。

## 共用行動應用程式中物件的URL 

您現在可以在Workfront行動應用程式上的下列物件上共用URL：

* 專案
* 任務
* 問題
* 時程表
* 文件

您可以在下列應用程式中共用物件的URL：

* 文字訊息
* 電子郵件
* 儲存磁碟機（例如iCloud磁碟機）
* 其他已安裝的應用程式(例如Notes、Facebook)
* 您可以將物件的連結複製到剪貼簿，稍後再貼到任何其他應用程式中。 

## 設定中的相關內容說明

「設定」功能表下的所有區域已更新，區域右上角有「說明」圖示。 此圖示會提供說明網站中有關該區域的文章連結。 「設定」區域內的某些區段也已使用「說明」圖示更新。 

## 新增更精確的費用率

現在，您可以在建立費用型別時新增更精確的費用費率。 小數點後費用費率最多可包含4個字元（例如1.0375）。 這表示使用此比率的任何欄位都可以更精確。

在此變更前，費用費率最多只能包含小數點後的2個字元（例如1.03）。

如需建立費用率的詳細資訊，請參閱[建立自訂費用型別](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md)。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## R1預覽1和2發行網路研討會影片

此網路研討會由Workfront版本整備團隊於2017年1月19日主講。 此網路研討會著重於2017年的版本變更，並涵蓋了可在「預覽」中測試的新功能。
