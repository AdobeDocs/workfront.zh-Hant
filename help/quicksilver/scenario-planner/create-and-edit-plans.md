---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在「情境規劃工具」中建立和編輯計畫
description: 當排定貴公司較高層級策略的優先順序時，您可以建立計畫作為使用Workfront情境規劃工具的一部分。 如需計畫的詳細資訊，請參閱案例規劃工具中的計畫概要。
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '2396'
ht-degree: 0%

---

# 在[!DNL Scenario Planner]中建立和編輯計畫

當排定貴公司較高層級策略的優先順序時，您可使用[!DNL Workfront Scenario Planner]來建立計畫。 如需計畫的詳細資訊，請參閱 [!DNL Scenario Planner]](../scenario-planner/plans-overview.md)中的[計畫總覽。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 計畫*</p> </td> 
   <td> <ul></li>
   <li><p>新增：Ultimate </p></li>
   <p>新的Workfront Select或Workfront計畫無法使用「情境規劃工具」。 </p>
   <li><p>目前： [！UICONTROL Business]或更高版本</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權*</p> </td> 
   <td> <p>新增：淺色或更高</p> 
   <p>目前： [！UICONTROL Review]或以上</p> </td> 
  </tr> 
  <tr> 
   <td>產品* </td> 
   <td> <ul><li><p>針對新的Workfront計畫：</p><p> Adobe Workfront</li></p>
   <li><p>針對目前的Workfront計畫： </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront情境規劃工具</p></li></ul>

<p>如需詳細資訊，請參閱<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的存取權。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>存取層級 </td> 
   <td> <p>[！UICONTROL Edit]對的存取權 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>物件許可權 </p> </td> 
   <td> <p>[！UICONTROL Manage]計畫的許可權</p> <p>如需有關請求對計畫的額外存取權的資訊，請參閱<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中請求對計畫的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立或編輯計畫

您可以從頭開始建立計畫，也可以編輯與您共用的現有計畫。

>[!NOTE]
>
>建立計畫後，您即被視為計畫建立者和擁有者。 停用使用者時，計畫沒有擁有者，除非先前與連結共用，否則任何人都看不到計畫。

本文說明如何從頭開始建立計畫或編輯現有計畫。

如需有關計畫的所有考量事項，包括可用於計畫的資訊，請參閱 [!DNL Scenario Planner]](../scenario-planner/plans-overview.md)中的[計畫總覽。

如需有關刪除計畫的資訊，請參閱[刪除 [!DNL Scenario Planner]](../scenario-planner/delete-plans.md)中的計畫。

若要建立或編輯計畫：

{{step1-to-scenario-planner}}

您建立的現有計劃清單會顯示在[!DNL Workfront Scenario Planner]中。

1. （選擇性）按一下計劃清單右上角的&#x200B;**[!UICONTROL 篩選器]**&#x200B;圖示![](assets/filter-icon-34x37.png)，然後選取下列專案：

   | 篩選器 | 說明 |
   |---|---|
   | [!UICONTROL 全部] | 顯示您已建立或已與您共用的所有計畫。 |
   | [!UICONTROL 我的計畫] | 顯示您建立的計畫。 |
   | [!UICONTROL 與我共用] | 顯示與您共用的計畫。 |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. （選擇性）按一下&#x200B;**[!UICONTROL 搜尋]**&#x200B;圖示![](assets/search-icon.png)以輸入關鍵字，並在清單中快速找到計畫。

1. 按一下現有計畫的名稱以編輯它，然後繼續步驟7。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   或

   按一下左上角的&#x200B;**[!UICONTROL 新計畫]**&#x200B;以建立計畫並繼續步驟5。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   [!UICONTROL 新計畫]方塊隨即顯示。

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. （視條件而定）建立新計畫時，請指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL名稱]</td> 
      <td>輸入計畫的名稱。 這是必填欄位。</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>重要： <span style="font-weight: normal;">建立並儲存計畫後，您無法修改下列選取專案。</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE （[！UICONTROL全時相當的]）或[！UICONTROL小時]</span> </td> 
      <td> <p><span>選取下列其中一個選項，以指示您要如何估計此計畫的工作角色資訊：</span> </p> 
       <ul> 
      <li> <p><span><strong>FTE</strong>。 這是預設</span> </p> 
      <p><b>重要</b></p>  
      <p>對於[!DNL Scenario Planner]中的所有計算，[!DNL Workfront]會使用以下值： 1 FTE = 8小時。 </p> </li> 
      <li> <p><strong>[！UICONTROL小時]</strong> </p> </li> 
       </ul> <p><b>重要</b></p>

   您在此選取的選項決定計畫、計畫的案例與方案的工作角色資訊顯示方式</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL開始日期]</td> 
      <td> <p>選取您要計劃開始的月份和年份。 您只能在此欄位中選取月份。 [!DNL Workfront]假設計畫的開始日期是所選月份的第一天，而結束日期是月份結束期間的最後一天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL持續時間]</td> 
      <td> <p>從下拉式功能表中選取下列期間：</p> 
       <ul> 
        <li>1年。 這是預設持續時間。 </li> 
        <li>3年</li> 
        <li> <p>5年</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--for table above - how FTE is calcualted: NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>-->

