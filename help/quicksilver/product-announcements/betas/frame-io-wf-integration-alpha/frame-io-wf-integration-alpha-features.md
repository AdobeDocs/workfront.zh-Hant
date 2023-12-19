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
source-git-commit: 9e6033e495e83afa994b21996a4026ac484045a0
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Adobe Workfront與Frame.io原生整合alpha：功能和測試

透過這項整合，我們的目標是讓創意人員留在他們選擇的工具（CC或Frame.io）中執行其內容建立和同行審閱，同時讓專案經理協調工作，並從Workfront內部初始化和監控正式稽核流程。 最佳化兩種解決方案結合使用，即可達成此目的：Workfront管理內容核准的新檔案核准，以及Frame.io提供的內容檢閱功能。 整體而言，新檔案核准和Frame.io將形成我們新的端對端內容稽核和核准體驗。 

若要進一步瞭解Alpha的運作方式以及參與的方式，請參閱 [Adobe Workfront與Frame.io整合alpha：概觀](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).

>[!NOTE]
>
>如果您的公司未參與此Alpha方案，您可能會看到這些頁面，請務必謹慎處理這些資訊，並聯絡Workfront或Frame.io管理員以取得詳細資訊。
>

## 示範影片

>[!VIDEO](https://video.tv.adobe.com/v/3426406/)

## 基本測試案例

為了讓您輕鬆測試Alpha程式的新功能，我們已建立新的測試Frame.io帳戶，並將其連線到名為的新群組 `Frame.io alpha testing` 在現有的Workfront預覽或沙箱環境中。

若要測試功能，請登入您的Workfront預覽或沙箱執行個體，然後執行下列步驟：

1. **協調員：** 在Workfront中，建立專案，使用 `Frame.io alpha testing` 群組已指派為專案群組。

1. **協調員：** 在Workfront中，將需要創意工作的任務標示為已啟用框架（在任務詳細資料中），並將您的創意指派給它（如果您想要測試整個工作流程，也請指派您自己）。

>[!NOTE]
>
>子工作無法標籤為框架已啟用。
>

1. **協調員：** 上傳您的創意簡報並將專案狀態變更為「目前」。

1. **創意內容：** 檢查您的電子郵件，以取得新建立Frame.io專案的邀請

1. **創意內容：** 按一下邀請電子郵件中的「加入專案」按鈕，加入Frame.io專案、檢閱專案內的創意簡報，並在您選擇的Creative Cloud工具中開始建立內容。

1. **創意內容：** 將您建立的資產上傳到Frame.io，並選取其中一個指派的啟用Frame任務，將其新增到連結的Workfront專案。 選取選項以將工作標示為完成。

1. **協調員：** 在Workfront中，於啟用框架的任務中找到連結的Frame.io資產，並檢查任務的狀態是否變更為「完成」。

1. **協調員：** 將稽核者/核准者指派給連結的Frame.io資產。 如果您想要測試整個工作流程，請將自己指派為核准者。 (如需指派檢閱/核准者的詳細資訊，請參閱 [新增其他核准者或稽核者至檔案](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md))。

1. **利害關係人：** 在Workfront中，在首頁、檔案詳細資料或收到的電子郵件通知中檢視您的核准請求。 在Frame.io Viewer中開啟資產、留下包含意見回饋的評論，然後做出決定。

1. **協調員：** 在Workfront中，檢視Frame.io連線檔案的「更新」區段內利害關係人建立的評論，以及「核准」區段或檔案摘要窗格內的決定。

1. **創意內容：** 在Frame.io中，請注意針對您的資產所作出的整體核准決定。

1. **創意內容：** 在Frame.io中，將更新版本新增至連線資產的版本棧疊中，以套用要求的變更。

1. **協調員：** 在Workfront中，將核准者/稽核者指派給新上傳的版本，並監控進度，直到該版本達到登出為止。

## 詳細測試案例

對於想要測試其他功能的參與者，我們已建立更複雜的測試情境。 您可以在此處下載此詳細測試案例的指南： [WF + Frame.io詳細測試案例逐步說明](/help/quicksilver/product-announcements/betas/assets/WF-Frame-Detailed-Test-Scenario-Walkthrough.pdf).

## 功能計畫

以下是我們要解決的主要使用案例相關資訊，以及我們目前計畫要處理的功能。 <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
>專案符號下 **「未來版本的潛在改善」** 視於alpha意見回饋和我們的開發計畫而定，頁首可能包含在未來版本中，也可能不包含在未來版本中。
>

### Workfront管理員可以在Workfront群組和Frame.io帳戶之間建立連線

* 在Workfront中，您可以將Workfront群組連線至Frame.io帳戶

* 將在Frame.io中建立新的Frame.io團隊，代表已連線的Workfront群組(請注意，此功能僅針對在生產環境中使用整合的客戶啟用。 仍在沙箱或預覽上測試的客戶將由Adobe團隊設定連線。)

**未來版本的潛在改善：**

* 從Frame.io帳戶中斷Workfront群組的連線

* 將Workfront群組連線到現有的Frame.io群組

### 專案專員可以設定要將哪些Workfront專案傳送到Frame.io，並將Workfront中指派的創意新增到Frame.io中的專案

* 可透過指派框架連線群組將Workfront專案標示為Frame.io已啟用

* 能夠將Workfront專案內的任務切換為框架任務，這反過來會在Frame.io內建立任務資料夾

* 假設Workfront專案已指派框架連線群組，且至少有一個框架已啟用任務，當Workfront專案狀態設為「目前」時，對應的連線專案會在Frame中建立，Workfront指派的使用者則會新增至Frame專案，並從Frame.io傳送電子郵件通知給他們

   * 指派給已啟用Frame之Workfront任務的使用者和團隊會新增為Frame.io專案的共同作業人員，並會收到通知（建立專案時和稍後時）

* 當建立專案時，新增至專案和啟用Frame之任務的檔案（創意簡介）將推送至Frame.io專案（在個別工作資料夾內）（觸發器：專案狀態設為「目前」）

   * 建議您先限制新增到專案中的檔案數量，然後再開始使用創意摘要，以避免傳送多份不必要的檔案至Frame.io

   * 初始專案同步化後新增的檔案/任務不會推送至Frame.io，只會推送給使用者/團隊

**未來版本的潛在改善：**

* 可在專案範本上設定啟用框架的任務

* 上傳至創意摘要的新版本將推送至框架

* 最佳化的專案同步處理（中斷專案連線、重新同步專案和檔案等）

### 在Frame.io中，創意人員可以將建立的資產傳送到Workfront專案進行正式審查

* 能夠將單一Frame.io資產連線到WF專案或任務。 資產參考將會在Workfront中建立

* 在Frame.io內上傳的新版本會自動在Workfront內的已連線資產上建立新檔案版本

* 能夠從Frame.io中將參照的Workfront工作標示為完成

* 萬一刪除已連線的Workfront檔案，該檔案會保留在Frame.io中，並可重新連線到相同或其他專案任務

**未來版本的潛在改善：**

* 能夠一次傳送多個Frame.io資產至Workfront

* 從Frame.io針對Workfront專案/任務記錄時間

### 專案專員可將正式核准流程指派給從Frame.io連結的檔案

* 可以將Workfront使用者和團隊新增到Frame.io連線檔案的新檔案核准

* 當使用者/團隊從已啟用Frame的檔案中取消共用時，他們也將失去對Frame.io Viewer中資產的存取權

**未來版本的潛在改善：**

* 以單一檢閱傳送多個資產

* 將核准者/稽核者大量指派給Workfront檔案

### 利害關係人可以在Frame.io Viewer中進行檢閱和核准

* 利益相關者將會收到通知，並且可以在Frame.io檢視器中檢視框架連線檔案

* Frame.io檢視器可從Workfront內的不同位置存取，例如檔案清單、檔案詳細資訊、Workfront首頁

* 能夠利用Frame.io Viewer提供的現有檢閱和註解功能(將與Workfront的更新流同步)

* 能夠從Frame.io檢視器內作出新檔案核准決定
