---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在方案計畫員中建立和編輯計畫
description: 在排定公司較高層次策略的優先順序時，您可以建立計畫，作為使用Workfront方案計畫器的一部分。 有關計畫的詳細資訊，請參閱方案計畫器中的計畫概覽。
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2402'
ht-degree: 1%

---

# 在 [!DNL Scenario Planner]

您可以使用 [!DNL Workfront Scenario Planner]，排定公司較高層次策略的優先順序。 如需計畫的詳細資訊，請參閱 [中的計畫概覽 [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 計劃*</p> </td> 
   <td>[!UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權*</p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>產品</td> 
   <td> <p>您必須為 [!DNL Adobe Workfront Scenario Planner] 存取本文所述功能。</p> <p>有關獲取[!UICONTROL Workfront方案規劃器]的資訊，請參閱 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!UICONTROL方案規劃器]所需的訪問權</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>訪問級別配置* </td> 
   <td> <p>[!UICONTROL Edit]或更高版本 [!DNL Scenario Planner]</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>物件權限 </p> </td> 
   <td> <p>[!DNL Manage] 計畫的權限</p> <p>有關請求對計畫進行額外訪問的資訊，請參閱 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 建立或編輯計畫

您可以從頭建立計畫，也可以編輯已與您共用的現有計畫。

>[!NOTE]
>
>建立計畫後，您將被視為計畫建立者和責任人。 停用使用者時，計畫沒有擁有者，除非先前已與連結共用，否則任何人都看不到。

本文說明如何從頭建立計畫，或如何編輯現有計畫。

有關計畫的所有考慮事項，包括計畫可用的資訊，請參閱 [中的計畫概覽 [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

有關刪除計畫的資訊，請參閱 [刪除 [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

要建立或編輯計畫，請執行以下操作：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png)，然後按一下 [!UICONTROL 藍本].

   您建立的現有計劃清單會顯示在 [!DNL Workfront Scenario Planner].

1. （選用）按一下 **[!UICONTROL 篩選]** 圖示 ![](assets/filter-icon-34x37.png)在計劃清單的右上角，從以下項中選擇：

   | 篩選器 | 說明 |
   |---|---|
   | [!UICONTROL 全部] | 顯示您建立或已與您共用的所有計畫。 |
   | [!UICONTROL 我的計劃] | 顯示您建立的計畫。 |
   | [!UICONTROL 與我共用] | 顯示與您共用的計畫。 |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. （選用）按一下 **[!UICONTROL 搜尋]** 圖示 ![](assets/search-icon.png) 鍵入關鍵字並在清單中快速找到計畫。

1. 按一下現有計畫的名稱以編輯它，然後繼續步驟7。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   或

   按一下 **[!UICONTROL 新計畫]** 在左上角以建立計畫並繼續步驟5。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   此 [!UICONTROL 新計畫] 框。

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. （條件性）建立新計畫時，請指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL名稱]</td> 
      <td>鍵入計畫的名稱。 這是必填欄位。</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>重要： <span style="font-weight: normal;">建立並保存計畫後，無法修改以下選項。</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE（[!UICONTROL等同全時間]）或[!UICONTROL小時數]</span> </td> 
      <td> <p><span>選擇以下選項之一，以指明要如何估計此計畫的任務職責資訊：</span> </p> 
       <ul> 
      <li> <p><span><strong>FTE</strong>. 這是預設值 </span> </p> 
      <p><b>重要</b></p>  
      <p>針對 [!DNL Scenario Planner], [!DNL Workfront] 使用下列值：1 FTE = 8小時。 </p> </li> 
      <li> <p><strong>[!UICONTROL小時]</strong> </p> </li> 
       </ul> <p><b>重要</b></p>

   您在此處選擇的選項決定如何顯示計畫、計畫方案和方案的任務職責資訊</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL開始日期]</td> 
      <td> <p>選擇要開始計畫的月份和年份。 您只能在此欄位中選取月。 [!DNL Workfront] 假設計畫的開始日期是所選月份的第一天，而結束日期是其持續時間內月末的最後一天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL持續時間]</td> 
      <td> <p>從下拉式選單中選取下列持續時間：</p> 
       <ul> 
        <li>1 年. 這是預設持續時間。 </li> 
        <li>3年</li> 
        <li> <p>5年</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--for table above - how FTE is calcualted: NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>-->

1. （有條件）按一下 **[!UICONTROL 下一個]**.

   計畫的時間軸顯示為 **[!UICONTROL 初始方案]**.

   如需建立其他案例的詳細資訊，請參閱 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. （可選）從時間軸下拉菜單中，選擇下表中的一個選項，以更改查看計畫時間軸的方式。

   ![](assets/month-dropdown-with-all-options.png)

   | 下拉式功能表選項 | 說明 |
   |---|---|
   | [!UICONTROL 月] | 按月顯示時間軸。 這是一年計畫的預設和唯一選項。 |
   | [!UICONTROL 季度] | 按季度顯示時間軸。 此選項僅在 [!UICONTROL 持續時間] 三五年。 這是3年計畫的預設選項。 |
   | [!UICONTROL 年] | 按年顯示時間軸。 此選項僅在 [!UICONTROL 持續時間] 計畫是五年。 這是5年計畫的預設選項。 |

1. （可選）從左到右滾動以查看計畫的整個持續時間。
1. （選用）按一下 **[!UICONTROL 今天]** 指示線，返回當天。

   ![](assets/today-indicator-350x160.png)

1. 按一下 **[!UICONTROL 作業角色]** 框，添加將可用於執行計畫的作業角色。

   此 [!UICONTROL 作業角色] 框。

   >[!TIP]
   >
   >職責分配單位（FTE或小時） [!DNL Workfront] 此計畫的用途會以括弧顯示在方塊標題中。

   ![](assets/adding-people-to-plan-350x206.png)

1. 按一下 **[!UICONTROL 開始鍵入作業角色]** 欄位，從清單中選擇角色，或開始鍵入活動作業角色的名稱。

   按一下此欄位時，系統中的所有活動作業角色都會列出。

   這會將作業角色新增至「作業角色」欄。

1. 更新或複查作業角色的以下資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL最大可用值]（適用於FTE） </p> <p role="rowheader">或 </p> <p role="rowheader"><span>[!UICONTROL可用總計]（小時）</span> </p> </td> 
      <td> <p><span>根據您選擇使用小時還是FTE來進行計畫，請鍵入</span> 職務角色FTE的數量 <span>或小時</span> 可在以下欄位中執行計畫工作： </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL可用總數]</strong> （代表小時）:指出方案期間所有月份的總小時數。 依預設， [!DNL Workfront] 在方案期間的所有月份中，「可用總數」除以平均數。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果為設計器輸入1200小時，這表示當計畫[!UICONTROL持續時間]為1年時，在計畫期間，設計器每月可用100小時。 </p> </li> 
        <li> <p><b>[!UICONTROL最大可用值]</b> （適用於FTE）:指定在計畫期間每個月可用職務職責的FTE數。 依預設， <strong>Workfront</strong> 將[!UICONTROL可用數量上限]指派給方案期間的每個月。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>如果為顧問輸入1名FTE，這表示在計畫期間，顧問每月可為1名FTE使用。 </p> <p>您可以輸入小於1 FTE的數字。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>0.5的顧問職位意味著顧問將將其一半的FTE（通常為4小時，其中8小時為1名FTE）用於執行此計畫。 對於方案計畫器中的所有計算，Workfront使用以下值：1 FTE = 8小時。 </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL要求的最大值]（適用於FTE）</p> <p role="rowheader">或 </p> <p role="rowheader"><span>[!UICONTROL所需總計]（小時）</span> </p> </td> 
      <td> <p><span>根據您是選擇使用小時還是FTE進行計畫，請複查</span> 職務角色FTE的數量 <span>或小時</span> 在方案中完成計畫所需的資料。 檢閱下列欄位：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL需要總計]</strong> （代表小時）:計畫期間所有月份所需的總小時數。</p> </li> 
        <li> <p><strong>[!UICONTROL最大需要值]</strong> （適用於FTE）:計畫期間任何月份所需的FTE數上限。 </p> </li> 
       </ul> <p>提示：此 <span>最大值</span> FTE數 <span>或總小時數</span> 開始新增方案後，該作業角色的必要項目會隨即顯示。 有關向計畫添加方案的資訊，請參閱 <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>.</p> </td> 
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
      <td role="rowheader">[!UICONTROL每小時費率]</td> 
      <td> <p>這是作業角色的[!UICONTROL成本小時]比率。 每小時費率會以您的系統貨幣顯示。 有關為系統設定匯率的資訊，請參閱 <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可選）暫留在作業角色的名稱上，或在更新角色資訊後按一下「 」標籤，然後按一下「 」 **[!UICONTROL 垃圾桶圖示]** ![](assets/delete.png) 從計畫中刪除它。
