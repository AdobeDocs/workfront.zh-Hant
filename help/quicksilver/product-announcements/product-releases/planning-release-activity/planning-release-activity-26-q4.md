---
content-type: release-notes
title: Adobe Workfront Planning 2026年第四季發行活動
description: 這是2026年第四季度Adobe Workfront規劃產品的發行活動。
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 9b6b1157cf93418e8863f2e99ebe87414a23378d
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# Adobe Workfront Planning 2026年第四季發行活動

本文介紹2026年第四季發行的Workfront Planning功能。

如需針對Adobe Workfront Planning發行之所有功能的清單，請參閱[Adobe Workfront Planning發行活動：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

## 已更新相依已連線記錄欄位的欄標題

>[!NOTE]
>
>預覽： 2026年8月20日
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日

我們針對表格檢視中相依的已連線記錄欄位，在視覺上改善欄標題。

如需詳細資訊，請參閱[管理相依連線](/help/quicksilver/planning/architecture/manage-dependent-connections.md)。

## 拖放多列時的表格檢視增強功能

>[!NOTE]
>
>預覽： 2026年8月13日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日
>[!BADGE 不在排程]{type=Neutral}內

在表格檢視中拖放多列時，會有新的視覺指示器。 更突出的加號和數字指示器現在會顯示為拖放動作選取了多少列。

如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。

<!--

## Collapse and expand all groupings in the timeline view

>[!NOTE]
>
>Preview: August 13, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

Timeline views now include Collapse all and Expand all options for grouped timelines. This makes it easier to navigate large roadmap views: you can quickly reduce the view to grouping headings, then expand only the sections you want to review.

For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).

-->

## 使用全域記錄型別時，將提交的請求物件路由到正確的工作區

>[!NOTE]
>
>預覽： 2026年8月13日
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日

透過提交請求表單為全域記錄型別建立的記錄現在會自動路由到從中提交記錄的工作區。

透過從全域記錄型別的次要工作區提交請求而建立的記錄會新增到該次要工作區。 透過從原始工作區提交請求，或從主請求區域提交請求所建立的記錄會新增到原始工作區。

如果輸入表單包含Workspace欄位，且使用者在提交前選取工作區，則無論表單從何處啟動，請求都會路由至所選的工作區。 這可確保從建立記錄的那一刻起，就將其組織在預期的工作區中。

如需詳細資訊，請參閱[提交Adobe Workfront Planning要求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)。

## Workfront Planning解決方案架構者技能簡介

>[!NOTE]
>
>預覽： 2026年8月10日
>生產： 2026年8月10日

我們將推出一項新技能，即Workfront Planning解決方案架構師，其將Workfront Planning的代理式最佳實務指引直接帶入Claude：

* **設定**&#x200B;要規格的新Planning工作區，而Workfront MCP伺服器會在您的環境中執行安裝程式。
* **稽核**&#x200B;大規模反圖樣的現有設定。
* **根據建議的限制（記錄、連線、階層深度）檢查使用量**。
* **隨時詢問有關Planning的問題**。

除了初始設定，這項技能還支援持續性治理，在造成摩擦之前捕捉配置漂移、在限制成為阻隔器之前標籤接近的限制、在每個工作區中強制實施一致的標準（無論設定者為何），並為團隊中的任何成員提供準確的答案，而不需要等候專家。 總體而言，這涵蓋了正確設定工作區的完整生命週期，並隨著使用量增加而維持運作方式。

如需詳細資訊，請參閱[可直接安裝的技能](/help/quicksilver/workfront-basics/workfront-mcp-server/direct-skills.md)。

## 在表格檢視中拖放列

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>所有人的生產： 2026年10月15日

在表格檢視中拖放列的體驗已改善視覺效果。

如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。


## 相依的已連線記錄欄位

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

Workspace管理員現在可以定義已連線記錄型別之間的相依性。 例如，確定區域欄位只會顯示與所選地理繫結的值。 這直接在連線欄位設定中設定：當從地域記錄型別新增連線到相依記錄型別（例如地區）時，新設定可讓工作區管理員使用在這些記錄型別之間已建立的關係，將其標籤為相依於地域記錄型別。

設定之後，參考這兩個欄位（例如促銷活動）的任何記錄型別都會立即看到效果：選取地理值會將區域選擇器縮小為僅包含實際連結至該地理的區域。 這會自動強制執行您的記錄結構，消除不相符的組合，並減少手動清除作業。

此更新包含下列功能：

* 在連線記錄型別時，我們在「新連線」標籤中新增了新的「連線設定」區段
* 我們已在新區段中新增「使該連線相依性」設定


如需詳細資訊，請參閱[管理相依連線](/help/quicksilver/planning/architecture/manage-dependent-connections.md)。




## 在表格檢視中顯示記錄的新註解指標

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

我們新增了一個指標，顯示記錄中何時有未讀取的評論。 指標顯示在表格檢視中記錄的主要欄位的右上角。

如需詳細資訊，請參閱[管理記錄註解](/help/quicksilver/planning/records/manage-record-comments.md)。

## 可自訂的記錄色彩和連線色彩編碼

>[!NOTE]
> 
>預覽： 2026年7月23日
>生產快速發行： 2026年8月13日
>所有人的生產： 2026年10月15日

記錄現在支援可自訂的調色盤，可讓您將自動指派給新記錄的顏色更新為標準或自訂顏色。

此增強功能包含下列變更： 

* 我們在下列區域新增了「顏色」選項：
  * 表格檢視中的欄點陣圖示。 
  * 時間軸和行事曆檢視的「設定」區域中的「長條圖樣式」區段

    開啟「顏色」設定時，指定給新記錄的顏色會顯示在這些檢視中顯示記錄的所有位置。 

* 顏色圓圈會新增到記錄的「詳細資訊」頁面。 
* 您現在可以在依欄位值著色時，將單一、多重選取和連線的記錄欄位新增至時間軸和行事曆檢視中長條的顏色編碼。 
* 當您建立連線的記錄欄位時，除了記錄名稱和影像之外，還可以啟用顯示顏色。 
* 「設定」區域中的「顏色」區段也藉由移除「無」選項而簡化。  

如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。 

## 規劃Designer現在需要接受Beta合約

>[!NOTE]
>預覽和生產（所有客戶）： 2026年7月20日
>[!BADGE 不在排程]{type=Neutral}內

規劃Designer現在需要使用已接受的Beta合約。 您的公司不需要簽署AI合約。 這適用於所有客戶。

為此，我們已將「設定」區段中「選擇加入AI Betas」區段下的「規劃Designer」選項移動。

在沒有已接受的Beta合約的情況下啟動Planning Designer時，現在會在工作區產生器開啟之前提示接受該協定。

如需詳細資訊，請參閱[開始使用Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md)。
