---
title: 'Adobe Workfront規劃常見問題集'
description: 身為行銷營運領導者，您可以使用Adobe Workfront Planning來組織所有團隊在行銷生命週期中的工作。 以下是Workfront Planning的一些常見問題。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '1630'
ht-degree: 0%

---


# Adobe Workfront規劃常見問題集

<!-- add to TOC and mini TOC-->

本文包含有關Adobe Workfront Planning最常見問題的清單。

如需Workfront Planning的詳細資訊，請參閱 [Adobe Workfront規劃概觀](/help/quicksilver/planning/general/planning-overview.md).

## 什麼是Workfront規劃？

Workfront Planning先前稱為Project Maestro，這項新功能可讓團隊集中規劃端對端作業，例如行銷活動、銷售、產品管理、服務等。 規劃可讓您透過自訂記錄、在營運生命週期中彈性連線，以及提升所有利害關係人的可見度，來為您的理想記錄系統建模。

## Workfront規劃如何融入更廣泛的Workfront產品？

Workfront規劃模組是三個相異但連結的Workfront功能之一，這些功能共同建立行銷記錄系統。 這三項功能包括：

* 計畫： Workfront計畫中包含的新進階功能。

* 工作流程：您目前在Workfront中使用的合作工作管理功能（專案管理、資源管理等）。

* 自動化和整合：以Workfront Fusion為動力之全面整合和自動化功能。

## Workfront Planning何時發行？

面向一般受眾的最新規劃Workfront版本為2024年8月28日。 如需目前發行之功能的最新資訊，請參閱 [Adobe Workfront Planning發行活動](/help/quicksilver/planning/general/release-activity.md).

<!-- To verify this: are we even saying "Beta"? - What happens after the beta program concludes? 

Beta participants that want to leverage Planning in production will be able to purchase it at the GA date. We encourage you to reach out to your sales rep to discuss further details. The environment used for the beta program is not in production and will not be migrated. The data stored in the beta environment will be available until December 2024. -->



客戶問題 — 第6/13#1研討會



簡短建立的程式（AI使用提取各種檔案來動態建立簡報）。 那是Beta版的一部分嗎？

我們預計此功能將會進行測試。

我們必須移轉至IMS嗎？

是，想要購買Planning的客戶必須移轉至ABP。

您可以提供不同工作區的範例嗎？

您可以在不同層級擁有工作區，而且由於系統的彈性，可在團隊和個人層級上真正提供多種用途。 主要使用案例是組織的大型集中式工作區。 工作區的一些特定範例為： ......

工作區可以共用資金帳戶嗎？

工作區可以彼此對話嗎？ 或者，是否必須在每個工作區中輸入資訊？