1. 按一下 **[!UICONTROL 職務角色分配]**.

   工作角色分配面板會針對方案期間的所有月份顯示。

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. 鍵入作業角色的名稱以將其添加到 **[!UICONTROL 開始鍵入作業角色欄位]**，然後在清單上出現時按一下Enter 。 這會將工作角色新增至 [!UICONTROL 作業角色] 欄。
1. 針對藍本的每個月更新或檢閱下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL工作角色]（FTE或小時）</td> 
      <td>工作角色分配面板中將顯示方案可用的工作角色和方案上的方案所需的工作角色。 指明職務職責估計是在FTE中還是在列標題中的小時。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL可用](最大值 &lt;number of="" ftes=""&gt;) </p> 
       <div> 
        <p>或</p> 
        <p>[!UICONTROL可用]（總計） &lt;number of="" hours=""&gt;) </p> 
       </div> </td> 
      <td> <p><span>根據您選擇使用小時數還是FTE來進行計畫、複查或更新</span> 每月職務角色FTE數 <span>或小時</span> 適用於下列欄位中的案例：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL可用](最大值 &lt;number of="" ftes=""&gt;)</strong>:括弧中的數字顯示藍本月份任何月份可用的角色數量上限。 查看或更新方案每個月的FTE數。 更改每月分配可能會更新括弧內的FTE數。 </p> </li> 
        <li> <p><span><strong>[!UICONTROL可用]（總計） &lt;number of="" hours=""&gt;)</strong>:括弧中的數字顯示藍本中所有月份可用的總小時數。 檢閱或更新藍本每個月的小時數。 變更每月分配會更新括弧中的小時數。</span> </p> </li> 
       </ul> <p>手動更新每月職務角色分配是解決方案上方案之間職務角色衝突的另一種方式。 </p> <p>提示：   <p><span>若要更新幾個月的每月角色可用性，請在任何月份的[!UICONTROL可用]欄位中鍵入小時數或FTE，然後拖動欄位的角到相鄰月份，以複製每個月的相同值。 刪除它以更新所有月份。</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL必要](最大值 &lt;number&gt;)</p> 
       <div> 
        <p role="rowheader">或</p> 
        <p role="rowheader">[!UICONTROL必要]（總計） &lt;number&gt;)</p> 
       </div> </td> 
      <td> <p><span>根據您是選擇使用小時還是FTE進行計畫，請複查</span> 在以下欄位中，方案所需的每月職務角色FTE數或小時數： </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL必要](最大值 &lt;number of="" ftes=""&gt;)</strong>:括弧中的數字顯示藍本月份任何月份所需的角色數上限。 </p> </li> 
        <li> <p><span><strong>[!UICONTROL必要]（總計） &lt;number of="" hours=""&gt;)</strong>:括弧中的數字顯示藍本中所有月份所需的總小時數。</span> </p> </li> 
       </ul> <p>提示：無法修改所需的FTE數 <span>或小時</span> 為工作角色。 在您開始新增方案及其工作角色需求後，會針對方案填入此數字。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL差異]</td> 
      <td> 
       <div> 
        <p>藍本所需和可用職務角色數量之間的月差。 [!DNL Workfront] 使用以下公式計算每個月的每個職務職責的差異：</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> （在FTE或小時內） </p> 
        <p>提示：當差異顯示負數時，方案需要的任務角色比計畫可用的任務角色更多。 您的資源被過度分配。 </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL利用率] %</td> 
      <td> 
       <div> 
        <p>利用率百分比顯示方案中方案實際使用（或需要）的可用作業角色數。 </p> 
        <p>[!DNL Workfront] 使用以下公式計算每月每個任務職責的利用率： </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>根據資源的分配，利用率百分比可能以下列顏色顯示：</p> 
        <ul> 
         <li> <p><b>綠色</b>:可用和所需的作業角色數相符。 資源被完全分配，利用率百分比為100%。 </p> </li> 
         <li> <p><b>紅色</b>:所需的任務角色數多於計畫可用的任務角色數。 資源被過度分配，利用率百分比高於100%。</p> </li> 
         <li> <p><b>藍色</b>:可用的作業角色數多於所需的數量。 資源分配不足，利用率低於100%。 </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 套用]** 保存每月作業角色分配

   或

   按一下 **[!UICONTROL 取消]** 關閉作業角色分發清單並返回方案。

