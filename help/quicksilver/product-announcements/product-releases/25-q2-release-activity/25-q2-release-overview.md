---
title: 2025年第二季版本總覽
description: 此頁面提供2025年第二季度版本中包含的功能相關資訊。 這些增強功能預計會在整個季度內於生產環境中提供。
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9b78a58e-7ced-4b13-8108-40bd36339667
source-git-commit: 75ff6f954c1a53a36d64c4f428097fe9a0c4b053
workflow-type: tm+mt
source-wordcount: '1722'
ht-degree: 0%

---

# 2025年第二季版本總覽

此頁面提供2025年第二季度版本中包含的功能相關資訊。 這些增強功能預計會在整個季度內於生產環境中提供。

<span class="preview">週期外功能（在2025年第二季發行日期之前發佈到生產環境的功能）會以黃色標示。</span>

## 發行排程

Workfront版本編號代表每月和每季的版本追蹤。 第一個數字代表年份，第二個數字代表發行月份。 範例： 2025年4月版本的編號為25.4。

除非另有指定，否則每月和每季發行計畫於每月第二整週的星期四提供。

| 每月發行 | 每季發行 |
| ----------------- | ----------------- |
| <ul><li>25.2 （2025年2月13日）</li><li>25.3 （2025年3月13日）</li><li>25.4 （2025年4月10日）</li></ul> | <ul><li>25.4 （2025年4月10日）</li></ul> |

