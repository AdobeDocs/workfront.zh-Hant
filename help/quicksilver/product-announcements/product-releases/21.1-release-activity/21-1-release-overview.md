---
content-type: release-notes
keywords: 附註，每季，更新
navigation-topic: product-releases
title: 21.1版本概觀
description: 21.1版已於的當周提供於生產環境中使用。
author: Luke
feature: Product Announcements
exl-id: 3affee76-347e-4610-b255-4b1bb4414c5d
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '3635'
ht-degree: 0%

---

# 21.1版本概觀

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 21.1 release was made available in the Production environment the week of .</p>
-->

本頁提供Adobe Workfront Classic和21.1版中新Adobe Workfront體驗功能的相關資訊。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

通過此版本，我們推出了新功能和增強功能，以幫助您通過適應性強的策略、自動化的工作流程和連接的數字基礎架構引領2021年的復出，從而在整個企業中取得成功。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 21.1 release nears its planned Production release, this page will be updated with all functionality included with 21.1.</p>
-->

目前提供這些增強功能

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the Preview environment and will be made available
</MadCap:conditionalText>
-->

在生產環境中。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the first quarter of 2021
</MadCap:conditionalText>
-->

在2021年2月15日當周發行。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.workfront.com/" target="_blank">Adobe Workfront Status Site</a>.
</MadCap:conditionalText>
-->

## Adobe Workfront增強功能