1. （視條件而定）按一下&#x200B;**[!UICONTROL 下一步]**。

   計畫的時間表會顯示為&#x200B;**[!UICONTROL 初始情境]**。

   如需建立其他情境的相關資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md)中建立和比較計畫情境。

1. （選擇性）從時間表下拉式功能表中，選取下表中的其中一個選項，以變更您檢視計畫時間表的方式。

   ![](assets/month-dropdown-with-all-options.png)

   | 下拉式功能表選項 | 說明 |
   |---|---|
   | [!UICONTROL 個月] | 按月顯示時間表。 這是一年計畫的預設且唯一選項。 |
   | [!UICONTROL 季] | 依季度顯示時間軸。 只有在計畫的[!UICONTROL 期間]為3或5年時，才能使用此選項。 這是3年計畫的預設選項。 |
   | [!UICONTROL 年] | 按年顯示時間軸。 只有在計畫的[!UICONTROL 期間]為5年時，才能使用此選項。 這是5年計畫的預設選項。 |

1. （可選）從左向右捲動以檢視計畫的整個期間。
1. （選用）按一下&#x200B;**[!UICONTROL Today]**&#x200B;指標行以返回當天。

   ![](assets/today-indicator-350x160.png)

1. 按一下計畫標題中的&#x200B;**[!UICONTROL 工作角色]**&#x200B;方塊，新增可用於執行計畫的工作角色。

   顯示[!UICONTROL 工作角色]方塊的詳細資料。

   >[!TIP]
   >
   >[!DNL Workfront]用於此計畫的角色配置單位（FTE或時數）會顯示在方塊標題的括弧中。

   ![](assets/adding-people-to-plan-350x206.png)

1. 按一下&#x200B;**[!UICONTROL 開始輸入工作角色]**&#x200B;欄位，然後從清單中選取角色，或開始輸入作用中工作角色的名稱。

   當您按一下此欄位時，系統中所有作用中的職位角色都會列出。

   這會將工作角色新增至工作角色欄。

1. 更新或檢閱工作角色的下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[！UICONTROL可用上限] （適用於FTE） </p> <p role="rowheader">或 </p> <p role="rowheader"><span>[！UICONTROL總計可用] （小時）</span> </p> </td> 
      <td> <p><span>根據您選取使用計畫的時數或FTE，在下列欄位中輸入</span>可用於執行計畫的工作角色FTE數量<span>或時數</span>： </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[！UICONTROL總計可用]</strong> （小時）：表示案例期間所有月份的總小時數。 根據預設，[!DNL Workfront]會將可用的總數平均分配到情境期間的所有月份。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果您為Designer輸入1200小時，這表示在計畫期間每個月100小時都可使用Designer，而計畫[！UICONTROL Duration]為1年。 </p> </li> 
        <li> <p><b>[！UICONTROL可用上限]</b> （適用於FTE）：表示在計畫期間每個月可使用該工作角色的FTE數量。 根據預設，<strong>Workfront</strong>會將[！UICONTROL Max available]數字指派給案例期間內的每個月。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果您為顧問輸入1 FTE，這表示顧問在計畫期間每個月都有1 FTE可用。 </p> <p>您可以輸入小於1 FTE的數字。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>0.5顧問工作角色表示顧問將花費一半的FTE （通常是4小時，其中8小時是1 FTE）來處理此計畫。 對於「情境規劃工具」中的所有計算，Workfront會使用以下值： 1 FTE = 8小時。 </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[！UICONTROL Max required] （適用於FTE）</p> <p role="rowheader">或 </p> <p role="rowheader"><span>[！UICONTROL總共需要] （適用於小時）</span> </p> </td> 
      <td> <p><span>根據您選擇使用計畫的時數或FTE，檢閱</span>完成情境中方案所需的工作角色FTE數量<span>或時數</span>。 檢閱下列欄位：</p> 
       <ul> 
        <li> <p><strong>[！UICONTROL總共需要]</strong> （針對小時）：計畫期間所有月份所需的總小時數。</p> </li> 
        <li> <p><strong>[！UICONTROL Max required]</strong> （適用於FTE）：計畫期間任何月份所需的FTE數目上限。 </p> </li> 
       </ul> <p>秘訣：在您開始新增方案後，會顯示該工作角色所需的<span>最大</span>個FTE數量<span>或總時數</span>。 如需將方案新增至計畫的詳細資訊，請參閱<a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中建立和編輯方案。</p> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">[!UICONTROL Avg utilization]</td> 
       <td> <p>(NOTE: this field was removed in 21.2 - May 2021) </p> <p>[!DNL Workfront] calculates the average utilization for each job role using the job role FTEs associated with initiatives (required) and the job role FTEs associated with the plan (available). </p> <p> [!DNL Workfront] calculates the job role utilization percentage for a plan using the following formula: </p> <p><code>Job role utilization percentage = Sum [(Required job roles for each month of the plan *100)/ (Available job roles for each month of the plan)] / Number of months in the Duration of the plan</code> </p> 
        <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, if you have a plan with a duration of 12 months and an initiative with the duration of 2 months, where you use 1 Designer for your initiative (required job role) and there are 2 Designers available on the plan (available), the Utilization percentage for the Designer job role is calculated as follows:</p> 
         <p><code>Designer utilization percentage = [(1/2 + 1/2) * 100] / 12 = 100 / 12 = 8.3%</code> </p> 
        </div> <p>As you add job roles to the plan and indicate the Available amount for each one, the [!UICONTROL Utilization] value for each role also updates and [!DNL Workfront] calculates a utilization percentage for the plan. For information about how [!DNL Workfront] calculates the Job Role Utilization for a plan, see <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Plans overview in the [!DNL Scenario Planner]</a>. </p> <p>Tip: The Utilization percentage is rounded and has one decimal. </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">[！UICONTROL小時費率]</td> 
      <td> <p>這是工作角色的[！UICONTROL成本小時]費率。 小時費率會以您系統的貨幣顯示。 如需有關設定系統匯率的資訊，請參閱<a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）將滑鼠停留在工作角色的名稱上，或在更新角色資訊後按一下索引標籤，然後按一下&#x200B;**[!UICONTROL 垃圾桶圖示]** ![](assets/delete.png)以將其從計畫中移除。