>[!NOTE]
>
>對於每季的最終發行（本季25.4版），快速發行排程中的使用者將提前一天收到發行。
>
>如需快速發行程式的詳細資訊，請參閱[啟用或停用快速發行程式](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。

## Adobe Workfront增強功能

* [管理員增強功能](#administrator-enhancements)
* [檔案管理增強功能](#document-management-enhancements)
* [行動裝置增強功能](#mobile-enhancements)
* [專案增強功能](#project-enhancements)
* [報告增強功能](#reporting-enhacements)
* [其他增強功能](#other-enhancements)

### 管理員增強功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            自訂表單邏輯的增強功能</a></p><p>[！BADGE In Production ]{type=Informative}</p>
            <p>自訂表單邏輯產生器有更新的介面，為您提供建立邏輯規則的更多空間。 此新設計可更輕鬆地容納未來可能新增的其他邏輯型別。</p><p>除了目前的顯示和略過邏輯選項外，您也可以使用驗證邏輯。</p>
        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <li>預覽版本： 2025年3月13日</li>
                <li>適用於所有客戶的生產版本：第25.4版本（2025年4月）</li>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            新增到計算自訂欄位的運算式</a></p>
            [！BADGE In Production ]{type=Informative}
            <p>Workfront計算自訂欄位現在提供下列運算式：ARRAY、FORMAT、SWITCH、SORTASCARRAY、SORTDESCARRAY、ARRAYLENGTH、ARRAYELEMENT和ADDHOUR。 計算編輯器和Experience League上提供每個運算式的定義和範例。</p>
        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <li>預覽版本： 2025年1月31日</li>
                <span class="preview"><li>所有客戶的生產版本： 2025年1月31日</li></span>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### 檔案管理增強功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            校訂檢視器中可用的新檔案核准決定按鈕</a></p>
            <p>新檔案核准決定按鈕現在會出現在校訂檢視器中。 現在，當您建立簡單的校訂，然後從檔案摘要新增核准者和稽核者時，他們可以直接在校訂檢視器中做出決定。</p>
        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <li>預覽版本： 2025年4月9日</li>
                <li>有限客戶的生產版本：25.4版本（2025年4月）</li>
            </ul>
        </td>
    </tr>                        
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            案頭校訂檢視器更新 </a></p>[！BADGE In Production ]{type=Informative}
            <p>案頭校訂檢視器已更新至2.1.45版。此更新可讓檢視器使用
            <ul><li>Electron 35版</li><li>Chromium 134版</li><ul></p>
        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <li>預覽版本： 2025年3月20日</li>
                <span class="preview"><li>所有客戶的生產版本： 2025年3月20日</li></span>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            在檔案報告中一次編輯多個檔案 </a></p>[！BADGE In Production ]{type=Informative}
            <p>您現在可以在檔案報告中一次編輯多個檔案。 您可以編輯說明並更新自訂表格。</p>
        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <li>預覽版本： 2025年2月6日</li>
                <span class="preview"><li>所有客戶的生產版本： 2025年3月13日</li></span>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### 行動裝置增強功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">
            行動應用程式中校訂的增強功能(僅限iOS)</a><p>[！BADGE In Production ]{type=Informative}</p></p>
            <p>Adobe Workfront行動應用程式中的校訂功能有數個增強功能：
            <ul>
            <li>您現在可以從您的行動電子郵件應用程式，透過與您共用的連結開啟校訂檔案。 以前不支援電子郵件中的連結，因此您必須從Workfront行動應用程式存取校樣。</li>
            <li>行動應用程式現在支援多媒體校訂檔案。</li>
            </ul>
            </p>
        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <li>預覽版本：不適用</li>
                <span class="preview"><li>所有客戶的生產版本： 2025年3月12日</li> 
            </ul>
            <p><b>適用於下列環境：</b></p>
            <ul>
                <li>iOS行動應用程式</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### 專案增強功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-project-enhancements.md" class="MCXref xref" xrefformat="{para}">
            在編輯專案方塊中編輯專案時，為專案新增註解</a><p>[！BADGE In Production ]{type=Informative}</p>
            <p>您現在可以在「編輯專案」方塊中編輯專案時，將註解新增至專案。 您也可以在大量編輯專案時，一次為多個專案新增註解。 在此更新之前，編輯專案時不存在此功能。</p>
        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <li>預覽版本： 2025年2月13日</li>
                <li>快速發行生產：第25.3發行版本（2025年3月）</li>
                <li>適用於所有客戶的生產版本：第25.4版本（2025年4月）</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### 報表增強功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">
            Data Connect現在提供檔案核准和決定資料</a><p>[！BADGE In Production ]{type=Informative}</p>
            <p>您現在可以在Data Connect中存取檔案核准和決定的資料。 此資料集橋接來自Workfront校訂功能和Workfront檔案上發生的Frame.io核准的檔案。 您現在將能夠透過BI視覺效果說明週期時間、週期數和時間表對延遲核准的影響。</p>
        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <li>預覽版本： 2025年3月25日</li>
                <li>所有客戶的生產版本： 2025年3月25日</li>
            </ul>
        </td>
    </tr>                          
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront行事曆的更新</a></p><p>[！BADGE In Production ]{type=Informative}</p>
            <p>我們已將Workfront行事曆的外觀與風格更新為與Workfront其他區域一致的現代化設計。 與目前的Workfront行事曆在功能上有細微的差異，包括：
            <ul>
            <li>如何將臨時專案新增至行事曆</li>
            <li>如何建立及重新命名行事曆</li>
            <li>行事曆動作已移至行事曆名稱旁的「更多」功能表</li>
            <li>檢視行事曆資訊的新側面板</li>
            <li>及更多內容</li>
            <ul>        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <li>預覽版本： 2025年2月27日</li>
                <li>此功能將分三階段推出至「生產」環境：從25.4版（2025年4月10日）開始，到2024年4月17日完成</li>
            </ul>
        </td>
    </tr>                          
</tbody>
</table>

### 其他增強功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            升級至具有版本升級端點的新事件訂閱版本</a></p>
            [！BADGE In Production ]{type=Informative}
            <p>Workfront現在提供不同版本的事件訂閱。 新版本並非變更Workfront API，而是變更事件訂閱功能。 您可以將活動訂閱切換至新版本，而不會在活動訂閱中造成間隙</p>
        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <span class="preview"><li>所有客戶的生產版本： 2025年3月6日</li></span>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            在Workfront更新摘要中將Adobe Admin Console使用者變更顯示為「系統」</a></p><p>[！BADGE In Production ]{type=Informative}</p><p>現在，當Adobe Admin Console管理員變更Workfront使用者的使用者資訊時，Workfront會在使用者更新區域的系統活動標籤中，將此變更記錄為屬於「系統」。 他向Adobe Admin Console管理員求助。</p>
        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <li>預覽版本： 2025年1月23日</li>
                <li>快速發行生產：25.2版（2025年2月13日）</li>
                <li>適用於所有客戶的生產版本：第25.4版本（2025年4月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            2025年第二季時間範圍內的外觀和感覺更新</a></p>
            <p>在2025年第二季時間範圍內，對Adobe Workfront應用程式的各個區域外觀和感覺進行了小幅更新。 檢閱特定發行日期的個別發行說明。</p>
        </td>
        <td>
            <p><b>將於下列日期提供：</b></p>
            <ul>
                <li>預覽版本：在整個2025年第二季度版本時間範圍內</li>
                <span class="preview"><li>生產版本：檢閱特定日期的發行說明</li></span>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### 即將從Workfront移除的功能

下列功能即將從Workfront中移除：

#### API 2-15版已淘汰

隨著我們持續增強Workfront平台，務必讓API保持最新狀態。 這可確保最佳效能和安全性，並支援新功能。 因此，我們將淘汰Workfront API 2-15版。

* **2025年9月**：目前不支援的API版本2-14將被棄用。 在此日期之後，您將無法再存取這些版本。
* **2025年12月**： API 15版將被棄用。

#### 我們正在移除專案中的舊版敏捷檢視

專案中的舊版敏捷檢視將在2025年3月13日的25.3版本中從Workfront移除。 您仍然可以按一下面板圖示，在專案的敏捷檢視中檢視您的任務。 現有的舊版敏捷工具仍可在「團隊」區域中使用。

下圖顯示將移除的舊版敏捷選項：
![舊版敏捷檢視連結](assets/project-agile-board-view.png)


#### 增強型Analytics淘汰

由於使用率低且不斷下降，我們已決定在2025年5月25日當週淘汰增強型分析產品。
建議您考慮改用Data Connect產品。 Data Connect可讓您使用慣用的商業智慧工具，建立類似的可自訂視覺效果。
如需關於此棄用的詳細資訊，請參閱[Enhanced Analytics棄用指南](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)。

## 公告

### 介面現代化

我們正在更新整個Adobe Workfront的介面，以改進使用者體驗，並將其與其他Adobe應用程式統一。 這些變更會在標準發行排程之外發行。 如需這些變更的清單，請參閱[介面現代化](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)。

### Workfront Fusion增強功能

>[!IMPORTANT]
>
>Workfront Fusion檔案已移至新位置。 如需Fusion的資訊、指示和發行版本，請造訪[Workfront Fusion檔案](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/home)。
>
>每篇目前的Fusion檔案文章都包含一個連結，指向新位置中對應的文章。 請更新您的書籤。
>
>目前的Fusion檔案集已不再更新，不久將會移除。

Workfront Fusion的新功能可在標準發行排程以外的生產環境中使用。 如需最新功能的詳細資訊，請參閱[Adobe Workfront Fusion發行活動](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)。

### Workfront規劃增強功能

Workfront Planning的新功能可在生產環境中使用。 如需最新功能的詳細資訊，請參閱[Adobe Workfront規劃2025年第二季發行活動](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q2.md)。

### Workfront Scenario Planner增強功能

此版本中目前沒有Scenario Planner更新。 在有更新可用時，此區域將會更新。

### Workfront Proof增強功能

此版本目前沒有Workfront Proof更新。 在有更新可用時，此區域將會更新。

### Workfront目標增強功能

此版本中目前沒有Workfront目標更新。 在有更新可用時，此區域將會更新。

### API 19版

針對API版本19，我們已修改一些資源和端點。 有些變更支援新功能，有些則讓您更輕鬆地透過API使用可用資訊。

如需新增和更新的詳細資訊，請參閱[ API 19](/help/quicksilver/wf-api/api/new-api-version-19.md)版的新增功能。

如需目前支援哪些API版本的資訊，請參閱[API版本設定與支援排程](/help/quicksilver/wf-api/api/api-version-support-schedule.md)。

### Workfront 維護更新

如需2025年第二季期間所進行維護更新的相關資訊，請參閱[Workfront維護更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)。

### 訓練更新

探索每個Adobe Workfront產品版本的學習計畫、學習路徑、影片和指南的最新更新。 如需詳細資訊，請參閱[Workfront教學課程頁面](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html)的「新增功能」一節。
