---
content-type: reference
navigation-topic: betas
title: 'Adobe Workfront和Frame.io原生整合alpha：功能'
description: Adobe Workfront和Frame.io原生整合Alpha的計畫功能
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
source-git-commit: 0ad33f377086f71699c550e2300731056a834e72
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Adobe Workfront與Frame.io原生整合alpha：功能

## 使用案例和功能測試

透過這項整合，我們的目標是讓創意人員留在他們選擇的工具（CC或Frame.io）中執行其內容建立和同行審閱，同時讓專案經理協調工作，並從Workfront內部初始化和監控正式稽核流程。 最佳化兩種解決方案結合使用，即可達成此目的：Workfront管理內容核准的新檔案核准，以及Frame.io提供的內容檢閱功能。 整體而言，新檔案核准和Frame.io將形成我們新的端對端內容稽核和核准體驗。 

若要進一步瞭解Alpha的運作方式以及參與的方式，請參閱 [Adobe Workfront與Frame.io整合alpha：概觀](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>如果您的公司未參與此Alpha方案，您可能會看到這些頁面，請務必謹慎處理這些資訊，並聯絡Workfront或Frame.io管理員以取得詳細資訊。

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off-->

## 功能計畫

以下是我們要解決的主要使用案例相關資訊，以及我們目前計畫要處理的功能。 <!--, along with documentation to get you started testing.-->


### Workfront管理員可以在Workfront群組和Frame.io帳戶之間建立連線

* _在Workfront中，您可以將Workfront群組連線至Frame.io帳戶_

* 將在Frame.io中建立新的Frame.io群組，代表已連線的Workfront群組

**未來版本的潛在改善：**

* 從Frame.io帳戶中斷Workfront群組的連線

* 將Workfront群組連線到現有的Frame.io群組

### 專案專員可以設定要將哪些Workfront專案傳送到Frame.io，並將Workfront中指派的創意新增到Frame.io中的專案

* 可透過指派框架連線群組將Workfront專案標示為Frame.io已啟用

* _增強功能：能夠將Workfront專案內的任務切換為框架任務，這反過來會在Frame.io內建立任務資料夾_

* 當Workfront專案狀態設定為「目前」時，對應的已連線專案會在Frame中建立，Workfront指派的使用者會新增至Frame專案，並從Frame.io傳送電子郵件通知給他們

   * 所有Workfront專案成員（使用者和團隊）將新增為Frame.io專案的共同作業人員（于專案建立時及稍後時）

   * _變更：指派給已啟用Frame之Workfront任務的使用者和團隊將新增為Frame.io專案的共同作業人員，並會收到通知（專案建立時和稍後時）_

* 當建立專案時，新增至專案和啟用Frame之任務的檔案（創意簡介）將推送至Frame.io專案（在個別工作資料夾內）（觸發器：專案狀態設為「目前」）

   * 建議您先限制新增到專案中的檔案數量，然後再開始使用創意摘要，以避免傳送多份不必要的檔案至Frame.io

* _增強功能：若從已啟用框架的Workfront任務中明確取消指派，則會從Frame.io專案中移除使用者/團隊_

**未來版本的潛在改善：**

* 可在專案範本上設定啟用框架的任務

* 上傳至創意摘要的新版本將推送至框架

* 最佳化的專案同步處理（中斷專案連線、重新同步專案和檔案等）

### 在Frame.io中，創意人員可以將建立的資產傳送到Workfront專案進行正式審查

* 能夠將單一Frame.io資產連線到WF專案或任務。 資產參考將會在Workfront中建立

* 在Frame.io內上傳的新版本會自動在Workfront內的已連線資產上建立新檔案版本

* _增強功能：能夠從Frame.io中將參照的Workfront工作標示為完成_

* _增強功能：萬一刪除已連線的Workfront檔案，檔案會保留在Frame.io中，並可重新連線至相同或其他專案任務_

**未來版本的潛在改善：**

* 能夠一次傳送多個Frame.io資產至Workfront

* 從Frame.io針對Workfront專案/任務記錄時間

### 專案專員可將正式核准流程指派給從Frame.io連結的檔案

* 可以將Workfront使用者和團隊新增到Frame.io連線檔案的新檔案核准

* _增強：當使用者/團隊從已啟用Frame的檔案中取消共用時，他們也將失去對Frame.io Viewer中資產的存取權_

**未來版本的潛在改善：**

* 以單一檢閱傳送多個資產

* 將核准者/稽核者大量指派給Workfront檔案

### 利害關係人可以在Frame.io Viewer中進行檢閱和核准

* 利益相關者將會收到通知，並且可以在Frame.io檢視器中檢視框架連線檔案

* Frame.io檢視器可從Workfront內的不同位置存取，例如檔案清單、檔案詳細資訊、Workfront首頁

* 能夠利用Frame.io Viewer提供的現有檢閱和註解功能(將與Workfront的更新流同步)

* _能夠從Frame.io檢視器內作出新檔案核准決定_

### 在Frame.io中，創意人員將會收到有關已連線Frame.io資產上所做整體決策的通知

* _增強功能：整體檔案核准狀態會顯示在Frame.io內的資產上_

### 專案專員可將最終資產傳送至AEM

* _增強功能：可使用現有的Workfront + AEM Asset CS聯結器，將包含中繼資料的框架連線檔案傳送至AEM_