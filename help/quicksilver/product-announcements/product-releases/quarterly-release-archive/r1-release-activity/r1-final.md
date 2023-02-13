---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1最終
description: 下列功能目前在「預覽」或「測試版」中不可用，但將在R1 - EDIT ME中發佈到生產環境。
author: Luke
feature: Product Announcements
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 0%

---

# R1最終

下列功能目前在預覽或測試版中不可用，但將發佈到R1的生產環境：

## 從我的工作區(Workfront)進行校樣的核准決策

現在，當使用者將您新增至校樣並授予核准者角色或審核者與核准者角色(來自獨立的ProofHQ應用程式或使用Workfront內的自動化工作流程)時，核准請求會顯示在「我的工作」區域的「核准」標籤上。 然後，您就可以直接從Workfront檢視證明，並對證明做出核准決定。

如需如何使用自動化工作流程將使用者新增至校樣的詳細資訊，請參閱 [在Adobe Workfront內共用證明](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [在Adobe Workfront內共用證明](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

有關如何從「我的工作」區域做出審批決策的資訊，請參閱 [核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## 「我的工作區」內的校對核准報告(Workfront)

您現在可以根據「校樣核准」物件建立報表。 此報表可讓您報告來自使用者「我的工作」區域的校樣核准，而尚未做出決策。

校樣核准報表包含下列資訊：

* 已提交供批准的文檔
* 核准者的名稱
* 校樣版本
* 校訂 ID
* 校樣建立日期

根據對象建立報表時，可以訪問此批准，如 [建立自訂報表](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

如需「校樣核准」物件報表的詳細資訊，請參閱 [了解Adobe Workfront中的物件](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 區段 [了解Adobe Workfront中的物件](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 使用拖放功能自動產生新版本的檔案校樣(Workfront)

當您使用拖放方法來新增需要校對的檔案新版本時，會自動產生校樣。 校樣的選項和工作流程與原始校樣或舊版相同。

以前，當您添加新版本的文檔時，新版本不會自動生成校樣，您必須重新生成新版本的校樣。

使用「文檔更多」菜單上載新版本時，不會自動生成校樣。

如需詳細資訊，請參閱

## 讓所有校對使用者都能直接從Workfront介面(Workfront)存取ProofHQ

現在，您可以讓系統中的所有測試使用者直接從Workfront介面順暢地存取您的ProofHQ Premium帳戶。 啟用後，所有測試用戶在全局導航欄中都會看到一個ProofHQ表徵圖，該表徵圖將他們導向到ProofHQ站點。

預設不會啟用此選項。 若要啟用此選項，請聯絡Workfront技術支援，並向您系統中所有測試使用者請求此存取權。

如需詳細資訊，請參閱 [從Adobe Workfront存取Workfront校樣](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) in  [從Adobe Workfront存取Workfront校樣](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

在此變更前，只有Workfront管理員可以從Workfront介面直接存取ProofHQ網站。

## 傳出郵件的TLS安全連線新選項(Workfront)

當您選擇使用自己的電子郵件伺服器管理Workfront通訊時，您現在可以啟用傳出郵件，以使用TLS安全連線。

在此增強之前，您只能通過SSL安全連接來啟用傳出郵件。

有關配置傳出郵件的詳細資訊，請參見。

## 在預覽沙箱環境中管理電子郵件的新欄位

Workfront現在會停用「預覽沙箱」環境和「自訂重新整理」環境中的所有電子郵件通訊。 如果您想要從「預覽沙箱」或「自訂重新整理」環境接收電子郵件通知，您必須在使用者設定中啟用此功能。

如需詳細資訊，請參閱下列資訊：

* [Adobe Workfront預覽沙箱環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) in [Adobe Workfront預覽沙箱環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* 在「自訂重新整理沙箱接收電子郵件」 [Adobe Workfront自訂重新整理沙箱環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Office 365展望(Workfront)

Outlook 365的Workfront增益集現已推出。 

如需有關使用外接程式的詳細資訊，請參閱 [將Workfront插件與Outlook for Office 365一起使用。](https://support.workfront.com/hc/en-us/sections/205046167)

## 在行動應用程式中搜尋(Workfront)

您現在可以在行動應用程式內搜尋物件，類似於在Web應用程式中搜尋的方式。 新的搜尋功能會先尋找「最近的項目」清單中的項目，以及先前已下載至行動裝置的物件。 「最近的項目」清單與您在Web應用程式中看到的清單相同。

>[!NOTE]
>
>此功能將於2017年5月第一週推出。

如需行動應用程式的詳細資訊，請參閱  

## 改善行動應用程式中的說明：Tutorials(Workfront)

從4月的行動版開始，您會看到新的教學課程畫面，引導您完成行動體驗。 當您首次登入行動應用程式且首次使用功能時，將會看到簡短的教學課程，說明功能的運作方式。 教學課程僅顯示一次，這是您首次使用特定功能時顯示的。

如需行動應用程式的詳細資訊，請參閱。

## 在PDF文檔中搜索(ProofHQ)

您現在可以在PDF文檔、Office文檔和靜態網頁中執行搜索。

如需詳細資訊，請參閱  [在校樣內搜尋內容](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## 更新全域導覽列(ProofHQ)

與Workfront整合的ProofHQ Premium帳戶現在可在ProofHQ內的全域導覽列中看到下列改善項目：

* 新用戶配置檔案圖片 
* 更新外觀

## 在自訂檢視(ProofHQ)中包含其他資訊

您現在可以在自訂檢視中包含下列其他資訊：

* **收件者層級資料**\
   您可以設定自訂檢視，加入下列與收件者層級資料相關的欄：角色、位置、電子郵件警報、我的截止日期、新增至校樣的日期，以及收件者搜尋。\
   如需詳細資訊，請參閱 [在Workfront校樣中建立和管理自訂檢視](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **校對資料**\
   您可以設定自訂檢視，加入下列與校對資料相關的欄：注釋計數（所有版本）、磁碟大小、校樣類型、每個版本的檔案數、注釋附件資料（磁碟大小、檔案名）以及按子資料夾篩選。\
   如需詳細資訊，請參閱 [在Workfront校樣中建立和管理自訂檢視](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **與自動化工作流程相關的階段層級資料**\
   您可以設定自訂檢視，以包含與自動化工作流程的個別階段相關的下列欄：SOCD狀態、階段截止時間、活動階段名稱、下一階段名稱、階段名稱和模板。\
   如需詳細資訊，請參閱 [在Workfront校樣中建立和管理自訂檢視](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## 校對報表（原稱Analytics）(ProofHQ)的改良

報表功能（舊稱Analytics）包含下列改良功能：

* 新的預設報表類型：

   * 證明週轉時間
   * 延遲審批百分比
   * 校樣首次活動時間
   * 評論和答復的數量

* 列印報表
* 更新外觀

## 在預覽環境(ProofHQ)中檢視ProofHQ功能

發佈至ProofHQ的功能將首先可在預覽環境中測試，然後再發佈至生產環境。

此新的發佈功能工作流程可在生產環境前預覽，讓您為ProofHQ生產環境的未來更新做好更多準備。

如需ProofHQ預覽環境的詳細資訊，請參閱 [預覽沙箱測試環境 — Workfront校樣](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
