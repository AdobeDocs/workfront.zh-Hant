---
product-area: documents
navigation-topic: approvals
title: 資產檢閱和核准概觀
description: 進一步瞭解Workfront中的正式稽核和核准流程。
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 7e970f4f707937a62f68c191a7cbd5dfa26e471c
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# 資產檢閱和核准概觀

新的資產檢閱和核准工作流程是圍繞Workfront與Frame.io之間的緊密整合而建置。 此整合可充分利用每個產品所提供的功能，並結合這些功能，創造一種體驗，讓內容建立中涉及的所有人員都能夠使用他們選擇的工具，同時能即時存取跨兩個系統同步的評論、檔案和狀態更新。

如需有關Frame.io的詳細資訊，請參閱 [Frame.io快速入門](https://support.frame.io/en/collections/49298-getting-started).

## Workfront中的工作啟動和規劃

Workfront管理員可啟用Workfront與Frame.io之間的整合，方法是在「設定」區域中設定預設Frame.io帳戶，然後在Workfront中指定Frame.io使用者。 這允許協調員使用Workfront專案及正式檢閱和核准來計畫和啟動工作。

### 設定預設的Frame.io帳戶

Workfront管理員會在Workfront的「設定」區域中新增預設Frame.io帳戶，以起始Workfront和Frame.io整合。 設定預設的Frame.io帳戶後，整合會在Workfront和Frame.io之間建立連線的專案。

如需詳細資訊，請參閱 [].

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### 啟用Frame.io使用者

經常使用Frame.io的Workfront使用者應標示為Frame.io使用者。 Workfront管理員可以在Workfront使用者設定檔中指定Frame.io使用者。

當使用者在Workfront中標籤為Frame.io使用者並被新增到專案時，

* 他們在Frame.io中新增為共同作業人員
* 他們可以從Frame.io將資產傳送到Workfront以進行正式檢閱和核准

>[!TIP]
>
>我們建議讓經常使用創意工具及上傳資產的使用者能夠以Frame.io使用者的身分檢閱和核准。


如需詳細資訊，請參閱 [].

![](assets/Frame-enabled-user.png)


### 建立與Frame.io連線的專案

一旦新增預設Frame.io帳戶並指定Frame.io使用者後，專案專員即可建立與Frame.io連線的Workfront專案。 建立連線的專案時，您可以

* **將Frame.io使用者指派給任務**：啟用Frame.io的使用者指派給任務時，會收到電子郵件通知，告知有工作需要完成。
* **與Frame.io使用者共用專案**：與啟用Frame.io的使用者共用的專案可授予他們對Frame.io內專案的存取權。
* **與Frame.io共用創意素材**：您可以使用單向同步專案資料夾，直接從Workfront傳送指示和資料給Frame.io中的創意使用者。
* **追蹤任務進度**：創意人員無需離開Frame.io，即可傳送完成的資產並標籤任務完成。

如需詳細資訊，請參閱 [].

<!--Preassign approval templates to tasks coming in the future-->


## 在Frame.io中建立內容與共同作業

創意人員可以留在他們選擇的工具中，並自由地在Frame.io中建立、迭代及執行對等稽核。

將創意內容新增至已連線的專案時，他們可以在不離開Frame.io的情況下執行以下操作：

* 專案協調員的存取指示
* 進行非正式的同行評審
* 將完成的資產傳送到Workfront進行正式檢閱和核准
* 變更任務的狀態或將其標籤為完成
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

如需有關在Frame.io中檢閱資產的詳細資訊，請參閱

## 檢閱及核准資產

一旦創意內容從Frame.io將完成的資產傳送到Workfront，專案協調員就可以在Workfront中啟動正式的稽核和核准流程。

建立核准後，使用者會返回Frame.io以評論和標示資產。 他們也可以在Frame.io檢視器中做出核准決定。

### 在Workfront中啟動正式稽核和核准

專案專員可在Workfront的「設定」區域中建立一次性稽核和核准或可重複核准範本。 在Frame.io中進行的所有檢閱和核准活動也會記錄在Workfront中。

專案專員可選擇指派稽核者、核准者，或兩者的組合：

* **檢閱者** 可以評論和標示資產。 完成後，他們可以將其稽核標籤為完成。 <!--example of when to add reviewers-->
* **核准者** 可以在標籤資產上加上註解。 他們必須決定推進核准程式。



在Frame.io中所做的任何評論都會反映在Workfront的「更新」索引標籤中。 在Workfront中進行的回覆不會反映在Frame.io中。

標示為「僅限團隊」的註解不會出現在「Workfront更新」標籤中。

檢閱者和核准者可新增至一次性使用或核准範本：

<!--can also assign teams and set deadline-->

* **單一使用核准**：設定核准截止日期

* **核准範本**
在Workfront設定區域中，具有Standard授權的使用者可以建立可繼續使用的核准範本。 在範本中，使用者可以指定時間範圍並新增稽核者和核准者。 <!--do we want to mention any upcoming plans here? -->

  建立範本後，可將其套用至從Frame.io傳送的資產，以在Workfront中開始正式的稽核和核准流程。
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* 從Workfront上傳資產並將其傳送到框架以供檢閱和核准 — 即將推出？

### 核准Frame.io中的資產

Frame.io連線的資產利益關係人可以在Frame.io檢視器中檢閱和核准，其註解同步至Workfront更新流、決定等。

<!-- include screenshot from frame.io-->

如果您只在Frame中工作，可以透過電子郵件通知您有要求。

如果您只在Workfront中工作，則可以在首頁中使用核准Widget。

您工作時隨時可以從存取Frame.io檢視器

**從Frame.io核准資產**
如何通知他們

做出決定 — 核准、核准變更、需要工作

**從Workfront核准資產**
如何通知他們

首頁等待我的核准Widget

電子郵件 — 截止日期電子郵件72、24和截止日期。

系統會要求外部WF使用者為框架建立登入

如果資產未連線框架，他們可以在WF中檢視縮圖並使用註解流。 可做出檢閱和核准決定。

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### 追蹤檢閱和核准量度

首頁中的Widget核准速度報表？

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## 行銷活動資產核准工作流程範例

介紹段落？

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
