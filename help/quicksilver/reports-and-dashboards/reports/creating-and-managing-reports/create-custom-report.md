---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 建立自訂報表
description: 瞭解如何建立報表可協助您在Adobe Workfront中提供組織所需資訊的存取權。 您可以使用Workfront提供的任何內建報表，或從頭開始建立自己的報表。
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '1809'
ht-degree: 1%

---


# 建立自訂報表

瞭解如何建立報表可協助您在Adobe Workfront中提供組織所需資訊的存取權。 您可以使用Workfront提供的任何內建報表，或從頭開始建立自己的報表。

如需內建報表的詳細資訊，請參閱 [使用Adobe Workfront內建報告](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

如需有關複製報表以建立報表的資訊，請參閱 [建立報告副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

如需建立及管理報表（包括課程、影片和教學課程）的詳細資訊，請參閱Adobe Experience League網站上的「學習」一節。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>您將取得所建立報表的管理許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 建立報告 {#create-a-report}

若要觀看如何建立報告的影片，請參閱此 [建立自訂報表](#Walk-thr) 底下。

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) 按一下「 」 **報表**.
1. 按一下 **新報告**，然後選取您要用於報表的物件型別。

   Report Builder隨即載入。

   如需可用物件報表的特定資訊，請參閱區段 [物件報表](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 在文章中 [瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >您也可以製作現有報表的副本，以建立報表。 如需詳細資訊，請參閱 [建立報告副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. 在Report Builder中，將下列專案新增至報表：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>功能</th> 
      <th>說明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>欄（檢視）</td> 
      <td> <p>在報表中新增欄可決定報表所包含的資訊。</p> <p>若要瞭解如何新增欄，請參閱 <a href="#add-columns-view-to-a-report" class="MCXref xref">新增欄（檢視）至報表</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>群組</td> 
      <td> <p>在報表中新增群組，會決定報表的整理方式。</p> <p>若要瞭解如何新增群組，請參閱 <a href="#add-groupings-to-a-report" class="MCXref xref">新增群組至報表</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>篩選器</td> 
      <td> <p>將篩選規則新增至報表可決定您在報表中看到的資訊。</p> <p>若要瞭解如何新增篩選器，請參閱 <a href="#add-filters-to-a-report" class="MCXref xref">新增篩選器至報表</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>圖表</td> 
      <td> <p>將圖表新增至報表，可決定如何以視覺化方式呈現報表中的資訊。</p> <p>若要瞭解如何新增圖表，請參閱 <a href="#add-a-chart-to-a-report" class="MCXref xref">新增圖表至報表</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在報告建立過程中的任何時候，按一下 **套用** 以儲存變更。
1. 完成後，按一下 **儲存+關閉**.

### 新增欄（檢視）至報表 {#add-columns-view-to-a-report}

1. 開始建立報表，如 [建立報告](#create-a-report) 一節。
1. 在Report Builder中選取 **欄（檢視）** 標籤以識別報表中顯示的欄。
1. （選用）按一下 **套用現有檢視** 以使用現有檢視。

   如需有關建立新檢視的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 若要新增欄，請按一下 **新增欄**.

   或

   若要變更現有欄，請選取您要變更的欄，然後按一下目前名稱旁的(x)。

1. 開始輸入您要新增的欄位。 如果欄位可供使用，則會針對可與其關聯的每個物件填入欄位。 按一下欄位名稱以將其新增至欄。

   如需有關您在欄中看到的欄位的詳細資訊，請參閱 [Adobe Workfront術語表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![](assets/nwe-add-column-typeahead-350x459.png)

1. （選用）在 **欄設定** 區域，選取 **依此欄排序** 若要以遞增的字母遞減順序來排序欄中的值，請指出清單是否應使用此欄作為第一個排序。

   如果您想要先依一欄中的值排序，接著依第二欄中的值排序，則可以在報表檢視中進行多個層級的排序，依此類推。

   如果根據第一個排序標準有多個結果相同，則會依第二個排序標準的順序排序。 如果根據第一和第二排序標準有多個結果相同，則會根據第三排序標準排序等。

   >[!NOTE]
   >
   >如果您新增的欄位所參照的物件與您報告的物件距離太遠，您可能無法依此欄位排序。\
   >例如，問題報告無法依專案所有者欄位排序，因為它參考了3個額外的物件：專案、所有者和名稱。 不過，您仍可將此欄位新增至問題報告，並檢視相關資訊。

   <!--outdated: To learn more about cross-object references in reports, see the section "Advanced Reporting Part 1 of 3" in the [Reports and Dashboards Learning Path](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).-->

1. （選擇性）如果您要使用群組，而且想要彙總（彙總）欄中的資訊，請按一下 **此欄的摘要方式** 中的下拉式清單 **欄設定** 區域，然後選取您要用來彙總欄中資訊的選項。

   彙總資訊會顯示在群組列的欄中。

   ![分組的彙總摘要](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   如需彙總資料欄中資料的詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >當您彙總分組中下列欄位的值時，下列例外情況適用於父系物件（例如父系任務）：
   >
   >* 除「實際時數」（例如「計畫/實際勞力成本」、「計畫/實際費用成本」、「計畫/實際成本」、「計畫時數」）之外的所有數字與幣別欄位，只會彙總子任務與獨立任務的值。 它們不會彙總父系任務的值或父系父系的值。
   >* 實際小時彙總主要父系和獨立任務的值；它們不會彙總父系任務的父系或子系任務的數量。
   >* 數字和貨幣值的自訂資料欄位會彙總所有工作：父項、子項、父項的父項以及獨立工作。

   如需在報表中使用群組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. （選用）按一下 **進階選項** 指定欄的下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">自訂欄標籤</td> 
      <td> <p>指定欄的自訂標籤。 此標籤會取代預設標籤。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">欄位格式</td> 
      <td> <p>選取您要為欄中的欄位顯示值的格式。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在報告面板上顯示此欄</td> 
      <td> <p>當報告與其他報告並排顯示時，選取此選項可在控制面板上顯示此欄。 取消選取此選項時，在報告並排顯示的儀表板上檢視報告時不會顯示此欄。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">欄規則</td> 
      <td> <p>按一下 <strong>為此欄新增規則</strong> 以新增條件式格式至欄。 新增規則後，您可以定義欄位和文字樣式，以顯示符合該規則的欄位。 按一下 <strong>新增規則</strong> 定義完規則之後。 如需檢視中條件式格式的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">在檢視中使用條件式格式</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **套用** 以套用您目前的變更，並使用下列選項繼續編輯報告。

   按一下 **儲存+關閉** 如果您已完成編輯報表中的欄，並且要儲存報表。

### 新增群組至報表 {#add-groupings-to-a-report}

1. 開始建立報表，如 [建立報告](#create-a-report) 一節。
1. 在Report Builder中選取 **群組** 標籤以識別報告中專案的群組方式。
1. 按一下 **新增群組** 以新增群組。

   或

   選擇 **套用現有群組** 以選取現有群組
   ![](assets/nwe-add-grouping-350x230.png)

1. 開始輸入您要新增為群組的欄位。 如果欄位可供使用，則會針對可與其關聯的每個物件填入欄位。 按一下欄位名稱以將其新增到該群組。
1. （選用）您可以選擇按一下「 」，以文字模式建立群組 **切換到文字模式**. 如需有關使用文字模式的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   如需建立新群組的詳細資訊，請參閱 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. （選用）選取 **依預設摺疊此群組** 如果您希望此群組中的結果以收合方式顯示而非展開。

   此設定預設為停用，群組結果一律顯示在展開清單中。

   >[!TIP]
   >
   >* 當您在檢視清單時手動調整群組，Workfront會記住您的手動偏好設定，直到您登出為止。 當您重新登入時，清單會根據此設定顯示。
   >* 從圖表元素存取群組結果後，群組結果一律展開顯示。

1. （選擇性）您可以選擇建立矩陣群組，以格線格式顯示結果。

   如需建立矩陣報表的詳細資訊，請參閱 [建立矩陣報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. 按一下 **套用** 以套用您目前的變更，並使用下列選項繼續編輯報告。

   按一下 **儲存+關閉** 如果您已完成編輯報表中的群組，且您想要儲存報表。

### 新增篩選器至報表 {#add-filters-to-a-report}

1. 開始建立報表，如 [建立報告](#create-a-report) 一節。
1. 在Report Builder中選取 **篩選器** 標籤以識別您要納入報表的資訊量。
1. 按一下 **新增篩選器規則** 以新增自訂篩選器。\
   或\
   選擇 **套用現有篩選器** 以使用現有的篩選器。

   ![](assets/nwe-add-a-filter-350x93.png)

1. 若您按一下 **新增篩選器規則**，開始輸入您要新增為篩選的欄位。 如果欄位可供使用，則會針對可與其關聯的每個物件填入欄位。 按一下欄位名稱以將其新增至該篩選器。\
   使用篩選器修飾元來建置您的篩選器。 如需篩選修飾元的詳細資訊，請參閱 [篩選和條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   如需建立新篩選的詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （選用）您可以選擇按一下「 」，在文字模式中建立篩選器 **切換到文字模式**.

   如需有關使用文字模式的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. 按一下 **套用** 當您完成編輯報表中的篩選器以套用目前所做的變更，並使用下列選項繼續編輯報表時。

   按一下 **儲存+關閉** ，而且您想要儲存報表。

### 新增圖表至報表 {#add-a-chart-to-a-report}

1. 開始建立報表，如 [建立報告](#create-a-report) 一節。
1. 在Report Builder中選取 **圖表** 標籤，然後選取您要新增的圖表型別。

   ![](assets/nwe-add-a-chart-350x247.png)

   如需在報告中建立圖表的詳細資訊，請參閱 [新增圖表至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. 按一下 **套用** 以套用您目前的變更，並使用下列選項繼續編輯報告。

   按一下 **儲存+關閉** 如果您已完成編輯報告，並想要儲存報告。
