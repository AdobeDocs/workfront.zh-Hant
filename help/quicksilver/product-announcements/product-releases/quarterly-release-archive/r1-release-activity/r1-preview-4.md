---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1預覽4
description: 本頁介紹了R1.4版本在「預覽」環境中可用的所有更改。 此頁面上的功能已於2017年2月15日在預覽環境中提供使用。
author: Luke
feature: Product Announcements
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# R1預覽4

本頁介紹了R1.4版本在「預覽」環境中可用的所有更改。 此頁面上的功能已於2017年2月15日在預覽環境中提供使用。

有關在R1中進行的所有更改的清單，請參見 [Workfront R1版本](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## 更新項目、任務和問題批准

現在，為項目、任務和發行審批建立審批流程時，可以使用以下增強功能和更改： 

* 核准「步驟」現在稱為核准「階段」。
* 在每個階段包括多種類型的批准者。\
   包括使用者、團隊和工作角色。\
   在此更改之前，您只能包含同一類型的多個批准者。 例如，您可以包含多個工作角色，但不能包含工作角色和團隊。

* 已移除與修改現有全域核准程式相關的下列先前現存限制：

   * 修改的審批流程僅反映在審批流程尚未啟動或審批流程未修改的整個系統的對象上。 已啟動審批流程或已修改審批流程的對象不會隨您的更改而更新。
   * 您無法修改決定批准何時開始的狀態。

* 更新外觀。

如需建立核准程式的詳細資訊，請參閱 [建立工作項的審批流程](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

將核准程式與專案、任務或問題相關聯時，現在提供下列增強功能和變更：

* 更新外觀。
* 核准圖表會顯示在「核准」標籤上，以視覺化方式呈現先前、目前和未來的核准步驟。

有關將批准與項目、任務和問題關聯的詳細資訊，請參閱 [將新審批流程或現有審批流程與工作關聯](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 直接從「項目」頁更改項目的狀態

您不再需要編輯專案即可變更專案狀態。 您現在可以直接從專案的主要頁面變更專案的狀態。

如需詳細資訊，請參閱 [變更專案的狀態](../../../../manage-work/projects/manage-projects/change-project-status.md).

## 排程使用者停用

您現在可以排程在未來日期停用使用者。

在此增強功能之前，您只能立即手動停用使用者。

在多種情況下，將使用者排程為停用可能會很實用。 例如，如果您在Workfront中建立臨時聘用的使用者，可以將其設定為在合約結束時停用。

大量編輯使用者時，也可使用此功能。 

如需排程使用者停用的詳細資訊，請參閱 [停用或重新啟用使用者](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) 和 [新增使用者](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 「需要的動作」的新電子郵件摘要選項

「每日摘要傳送」選項現在可在「通知」設定的「需要動作」區域中使用。

如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

請記得更新與您的帳戶相關聯的電子郵件地址，以便能夠測試此功能。 這是必要操作，因為「預覽沙箱」會清除所有使用者的電子郵件地址。

## 資源回收筒改進：記錄在更新資料流中並接收電子郵件通知

在還原已刪除的專案、工作和問題時，已新增下列增強功能：

* 您現在會在還原物件後收到電子郵件通知。\
   身為Workfront管理員，您現在會在還原先前已刪除的專案、任務或問題後收到電子郵件通知。 電子郵件通知會通知您還原程式的狀態。\
   如需在Workfront中還原物件的詳細資訊，請參閱 [還原已刪除的項](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* 當恢復對象時，刪除和恢復對象現在記錄在對象本身的更新流和父對象的更新流中。\
   以前，只有刪除記錄在父對象的更新流中。\
   例如，在恢復任務時，將向項目和任務本身的更新流添加一條消息，指明已恢復任務。 (子任務中不記錄刪除和恢復。 有關子任務的刪除和恢復的資訊僅在父任務上可用。)\
   如需詳細資訊，請參閱 [還原已刪除的項](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## 更新管理群組成員資格的對話方塊

提供新的群組和子群組管理介面，提供更簡單、更方便使用的體驗。

「群組擁有者」欄位和「群組成員」欄位現已結合為單一欄位，其中列出群組成員清單如下。 此外，您可以篩選群組成員清單，並變更其為擁有者或成員。 

有關向組添加子組以及將用戶指定為組的成員或組所有者的詳細資訊，請參閱 [建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) 和 [建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## 複製行動應用程式中的文字

您可以複製行動應用程式中可見之所有物件之下列欄位中的文字：

* 名稱
* 說明
* 參考號碼
* 註解

此功能應在2月13日當周發行至iOS和Android應用程式商店。