* [管理員增強功能](#administrator-enhancements)
* [資源管理增強功能](#resource-management-enhancements)
* [專案管理增強功能](#project-management-enhancements)
* [增強的分析功能](#enhanced-analytics-improvements)
* [整合增強功能](#integration-enhancements)
* [行動裝置增強功能](#mobile-enhancements)
* [其他增強功能](#other-enhancements)

### 管理員增強功能 {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期和環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">引入新的「存取層級」設定來複製專案</a> </p> <p>為了讓您作為系統管理員能夠更好地控制規劃人員可以對項目執行什麼操作，我們引入了允許您啟用或禁用其複製項目能力的新設定，使訪問級別的項目的編輯訪問更加精細。 在此變更前，當您啟用使用者的「編輯」專案存取權時，他們會自動擁有複製專案的存取權。 使用新功能，您可以讓使用者存取編輯專案的權限，而無需借由停用新的「複製」設定來複製專案。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2021年1月13日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#in" class="MCXref xref" xrefformat="{para}">在物件的「自訂表單」中，在多選下拉式欄位中選取所有項目</a> </p> <p>在對象的「詳細資訊」(Details)頁面上，在「自定義表單」上填寫多選下拉欄位時，如果需要選擇所有可用選項，可以按一下「全部選擇」。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2021年1月13日</p> <p>生產版本：隨著第21.1發行版本 <span style="color: #dc143c; font-weight: bold;">（目前無法在您提交新請求時使用。）</span></p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#recalcul" class="MCXref xref" xrefformat="{para}">重新計算對象的所有自定義表單欄位</a> </p> <p>現在可更輕鬆確保計算的自訂欄位中的所有資料都為物件最新。 新的「重新計算表達式」菜單選項可讓您快速重新計算這些欄位中的所有資料。</p> <p>當某人編輯另一個物件中的資料時（該物件中的已計算自訂欄位已參照），這個用法特別有用。</p> <p>過去，使用者必須使用因應措施，以確保計算自訂欄位中的所有資料都為最新資料。 例如，他們編輯了對象以及其他對象，以使用可用於批量編輯的重新計算選項。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月10日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#unlock" class="MCXref xref" xrefformat="{para}">解鎖組管理員的任務和問題首選項</a> </p> <p>Workfront管理員現在可以解除鎖定個別任務和問題偏好設定，讓群組管理員擁有更大的自治權。 當首選項解除鎖定時，組管理員可以為其組配置該首選項，以滿足每個組的獨特需要和內部進程。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月2日</p> <p>生產版本：隨著第21.1發行版本 <span style="color: #dc143c; font-weight: bold;">(在2021年6月24日之前，這是分階段推出的一部分，僅針對叢集4和6的客戶以及其他一些客戶。 現在，所有客戶都可在生產環境中使用。)</span></p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">分別配置產品組合和程式的訪問級別設定</a> </p> <p>現在管理使用者對產品組合和方案的存取權限更為輕鬆，因為您可以個別設定其存取層級設定。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月2日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">在「自訂表單」中編輯資訊時，選取系列中的所有核取方塊</a> </p> <p>在對象的「詳細資訊」頁上，當您填寫包含複選框的「自定義表單」欄位時，如果需要選擇所有可用複選框，則可以按一下「全部選擇」。</p> <p>只有在欄位包含超過2個核取方塊時，才會顯示此選項。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月2日</p> <p>生產版本：隨著第21.1發行版本 <span style="color: #dc143c; font-weight: bold;">（目前無法提交請求）。</span></p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur2" class="MCXref xref" xrefformat="{para}">設定Workfront電子郵件允許清單</a> </p> <p>為了更妥善保護您的資料，您現在可以使用電子郵件網域允許清單：</p> 
    <ul> 
     <li> <p>如果Workfront電子郵件包含儲存在Workfront中的報表或檔案，請控制其可前往的位置</p> </li> 
     <li> <p>控制電子郵件網域可以位於使用者可在其使用者設定檔中指定的電子郵件地址中</p> </li> 
    </ul> <p>例如，如果您想要保護敏感資料，例如列出您面臨風險之客戶的報表，則只能在電子郵件允許清單中納入您的內部電子郵件網域或網域。 如此一來，使用者就無法將該報表(或任何其他Workfront報表)傳送至外部電子郵件地址。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年11月20日</p> <p>生產版本：隨著第21.1發行版本 </p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">為子組分配組管理員</a> </p> <p>為了讓您的組織級別更容易獨立運行，我們添加了將組管理員分配給子組的能力。 現在，您可以確保將子組管理委派給正確的人員。</p> <p>以前，只有頂級組才能有組管理員，這些管理員管理了頂級組下的所有子組。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年11月20日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#work" class="MCXref xref" xrefformat="{para}">在「組」區域中使用組項目和審批流程</a> </p> <p>如果您是群組管理員，現在將群組的專案和核准程式列在「群組」區域中，您就能輕鬆檢視及處理這些專案和核准程式。 </p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年11月20日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur3" class="MCXref xref" xrefformat="{para}">設定群組的事件通知</a> <span style="color: #dc143c; font-weight: bold;">預覽新增功能！</span></p> <p>Workfront管理員現在可讓群組管理員為其頂層群組設定事件通知，以賦予群組管理員更多自治權。 子組會從其父組繼承事件通知配置。</p> <p>以前，事件通知只能由系統層級的Workfront管理員設定，這表示所有群組都必須使用同一組事件通知。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2021年1月22日</p> <p>生產版本：隨著第21.1發行版本 <span style="color: #dc143c; font-weight: bold;">(最初僅供叢集4的客戶在分階段推出時使用；不久後可用於其他群集)</span></p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">查看組中使用和分配的許可證數</a> </p> <p>要確定許可證的分配程度，您現在可以查看組中使用的許可證數，以及組下的任何子組。</p> <p>如果管理頂級組，則可以查看組（及其子組）中使用的許可證數以及為組分配的許可證數上限。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年11月20日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 資源管理增強功能 {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期和環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workload" class="MCXref xref" xrefformat="{para}">項目的工作負載平衡器</a> </p> <p>現在，工作負載平衡器可在項目中使用。 現在，您可以選擇使用工作負載平衡器或調度工具來管理項目資源。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月17日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront平衡器適用於團隊</a> </p> <p>工作負載平衡器現在可在團隊中使用。 現在，您可以選擇使用工作負載平衡器或調度工具來管理您的團隊資源。 </p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年11月20日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 專案管理增強功能 {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期和環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">現在可在專案的「量度」區段中使用匯出</a> </p> <p>若要更輕鬆共用專案的狀態和進度，您現在可以將專案「量度」區段中的整個控制面板匯出為.png檔案。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2021年1月15日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#update" class="MCXref xref" xrefformat="{para}">更新從問題更新轉換的項目或任務完成的問題百分比</a> </p> <p>我們已更新問題完成百分比對於已轉換為專案或工作的問題的運作方式。 使用新功能時，當問題轉換為任務或項目時，問題完成百分比將與解決任務或項目完成百分比同步，當「在解決對象的狀態更改時自動更新可解決的問題狀態」設定從設定中啟用時。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2021年1月13日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#fields" class="MCXref xref" xrefformat="{para}">從「新請求」頁面移除的欄位</a> </p> <p>在重新設計「新請求」頁面時，我們已更新專案「佇列設定」區段中設定的「新問題欄位」。</p> <p>只有在從專案的「問題」區段建立問題時，才會顯示各種「新問題欄位」。 在「請求」區域中使用請求佇列提交問題時，系統不會顯示問題。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2021年1月13日</p> <p>生產版本：隨著第21.1發行版本 <span style="color: #dc143c; font-weight: bold;">（從版本中移除）</span></p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">在「請求」區域提交請求時的新體驗</a> </p> <p>為了與新的Workfront體驗保持一致，並在提交請求時提高效率，我們已重新設計「請求」區域的「新請求」方塊。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2021年1月13日</p> <p>生產版本：隨著第21.1發行版本 <span style="color: #dc143c; font-weight: bold;">(從發行中移除；將保持預覽狀態，並透過21.2發行至生產環境)</span></p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#share" class="MCXref xref" xrefformat="{para}">在提交請求時共用請求佇列的連結</a> </p> <p>現在，當您建立請求時，可以共用請求佇列、主題群組或佇列主題的連結。</p> <p>在提交新請求之前，您可以複製請求的請求佇列、主題群組或佇列主題的連結，並與其他使用者共用，或將其內嵌在控制面板中。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2021年1月13日</p> <p>生產版本：隨著第21.1發行版本 <span style="color: #dc143c; font-weight: bold;">(從發行中移除；將保持預覽狀態，並透過21.2發行至生產環境)</span></p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">新提交的請求清單</a> </p> <p>為了讓您以更簡單、更一致的方式管理您的「已提交請求」，我們已移除「請求」區域中的「我已提交的請求」和「所有請求」區段，並以新的「已提交」清單取代這些區段。 清單的外觀和風格與系統中的所有其他清單相符，可讓您篩選不同類別的已提交請求，並快速搜尋可能很難找到的請求。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月2日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#search" class="MCXref xref" xrefformat="{para}">搜尋您要指派給專案的群組並檢視其詳細資料</a> </p> <p>現在，在將群組指派至專案時，可更輕鬆確定您識別正確的群組。 將滑鼠指標暫留在「群組」方塊中找到的群組名稱上，然後按一下名稱旁顯示的資訊圖示，即可檢視「群組詳細資料」工具提示。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月17日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">新使用者委派報表</a> </p> <p>以前，任務、問題和項目核准委託的資訊只能由其所在區域的代表查看。 為了讓其他使用者看到此資訊，計畫使用者現在可以建立「使用者委派」報表，該報表會告訴您：</p> 
    <ul> 
     <li> <p>已將這些批准委託給其他用戶</p> </li> 
     <li> <p>已委派這些核准的使用者</p> </li> 
     <li> <p>這些代表團的開始和結束日期</p> </li> 
    </ul> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月17日</p> <p>生產版本： 2021年1月21日</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 增強的分析功能 {#enhanced-analytics-improvements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期和環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#people" class="MCXref xref" xrefformat="{para}">「人員」頁現在可用於所有群集</a> </p> <p>適用於叢集4的Workfront Classic現在提供「人員」頁面。 此頁包括按小組、資源能力和小組能力列出的活動的圖表。</p> <p>此頁面之前可在Workfront Classic和適用於所有其他叢集的新Workfront體驗中搭配20.3版本使用。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2021年1月28日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>新的Adobe Workfront體驗（先前提供）</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#enhanced" class="MCXref xref" xrefformat="{para}">現在預設會顯示增強的分析</a> </p> <p>注意：此變更僅適用於新新增至「版面範本」的使用者。 指派給自訂配置範本的使用者也不受此變更影響。</p> <p>在預設的「配置範本」中，現在預設會啟用「Analytics」區域，這表示指派給此「配置範本」的使用者現在可以在Workfront Classic的「全域導覽列」和新Workfront體驗的「主功能表」中看到「Analytics」區域。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行日期：2020年11月6日</p> <p>生產發行： 2020年12月3日</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#availab" class="MCXref xref" xrefformat="{para}">所有叢集皆可使用的增強分析功能</a> </p> <p>所有Workfront叢集（包括叢集6上的客戶）都可使用增強的分析。</p> <p>之前，Google雲端平台無法使用增強的分析功能，導致叢集6上的客戶無法存取Analytics區域。 現在，叢集6的企業和企業客戶可以存取Analytics區域。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年11月20日</p> <p>生產發行： 2020年12月3日</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 整合增強功能 {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期和環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Adobe Workfront通知增強功能(Microsoft Teams)</a> </p> <p>為了讓您透過Microsoft Teams更輕鬆使用Workfront，我們已針對從Workfront傳送的Microsoft Teams通知新增各種增強功能。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽版本：不適用</p> <p>生產版本： 2021年1月12日</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 行動裝置增強功能 {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期和環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Adobe Workfront應用程式中的新導覽階層連結</a> </p> <p>我們已將階層連結導覽新增至Workfront行動應用程式。 現在，您可以使用此功能來導覽至專案內的父工作項目。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽版本：不適用</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#rich" class="MCXref xref" xrefformat="{para}">Workfront應用程式上自訂表單支援的RTF文字</a> </p> <p>您現在可以在Workfront行動應用程式的自訂表單文字欄位中使用RTF格式。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽版本：不適用</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#sso" class="MCXref xref" xrefformat="{para}">SSO使用者現在可以透過Face ID或Fingerprint技術重新登入Workfront應用程式</a> </p> <p>如果貴組織使用SSO，您現在可以在工作階段逾時後，使用您的Face ID或Fingerprint登入Workfront行動應用程式。 但您最初必須使用SSO憑證登入。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽版本：不適用</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>
—&gt;

### 其他增強功能 {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>發行日期和環境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">事件訂閱失敗要求的更新</a> </p> <p>我們正在更新事件訂閱失敗的軟禁用要求。 除了現有需求，如果「事件訂閱」在2000次嘗試內都未成功傳送，現在將會軟性停用。 這是為了加強現有的70%故障規則，在某些情況下，這會導致過多的故障。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽版本：不適用</p> <p>生產版本： 2021年1月11日</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">「每日摘要」提供的「新團隊」欄位</a> </p> <p>已將「團隊核准」和「指派」欄位新增至「需要動作的每日摘要」電子郵件。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月17日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#replacin" class="MCXref xref" xrefformat="{para}">替換請求隊列中的POP電子郵件選項</a> </p> <p>我們正在將請求隊列的POP電子郵件選項替換為新的Workfront管理系統。 您仍可以透過電子郵件提交請求，但您需要在「請求佇列」區域中設定新的Workfront管理電子郵件地址。 </p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月17日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">在工時單上限制小時編輯</a> </p> <p>為了對工時單和工時編輯提供更多控制，我們添加了一個設定，允許您限制對工時單所有者和系統管理員進行工時編輯。</p> <p>以前，在訪問級別啟用了「工時單和工時」選項的用戶可以編輯任何工時單上的工時。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2021年1月21日</p> <p>生產版本：隨著第21.1發行版本</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">改進「工時單」區域中的篩選器和視圖</a> </p> <p>我們已新增專案和問題的篩選器，以及「搜尋」頁面中的「檢視」和「分組」選項。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月2日</p> <p>生產版本： 2021年1月21日</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#hide" class="MCXref xref" xrefformat="{para}">在工時單中隱藏加班框</a> </p> <p>如果您不在Workfront中追蹤加班，現在可以隱藏加班方塊以減輕使用者混淆。 您可以隱藏一次性工時單或工時單配置檔案的加班框。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月2日</p> <p>生產發行： 2020年12月16日</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#expand" class="MCXref xref" xrefformat="{para}">展開或折疊階層連結導覽中的項目</a> </p> <p>為了更輕鬆檢視完整的階層連結路徑，我們新增了展開和折疊功能。</p> <p>現在，任何截斷的項目都會在專案前分組，並加上文字「更多」。 例如，「3個以上」表示有3個物件沒有顯示。</p> <p>之前，您必須按一下省略號，才能在下拉式選單中顯示任何截斷的物件。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年1月7日</p> <p>生產版本： 2021年1月21日</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">階層連結導覽的新外觀和風格</a> </p> <p>為協助使用者更清楚識別他們在Workfront的位置，以及更輕鬆地在物件之間導覽，我們已對階層連結導覽進行幾項改善。</p> </td> 
   <td><strong>可於下列日期使用：</strong> <p>測試版預覽發行： 2020年12月10日</p> <p>生產版本： 2021年1月21日</p> <p><strong>適用於下列環境：</strong> </p> <p>全新Adobe Workfront體驗 </p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront目標增強功能

大部分Workfront Target目標版本的新功能都來自21.1版。 如需這些新功能（現已可在預覽中取得）的相關資訊，請參閱 [Adobe Workfront第21.1發行版本的目標](../../../product-announcements/product-releases/goals-release-activity/goals-release-21-1.md).

## Workfront方案規劃器增強功能

隨21.1版本推出Workfront Scenario Planner的新功能。 如需這些新功能（現已可在預覽中取得）的相關資訊，請參閱 [Adobe Workfront Scenario Planner 21.1版](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-1.md).

## Workfront Fusion增強功能

Workfront Fusion的新功能可在生產環境中依21.1版排程外的順序取得。 如需最新功能的詳細資訊，請參閱 [Adobe Workfront Fusion發行活動](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)

## API增強功能

API 12版現已可在20.4版中使用。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

如需新增功能和更新的相關資訊，請參閱 [API 12版的新功能](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWF_API%2FAPI%2Fnew-api-version-12.htm).

如需API版本的詳細資訊，請參閱 [API版本設定與支援排程](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

。

## Workfront 維護更新

如需21.1版本期間進行的維護更新相關資訊，請參閱 [Workfront維護更新](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## 佈告

* [Workfront 21.1版新增電子郵件IP位址](#new-ip-addresses-for-workfront-email-with-the-21-1-release)
* [事件訂閱的其他IP位址允許清單](#allowlist-of-additional-ip-addresses-for-event-subscriptions)
* [存取Workfront所需其他網域的允許清單](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Flash淘汰](#flash-deprecation)
* [21.1發行網路研討會](#21-1-release-webinar)
* [預覽發行順序中的變更](#change-in-preview-release-cadence)
* [Workfront一](#workfront-one)

### Workfront 21.1版新增電子郵件IP位址 {#new-ip-addresses-for-workfront-email-with-the-21-1-release}

為了提高電子郵件傳送的成功率，我們透過叢集1、2、3、4和5的21.1生產版本新增IP位址。

如需您需要為叢集新增哪些IP位址的詳細資訊，請參閱 [Adobe Workfront 21.1版新增電子郵件IP位址](../../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md).

要確定您正在執行哪個群集，請轉至「設定」>「系統」>「客戶資訊」。

### 事件訂閱的其他IP位址允許清單 {#allowlist-of-additional-ip-addresses-for-event-subscriptions}

為了增加成功的事件訂閱傳送，我們在2021年第一季度的21.1生產版本中新增了4個新IP位址。 您必須在2021年2月之前將這些IP位址新增至允許清單，確保您的使用者能繼續收到事件訂閱。

請連絡您的內部IT和/或安全部門，以取得新增文章中新IP的協助。 [事件訂閱API](../../../wf-api/general/event-subs-api.md).

### 存取Workfront所需其他網域的允許清單 {#allowlist-of-additional-domains-required-for-accessing-workfront}

如果您的組織使用防火牆，您必須將下列其他網域新增至允許清單，以確保不間斷地存取Workfront:

* event.split.io
* sdk.split.io

如需詳細資訊，請參閱 [配置防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Flash淘汰 {#flash-deprecation}

2020年11月19日，所有Flash型工具皆已從所有產品中移除。

請參閱以下文章，進一步了解每個特定Flash型工具的取代解決方案： [取代Adobe Workfront中的Flash型工具](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

### 21.1發行網路研討會 {#21-1-release-webinar}

Workfront 21.1發行網路研討會將於2月3日美國東部夏令時間上午11點/英國夏令時下午4點舉行。 報名參加網路講座 [此處](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&amp;partnerref=ac&amp;eventid=2934272&amp;sessionid=1&amp;key=5C231B3385686D1E224A49EBE0BF0E37&amp;regTag=&amp;V2=false&amp;sourcepage=register).

### 預覽發行順序中的變更 {#change-in-preview-release-cadence}

自2020年5月20日起，Workfront開始每週在預覽環境中提供功能。 在此變更前，通常每兩週會向預覽環境發行一次功能。

如需詳細資訊，請參閱 [變更Workfront預覽發行頻率常見問題集](https://one.workfront.com/s/article/Change-in-Workfront-Preview-release-cadence)

### Workfront一 {#workfront-one}

透過Workfront One，您將能從Workfront找到最重要的內容、資源和新聞 — 只要登入，一次就能集中發現。 我們已統一體驗、社群和訓練網站，讓您更輕鬆找到所需內容。

[深入了解Workfront One](https://www.workfront.com/campaigns/workfront-one).
