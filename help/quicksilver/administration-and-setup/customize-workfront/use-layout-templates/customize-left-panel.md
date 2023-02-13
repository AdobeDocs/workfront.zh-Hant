---
title: 使用版面範本自訂左側面板
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 在版面範本中，您可以自訂使用者在整個Adobe Workfront的左側面板區域中看到的內容。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: c0b0102eb1e1f45e794f962f7e905349f9e241eb
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---

# 使用版面範本自訂左側面板

在版面範本中，您可以自訂使用者在整個左側面板區域中看到的內容 [!DNL Adobe Workfront].

例如，您可以決定使用者在檢視任務時，在左側面板中看到哪些項目：

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>對順序和可見度所做的變更會反映在行動應用程式中。

如需群組版面範本的相關資訊，請參閱 [建立和修改群組的版面範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> 要在系統級別執行這些步驟，需要[!UICONTROL系統管理員]訪問級別。<p>要為組執行這些操作，您必須是該組的經理。</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂 [!DNL Workfront]:

1. 開始使用版面範本，如 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 按一下向下箭頭 ![](assets/dropdown-arrow.png) 在 **[!UICONTROL 自訂使用者看見的項目]**，然後按一下您要自訂的左側面板。

   >[!NOTE]
   >
   >如需 [!UICONTROL 首頁] 選項，請參閱 [自訂 [!UICONTROL 首頁] 和 [!UICONTROL 摘要] 使用版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). 如需清單選項的相關資訊，請參閱 [使用版面範本自訂篩選器、檢視和群組](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. 在 **[!UICONTROL 左側面板]** 清單中，執行下列任一操作，以決定使用者在左側面板中看到的選項([!DNL Workfront] 區域或對象類型):

   * 顯示 ![](assets/add-secondary-nav-item.png) 或隱藏 ![](assets/delete-secondary-nav-item.png) 項目。 任何沒有 ![](assets/add-secondary-nav-item.png) 或 ![](assets/delete-secondary-nav-item.png) 無法隱藏。

   * 拖曳項目 ![](assets/move-icon---dots.png) 以變更其左側面板的順序。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>選項</th> 
      <th>當用戶按一下以下內容時……</th> 
      <th>它們會看到您從下列項目中選擇的左側面板項目：</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL項目]</td> 
      <td>專案的名稱</td> 
      <td>[!UICONTROL任務]、[!UICONTROL項目詳細資訊]、[!UICONTROL業務案例]、[!UICONTROL更新]、[!UICONTROL文檔]、[!UICONTROL問題]、[!UICONTROL風險]、[!UICONTROL批准]、[!UICONTROL基線]、[!UICONTROL基線]、[!UICONTROL計費率]、[!UICONTROL記錄]、[!UICONTROL小時數、費用， [!UICONTROL工作負載平衡器], [!UICONTROL People], [!UICONTROL Utilization], [!UICONTROL隊列詳細資訊], [!UICONTROL路由規則], [!UICONTROL隊列主題], [!UICONTROL主題組], [!UICONTROL度量]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL任務]</td> 
      <td>任務的名稱</td> 
      <td> [!UICONTROL更新]、[!UICONTROL文檔]、[!UICONTROL任務詳細資訊]、[!UICONTROL子任務]、[!UICONTROL問題]、[!UICONTROL小時數]、[!UICONTROL批准]、[!UICONTROL費用]、[!UICONTROL前置任務]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL問題]</td> 
      <td>問題名稱</td> 
      <td> [!UICONTROL更新]、[!UICONTROL文檔]、[!UICONTROL問題詳細資訊]、[!UICONTROL小時數]、[!UICONTROL批准]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROLPortfolio]</td> 
      <td>產品組合的名稱</td> 
      <td>[!UICONTROL項目]、[!UICONTROL程式]、[!UICONTROLPortfolio詳細資訊]、[!UICONTROLPortfolio] [!UICONTROL優化]、[!UICONTROL文檔]、[!UICONTROL更新]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL程式]</td> 
      <td>方案的名稱</td> 
      <td>[!UICONTROL項目]、[!UICONTROL程式詳細資訊]、[!UICONTROL更新]、[!UICONTROL文檔]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL模板]</td> 
      <td>專案範本的名稱</td> 
      <td>[!UICONTROL模板任務]、[!UICONTROL模板詳細資訊]、[!UICONTROL更新]、[!UICONTROL文檔]、[!UICONTROL風險]、[!UICONTROL費用]、[!UICONTROL人員]、[!UICONTROL批准]、[!UICONTROL計費率]、[!UICONTROL隊列詳細資訊]、[!UICONTROL規則]、[!UICONTROL主題]主題組]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL模板任務]</td> 
      <td>模板任務的名稱</td> 
      <td>[!UICONTROL更新]、[!UICONTROL文檔]、[!UICONTROL模板任務詳細資訊]、[!UICONTROL子任務]、[!UICONTROL費用]、[!UICONTROL批准]、[!UICONTROL前置任務]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL計費記錄]</td> 
      <td>項目的開單記錄的名稱</td> 
      <td>[!UICONTROL計費記錄詳細資訊]、[!UICONTROL計費小時數]、[!UICONTROL計費支出]、[!UICONTROL固定收入]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL項目]</td> 
      <td>專案 <img src="assets/projects-in-main-menu.png"> 在[!UICONTROL主菜單]中 <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL項目]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL請求]</td> 
      <td>請求的名稱</td> 
      <td>[!UICONTROL新請求]、[!UICONTROL已提交請求]、[!UICONTROL所有請求]、[!UICONTROL草稿]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL控制面板]</td> 
      <td>控制面板的名稱</td> 
      <td>[!UICONTROL我的控制面板]、[!UICONTROL共用控制面板]、[!UICONTROL所有控制面板]<p><b>注意</b>:如果您使用版面範本，為[!UICONTROL報表]區域建立自訂標籤，位於 [!DNL Adobe Workfront Classic]，則會顯示在此清單底部。 若為使用者，這些量度會顯示在[!UICONTROL控制面板]區域的左側面板底部。</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum團隊]</td> 
      <td>Scrum團隊的名稱</td> 
      <td><p>[!UICONTROL迭代]、[!UICONTROL當前迭代]、[!UICONTROL積壓]、[!UICONTROL工作負載平衡器]、[!UICONTROL更新]、[!UICONTROL團隊設定]</p> <p><strong>注意：</strong> 此 <strong>[!UICONTROL當前小版本]</strong> 只有在小版本上至少存在一個任務或問題時，項目才會顯示在左側面板中。</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL看板組]</td> 
      <td>看板小組的名稱</td> 
      <td>[!UICONTROL工作負載平衡器]、[!UICONTROL看板板]、[!UICONTROL積壓]、[!UICONTROL更新]、[!UICONTROL團隊設定]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL瀑布團隊]</td> 
      <td>瀑布團隊的名稱</td> 
      <td>[!UICONTROL工作負載平衡器]、[!UICONTROL更新]、[!UICONTROL團隊請求]、[!UICONTROL團隊設定]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL迭代]</td> 
      <td>小版本的名稱</td> 
      <td>[!UICONTROL Stories]、[!UICONTROL問題]、[!UICONTROL Story Board]、[!UICONTROL概述]、[!UICONTROL自定義Forms]、[!UICONTROL更新] </td> 
     </tr> 
     <!--
      <tr> 
       <td>Company</td> 
       <td>The name of the company</td> 
       <td> <p>People (cannot be hidden), Billing Rates, Custom Forms </p> </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Timesheets</td> 
       <td>The name of the timesheet</td> 
       <td>My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden) </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Resourcing</td> 
       <td>The name of the resource</td> 
       <td>Planner (cannot be hidden), Workload Balancer, Utilization, Resource Pools </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>User Details</td> 
       <td>____________</td> 
       <td>Details (cannot be hidden), Org Chart, Time Off, Custom Forms </td> 
      </tr>
     --> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >最後3個項目 **[!UICONTROL 自訂使用者看見的項目]** 下拉式清單([!UICONTROL 清單], [!UICONTROL 首頁和摘要]，和 [!UICONTROL 品牌推廣])用於設定左側面板以外的區域。 如需相關資訊，請參閱下列文章：
