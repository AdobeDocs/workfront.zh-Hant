---
title: 2026年第二季版本總覽
description: 此頁面提供2026年第二季度版本中包含的功能相關資訊。 這些增強功能預計會在整個季度內於生產環境中提供。
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7e440fc0-45ad-4f73-ae7e-5374e4ae1480
source-git-commit: d721f04259046f271e9f420e445af6e87d67a5c0
workflow-type: tm+mt
source-wordcount: '1352'
ht-degree: 2%

---

# 2026年第二季版本總覽

本頁提供預定於2026年4月發行的2026年第二季度中所包含功能的相關資訊。

此頁面上的增強功能可在預覽環境中取得。 此頁面將在2026年第二季版本接近其計畫生產版本時以其他增強功能更新。


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>除非另有指定，否則每月和每季發行計畫於每月第二整週的星期四提供。
>
>| 每月發行 | 每季發行 |
>|----|----|
>| <ul><li>26.2 （2026年2月12日）</li><li>26.3 （2026年3月12日）</li><li>26.4 （2026年4月15日）</li></ul> | <ul><li>26.1 （2026年4月16日）</li></ul> |
>
>請注意，對於每季的最終發行（本季26.4版），快速發行排程中的使用者將提前一天收到發行（2026年4月15日）。
>
>如需快速發行程式的詳細資訊，請參閱[啟用或停用快速發行程式](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。

## Adobe Workfront增強功能

* [管理員增強功能](#administrator-enhancements)
* [檔案增強功能](#document-enhancements)
* [專案增強功能](#project-enhancements)
* [報告增強功能](#reporting-enhancements)
* [請求增強功能](#requesting-enhancements)
* [其他增強功能](#other-enhancements)

### 管理員增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
              <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>預覽</strong></td>
        <td><strong>快速發行</strong></td>
        <td><strong>每季</strong></td>
        </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">自訂季度已從專案偏好設定中移除</a><p>我們已將「自訂季度」區域從「專案偏好設定」區段移出。 它現在是「設定」中的獨立區段。</p>
        </td>
        <td><p>2025年3月5日</p></td>
        <td><p>2026年4月15日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">預設摺疊自訂表單區段</a><p>依預設，當表單本身展開時，自訂表單上的所有區段都會展開。 自訂表單設計工具上的新選項可讓您在使用者開啟表單時，將區段標示為預設摺疊。 此選項適用於區段層級，而非欄位。</p>
        </td>
        <td><p>2025年2月26日</p></td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}"> RTF文字欄位型別現在可用於自訂表單</a><p>自訂表單中的新<b>RTF</b>欄位型別是強大的文字編輯器，除了粗體、斜體、底線、專案符號、編號、超連結和區塊引號等傳統選項外，還有上標和下標、標題和表格等格式選項。 字元限制仍為15,000。</p>
        </td>
        <td><p>2026年1月29日</p></td>
        <td><p>2026年2月12日</p>
            <p>此功能已於2026年2月13日暫時從生產環境中移除。</p></td>
        <td><p>待定</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">Workfront電子郵件通知的新IP位址</a><p></p>
            <p>我們正在更新用來從Workfront傳送電子郵件通知的IP位址。 如果您的組織維護電子郵件或防火牆允許清單，您<b>必須</b>在下面新增新的IP位址，以確保繼續傳送Workfront通知。</p><p>這些更新套用至Workfront應用程式產生的所有傳出電子郵件，包括核准、提醒、校樣通知和其他系統訊息。</p>
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
        <td><p>2026年1月15日</p></td>
        <td><p>2026年1月15日</p></td>
        <td><p>2026年1月15日</p></td>
    <tr>
            </tbody>
        </table>

<!--

### Document enhancements

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>Feature</strong>
        </td>
        <td><strong>Preview</strong></td>
        <td><strong>Fast release</strong></td>
        <td><strong>Quarterly</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Multi‑stage approval workflows available for unified approvals</a><p></p>
            <p>Multi‑stage approval workflows are now available in unified approvals, helping organizations enforce structured, repeatable approval processes that reflect how work is reviewed in the real world. </p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-documents.md" class="MCXref xref" xrefformat="{para}">Set up and use multi-stage approval workflow templates</a><p></p>
            <p>You can now configure and reuse multi-stage approval workflow templates, making it easier to apply consistent governance across repeatable approval workflows. </p>
        </td>
        <td><p>February 26, 2025</p></td>
        <td><p>March 12, 2026</p></td>
        <td><p>April 16, 2026</p></td>
    </tr>
             </tbody>
        </table>   

-->

### 專案增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>預覽</strong></td>
        <td><strong>快速發行</strong></td>
        <td><strong>每季</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-projects.md" class="MCXref xref" xrefformat="{para}">當和單一或大量指派範本任務時更新體驗</a><p>[！BADGE Off Schedule]{type=Neutral}</p><p> 編輯單一範本任務或大量編輯範本任務時，我們已更新「編輯範本任務」方塊中的「工作總攬」區段。  </p>
        </td>
        <td><p>2026年2月5</p></td>
        <td><p>自2026年2月5日起</p></td>
        <td><p>自2026年2月5日起</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">單一或大量指派任務時更新體驗</a><p>[！BADGE Off Schedule]{type=Neutral}</p><p> 編輯單一任務或大量編輯任務時，我們已更新「編輯任務」方塊中的「工作總攬」區段。 </p>
        </td>
        <td><p>2026年1月26日</p></td>
        <td><p>自2026年2月5日起</p></td>
        <td><p>自2026年2月5日起</p></td>
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
        <td><strong>快速發行</strong></td>
        <td><strong>每季</strong></td>
    <tr>
        <td>
            建立報表時顯示<a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">自訂欄位標籤</a><p></p>
            <p>自訂欄位標籤現在顯示在報告建置工具中的欄位名稱和物件之前，可幫助您更輕鬆地找到欄位。 定義清單中的篩選器、檢視和分組時，也會顯示欄位標籤。</p>
        </td>
        <td><p>2025年2月26日</p></td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
   <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">可共用的報告資料夾</a><p></p>
            <p>您現在可以使用共用報告資料夾來整理和共用報告。 這項新功能可協助管理大量報表的團隊維持可擴充且一致的存取控制。</p>
        </td>
        <td><p>2025年2月26日</p></td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-reports.md" class="MCXref xref" xrefformat="{para}">已改善畫布儀表板中圖表群組的日期標籤</a><p></p>
            <p>按日期分組資料的圖表現在會顯示更清晰、更易讀取的日期標籤。 透過此更新，日期標籤會根據選取的「分組依據」選項（例如日、周、月或年）動態調整，使圖表更易於快速閱讀和理解。</p><p>注意：畫布儀表板目前是測試版。</p>
        </td>
        <td><p>2025年2月26日</p></td>
        <td><p>2026年3月12日</p></td>
        <td><p>2026年4月16日</p></td>
    </tr>
             </tbody>
        </table>

### 請求增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>預覽</strong></td>
        <td><strong>快速發行</strong></td>
        <td><strong>每季</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-requests.md" class="MCXref xref" xrefformat="{para}">已更新增強型檢視的共用體驗</a><p></p>
            <p>在新請求區域，當您與使用者共用增強型檢視並授予他們檢視許可權時，使用者可以修改檢視元素並將這些變更儲存到使用者的個人偏好設定。 他們現在可以選擇儲存包含其變更的檢視復本，或將共用檢視重設為原始設定。 他們可以進一步與他人共用複製的檢視。 </p>
        </td>
           <td><p>2025年2月26日</p></td>
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
        <td><strong>快速發行</strong></td>
        <td><strong>每季</strong></td>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience現在可供更多Workfront組織使用</a><p></p>
            <p>為了讓組織能夠存取Adobe Unified Experience的優點，我們繼續將其提供給現有的Workfront客戶。</p>
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

## 其他區域發行說明

### Workfront Fusion增強功能

Workfront Fusion的新功能可在標準發行排程以外的生產環境中使用。 如需最新功能的詳細資訊，請參閱[Adobe Workfront Fusion發行活動](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)。

### Workfront規劃增強功能

Workfront Planning的新功能可在生產環境中使用。 如需最新功能的詳細資訊，請參閱[Adobe Workfront Planning的2026年第二季度發行活動](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q2.md)。

此版本尚無下列專案的更新：

* 情境規劃工具
* 校樣
* 目標

## 案頭校訂檢視器更新

### 2.1.54 版

**所有客戶的生產版本： 2025年12月11日**

案頭校訂檢視器已從2.1.52更新至2.1.54。此更新包含內部工具更新，不會影響一般使用者功能。

2.1.53版也包含內部工具變更。

此更新同時適用於Mac和Windows。

## 公告

### Workfront規劃試用版現已推出

[!BADGE 關閉排程]{type=Neutral}

>[!NOTE]
>
>* 所有人的預覽和生產： 2026年3月2日
>* 您必須接受環境中可用的試用合約，才能存取Planning試用環境。
>* 您不需要簽署Adobe AI代理程式合約，就能在試用期間使用Planning Designer。

Workfront規劃試用版現在可供所有Workfront客戶使用。

自2026年3月2日起，免費試用版將為Workfront客戶提供存取Workfront Planning的60天Prime授權。 試用期將於2026年5月1日結束。

免費的Workfront Planning試用版提供下列功能：

* 經組織的多工作區規劃環境
* 範例資料，讓您瞭解從何處開始
* 產品內培訓和指導
* 在設定期間針對特定角色量身打造明確里程碑。
* Planning Designer — 由AI支援的助手，可幫助您建置您想要的環境

如需詳細資訊，請參閱[開始使用Adobe Workfront Planning免費試用](/help/quicksilver/planning/general/trial-workfront-planning.md)。

### API 21版

Workfront API版本21已於2025年10月23日發行。 針對API 21版，我們已修改一些資源和端點。 有些變更支援新功能，有些則讓您更輕鬆地透過API使用可用資訊。

>[!IMPORTANT]
>
>此API版本變更包含重大變更，可能會影響您現有的API呼叫。 這是因為API版本21使用事件訂閱版本2。
>
> 若為多選欄位，事件訂閱版本2一律會以陣列形式傳送。 如果選取多個值，第1版會傳送陣列。 如果只選取一個值，則會傳送字串。

如需新增和更新的詳細資訊，請參閱[ API 21](/help/quicksilver/wf-api/api/new-api-version-21.md)版的新增功能。

如需API版本的資訊，請參閱[API版本設定與支援排程](/help/quicksilver/wf-api/api/api-version-support-schedule.md)。

### 其他Workfront整合轉換

為了提供更穩定且更可擴充的整合，我們改用現代、彈性的整合方法，即使用Workfront自動化與整合(Fusion)。 在此轉換過程中，下列整合功能在&#x200B;**2026年2月28日**&#x200B;之後將無法使用：

* 適用於 G Suite 的 Workfront
* 適用於 Jira 的 Workfront
* 適用於Salesforce的Workfront。

為了滿足貴組織與Google Workspace的整合需求，我們建議您使用Workfront自動化和整合。
如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。


### Workfront 維護更新

如需2025年第二季期間所進行維護更新的相關資訊，請參閱[Workfront維護更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)。

### 訓練更新

探索每個Adobe Workfront產品版本的學習計畫、學習路徑、影片和指南的最新更新。 如需詳細資訊，請參閱[Workfront教學課程頁面](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html)的「新增功能」一節。
