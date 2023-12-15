---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 還原已刪除的專案
description: 如果您是Workfront管理員，可以在Adobe Workfront中還原在過去30天內刪除的專案、任務、問題、檔案和範本。 30天後，這些專案會永久刪除且無法還原。 當您還原物件時，也會還原其所有子物件和欄位。 例如，如果您還原專案，專案中的所有任務、問題、檔案、小時、附註、指派和自訂資料也會還原。items
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 1%

---

# 還原已刪除的專案

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

如果您是Workfront管理員，可以在Adobe Workfront中還原在過去30天內刪除的專案、任務、問題、檔案和範本。 30天後，這些專案會永久刪除且無法還原。

當您還原物件時，也會還原其所有子物件和欄位。 例如，如果您還原專案，所有任務、問題、檔案、小時、附註、指派和專案中的自訂資料也會還原。

群組管理員也可以為其管理的群組還原這些物件。

>[!IMPORTANT]
>
>* 如果您刪除報告、控制面板、使用者、群組、團隊或反複專案，將無法還原。
>* 在群組中，當群組管理員以外的人員直接將檔案上傳到物件的「檔案」區域時，只有Workfront管理員可以恢復檔案。
>
>* 如果您移動任務或問題並選擇不移動附加到任務或問題的檔案，檔案將被刪除並放入資源回收筒30天。 管理員可以將其還原，並重新附加至已移動的任務或問題。 如果任務或問題在移動後已被刪除，檔案會還原到管理員使用者頁面的「檔案」區域中，管理員會還原檔案。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

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
   <td><p>新增：標準</p>
   或
   <p>目前：計畫</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫或授權型別，請連絡您的Workfront管理員。

## 當您還原專案、任務或問題時復原的資訊

當您還原專案、任務或問題時，下列相關資訊將會與其一併復原：

* 更新區域中的評論和回覆
* 核准
* 指派
* 自訂表單
* 佇列設定
* 業務案例，包括計分卡、目標和風險
* 專案團隊
* 日期
* 問題
* 任務
* 子任務
* 狀態
* 財務資訊：

   * 計費記錄
   * 收費率
   * 費用

* 時間表資訊：

   * 前置任務
   * 任務限制
   * 期間型別

* 基準線

  當您還原父系專案或任務時，會復原任務基準線，但當您還原個別刪除的任務時，則不會復原。

* 小時（和小時ID）

  是否將時數還原至已刪除的專案取決於您在設定時程表和時數的偏好設定時選擇的設定。 如需詳細資訊，請參閱 [設定刪除和還原物件時的影響時間](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* 專案的URL

  還原後，專案的URL會維持不變。 如果人員已建立專案的瀏覽器書籤，則仍然有效。

* 存取權和許可權

  在專案被刪除之前便擁有專案存取許可權的使用者，會在專案還原後重新取得存取許可權。

* 檔案（包括校訂檔案）

  還原檔案和檔案版本時，請考量下列事項：

   * 個別刪除的檔案可以個別還原。

     當您還原父級時，會復原已刪除的檔案及其父級專案、任務或問題，但您無法個別還原。

   * 檔案或檔案校訂的所有版本都會在檔案還原時還原。\
     個別刪除的檔案或檔案校訂的個別版本無法復原。

## 當您還原專案、任務或問題時，未復原的資訊

當您還原專案、任務或問題時，以下關聯資訊不會隨專案、任務或問題一起復原：

* 贊
* 簽署
* 請求佇列中的錄取電子郵件地址
* 我的最愛

  您在刪除專案、任務或問題之前新增到我的最愛功能表，在還原後不會重新出現在我的最愛功能表中。

* 解析物件

  解決物件是使用選項設定的轉換問題 **保持初始問題並將其解決方案連結至此** &lt;**專案** 或 **任務)**>. 如果您刪除父級專案或任務，則問題不再被識別為解決物件，因為沒有連結將其連線到專案或任務。 如果您還原父系，則連結不會還原。

  如需有關Workfront管理員或群組管理員如何在轉換時設定問題以符合解析物件的詳細資訊，請參閱 [設定系統範圍的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) 和 [設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

  如需轉換問題的詳細資訊，請參閱 [在Adobe Workfront中轉換問題的概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

## 還原專案

{{step-1-to-setup}}

1. 按一下 **資源回收筒** > **最近刪除**.
1. 按一下 **專案**， **任務**， **問題**， **範本**，或 **檔案** 標籤，視您要還原的專案型別而定。

   專案會依據 **刪除日期** 欄。

1. 最多選取10個要還原的專案。

   如果您刪除子項任務，它會顯示在清單中。

   如果您刪除父系任務，則清單中只會顯示父系任務。 但是，當您還原父任務時，所有子任務都會還原。

1. 按一下 **還原** 將選取的專案還原至其原始位置。
1. （可選）若要快速檢視還原的專案，請遵循中的步驟 [檢視還原的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   如需有關還原專案後所發生情況的詳細資訊，請參閱區段 [還原專案後會發生什麼事](#what-happens-after-you-restore-items) 本文章內容。

## 還原專案後會發生什麼事 {#what-happens-after-you-restore-items}

* 當您恢復任務和子任務時，會按照刪除之前的順序顯示。

  但是，如果刪除任務時其他任務的順序發生變更，任務可能會恢復至任務或子任務清單的底部。

* 還原專案之後：

   * 系統會顯示訊息，讓您知道是否成功。

     您也會收到電子郵件通知。 如果您還原多個專案，電子郵件會列出這些專案。

   * 註解會顯示在專案、任務或問題的更新區域中，以及父物件的更新區域中。

     當您還原檔案或範本時，不會發生這種情況。

## 已還原的校訂

當某人還原具有校訂的檔案時，校訂的校訂活動頁面可能會顯示您組織例項中列出的第一個作用中Workfront管理員的名稱（依設定檔ID的順序），而非還原校訂的實際人員。
