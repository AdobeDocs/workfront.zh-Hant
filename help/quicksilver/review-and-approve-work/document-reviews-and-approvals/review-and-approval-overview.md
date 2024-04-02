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
source-git-commit: 63160895fc77994fdecd7aca8769b7d236d285d6
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---


# 資產檢閱和核准概觀

新的資產檢閱和核准工作流程是圍繞Workfront與Frame.io之間的緊密整合而建置。 此整合可充分利用每個產品所提供的功能，並結合這些功能，創造一種體驗，讓內容建立中涉及的所有人員都能夠使用他們選擇的工具，同時能即時存取跨兩個系統同步的評論、檔案和狀態更新。

<!-- link to frame docs-->

## Workfront中的工作啟動和規劃

專案協調員從Workfront開始。 專案已建立、任務已指派、指示已傳送。

專案協調員建立WF專案，使用同步的專案資料夾將資訊和支援資料傳送給Frame.io內的創意人員

從頭開始或透過範本設定核准工作流程

指派任務

將專案設為目前或等於建立框架專案和警示創意

### 設定預設的Frame.io帳戶

Workfront管理員會在Workfront的「設定」區域中新增預設Frame.io帳戶，以啟動Workfront和Frame.io整合。 一旦設定了預設的Frame.io帳戶，整合即可在Workfront和Frame.io之間建立連線的專案。

如需詳細資訊，請參閱 [].


<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->


### 啟用Frame.io使用者

經常使用Frame.io的Workfront使用者應標示為Frame.io使用者。 Workfront管理員可以在Workfront使用者設定檔中指定Frame.io使用者。

當使用者在Workfront中標示為Frame.io使用者並新增至專案時：

* 他們在Frame.io中新增為共同作業人員
* 他們可以從Frame.io將資產傳送到Workfront以進行正式檢閱和核准

如需詳細資訊，請參閱 [].

![](assets/Frame-enabled-user.png)

>[!TIP]
>
>我們建議讓經常使用創意工具及上傳資產的使用者能夠以Frame.io使用者的身分檢閱和核准。

### 建立與Frame.io連線的專案

專案專員可建立與Frame.io連線的Workfront專案。 建立連線的專案時，您可以

* **將Frame.io使用者指派給任務**：當啟用Frame.io的使用者被指派到有工作要完成的工作時，系統會以電子郵件通知他們。
* **與Frame.io使用者共用專案**：與啟用Frame.io的使用者共用的專案可授予他們對Frame.io內專案的存取權。
* **與Frame.io共用創意素材**：您可以使用單向同步專案資料夾，直接從Workfront傳送指示和資料給Frame.io中的創意使用者。
* **追蹤任務進度**：創意人員無需離開Frame.io，即可傳送完成的資產並標籤任務完成。

如需詳細資訊，請參閱 [].

<!--Preassign approval templates to asks coming in the future-->


## 在Frame.io中建立內容與共同作業

創意人員可以留在他們選擇的工具中，並自由地在Frame.io中建立、迭代及執行同級稽核。

將創意內容新增至整合專案時，他們可以在不離開Frame.io的情況下完成以下所有操作：

* 專案協調員的存取指示
* 進行非正式的同行評審
* 將完成的資產傳送到Workfront進行正式檢閱和核准
* 變更任務的狀態或將其標籤為完成
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->


## 在Workfront中檢閱和核准資產

一旦創意內容從Frame.io將完成的資產傳送到Workfront，專案協調員就可以在Workfront中展開正式的稽核和核准流程。 所有檢閱和核准活動都會記錄在Workfront中。

在Frame.io中所做的任何評論也會反映在Workfront的「更新」索引標籤中。 在Workfront中進行的回覆不會在Frame.io中反映。

標示為「僅限團隊」的註解不會出現在「Workfront更新」標籤中。

### 啟動正式稽核和核准

您可以建立一次性稽核和核准，或在workfront的設定區域中建立可執行的核准範本：

您可以選擇指派稽核者、核准者或兩者的組合：

* **檢閱者** 可以註解及標籤資產。 完成後，他們可以將其稽核標籤為完成。 <!--example of when to add reviewers-->
* **核准者** 可以註解、標籤資產，而且必須做出決定才能推進核准流程。

檢閱者和核准者可新增至一次性使用或核准範本：

<!--can also assign teams and set deadline-->

* **單一使用核准**：設定核准截止日期

* **核准範本**
在Workfront設定區域中，具有Standard授權的使用者可以建立可繼續使用的核准範本。 在範本中，使用者可以指定時間範圍並新增稽核者和核准者。 <!--do we want to mention any upcoming plans here? -->

  建立範本後，可將其套用至從Frame.io傳送的資產，以在Workfront中開始正式的稽核和核准流程。
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

### 檢閱和核准通知

與其他區段結合？

首頁等待我的核准Widget電子郵件 — 截止日期電子郵件72、24和截止日期。

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### 檢閱及核准資產

Frame.io連線的資產利益關係人可以在框架檢視器中檢閱和核准，其註解同步至workfront更新流、決定等

<!-- include screenshot from frame.io-->

系統會要求外部WF使用者為框架建立登入

如果資產未連線框架，他們可以在WF中檢視縮圖並使用註解流。 可進行稽核和核准決定。

### 追蹤檢閱和核准量度

首頁核准速度報表中的Widget

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


* 從Workfront上傳資產並將其傳送到框架以供檢閱和核准 — 即將推出？

## 行銷活動資產核准工作流程範例

介紹段落？

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->