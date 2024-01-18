---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Final
description: 2018.3版本活動
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 0%

---

# R1 Final

下列功能目前在「預覽」或Beta版中無法使用，但將在R1中發佈到「生產」環境：

## 從我的工作區域(Workfront)對校訂進行核准決策

現在，當使用者將您新增到校訂並授予核准者角色或檢視者和核准者角色(來自獨立的ProofHQ應用計畫或使用Workfront中的自動工作流程)，核准請求顯示在您的我的工作區域的核准索引標籤中。 然後您可以直接從Workfront檢視校樣並對校樣做出核准決定。

有關如何使用自動化工作流程將使用者新增到校訂的資訊，請參閱 [在Adobe Workfront中共用校訂](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) 在 [在Adobe Workfront中共用校訂](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

如需如何從「我的工作」區域做出核准決定的相關資訊，請參閱 [核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md) 在 [核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## 我的工作區域(Workfront)內的校訂核准報表

您現在可以根據校訂核准物件建立報告。 此報表可讓您報告來自使用者「我的工作」區域（尚未做出決定）的校訂核准。

校訂核准報告包含下列資訊：

* 已提交核准的檔案
* 核准者的名稱
* 校訂版本
* 校訂 ID
* 校訂建立日期

根據物件建立報告時，您可以存取此核准，如所述 [建立自訂報表](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

如需校訂核准物件報告的詳細資訊，請參閱 [瞭解Adobe Workfront中的物件](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 中的區段 [瞭解Adobe Workfront中的物件](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 使用拖放功能自動生成檔案校訂的新版本(Workfront)

當您使用拖放方法來新增需要校訂的檔案的新版本時，會自動產生校訂。 校訂的選項和工作流程與原始校訂或先前版本相同。

先前，當您新增檔案的新版本時，新版本不會自動產生校訂，且您必須為新版本重新產生校訂。

當您使用檔案更多選單上傳新版本時，校樣不會自動產生。

如需詳細資訊，請參閱以下小節：

## 讓所有校訂使用者直接從Workfront介面(Workfront)存取ProofHQ

現在您可以讓系統中的所有校訂使用者直接從Workfront介面順暢存取您的ProofHQ Premium帳戶。 啟用後，所有校訂使用者會在全域導覽列中看到ProofHQ圖示，將他們導向至ProofHQ網站。

預設不會啟用此選項。 若要啟用此選項，請聯絡Workfront技術支援並請求系統中的所有校訂使用者取得此存取權。

如需詳細資訊，請參閱 [從Adobe Workfront存取Workfront校訂](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) 在  [從Adobe Workfront存取Workfront校訂](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

在此變更之前，只有Workfront管理員可以從Workfront介面直接存取ProofHQ網站。

## 傳出郵件的TLS安全連線新選項(Workfront)

當您選擇使用您自己的電子郵件伺服器來管理Workfront通訊時，您現在可以啟用外寄郵件以使用TLS安全連線。

在此增強功能之前，您只能透過SSL安全連線啟用外寄郵件。

如需設定傳出郵件的詳細資訊，請參閱。

## 在預覽Sandbox環境中管理電子郵件的新欄位

Workfront現在會停用來自「預覽」沙箱環境和「自訂重新整理」環境的所有電子郵件通訊。 如果您想從「預覽沙箱」或「自訂重新整理」環境接收電子郵件通知，您必須在使用者設定中啟用此功能。

如需詳細資訊，請參閱下列資訊：

* [Adobe Workfront預覽沙箱環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 在 [Adobe Workfront預覽沙箱環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* 中的「從自訂重新整理沙箱接收電子郵件」 [Adobe Workfront自訂重新整理沙箱環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook for Office 365 (Workfront)

適用於Outlook 365的Workfront增益集現已推出。 

如需使用增益集的詳細資訊，請參閱 [搭配Outlook for Office 365使用Workfront增益集。](https://support.workfront.com/hc/en-us/sections/205046167)

## 在行動應用程式中搜尋(Workfront)

您現在可以在行動應用程式內搜尋物件，其方式與您在網頁應用程式中搜尋類似。 新的搜尋功能會先尋找「最近使用的專案」清單中的專案，以及先前已下載至行動裝置的物件。 「最近使用的專案」清單與您在Web應用程式中看到的清單相同。

>[!NOTE]
>
>此功能將於2017年5月的第一個星期推出。

如需行動應用程式的詳細資訊，請參閱下列「在行動中搜尋」一節：  

## 改善行動應用程式說明：Tutorials(Workfront)

從4月的行動版開始，您將會看到新的教學課程畫面，引導您瞭解行動體驗。 當您首次登入行動應用程式，且首次使用功能時，將會看到簡短的教學課程，說明該功能的運作方式。 第一次使用特定功能時，教學課程只會顯示一次。

如需行動應用程式的詳細資訊，請參閱。

## 在PDF檔案中搜尋(ProofHQ)

您現在可以在PDF檔案、Office檔案和靜態網頁中執行搜尋。

如需詳細資訊，請參閱  [搜尋校訂中的內容](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## 更新全域導覽列(ProofHQ)

與Workfront整合的ProofHQ Premium帳戶現在可在ProofHQ中看到下列全域導覽列改善：

* 新使用者個人資料圖片 
* 更新外觀

## 在自訂檢視(ProofHQ)中包含其他資訊

您現在可以在自訂檢視中加入下列額外資訊：

* **收件者層級資料**\
  您可以設定自訂檢視以包含與收件者層級資料相關的下列欄：角色、位置、電子郵件警示、我的截止日期、新增到校訂的日期和收件者搜尋。\
  如需詳細資訊，請參閱 [在Workfront Proof Proof中建立和管理自訂檢視](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **校訂資料**\
  您可以設定自訂檢視以包含下列與校訂資料相關的欄：註解計數（所有版本）、磁碟大小、校訂型別、每個版本的檔案數、註解附件資料（磁碟大小、檔案名稱）以及依子資料夾篩選。\
  如需詳細資訊，請參閱 [在Workfront Proof Proof中建立和管理自訂檢視](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **與自動化工作流程相關的階段層級資料**\
  您可以設定自訂檢視，以包含與自動化工作流程個別階段相關的下列欄：SOCD狀態、階段截止日期、作用中階段名稱、下一個階段名稱、階段名稱和範本。\
  如需詳細資訊，請參閱 [在Workfront Proof Proof中建立和管理自訂檢視](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## 校訂報表（先前稱為Analytics）的改善(ProofHQ)

報表功能（先前稱為Analytics）包含下列改善專案：

* 新預設報表型別：

   * 證明週轉時間
   * 延遲核准百分比
   * 校訂首次活動時間
   * 評論和回覆的數量

* 列印報表
* 更新外觀

## 在預覽環境中檢視ProofHQ功能(ProofHQ)

發佈到ProofHQ的功能將先在預覽環境中進行測試，然後再發佈到生產環境。

此生產前預覽功能發佈的新工作流程可讓您為未來更新ProofHQ生產環境做好準備。

如需ProofHQ預覽環境的詳細資訊，請參閱 [預覽Sandbox測試環境 — Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
