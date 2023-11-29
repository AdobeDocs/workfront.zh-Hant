---
content-type: reference
navigation-topic: betas
title: 'Adobe Workfront和Frame.io原生整合alpha：功能'
description: Adobe Workfront和Frame.io原生整合Alpha的計畫功能
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: 02e55be36d3b649aeb5b81d185538f77ac3d4ec7
workflow-type: tm+mt
source-wordcount: '1183'
ht-degree: 0%

---

# Adobe Workfront與Frame.io原生整合alpha：功能和測試

透過這項整合，我們的目標是讓創意人員留在他們選擇的工具（CC或Frame.io）中執行其內容建立和同行審閱，同時讓專案經理協調工作，並從Workfront內部初始化和監控正式稽核流程。 最佳化兩種解決方案結合使用，即可達成此目的：Workfront管理內容核准的新檔案核准，以及Frame.io提供的內容檢閱功能。 整體而言，新檔案核准和Frame.io將形成我們新的端對端內容稽核和核准體驗。 

若要進一步瞭解Alpha的運作方式以及參與的方式，請參閱 [Adobe Workfront與Frame.io整合alpha：概觀](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>如果您的公司未參與此Alpha方案，您可能會看到這些頁面，請務必謹慎處理這些資訊，並聯絡Workfront或Frame.io管理員以取得詳細資訊。

## 基本測試案例

為了讓您輕鬆測試Alpha程式的新功能，我們已建立新的測試Frame.io帳戶，並將其連線到名為的新群組 `Frame.io alpha testing` 在現有的Workfront預覽或沙箱環境中。

若要測試功能，請登入您的Workfront預覽或沙箱執行個體，然後執行下列步驟：

1. **協調員：** 在Workfront中，建立專案，使用 `Frame.io alpha testing` 群組已指派為專案群組。

1. **協調員：** 在Workfront中，將創意內容指派給專案或啟用影格的任務，並將專案狀態變更為「目前」。

1. **創意內容：** 檢查您的電子郵件，以取得新建立Frame.io專案的邀請

1. **創意內容：** 按一下邀請電子郵件中的「加入專案」按鈕，加入Frame.io專案、檢閱專案內的創意簡報，並在您選擇的Creative Cloud工具中開始建立內容。

1. **創意內容：** 將您建立的資產上傳到Frame.io，並將其新增到連結的Workfront專案（或指派已啟用框架的任務）。

1. **協調員：** 在Workfront中，在您的專案中找到連結的Frame.io資產，並指派檢閱者/核准者(如需指派檢閱/核准者的詳細資訊，請參閱 [新增其他核准者或稽核者至檔案](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md))。

1. **利害關係人：** 在Workfront中，在「首頁」或「檔案詳細資訊」中檢視您的核准請求，並在Frame.io檢視器中檢閱「框架連線」檔案，然後留下包含意見回饋的註解。

1. **協調員：** 在Workfront中，檢視利害關係人在Frame.io連線檔案的「更新」區段內建立的評論。

1. **利害關係人：** 在Frame.io檢視器中做出決定。

1. **創意內容：** 在Frame.io中，請注意針對您的資產所作出的整體核准決定。

1. **創意內容：** 在Frame.io中，將更新版本新增至連線資產的版本棧疊中，以套用要求的變更。

1. **協調員：** 在Workfront中，將核准者/稽核者指派給新上傳的版本，並監控進度，直到該版本達到登出為止。

## 功能計畫

以下是我們要解決的主要使用案例相關資訊，以及我們目前計畫要處理的功能。 <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
><span class="preview">醒目提示文字</span> 以下提及尚未實作，但將納入後續版本的功能。
>
>專案符號下 **「未來版本的潛在改善」** 視於alpha意見回饋和我們的開發計畫而定，頁首可能包含在未來版本中，也可能不包含在未來版本中。
>


### Workfront管理員可以在Workfront群組和Frame.io帳戶之間建立連線

* <span class="preview">在Workfront中，您可以將Workfront群組連線至Frame.io帳戶</span>

* 將在Frame.io中建立新的Frame.io群組，代表已連線的Workfront群組

**未來版本的潛在改善：**

* 從Frame.io帳戶中斷Workfront群組的連線

* 將Workfront群組連線到現有的Frame.io群組

### 專案專員可以設定要將哪些Workfront專案傳送到Frame.io，並將Workfront中指派的創意新增到Frame.io中的專案

* 可透過指派框架連線群組將Workfront專案標示為Frame.io已啟用

* <span class="preview">增強功能：能夠將Workfront專案內的任務切換為框架任務，這反過來會在Frame.io內建立任務資料夾</span>

* 當Workfront專案狀態設定為「目前」時，對應的已連線專案會在Frame中建立，Workfront指派的使用者會新增至Frame專案，並從Frame.io傳送電子郵件通知給他們

   * 所有Workfront專案成員（使用者和團隊）將新增為Frame.io專案的共同作業人員（于專案建立時及稍後時）

   * <span class="preview">變更：指派給已啟用Frame之Workfront任務的使用者和團隊將新增為Frame.io專案的共同作業人員，並會收到通知（專案建立時和稍後時）</span>

* 當建立專案時，新增至專案和啟用Frame之任務的檔案（創意簡介）將推送至Frame.io專案（在個別工作資料夾內）（觸發器：專案狀態設為「目前」）

   * 建議您先限制新增到專案中的檔案數量，然後再開始使用創意摘要，以避免傳送多份不必要的檔案至Frame.io

* <span class="preview">增強功能：若從已啟用框架的Workfront任務中明確取消指派，則會從Frame.io專案中移除使用者/團隊</span>

**未來版本的潛在改善：**

* 可在專案範本上設定啟用框架的任務

* 上傳至創意摘要的新版本將推送至框架

* 最佳化的專案同步處理（中斷專案連線、重新同步專案和檔案等）

### 在Frame.io中，創意人員可以將建立的資產傳送到Workfront專案進行正式審查

* 能夠將單一Frame.io資產連線到WF專案或任務。 資產參考將會在Workfront中建立

* 在Frame.io內上傳的新版本會自動在Workfront內的已連線資產上建立新檔案版本

* <span class="preview">增強功能：能夠從Frame.io中將參照的Workfront工作標示為完成</span>

* <span class="preview">增強功能：萬一刪除已連線的Workfront檔案，檔案會保留在Frame.io中，並可重新連線至相同或其他專案任務</span>

**未來版本的潛在改善：**

* 能夠一次傳送多個Frame.io資產至Workfront

* 從Frame.io針對Workfront專案/任務記錄時間

### 專案專員可將正式核准流程指派給從Frame.io連結的檔案

* 可以將Workfront使用者和團隊新增到Frame.io連線檔案的新檔案核准

* <span class="preview">增強：當使用者/團隊從已啟用Frame的檔案中取消共用時，他們也將失去對Frame.io Viewer中資產的存取權</span>

**未來版本的潛在改善：**

* 以單一檢閱傳送多個資產

* 將核准者/稽核者大量指派給Workfront檔案

### 利害關係人可以在Frame.io Viewer中進行檢閱和核准

* 利益相關者將會收到通知，並且可以在Frame.io檢視器中檢視框架連線檔案

* Frame.io檢視器可從Workfront內的不同位置存取，例如檔案清單、檔案詳細資訊、Workfront首頁

* 能夠利用Frame.io Viewer提供的現有檢閱和註解功能(將與Workfront的更新流同步)

* <span class="preview">能夠從Frame.io檢視器內作出新檔案核准決定</span>

### 在Frame.io中，創意人員將會收到有關已連線Frame.io資產上所做整體決策的通知

* <span class="preview">增強功能：整體檔案核准狀態會顯示在Frame.io內的資產上</span>

### 專案專員可將最終資產傳送至AEM

* <span class="preview">增強功能：可使用現有的Workfront + AEM Asset CS聯結器，將包含中繼資料的框架連線檔案傳送至AEM</span>
