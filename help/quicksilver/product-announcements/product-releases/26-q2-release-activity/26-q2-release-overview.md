---
title: 2026年第二季度發佈概述
description: 本頁提供有關2026年第二季度版本中包含的功能的資訊。 這些增強功能計畫在整個季度的生產環境中提供。
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7e440fc0-45ad-4f73-ae7e-5374e4ae1480
source-git-commit: 93c22854ccc405c442331ac392d919d63b8a8aa8
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 2%

---

# 2026年第二季度發佈概述

本頁提供有關計畫於2026年4月發佈的2026年第二季度產品中包含的功能的資訊。

此頁上的增強功能可在預覽環境中使用。 隨著2026年第二季度的生產計畫發佈接近，本頁將隨之更新，並附帶更多增強功能。


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>除非另有說明，每月和每季度的稿件計畫在本月第二完整周的星期四提供。
>
>| 每月發佈 | 季度發佈 |
>|----|----|
>| <ul><li>26.2（2026年2月12日）</li><li>26.3（2026年3月12日）</li><li>26.4（2026年4月15日）</li></ul> | <ul><li>26.1（2026年4月16日）</li></ul> |
>
>請注意，對於每個季度（本季度為26.4）的最終版本，快速發佈計畫的用戶將提前一天（2026年4月15日）收到該版本。
>
>有關快速發佈進程的詳細資訊，請參閱[啟用或禁用快速發佈進程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。

## Adobe Workfront增強

* [管理員增強](#administrator-enhancements)
* [文檔增強](#document-enhancements)
* [項目增強](#project-enhancements)
* [報告增強功能](#reporting-enhancements)
* [請求增強](#requesting-enhancements)
* [其他增強功能](#other-enhancements)

### 管理員增強

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
              <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>預覽</strong></td>
        <td><strong>快速發佈</strong></td>
        <td><strong>每季</strong></td>
        </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">從項目首選項中刪除的自定義季度</a><p>我們已將「自訂季度」區域從「專案偏好設定」區段移出。 它現在是「設定」中的獨立區段。</p>
        </td>
        <td><p>2026年3月5日</p></td>
        <td><p>2026年4月15日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">預設情況下折疊自定義表單節</a><p>預設情況下，在展開表單本身時，會展開自定義表單上的所有節。 自定義表單設計器上的一個新選項允許您在用戶開啟表單時標籤要預設折疊的節。 此選項在節級別應用，而不是在欄位上應用。</p>
        </td>
        <td><p>2026年2月26日</p></td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> RTF文字欄位型別現在可用於自訂表單</a><p>自定義表單中新的<b>富格文本</b>欄位類型是強健的文本編輯器，除了粗體、斜體、下划線、項目符號、編號、超連結和塊引號等傳統選項外，還具有上標和下標、標題和表格等格式選項。 字元限制仍為15,000。</p>
        </td>
        <td><p>2026年1月29日</p></td>
        <td><p>2026年2月12日</p>
            <p>此功能已於2026年2月13日從生產環境中暫時刪除。</p></td>
        <td><p>待定</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Workfront電子郵件通知的新IP位址</a><p></p>
            <p>我們正在更新用來從Workfront傳送電子郵件通知的IP位址。 如果您的組織維護電子郵件或防火牆允許清單，您<b>必須</b>在下面新增新的IP位址，以確保繼續傳送Workfront通知。</p><p>這些更新適用於Workfront應用程式生成的所有出站電子郵件，包括批准、提醒、證明通知和其他系統消息。</p>
            <ul>
            <li>美國：
            <ul>
            <li>206.55.149.212</li>
            <li>206.55.149.214</li>
            <li>206.55.149.215</li>
            <li>206.55.149.213</li>
            <li>206.55.149.211</li>
            </ul>
            </li>
            <li>歐盟： 
            <ul>
            <li>24.110.76.224</li>
            <li>24.110.76.223</li>
            </ul>
            </li>
            </ul> </p>
        </td>
        <td><p>2026年1月15</p></td>
        <td><p>2026年1月15</p></td>
        <td><p>2026年1月15</p></td>
    <tr>
            </tbody>
        </table>

### 文檔增強

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>預覽</strong></td>
        <td><strong>快速發佈</strong></td>
        <td><strong>每季</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">由Workfront和Frame.io支援的統一審查和批准</a><p></p>
            <p>我們很高興能推出由Workfront和Frame.io支援的統一審查和批准，這是一種簡化的審查和批准體驗，將規劃、校對和協作集中到一個連接的工作流中。
 </p>
        </td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月15日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">可用於統一審批的多階段審批工作流</a><p></p>
            <p>現在，多階段審批工作流可用於統一審批，幫助組織實施結構化、可重複的審批流程，以反映在真實世界中如何審查工作。 </p>
        </td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月15日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">設定和使用多階段審批工作流模板</a><p></p>
            <p>您現在可以配置和重新使用多階段審批工作流模板，從而更輕鬆地跨可重複審批工作流應用一致的治理。 </p>
        </td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月15日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
             </tbody>
        </table>


### 項目增強

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>預覽</strong></td>
        <td><strong>快速發佈</strong></td>
        <td><strong>每季</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-projects.md" class="MCXref xref" xrefformat="{para}">更新的時間和單個或批量分配模板任務的體驗</a><p>[!BADGE 關閉計畫]{type=Netral}</p><p> 在編輯單個模板任務或批量編輯這些任務時，我們已更新了「編輯模板任務」(Edit Template Tasks)框中的「工作總攬」(Assignments)部分。  </p>
        </td>
        <td><p>2026年2月5</p></td>
        <td><p>2026年2月5日起</p></td>
        <td><p>2026年2月5日起</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">單次或批量分配任務時更新的體驗</a><p>[!BADGE 關閉計畫]{type=Netral}</p><p> 在編輯單個任務或批量編輯任務時，我們已更新了「編輯任務」(Edit Tasks)框中的「工作總攬」(Assignments)部分。 </p>
        </td>
        <td><p>2026年1月26日</p></td>
        <td><p>2026年2月5日起</p></td>
        <td><p>2026年2月5日起</p></td>
    </tr>
            </tbody>
        </table>

### 報告增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>預覽</strong></td>
        <td><strong>快速發佈</strong></td>
        <td><strong>每季</strong></td>
        </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">資料連接連接的新身份驗證選項</a><p></p>
            <p>現在，您可以使用RSA密鑰或寫程式訪問令牌(PAT)連接對資料連接進行身份驗證，從而為傳統的用戶名/密碼憑據添加了更安全、更靈活的替代方案。 </p>
        </td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">生成報告時顯示的自定義欄位標籤</a><p></p>
            <p>自定義欄位標籤現在顯示在報表生成工具中的欄位名稱和對象之前，從而幫助您更輕鬆地查找欄位。 在清單中定義篩選器、視圖和分組時，也會顯示欄位標籤。</p>
        </td>
        <td><p>2026年2月26日</p></td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
   <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">可共用的報告資料夾</a><p></p>
            <p>您現在可以使用共用報告資料夾來整理和共用報告。 這項新功能可協助管理大量報表的團隊維持可擴充且一致的存取控制。</p>
        </td>
        <td><p>2026年2月26日</p></td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">畫布儀表板中圖表分組的改進日期標籤</a><p></p>
            <p>按日期分組資料的圖表現在顯示更清晰、更易讀的日期標籤。 通過此更新，日期標籤會根據選定的「分組依據」選項（如日、周、月或年）動態調整，使圖表更易於一目瞭然地閱讀和解釋。</p><p>注：畫布儀表板當前位於Beta中。</p>
        </td>
        <td><p>2026年2月26日</p></td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
             </tbody>
        </table>

### 請求增強

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>預覽</strong></td>
        <td><strong>快速發佈</strong></td>
        <td><strong>每季</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-requests.md" class="MCXref xref" xrefformat="{para}">已更新增強視圖的共用體驗</a><p></p>
            <p>在「新建請求」區域中，當您與用戶共用增強視圖並授予其「查看」權限時，用戶可以修改視圖元素，這些更改將保存到用戶的個人首選項中。 現在，他們可以選擇保存包含更改的視圖副本或將共用視圖重置為其原始設定。 它們可以進一步與他人共用複製的視圖。 </p>
        </td>
           <td><p>2026年2月26日</p></td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月16日</p></td>
 </tr>
            </tbody>
        </table>

### 其他增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>預覽</strong></td>
        <td><strong>快速發佈</strong></td>
        <td><strong>每季</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-other.md" class="MCXref xref" xrefformat="{para}">Adobe統一體驗現已可供更多Workfront組織使用</a><p></p>
            <p>為了讓組織能夠獲得Adobe統一體驗的好處，我們將繼續將它提供給現有的Workfront客戶。</p>
        </td>
        <td><p>2025年12月11日</p></td>
        <td><p>2026年2月11日</p></td>
        <td><p>2026年2月11日</p></td>
    </tr>
            </tbody>
        </table>


<!--### Functionality soon to be removed from Workfront-->

<!--

## Interface modernization

We are updating the interface throughout Adobe Workfront to improve the user experience and unify it with other Adobe applications. These changes are released outside the standard release schedule. For a list of these changes, see [Interface Modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

-->

## 發佈其他領域的說明

### Workfront融合增強

WorkfrontFusion的新功能在生產部門在標準發佈時間表之外的地方提供。 有關最新功能的詳細資訊，請參閱[Adobe WorkfrontFusion發行活動](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)。

### Workfront規劃功能增強

Workfront規劃的新功能可在生產中提供。 有關最新功能的詳細資訊，請參閱[Adobe Workfront規劃](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q2.md)的2026年第二季度發佈活動。

此時在發行版中沒有以下內容的更新：

* 情境規劃工具
* 校樣
* 目標

## 案頭校對查看器更新

### 2.1.54 版

**所有客戶的生產版本： 2025年12月11日**

案頭校對查看器已更新為2.1.52至2.1.54。此更新包括內部工具更新，不影響最終用戶功能。

2.1.53版還包括內部工具更改。

此更新適用於Mac和Windows。

## 公告

### Workfront計畫試用現已推出

[!BADGE 關閉計畫]{type=Neutral}

>[!NOTE]
>
>* 所有人的預覽和生產： 2026年3月2日
>* 您必須接受環境中可用的試用合約，才能存取Planning試用環境。
>* 在試用期內，您無需簽署Adobe AI代理協定即可使用計畫Designer。

Workfront規劃試驗現已面向所有Workfront客戶。

免費試用將從2026年3月2日起為Workfront客戶提供60天Prime許可證訪問Workfront規劃。 審判期於2026年5月1日結束。

免費的Workfront規劃試驗提供以下內容：

* 管理的多工作區規劃環境
* 範例資料，讓您瞭解從何處開始
* 產品內培訓和指導
* 在設定期間針對特定角色量身打造明確里程碑。
* Planning Designer — 由AI支援的助手，可幫助您建置您想要的環境

有關詳細資訊，請參閱[開始使用Adobe Workfront計畫免費試用版](/help/quicksilver/planning/general/trial-workfront-planning.md)。

### API版本21

WorkfrontAPI第21版於2025年10月23日發行。 對於API版本21，我們修改了一些資源和端點。 某些更改支援新功能，而其他更改則使您能夠更輕鬆地使用通過API提供的資訊。

>[!IMPORTANT]
>
>此API版本更改具有中斷更改的功能，可能會影響您現有的API調用。 這是由於API版本21使用事件訂閱版本2。
>
> 對於多選欄位，事件訂閱版本2始終作為陣列發送。 如果選擇了多個值，則版本1發送了一個陣列。 如果只選擇了一個值，則它發送了一個字串。

有關新增和更新內容的資訊，請參閱[API版本21](/help/quicksilver/wf-api/api/new-api-version-21.md)中的新增內容。

有關API版本的資訊，請參閱[API版本控制和支援計畫](/help/quicksilver/wf-api/api/api-version-support-schedule.md)。

### 其他Workfront一體化過渡

為了提供更穩定、更可擴展的整合，我們正在轉向使用Workfront自動化和整合(Fusion)的現代、靈活的整合方法。 作為此過渡過程的一部分，以下整合在2026年2月28日&#x200B;**之後將不可用：**

* 適用於 G Suite 的 Workfront
* 適用於 Jira 的 Workfront
* Workfront為Salesforce。

我們建議使用Workfront自動化和整合來滿足您組織與Google工作區的整合需求。
有關Workfront自動化和整合的概述，請參閱[Adobe Workfront融合概述](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。


### Workfront 維護更新

有關在2026年第二季度發佈期間進行的維護更新的資訊，請參閱[Workfront維護更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)。

### 培訓更新

瀏覽每個Adobe Workfront產品版本對學習計畫、學習路徑、視頻和指南的最新更新。 有關詳細資訊，請參閱[WorkfrontTutorials頁面](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html)的「新內容」部分。