1. 按一下&#x200B;**[!UICONTROL 工作角色分配]**。

   工作角色分佈面板會針對情境期間的所有月份顯示。

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. 在&#x200B;**[!UICONTROL 開始輸入工作角色欄位]**&#x200B;中輸入工作角色的名稱以將其新增至計畫，然後在其出現在清單上時按一下「輸入」。 這會將工作角色新增至[!UICONTROL 工作角色]欄。
1. 更新或檢閱情境每個月的下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL工作角色] （FTE或小時）</td> 
      <td>可用於情境的工作角色和情境上的方案所需的工作角色都會顯示在工作角色分佈面板中。 有指示工作角色估計是以FTE還是以欄標題中的小時表示。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL可用] （最大&lt;FTE數&gt;） </p> 
       <div> 
        <p>或</p> 
        <p>[！UICONTROL可用] （總計&lt;小時數&gt;） </p> 
       </div> </td> 
      <td> <p><span>根據您選擇使用計畫的時數或FTE，檢閱或更新</span>下列欄位中適用於情境的每月工作角色FTE數量<span>或時數</span>：</p> 
       <ul> 
        <li> <p><strong>[！UICONTROL可用] （最大&lt;FTE數&gt;）</strong>：括弧中的數字顯示情境中任一月份可用的角色數上限。 檢閱或更新情境每個月的FTE數量。 變更每月配置可能會更新括弧中的FTE數量。 </p> </li> 
        <li> <p><span><strong>[！UICONTROL Available] （總計&lt;number of hours&gt;）</strong>：括弧中的數字顯示情境中所有月份可用的總時數。 檢閱或更新情境每個月的小時數。 變更每月配置會更新括弧中的小時數。</span> </p> </li> 
       </ul> <p>手動更新每月工作角色分配是解決情境上方案之間工作角色衝突的另一種方式。 </p> <p>秘訣：   <p><span>若要將每月角色可用性更新幾個月，請在任何月份的[！UICONTROL Available]欄位中輸入小時數或FTE，然後拖曳欄位角落至相鄰月份，以複製每個月的相同值。 拖放以更新所有月份。</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[！UICONTROL必填] （最大&lt;number&gt;）</p> 
       <div> 
        <p role="rowheader">或</p> 
        <p role="rowheader">[！UICONTROL Required] （總計&lt;number&gt;）</p> 
       </div> </td> 
      <td> <p><span>根據您選擇使用計畫的時數或FTE，檢閱</span>下列欄位中案例所需的每月工作角色FTE或時數： </p> 
       <ul> 
        <li> <p><strong>[！UICONTROL Required] （最大&lt;FTE數&gt;）</strong>：括弧中的數字顯示情境中任一月份所需的角色數上限。 </p> </li> 
        <li> <p><span><strong>[！UICONTROL Required] （總計&lt;number of hours&gt;）</strong>：括弧中的數字顯示案例中所有月份所需的總時數。</span> </p> </li> 
       </ul> <p>秘訣：您無法修改工作角色所需的FTE數量<span>或時數</span>。 此數字會在您開始新增行動方案及其工作角色需求後填入情境。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL差異]</td> 
      <td> 
       <div> 
        <p>案例所需與可用職務角色數量之間的每月差異。 [!DNL Workfront]使用下列公式計算每個月每個職務角色的差異：</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> （FTE或小時） </p> 
        <p>提示：當差異顯示負數時，案例需要的工作角色比計畫可用的更多。 您的資源配置過多。 </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用率] %</td> 
      <td> 
       <div> 
        <p>使用率百分比會顯示有多少可用的職務角色已實際使用（或需要）在情境中的方案。 </p> 
        <p>[!DNL Workfront] 使用下列公式計算每個工作角色每月的使用率： </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>視您的資源配置而定，使用率百分比可能會以下列顏色顯示：</p> 
        <ul> 
         <li> <p><b>綠色</b>：可用和所需的工作角色數量相符。 資源已完全配置，使用率為100%。 </p> </li> 
         <li> <p><b>紅色</b>：所需的工作角色比計畫可用的多。 資源配置過多，使用率百分比高於100%。</p> </li> 
         <li> <p><b>藍色</b>：可用的職務角色超過其需求量。 資源配置不足，使用率百分比低於100%。 </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 套用]**&#x200B;以儲存每月工作角色分配

   或

   按一下&#x200B;**[!UICONTROL 取消]**&#x200B;關閉工作角色通訊群組清單並返回案例。

