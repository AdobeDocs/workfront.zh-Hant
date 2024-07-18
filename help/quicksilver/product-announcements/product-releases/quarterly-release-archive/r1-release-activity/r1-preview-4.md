---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1預覽4
description: 本頁說明R1.4版本預覽環境中所有可用的變更。 此頁面的功能已於2017年2月15日在預覽環境中推出。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# R1預覽4

本頁說明R1.4版本預覽環境中所有可用的變更。 此頁面的功能已於2017年2月15日在預覽環境中推出。

如需R1中所有變更的清單，請參閱[Workfront R1版本](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md)。

## 已更新的專案、任務和問題核准

建立專案、任務和問題核准的核准流程時，現在可以使用以下增強功能和變更： 

* 核准「步驟」現在稱為核准「階段」。
* 在每個階段包含多種核准者型別。\
  這包括使用者、團隊和職位角色。\
  在此變更之前，您只能包含相同型別的多個核准者。 例如，您可以包含多個職務角色，但不能包含職務角色和團隊。

* 下列與修改現有全域核准程式相關的既存限制已移除：

   * 修改過的核准程式只會反映在整個系統中的物件上，其中核准程式尚未開始或核准程式尚未修改。 已啟動核准流程或已修改核准流程的物件不會更新您的變更。
   * 您無法修改決定核准何時開始的狀態。

* 更新外觀。

如需建立核准流程的詳細資訊，請參閱[建立工作專案的核准流程](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

將核准流程與專案、任務或問題建立關聯時，現在可以使用以下增強功能和變更：

* 更新外觀。
* 核准圖表會顯示在核准標籤上，以視覺化方式呈現先前、目前和未來的核准步驟。

如需將核准與專案、任務和問題相關聯的詳細資訊，請參閱[將新的或現有的核准程式與工作相關聯](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。

## 直接從專案頁面變更專案狀態

您不再需要編輯專案即可變更專案狀態。 您現在可以直接從專案首頁面變更專案狀態。

如需詳細資訊，請參閱[變更專案狀態](../../../../manage-work/projects/manage-projects/change-project-status.md)。

## 排程使用者停用

您現在可以排程在未來日期停用的使用者。

在此增強功能之前，您只能立即手動停用使用者。

排程要停用的使用者在各種情況下可能很有用。 例如，如果您在Workfront中建立臨時聘用的使用者，您可以將他們設定為在合約結束時停用。

大量編輯使用者時，此功能也可使用。 

如需排程使用者停用的詳細資訊，請參閱[停用或重新啟用使用者](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)以及[新增使用者](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

## 「需要動作」的新電子郵件摘要選項

每日摘要傳送選項現在可在通知設定的「所需動作」區域使用。

如需詳細資訊，請參閱[修改您自己的電子郵件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

請記得更新與您的帳戶相關聯的電子郵件地址，以便測試此功能。 此為必要操作，因為「預覽沙箱」會清除所有使用者的電子郵件地址。

## 資源回收筒改善：記錄在更新流中並接收電子郵件通知

在還原已刪除的專案、任務和問題時新增了下列增強功能：

* 您現在會在還原物件後收到電子郵件通知。\
  作為Workfront管理員，您現在會在還原先前已刪除的專案、任務或問題後收到電子郵件通知。 電子郵件通知會通知您還原過程的狀態。\
  如需有關在Workfront中還原物件的詳細資訊，請參閱[還原已刪除的專案](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

* 當物件還原時，物件的刪除和還原現在會記錄在物件本身的更新流和父物件的更新流中。\
  以前，只有刪除記錄在父物件的更新流中。\
  例如，當任務還原時，訊息會新增至專案和任務本身的更新流，表示任務已還原。 （子任務上不會記錄刪除和還原）。 有關子任務的刪除和還原的資訊僅可在父任務上使用。)\
  如需詳細資訊，請參閱[還原已刪除的專案](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

 

## 更新管理群組成員資格的對話方塊

管理群組和子群組有一個新介面，可提供更簡單、更方便使用的體驗。

「群組擁有者」欄位和「群組成員」欄位現在合併為單一欄位，下方列出群組成員清單。 此外，您可以篩選群組成員的清單，並變更他們是「擁有者」還是「成員」。 

如需新增子群組至群組，以及指定使用者為群組成員或群組擁有者的詳細資訊，請參閱[建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)和[建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)。 

 

## 複製行動應用程式中的文字

您可以複製行動應用程式中可見之所有物件的下列欄位中的文字：

* 姓名
* 說明
* 參考號碼
* 評論

此功能應在2月13日當週同時發行給iOS和Android應用程式商店。
