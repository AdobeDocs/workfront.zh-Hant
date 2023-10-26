---
product-area: betas
navigation-topic: new-commenting-exprience-beta
title: 新的評論體驗發行活動
description: 檢閱Adobe Workfront新評論體驗的每週發行活動。
author: Alina
feature: Product Announcements
role: User, Admin
exl-id: 276b28f0-3955-4a0e-aa31-604b291f2f14
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '2209'
ht-degree: 2%

---

# 新的評論體驗發行活動

<!--take the badge out when it comes to production GA for everyone-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases. </span>  
* <span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)</span> -->


>[!IMPORTANT]
>
>本文資訊是指在Beta版階段期間針對新評論體驗所發行的功能。
>
>新評論體驗的Beta版計畫從2023年4月開始，到2023年10月結束。
>
>從2023年第四季度發行（2023年10月）開始，測試版期間發行的功能已可供所有客戶使用，並且測試版計畫已關閉。
> 
><br>如需詳細資訊，請參閱下列文章： </br>
>
>* 如需有關新體驗測試版期間發行的功能的資訊，請參閱 [新的評論體驗](../../betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>* 如需新的評論體驗測試版計畫關閉後，針對評論體驗所發行功能的相關資訊，請參閱目前的產品發行概觀頁面。

<!--
 This page contains information about the release timeline for the new commenting experience which is currently ongoing in Adobe Workfront. 

For general information on the new commenting experience, including a list of features that are currently available or in research, see [New commenting experience](../new-commenting-experience-beta/unified-commenting-experience.md). 


>[!IMPORTANT]
>
>The new commenting experience launched in Beta with the 23.2 release. For information about the original release, see [23.2 Release overview](../../product-releases/23.2-release-activity/23-2-release-overview.md). 
>
>Features that are released to the Workfront objects that support the beta commenting experience are also released to the Updates section of the following objects as the only commenting experience: 
>* Goals
>* Cards in the Boards area. 

-->

## 新的評論體驗發行時間表

新的註解體驗為Workfront物件的「更新」區段帶來全新的設計。

如需哪些Workfront物件會顯示「更新」區段的資訊，請參閱 [更新區段概觀](../../../workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

以下是新註解體驗發行至生產環境的計畫時間表，其中包含關鍵里程碑。 除了下列里程碑，我們將繼續透過較小的增強功能改善評論體驗。

如需Beta版期間及發行時間所發行功能的詳細資訊，請參閱 [Beta版期間發行的功能](#features-released-during-the-beta-period) 一節。

如需有關Beta版結束後針對新評論體驗所發行功能的資訊，請參閱目前的版本概觀頁面。

以下是新評論體驗發行的計畫時間表：

* 第23.2發行版本（2023年4月6日）：
   * 啟動問題的評論體驗Beta版
   * 發佈目標的新評論體驗（作為唯一體驗）
* 第23.3發行版本（2023年7月20日）：
   * 啟動專案、任務和檔案的評論體驗測試版。
   * 針對展示板區域中的卡片發行新的註解體驗（作為唯一體驗）
* 在2023年第四季版本（限量版，僅供選擇快速版本的客戶使用）：
   * 發行新的範本、範本任務、計畫、投資組合、團隊、使用者和時程表的評論體驗（作為唯一體驗）
   * 更新專案、任務、問題和檔案的評論體驗Beta版，使其成為預設選項。 「Beta」標籤會移除。
* 2023年第四季(23.10)版本（2023年10月26日）
   * 發行新的範本、範本任務、計畫、投資組合、團隊、使用者和時程表的評論體驗（作為唯一的體驗）給所有客戶。
   * 將專案、任務、問題和檔案的新註解體驗設為預設選項。

  >[!IMPORTANT]
  >
  >    這將結束新評論體驗的Beta階段。

   * 自此日期開始針對評論體驗發佈的所有功能，都是目前定期每月和季度發行的一部分。
* 2023年底：
   * 將舊版註釋體驗保留為下列物件的次要選項：專案、任務、問題和檔案。 新的註解體驗是所有使用者的預設選項。

  >[!NOTE]
  >
  >    反複專案將繼續擁有舊版評論體驗。 新的註解體驗將不可用於反複專案。

* 2024年第一季（2024年1月）：

   * 移除切換回舊版註解資料流的選項，並使新註解資料流成為所有物件的唯一體驗，版序除外。

## Beta版期間發行的功能

本節中說明的功能現在可供所有客戶及所有環境使用。

在23.2版（2023年4月6日）和2023年第四季度（2023年10月26日）之間的測試階段，以下功能被新增到評論體驗中。

以下資訊是指每週的發行活動，從最近的更新開始。

### 2023年10月16日起一週

#### 以其他使用者身份登入時，在評論時新增「代表&lt;使用者名稱>」資訊

重新設計評論體驗時，我們已在Workfront或群組管理員以其他使用者身份登入時新增評論時移除「代表&lt;使用者名稱>」指標。 此資訊現在已還原。

所有客戶的預覽和生產： 2023年10月19日。

### 2023年9月11日起一週

#### 新的評論體驗會擷取從2019年1月1日開始的資訊

專案、任務、問題和檔案現在顯示從2019年1月1日起的更新。 在此增強功能之前，新的註釋體驗僅擷取這些物件自2022年6月以來的更新。

如需詳細資訊，請參閱 [新的評論體驗](../new-commenting-experience-beta/unified-commenting-experience.md).

所有客戶的預覽和生產： 2023年9月11日。

### 2023年8月21日起一週

#### 變更「註解」標籤上的時間戳記格式

我們已更新新註解流之「註解」索引標籤中使用者註解的時間戳記格式。 作為此變更的一部分，目前年份的評論不再在時間戳記中顯示年份。 將游標暫留在時間戳記上會顯示完整日期，包括年份。

變更不會影響「系統活動」標籤中的系統更新。

所有客戶的預覽和生產： 2023年8月24日

### 2023年8月14日起一週

[觀看2023年8月14日當週所發行所有功能的影片示範](https://video.tv.adobe.com/v/3422912/){target=_blank}

#### 其他物件的新註解體驗

<!--
[!BADGE In production for Fast Release ]{type=Positive}
-->

在23.3版發佈至生產環境後不久，以下物件將可使用新的評論體驗：範本任務、範本、時程表、團隊、使用者、計畫、投資組合。

這將是這些物件的唯一註解體驗，因為當您存取它們時，舊版註解體驗會被移除。

如需詳細資訊，請參閱 [新的評論體驗](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

預覽版本： 2023年8月17日

快速發行的生產版本：23.8版（2023年8月31日）

適用於所有客戶的生產版本：第23.10版本（2023年10月）

#### 新評論資料流的新設計更新

<!--
[!BADGE In production for Fast Release ]{type=Positive}
-->

我們重新設計了新的評論流，以提供更新的外觀。 部分改善包括：

* 註解資料流的內容會以頁面為中心，而非佔據整個頁面寬度。

* 「更多」選單圖示會重新放置到註解的右上角，而非「讚」按鈕旁邊。

* 現在，「讚」和「回覆」按鈕彼此相鄰。

* 「記錄時間」按鈕已重新放置於註解區域的右上角。

* 已新增新增新增新增回覆提示，以提示使用者將回覆新增至現有回覆。

* 每個註解對話串之間有一條分隔線

如需詳細資訊，請參閱 [更新索引標籤總覽](../../../workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

預覽版本： 2023年8月17日

快速發行生產：23.8版（2023年8月31日）

每季發行生產：23.10版（2023年10月）

#### 新的評論體驗是專案、任務、問題和檔案的預設體驗

<!--
[!BADGE In production for Fast Release ]{type=Positive}
-->

我們正在將新的註解體驗設定為下列物件的預設體驗：專案、任務、問題和檔案。  存取這些物件時，舊版註解體驗仍會作為替代選項。

為了支援這項變更，我們也將的「註解測試版」切換重新命名為「新註解」。

如需詳細資訊，請參閱 [新的評論體驗](../new-commenting-experience-beta/unified-commenting-experience.md).

預覽版本： 2023年8月17日

快速發行生產：23.8版（2023年8月31日）

每季發行生產：23.10版（2023年10月）

#### 在更新中標籤使用者時的頭像改善

為了讓您更清楚地瞭解哪些使用者在更新中被標籤，我們現在會在更新中顯示被標籤的使用者名稱（最多兩個使用者）。 如需詳細資訊，請參閱 [在更新中標籤其他人](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

預覽版本： 2023年8月17日

快速發行生產：23.8版（2023年8月31日）

適用於所有客戶的生產：23.10版（2023年10月）

### 2023年8月7日當週

#### 新增表情符號至更新

您現在可以使用新註解體驗中的RTF工具列選項，將表情符號新增到註解中。

如需詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 說明檔案將在發行時更新。

預覽和生產： 2023年8月10日

### 2023年7月10日起一週

#### 自動標籤所有執行緒參與者

評論擁有者現在會在對話串中自動標籤。 在此更新之前，僅限使用「@name」標籤，或將其新增到已標籤使用者清單中顯示的「標籤人員或團隊」區段來標籤的使用者。 有了它，您現在就可以根據需要從對話串中移除評論的所有者，即使他們之前沒有手動標籤。

預覽版本： 2023年7月12日

生產版本： 2023年7月13日

### 2023年7月3日當週

#### 記錄時間的新介面

我們重新設計了介面，用於從新評論體驗的更新區域記錄時間。

如需詳細資訊，請參閱 [記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md).

預覽版本： 2023年7月5日

生產版本： 23.3版（2023年7月）

### 2023年6月26日起一週

#### 在新回覆中引用註解內容

現在，您能夠複製註解的內容，並在使用新的註解體驗時，以新引號的形式新增到相同對話串的回覆中。

如需詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

預覽： 2023年6月28日

生產版本： 2023年6月29日

### 2023年6月12日起一週

#### 面板區域中卡片的新註解體驗

新的註解體驗現在可用於面板區域中的卡片。 這是卡片唯一可用的體驗。 如需詳細資訊，請參閱 [23.3版本總覽](../../product-releases/23.3-release-activity/23-3-release-overview.md).

預覽： 2023年6月15日

提前選擇加入的生產版本： 2023年6月22日

適用於所有客戶的生產：23.3版（2023年7月）

#### 將區塊引號新增至註解

您現在可以使用新註解測試版體驗中的RTF工具列選項，將區塊引號新增到註解中。

如需詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

預覽： 2023年6月14日

生產： 2023年6月15日

#### 改善編輯評論時的體驗

您現在可以在編輯註解時使用下列快速鍵：

* CTRL + Z (Mac為CMD + Z)可復原變更

* CTRL + Y (Mac為CMD + Y)以重做變更

在這些增強功能之前，您無法在編輯註解時復原或重做變更。 如需詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

預覽： 2023年6月13日

生產： 2023年6月13日

<!--I used the date when I found them in Prod. Not sure when these released, but it could have been before this date-->

### 2023年5月29日起一週

#### 專案、任務和檔案的新註解測試版體驗

新的評論測試版體驗現在可用於專案、任務和檔案。 在此更新之前，評論Beta版體驗僅適用於問題和目標。

預覽： 2023年6月1日

生產： 23.3版（2023年7月）

>[!NOTE]
>
>從2023年6月1日開始針對新註解Beta版體驗發佈的任何功能，在23.3版發佈至生產環境後，都可在生產環境中用於專案、任務和檔案。 如需詳細資訊，請參閱 [23.3版本總覽](../../../product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

#### 編輯評論後新增「已編輯」標籤的外觀

在新的註解測試版體驗中編輯註解時，「已編輯」標籤會新增到註解中。 此標籤現在具有原來發佈的新外觀。 註解的日期和時間戳記是原始註解的日期和時間。 不是進行編輯時的日期和時間戳記。  如需詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

預覽： 2023年5月31日

生產： 2023年6月1日

#### 子物件的註解會向上彙整至父物件

啟用註解Beta版體驗時，與子物件相關聯的註解現在會向上彙整至父物件。 例如，檔案中的註解現在會顯示在附加檔案的問題上。 如需詳細資訊，請參閱 [更新區段總覽](../../../workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

預覽： 2023年6月1日

生產： 2023年6月1日

#### 在新的評論Beta版體驗中記錄時間

使用新的註解測試版體驗時，您可以從更新區域記錄問題、任務和專案的時間。 如需詳細資訊，請參閱 [記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md).

預覽： 2023年6月1日

生產： 23.3版（2023年7月）

### 2023年5月15日起一週

#### 改善在評論中新增超連結時的體驗

您現在可以使用下列快速鍵將超連結新增至註解：

* CTRL + V (Mac為CMD + V)在選取的文字上貼上連結
* CTRL + K (Mac為CMD + K)開啟「新增連結」方塊。

在這些增強功能之前，您只能按一下RTF工具列中的連結圖示來新增超連結。 如需詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

預覽： 2023年5月17日

生產： 2023年5月18日

### 2023年5月1日起一週

#### 當從註解中移除附件或移除包含附件的註解時，會從「檔案」區域移除影像

移除或編輯包含附件的註解時，我們正在變更附件的工作方式。 現在，當您編輯註解並移除附件時，或者當您刪除包含附件的註解時，附件也會從「檔案」區域中移除。 在此變更之前，在先前的註解體驗中，附件仍保留在您的「檔案」區域中。 如需詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

依預設，可用於下列日期發表測試版體驗和Workfront目標註解的問題：

* 預覽和生產： 2023年5月4日


### 2023 年 4 月 27 日

針對註解Beta版的問題和目標發佈了以下維護更新：

編輯註解時編輯附加影像. 如需詳細資訊，請參閱文章中的「4月27日維護更新」一節 <a href="https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=en#updates-in-april-2023">2023年4月更新</a>.

### 2023 年 4 月 20 日

針對註解Beta版的問題和目標發佈了以下維護更新：

在離開目標更新和註解測試版體驗中的問題時，將影像保留為草稿. 如需詳細資訊，請參閱文章中的「4月20日維護更新」一節 <a href="https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=en#updates-in-april-2023">2023年4月更新</a>.

### 2023 年 4 月 17 日

針對註解Beta版的問題和目標發佈了以下維護更新：

在問題 (新的註解 Beta 體驗) 和目標的更新區段顯示螢幕可見區域外的新註解. 如需詳細資訊，請參閱文章中的「4月17日維護更新」一節  <a href="https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=en#updates-in-april-2023">2023年4月更新</a>.


### 2023年4月6日當週

新的發表評論測試版體驗已針對問題推出。
針對Workfront物件的評論測試版所發行的相同功能，會針對有權存取Workfront目標的所有使用者同時發行目標。 如需詳細資訊，請參閱 [23.2版本總覽](../../product-releases/23.2-release-activity/23-2-release-overview.md).