1. 按一下計畫標題中的&#x200B;**[!UICONTROL 財務]**&#x200B;方塊，以新增此計畫的預算。

   顯示[!UICONTROL 財務]方塊的詳細資料。

   >[!TIP]
   >
   >[!DNL Workfront]用於此計畫的貨幣會顯示在方塊標題的括弧中。

1. 指定&#x200B;**[!UICONTROL 年度預算]**。

   >[!NOTE]
   >
   >如果您的計畫跨越數年，則必須指定每年的預算金額。

1. 按下Enter以儲存年度預算，然後按[!UICONTROL Tab]移至下一年。

   年度預算會自動平均分配至所選年度的每個月。

1. 按一下&#x200B;**[!UICONTROL 進階]**&#x200B;檢視每月預算分配。 年度和每月預算一律為舍入數字。 當預算金額因小數而無法平均分配至一年內的所有月份時，年度預算分配下會顯示&#x200B;**[!UICONTROL 剩餘]**&#x200B;指標。

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. 手動調整每月預算，以消除超出金額。

   當所有每月預算金額的總和大於年度預算時，年度預算分配下會顯示&#x200B;**[!UICONTROL 超過]**&#x200B;警告指標。 手動調整每月預算金額，直到它們等於或低於計畫的可用預算為止。

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. 停用&#x200B;**[!UICONTROL 包含人員成本]**&#x200B;設定，以排除與工作角色相關的成本，不計入計畫的整體成本。 固定成本一律計入計畫的整體成本。 此設定預設為啟用，會影響計畫上的所有情境。
1. 按一下[!UICONTROL Financial]方塊之外的任何位置，將其關閉。 您輸入的資訊會自動儲存。

   您現在可以開始在計畫上建立方案，並新增情境。

1. （建議）按一下&#x200B;**[!UICONTROL 新方案]**&#x200B;以新增方案。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   如需新增方案的詳細資訊，請參閱文章[，在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中建立和編輯方案。

1. （選擇性）複製現有情境以建立相同計畫的新情境。 如需建立和使用多個情境的詳細資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md)中建立和比較計畫情境。
1. 按一下&#x200B;**[!UICONTROL 儲存計畫]**。

   您的計畫已建立或已更新。

1. （選擇性）按一下計畫名稱右側的&#x200B;**[!UICONTROL 我的最愛圖示]** ![](assets/favorites-icon-small.png)，以將計畫新增至您的最愛清單。

1. （選用）複製計畫的URL，然後傳送給可能需要檢閱或更新計畫的任何其他使用者。 他們必須有存取層級中的至少[!UICONTROL 檢視]存取權才能檢視計畫。 使用者必須有[!UICONTROL 編輯]存取權才能進行編輯。 如果他們必須複查計畫的財務資訊，例如預算、成本及職務角色費率資訊，則他們也必須擁有存取層級[!UICONTROL 財務資料]的存取權。 如需[!DNL Scenario Planner]所需存取權的相關資訊，請參閱[使用 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md)所需的存取權。
