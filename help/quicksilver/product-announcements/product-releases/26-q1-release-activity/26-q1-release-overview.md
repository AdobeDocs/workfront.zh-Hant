---
title: 2026年第一季版本總覽
description: 本頁提供2026年第一季度版本中包含的功能相關資訊。 這些增強功能預計會在整個季度內於生產環境中提供。
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 353b71e59fc2dc2e1f806a560f04076586a32424
workflow-type: tm+mt
source-wordcount: '2949'
ht-degree: 1%

---

# 2026年第一季版本總覽

本頁提供預定於2026年1月發行的2026年第一季度版本中包含的功能相關資訊。

此頁面上的增強功能可在預覽環境中取得。 當2026年第一季版本接近其計畫生產版本時，此頁面將透過其他增強功能進行更新。


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>除非另有指定，否則每月和每季發行計畫於每月第二整週的星期四提供。
>
>| 每月發行 | 每季發行 |
>|----|----|
>| <ul><li>25.11 （2025年11月13日）</li><li>25.12 （2025年12月11日）</li><li>26.1 （2026年1月14日）</li></ul> | <ul><li>26.1 （2026年1月15日）</li></ul> |
>
>請注意，對於每季的最終發行（本季26.1版），快速發行排程中的使用者將提前一天收到發行（2026年1月14日）。
>
>如需快速發行程式的詳細資訊，請參閱[啟用或停用快速發行程式](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。

## Adobe Workfront增強功能

* [管理員增強功能](#administrator-enhancements)
* [檔案和核准增強功能](#documents-and-approvals-enhancements)
* [首頁增強功能](#home-enhancements)
* [整合增強功能](#integration-enhancements)
* [專案增強功能](#project-enhancements)
* [報告增強功能](#reporting-enhancements)
* [要求增強功能](#requests-enhancements)
* [其他增強功能](#other-enhancements)

### 管理員增強功能

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">管理配置範本中的優先順序</a>
            <p>您現在可以在版面配置範本中啟用或停用特定使用者的優先順序。 如果您先前已針對組織停用「優先順序」，則進行此變更後，其配置範本仍會停用。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2025年1月14日</td>
        <td>2025年1月15日</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">檢查已計算自訂欄位的多重表單衝突</a>
            <p>為了提供在自訂欄位上編輯運算式時可能影響哪些物件的可見度，我們新增了一個選項來檢查衝突。 此對話方塊會顯示所有可能因變更公式而受影響的物件（依物件型別分組）。 您可以導覽至每個物件的詳細資訊，並檢閱欄位以決定欄位應該從任何表單中移除還是運算式應該保持不變。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2025年1月14日</td>
        <td>2025年1月15日</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">輸入日期及自訂物件上儲存的識別碼</a><p>[！BADGE Off Schedule]{type=Neutral}</p>
            <p>輸入日期和由ID輸入的內容現在儲存在自訂表格、欄位和區段中。 您可以在報表中將這些資料選項作為篩選器、檢視或分組使用。 若要在「設定」中的自訂表單、欄位或區段清單中顯示它們，請新增「輸入日期」和「輸入者：名稱」作為新檢視或現有檢視中的欄。</p>
        </td>
        <td>2025年11月13日</td>
        <td>2025年11月13日</td>
        <td>2025年11月13日</td>
    </tr>  
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">編輯版面配置範本時按鈕名稱的更新</a>
            <p>為了提供與「設定」的其他區域（例如自訂表單設計工具）更加一致的方式，您在編輯版面配置範本時看到的按鈕已變更為「套用」、「儲存並關閉」和「取消」。 新選項「套用」可讓您將變更儲存至版面配置範本並繼續編輯。 以前，可用的選項為「儲存」和「取消」。 </p>
        </td>
        <td>2025年10月30日</td>
        <td>2025年11月13日</td>
        <td>2026年1月15日</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">已改善自訂欄位上使用作用中旗標的欄位管理</a>
            <p>當系統中有大量的自訂欄位時，在自訂表單和報告中的這些欄位可能會難以管理。 您現在可以使用新的<b>作用中</b>旗標將自訂欄位標示為非作用中。 在自訂表單上使用欄位或從「欄位」清單新增或編輯欄位時，此旗標可供使用。 </p>
        </td>
        <td>2025年10月30日</td>
        <td>2025年11月13日</td>
        <td>2026年1月15日</td>
    </tr>   
  </tbody>
</table>

### 檔案和核准增強功能

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">在Adobe Express中傳送評論時選擇Workfront專案<p>[！BADGE Off Schedule]{type=Neutral}</p> </a>
            <p>您可以選擇要將校樣傳送至的Workfront專案。 這有助於將所有相關的資產和校樣整理在同一個專案中。</p>
        </td>
        <td>2025年12月15日</td>
        <td>2025年12月15日</td>
        <td>2025年12月15日</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">具有Workfront校訂的Adobe Express跨組織支援<p>[！BADGE Off Schedule]{type=Neutral}</p> </a>
            <p>我們將推出具有Workfront校訂的Adobe Express跨組織支援。 此增強功能可讓跨多個IMS組織運作的客戶順暢地使用和管理校訂工作流程。</p>
        </td>
        <td>2025年11月13日</td>
        <td>2025年11月13日</td>
        <td>2025年11月13日</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Adobe Experience Manager現在可與Frame.io整合搭配使用 <p>[！BADGE Off Schedule]{type=Neutral}</p> </a>
            <p>現在，您可以使用Experience Manager Assets​來管理和儲存已通過檢閱和核准週期的數位資產。 此整合可讓您運用Adobe Experience Manager、Frame.io和Workfront的功能，簡化您的內容管理和共同作業程式。 </p>
        </td>
        <td>2025年10月30日</td>
        <td>2025年10月30日</td>
        <td>2025年10月30日</td>
    </tr>   
  </tbody>
</table>



### 首頁增強功能

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-home.md" class="MCXref xref" xrefformat="{para}">更新至首頁中的提及小元件</a>
            <p>我們對「首頁」中的「提及次數」小工具做了下列改良： <ul><li>在更新大多數Workfront物件的區域，現在也可以在首頁的提及小工具中獲得相同的體驗。 </li><li>「提及次數」Widget現在包含使用者在過去兩週內提出或標籤的評論</li><ul></p>
        </td>
        <td>2025年12月17日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>   
  </tbody>
</table>

### 整合增強功能

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">在Creative Cloud Express中傳送評論時選擇Workfront專案</a><p>[！BADGE Off Schedule]{type=Neutral}</p>
            <p>您可以選擇要將校樣傳送至的Workfront專案。 這有助於將所有相關的資產和校樣整理在同一個專案中。 </p>
        </td>
        <td>2025年12月15日</td>
        <td>2025年12月15日</td>
        <td>2025年12月15日</td>
    </tr>   
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">已更新Experience Manager Assets原生整合</a>之Adobe Workfront的資產選擇器
            <p>我們已升級Adobe Workfront中用於Experience Manager Assets整合的資產選擇器。 透過此升級，您現在可以選取AEM集合，並將其直接提取至Workfront。 </p>
        </td>
        <td>2025年11月20日</td>
        <td>2025年12月11日</td>
        <td>2026年1月15日</td>
    </tr>   
    <!-- <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">New version of Salesforce integration now available </a>
            <p>To stay up-to-date with recent changes to the Workfront API, we've created a new Salesforce integration. The new integration features the same functionality as the previous version, and was updated to avoid losing functionality deprecated in the API.</p><p>NOTE: The Workfront for Salesforce integration, including the new version, will not be available after **February 28, 2026**. </p>
        </td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
    </tr>   -->
  </tbody>
</table>

### 專案增強功能

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-projects.md" class="MCXref xref" xrefformat="{para}">輕度使用者可以在專案上登入時間</a>
            <p>輕度使用者現在可以直接在專案上記錄時間。 以前，只有Standard授權使用者可以在專案上記錄時數。</p>
        </td>
        <td>2025年12月11日</td>
        <td>2026年1月15日</td>
        <td>2026年1月15日</td>
    </tr>   
  </tbody>
</table>

### 報告增強功能

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">畫布儀表板中的貨幣更新</a>
            <p>我們已進行下列貨幣欄位更新：<ul><li>在Workfront中定義多種貨幣時，您現在可以在建立期間為儀表板選擇預設貨幣。 </li><li>建立報表時，您可以鎖定貨幣欄位。 這可確保儀表板層級的貨幣偏好設定不會影響這些值的顯示。</li><li>檢視控制面板時，使用者可以在Workfront中定義的任何貨幣之間切換。 這些變更會套用至整個儀表板，但鎖定的貨幣欄位除外</li></ul></p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
 <tr>
        <td>
            畫布儀表板中的<a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">快速搜尋表格結果</a>
            <p>我們在表格報表中新增了快速搜尋。 此搜尋可在所有頁面上運作，因此即使資料目前不可見，您也可以尋找資料。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">新的圓形圖顯示總計選項</a>
            <p>我們引進了新的「顯示總計」選項，可將圓餅圖轉換為環圈圖。 此功能可讓使用者顯示代表圖表中所有區段總計的中心值。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">畫布儀表板中圓形圖的新設定選項</a>
            <p>我們為圓形圖引進了兩個新的設定選項： <ul><li>隱藏區段標籤：如果區段標籤太長且影響圖表可讀性，您現在可以選擇隱藏圓形圖上的區段標籤。</li><li>隱藏和重新定點陣圖表圖例：您現在可以選擇隱藏圓形圖圖例。 您也可以將圖例的位置設定為圖表右側（預設）、左側、上方或下方。 </li></ul></p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">畫布儀表板群組計數改進</a>
            <p>我們已更新畫布儀表板中的分組列，以顯示目前頁面的記錄計數以及所有頁面分組的整體記錄計數。 </p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">在畫布儀表板中的報告中新增參考線功能</a>
            <p>您現在可以在長條圖、欄圖和折線圖中定義參考線，以設定四個序列式報表的目標或臨界值。 </p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">在畫布儀表板中自訂圖表報表的座標軸標籤</a>
            <p>您現在可以自訂圖表報表上的軸標籤。 此新功能可讓您輸入要顯示的取代軸標籤，而非預設物件和欄位路徑。 此外，您可以選擇完全隱藏軸標籤。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">在畫布儀表板中複製報告</a><p>[！BADGE Off Schedule]{type=Neutral}</p>
            <p>KPI、表格或圖表報表建立後，您現在可以在畫布控制面板中複製該報表。 複製後，您可在儲存前視需要編輯報表。</p>
        </td>
        <td>2025年10月23日</td>
        <td>2025年10月23日</td>
        <td>2025年10月23日</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">正在從報告篩選器移除欄位選項</a>
            <p>我們已移除下列先前在套用篩選器至報表時可使用的欄位選項：
            <ul>
            <li>其他群組識別碼</li>
            <li>其他角色ID</li>
            <li>其他團隊ID</li>
            </ul>
            </p>
        </td>
        <td>2025年11月6日</td>
        <td>2025年11月13日</td>
        <td>2026年1月15日</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">改善畫布儀表板中群組計數的顯示</a>
            <p>當表格報告有多個結果頁面且表格設定了分組時，表格現在會顯示目前頁面的記錄金額以及所有頁面的整體記錄計數。 例如，如果您的表格報表有7個群組，且第一頁顯示為3，則表格將顯示第3頁（共7頁）。</p>
        </td>
       <td>2025年11月6日</td>
        <td>2025年11月13日</td>
        <td>2026年1月15日</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">新護欄，改善畫布儀表板中的載入時間</a>
            <p>為避免載入時間延遲並改善畫布儀表板中的整體效能，我們已對可以新增到儀表板的儀表板元件數量套用了限制：
            <ul>
            <li>每個控制面板的報告：25個限制</li>
            <li>表格檢視的分組：5個限制</li>
            <li>與報表基本物件的距離： 10個限制</li>
            <li>表格檢視上的欄： 25限制</li>
            <li>儀表板層級篩選提示： 10個限制</li>
            </ul></p>
        </td>
       <td>2025年11月6日</td>
        <td>2025年11月13日</td>
        <td>2026年1月15日</td>
    </tr>   
  </tbody>
</table>

### 要求增強功能

<table style="table-layout:auto">
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
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">要求區域與我的要求Widget中現在有已建立的物件連結</a>
            <p>為了讓您更輕鬆地前往由特定請求建立的物件，我們已新增連結至「已建立的物件」欄。 現在，您可以按一下此欄中的連結，直接前往已建立物件的頁面。/p&gt;
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr> 
    <!--<tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Create groupings in the Requests list and My Requests widget</a>
            <p>To make it easier for you to find the requests you need, we've added groupings to the Requests list and the My Requests widget. Now, you can group requests by any column on the list. These groupings become part of the view that you are using when you create the grouping.</p>
        </td>
        <td>December 18, 2025</td>
        <td>January 14, 2026</td>
        <td>January 15, 2026</td>
    </tr> -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">新增自訂欄位至[請求]清單與[我的請求]小工具</a>
            <p>為了讓您更輕鬆地檢視您需要的資訊，我們新增了將自訂欄位新增為「請求」清單上的欄以及「首頁」中的「我的請求」Widget的功能。 現在，您可以從自訂表單新增欄位作為欄，並且該欄位中包含資訊的請求將在清單或Widget中顯示該資訊。</p><p>此功能僅在新的請求體驗中可用。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">要求篩選器現在提供</a>目前的使用者萬用字元
            <p>為了更方便篩選適用於您的請求，我們已建立目前的使用者萬用字元。 現在，篩選時，您可以選取「我（已登入使用者）」。 該篩選器將套用至正在檢視請求清單的使用者。   </p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">由AI提供支援的表單填寫現在可用於請求</a>
            <p>為了更方便建立請求，我們已建立由AI提供支援的表單填寫。 現在，您可以貼上提示或上傳檔案到請求表單，AI將提取相關資訊並填寫表單。  </p>
        </td>
        <td>2025年12月11日</td>
        <td>2025年12月11日</td>
        <td>2025年12月11日</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">在[要求]區域與[我的要求]介面工具集共用檢視</a>
            <p>為了更方便確保可檢視您所需的資訊，我們已新增將檢視共用至新報告體驗的功能。 現在，您可以與其他使用者、團隊或群組共用檢視。 </p>
        </td>
        <td>2025年12月4日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">將請求草稿儲存在新的請求體驗</a>
            <p>為了更方便建立及提交請求，我們已新增將草稿儲存至新請求體驗的功能。 現在，當您開始填寫並關閉請求時，請求會以草稿狀態儲存，並可在用於建立草稿的請求表單中找到。 之後，您可隨時重新開啟、更新及提交草稿。 </p>
        </td>
        <td>2025年11月20日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>  
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">刪除新請求體驗中的已提交請求</a>
            <p>為了更方便讓您的請求保持井然有序，我們已新增將請求刪除的功能至新的請求體驗。 現在，您可以刪除已提交的請求。 Workfront管理員和Workfront Planning Workspace管理員也可以刪除請求。</p>
        </td>
        <td>2025年11月20日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>   
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">複製新請求體驗中先前提交的請求，以建立新請求</a>
            <p>為了更方便提交請求，我們已新增將請求複製到新請求體驗的功能。 現在，您可以複製請求、編輯任何欄位，並將其提交為新請求。 </p>
        </td>
        <td>2025年11月20日</td>
        <td>2025年12月11日</td>
        <td>2026年1月15日</td>
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
    </tr>   
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">在2026年第一季度發行時間範圍內的外觀和感覺更新</a>
                        <p>在2026年第一季度發行時間範圍內，對Adobe Workfront應用程式的各個區域外觀和感覺進行了小幅更新。 </p>
                    </td>
                    <td><p>整個2026年第一季發行時間範圍<br /></p>
                    <td colspan="2"><p>快速發行：在發行至「預覽」後最少一週（除非另有指定）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                 <td>
                <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">多重選取欄位的選取限制</a>
              <p>使用者填寫表單時，允許多重選取的欄位（例如核取方塊和多重選取下拉選單）現在限製為5000個選取專案。</p>
             </td>
        <td>2025年10月30日</td>
        <td>2025年11月13日</td>
        <td>2026年1月15日</td>
             </tr>   
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Adobe Unified Experience現在可供更多Workfront組織使用</a><p></p>
            <p>為了讓組織能夠存取Adobe Unified Experience的優點，我們繼續將其提供給現有的Workfront客戶。</p>
        </td>
        <td><p>2025年12月11日</p></td>
        <td><p>2026年1月15日</p></td>
        <td><p>2026年1月15日</p></td>
    <tr>
            </tbody>
        </table>


### 即將從Workfront移除的功能

#### 25.11版本已棄用職務角色上的覆寫貨幣

作為財務模型簡化的一部分，我們將在10月30日的預覽版和25.11版本的所有客戶的生產版中淘汰工作角色的覆寫貨幣。 這項變更會影響貨幣和匯率在「設定」區域中職務角色的設定方式。

* 工作角色上的&#x200B;**覆寫貨幣**&#x200B;欄位將不再可用。
* 每個工作角色將具有單一貨幣及其相關成本和計費率。
* 所有現有的覆寫貨幣及其匯率值會自動移轉，成為該職務角色的唯一貨幣及匯率。

## 介面現代化

我們正在更新整個Adobe Workfront的介面，以改進使用者體驗，並將其與其他Adobe應用程式統一。 這些變更會在標準發行排程之外發行。 如需這些變更的清單，請參閱[介面現代化](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)。

## 其他區域發行說明

### Workfront Fusion增強功能

Workfront Fusion的新功能可在標準發行排程以外的生產環境中使用。 如需最新功能的詳細資訊，請參閱[Adobe Workfront Fusion發行活動](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)。

### Workfront規劃增強功能

Workfront Planning的新功能可在生產環境中使用。 如需最新功能的詳細資訊，請參閱[Adobe Workfront Planning的2026年第一季度發行活動](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q1.md)。

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

### 2.1.52 版

**所有客戶的生產版本： 2025年7月31日**

案頭校訂檢視器已更新至2.1.52版，解決錯誤修正問題。

2.1.51更新包含內部工具更新，不會影響一般使用者功能。

此更新同時適用於Mac和Windows。

## 公告

### API 21版

Workfront API版本21已於2025年10月23日發行。 針對API 21版，我們已修改一些資源和端點。 有些變更支援新功能，有些則讓您更輕鬆地透過API使用可用資訊。

>[!IMPORTANT]
>
>此API版本變更包含重大變更，可能會影響您現有的API呼叫。 這是因為API版本21使用事件訂閱版本2。
>
> 對於多選欄位，事件訂閱版本2一律會以陣列形式傳送。 如果選取多個值，第1版會傳送陣列。 如果只選取一個值，則會傳送字串。

如需新增和更新的詳細資訊，請參閱[ API 21](/help/quicksilver/wf-api/api/new-api-version-21.md)版的新增功能。

如需API版本的資訊，請參閱[API版本設定與支援排程](/help/quicksilver/wf-api/api/api-version-support-schedule.md)。

### 適用於Microsoft Teams的新版Workfront

隨著[Microsoft轉換至「新團隊」使用者端](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability)，傳統團隊使用者端在2025年7月1日之後將不再可用。 若要繼續使用Microsoft Teams和Workfront等整合式應用程式，客戶必須在此日期之前轉換至新Teams使用者端。

更新的Workfront整合現在可供使用，並且與新團隊體驗完全相容。 在大多數情況下，使用者轉換後，Workfront會自動顯示。 如果不適用，可從Microsoft Teams App Store手動安裝整合。 若要在New Teams使用者端中安裝或驗證Workfront整合，請參閱[為Microsoft Teams [!DNL Adobe Workfront] 安裝](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

### 適用於 Microsoft Outlook 的 Workfront

[Microsoft正在停用對舊版Exchange Online權杖](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支援，Workfront Outlook增益集目前使用這些權杖進行驗證。 Microsoft的這項變更已開始影響客戶，並將在2025年10月前持續分階段推出。

* **在Microsoft完全停用這些Token後，適用於Microsoft Outlook整合的Workfront將無法繼續運作。**

在這次變更中，Microsoft已決定變更代號重新啟用的方式。 在&#x200B;**2025年6月30日**&#x200B;之後，管理員將無法再自行重新啟用權杖 — 只有Microsoft支援可授予例外狀況。 **在2025年10月1日，所有租使用者的舊版代號將會關閉。 將不會授與例外。**

### 其他Workfront整合轉換

為了提供更穩定且更可擴充的整合，我們改用現代、彈性的整合方法，即使用Workfront自動化與整合(Fusion)。 在此轉換過程中，下列整合功能在&#x200B;**2026年2月28日**&#x200B;之後將無法使用：

* 適用於 G Suite 的 Workfront
* 適用於 Jira 的 Workfront
* 適用於Salesforce的Workfront。

為了滿足貴組織與Google Workspace的整合需求，我們建議您使用Workfront自動化和整合。
如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。


### Workfront 維護更新

如需2025年第一季度期間所進行維護更新的相關資訊，請參閱[Workfront維護更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)。

### 訓練更新

探索每個Adobe Workfront產品版本的學習計畫、學習路徑、影片和指南的最新更新。 如需詳細資訊，請參閱[Workfront教學課程頁面](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html)的「新增功能」一節。