在其目前狀態中，可設定的工作區數量是否有任何軟性限制(即 在此時間點後，效能會降低)？ 可設定之工作區數量的任何嚴格限制(例如 系統不允許超過這個#)？

貴組織的Workfront例項中最多1,000個工作區。 檔案的連結： https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/create-workspaces

是否可以插入系統中目前的物件，或者是否必須手動建置這些物件？

您可以建立具有WF投資組合、方案、專案、群組和公司的Planning記錄型別之間的連線。 建立連線（例如WF專案）之後，您就可以連結「計畫」表格中與WF專案的記錄。 這表示WF物件仍會在Workfront中建立和管理，但您可以根據Planning記錄進行調整。 您在這裡有一些檔案： https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/connect-record-types ，我們也計畫舉辦有關「連線」的意見回饋會！

在測試中，我注意到如果您新增許多記錄，當它們不在「表格檢視」中時，就很難區分。 有沒有辦法讓記錄有不同的顏色？ 如果能讓您根據顏色設定它們，這樣它們在時間軸和日曆檢視中就能更加突出，那就很好。

人員是Workfront人員或IMS人員？

Workfront執行個體

這些清單可以連結至多個工作區嗎？

我們計畫在工作區之間連結記錄型別！ 尚未就緒。

您新增的自訂欄位是否鎖定至建立該欄位的記錄型別？

不允許我與預設的[開始/結束日期]欄位建立連線。 如果要連線到已存在的欄位，是否應新增欄位？

是否有將真正的外部查閱樣式欄位規劃為Planning中的欄位型別？

任何計畫在記錄中預設只有「Created」、「Created by」、「Modified」和「Modified by」欄位 — 如果我們想要追蹤記錄，似乎都是欄位必須新增的耗用量？

由於模組連結到WF中的即時物件，它們是否會受到Planning測試版活動的影響？

我們要取得放入Fusion的變更更新，還是要分開管理？

是否有將與畫布儀表板整合的計畫？ 如何報告資料？

即將推出的控制面板畫布將視覺化Planning資料

我們是否能夠建立工作區範本？

此分類/記錄結構是否只在您購買Planning時才可用？  分類法結構對標準Workfront使用者也有好處

管理員是否能夠建立我們自己的範本？

不適用於Beta版期間。

您是否都有記錄的ERD可供規劃模型與記錄型別共用？ 目前不是ERD，但我們提供細微的說明文章，引導您完成建立和連線記錄型別的程式： https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/overview-of-record-types https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/connect-record-types

所以它的一次性（年度定價）可以使用PLANNING，而且我們可以根據需要新增更多使用者嗎？ 或按使用者收費？

Planning是一種付費方案，其目標正式發行日期為8月28日，您必須在當天購買Planning才能在「生產」中享用。 請與您的銷售代表合作以取得更多詳細資訊。

AI啟用是否僅適用於WF系統管理員？是否可以在特定存取層級上啟用，或者僅對特定使用者（1或2）啟用？

最初，只有主要系統管理員擁有存取權，因此他們能夠通過存取層級設定，讓組織內哪些人員將獲得存取權。 在6月21日之後，我們將為組織的其餘部分啟用AI，並根據系統管理員定義的設定，讓他們是否可存取。

在這裡建立的FIELDS會位於何處？ 現有的FIELDS是否可從我們為其他物件建立的欄位匯入？ 它們是否與其他建立的欄位分開？

目前，欄位位於其建立的記錄型別內，但我們針對H2 &#39;24有一個高優先順序的計畫，將Planning和Workfront欄位整合在集中式欄位庫中。

我們是否能夠根據在Planning中建立的記錄/欄位建立報告？

是！ 即將推出，透過Dashbaord畫布

我們也能使用API提取此資料嗎？

是！ 我們有API和Fusion聯結器可以使用。

從行銷工作區 — 最好有一個用於全球行銷團隊的主工作區，或者最好為每個業務線、國家/地區、品牌等各擁有個別工作區。 我發現最多可以有1000個工作區，而且可能會連線工作區。 是否可以在工作區之間連結記錄？ 使用案例是 — 允許每個產品自己的工作區，但具有共用記錄型別。 然後您會想要檢視結合所有內容的共用檢視。

我們可以將Portfolio和方案帶入行銷活動嗎？ 進而帶來專案？

是否可以在建立專案時將專案連結到工作區中的記錄，而無需前往工作區進行連結？

目前專案中有Planning區段，其中會顯示Planning記錄型別的所有連線記錄。 您可以新增或移除這些連線的記錄。 我們很快也會新增連結至任何其他Planning記錄型別中記錄的功能，即使該連線目前沒有任何連結的記錄。

我瞭解我們最終將能夠從組織外部的人員接收資訊/資料。 此功能何時會在測試版中推出？

工作區是否可用於依行銷活動中的工作角色進行資源和容量規劃？

我們可以連結工作區記錄來開始請求？

營業時間6/18

能夠將日期連結至已連線的Workfront資料。 目前是否在全部層級（專案、投資組合、計畫……）中有效？

可以，您可以透過查詢欄位來連線專案。

我如何知道有公開檢視已準備就緒可供檢視？

共用的公開檢視是可見的

如何在內部共用檢視？

每次建立新工作區時，您都必須重新共用檢視嗎？

是的，每次您建立新工作區時，它都會變成新的記錄型別。 檢視是記錄型別專屬的檢視，因此您必須重新共用。

縮圖可以來自內容嗎？ 亦即，將縮圖設定為.pdf或視訊。 我們與創意人員合作，並擁有可選用的縮圖檢視，這是讓團隊持續參與討論我們內容地圖的較高層級會議的絕佳方式 — 直接連結內容也很好。

您是否能自訂超出基本範圍的許可權？ 目前您可以使用其他Workfront物件來自訂貢獻/管理/檢視存取權的功能。

目前我們只有Workspace和「檢視」層級的許可權，但沒有記錄型別或個別記錄層級的許可權。

我們是否能自訂工作區圖示，就像自訂縮圖一樣？

是否有可自訂的API來使用我們自己的DAM而非Adobe的DAM？

我們已經建立了公用API以進行Planning，並擁有Fusion聯結器。 API檔案將會發佈，並且可用來建立連線。

我在Planning中看到值（員工使用Airtable）。 到目前為止，我們一直…… x之後奇怪的後端連線將會繫結到上午10點47分左右