>   * [使用版面範本自訂篩選器、檢視和群組](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [自訂 [!UICONTROL 首頁] 和 [!UICONTROL 摘要] 使用版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [品牌Adobe [!DNL Workfront] 使用版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)



1. （可選）如果要新增連結至組織其中一個控制面板的左側面板項目，請按一下 **[!UICONTROL 新增自訂區段]**，鍵入 **[!UICONTROL 自訂區段標題]** 針對項目，然後新增控制面板。

   控制面板項目會顯示在左側面板底部。 當使用者將游標暫留在左側面板上時，會在控制面板項目旁看到您輸入的自訂區段標題。

   >[!NOTE]
   使用者可以將自訂控制面板項目新增至自己的左側面板。 在版面範本中新增自訂控制面板項目時，您的項目會與其項目合併，而不會覆寫或重設這些項目。 如果您將使用者指派至具有自訂控制面板項目的新配置範本，也會是如此。 如需使用者如何自訂左側面板的詳細資訊，請參閱 [建立自訂標籤或區段](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

   如需控制面板的相關資訊，請參閱 [控制面板](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. 繼續自訂配置範本。

   或

   如果您已完成自訂，請按一下 **[!UICONTROL 儲存]**.

   >[!TIP]
   您可以按一下 [!UICONTROL 儲存] 您隨時可以保存進度，稍後繼續修改模板。