1. 按一下 **[!UICONTROL 財務]** 框，添加此計畫的預算。

   此 [!UICONTROL 財務] 框。

   >[!TIP]
   >
   >該貨幣 [!DNL Workfront] 此計畫的用途會以括弧顯示在方塊標題中。

1. 指定 **[!UICONTROL 年度預算]**.

   >[!NOTE]
   >
   >如果您的計畫跨越多年，則必須指定每年的預算金額。

1. 按Enter以儲存年度預算，然後 [!UICONTROL 標籤] 改到第二年。

   每年預算會針對所選年度的每個月自動平均分配。

1. 按一下 **[!UICONTROL 進階]** 查看每月預算分配。 每年和每月預算一律為四捨五入數字。 當預算金額因小數而無法平均分配給一年內的所有月份時a **[!UICONTROL 剩餘]** 指標顯示在年度預算分配下。

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. 人工調整每月預算以消除超出的金額。

   當所有每月預算金額的總計大於年度預算時， **[!UICONTROL 超過]** 警告指標顯示在年度預算分配下。 人工調整每月預算額，直到它們等於或低於計畫的可用預算。

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. 停用 **[!UICONTROL 包括人員成本]** 設定以排除與任務職責相關的成本，使其不計入計畫的總體成本。 固定成本始終以計畫的整體成本計算。 此設定預設為啟用，並影響計畫上的所有方案。
1. 按一下 [!UICONTROL 財務] 框來關閉它。 系統會自動儲存您輸入的資訊。

   您現在可以開始建立計畫的方案，並新增方案。

1. （建議）按一下 **[!UICONTROL 新舉措]** 新增計畫。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   有關添加計畫的資訊，請參閱文章 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. （可選）複製現有方案以建立相同計畫的新方案。 如需建立及使用多個案例的詳細資訊，請參閱 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. 按一下 **[!UICONTROL 保存計畫]**.

   已建立或更新您的計畫。

1. （選用）按一下 **[!UICONTROL 收藏夾表徵圖]** ![](assets/favorites-icon-small.png) 將計畫添加到您的收藏夾清單中。

1. （可選）複製計畫的URL，並傳送給可能需要檢閱或更新該計畫的任何其他使用者。 他們至少 [!UICONTROL 檢視] 在其存取層級存取，以便能夠檢視計畫。 他們肯定有 [!UICONTROL 編輯] 存取以編輯。 如果他們必須審核計畫的財務資訊，如預算、成本和職務職務費率資訊，則他們還必須能夠訪問 [!UICONTROL 財務資料] 在其存取層級。 如需 [!DNL Scenario Planner]，請參閱 [使用 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).
