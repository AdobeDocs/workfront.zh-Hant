---
title: 使用版面配置範本自訂左側面板
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 在版面配置範本中，您可以自訂使用者在整個Adobe Workfront的左側面板區域中看到的內容。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 0%

---

# 使用版面配置範本自訂左側面板

在版面配置範本中，您可以自訂使用者在整個[!DNL Adobe Workfront]的左側面板區域中看到的內容。

例如，您可以決定使用者在檢視任務時，會在左側面板中看到下列哪些專案：

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>對順序和可見性所做的變更會反映在行動應用程式中。

如需有關建立版面配置範本的資訊，請參閱[建立和管理版面配置範本](../use-layout-templates/create-and-manage-layout-templates.md)。

如需有關群組配置範本的資訊，請參閱[建立和修改群組的配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置版面範本後，您必須將其指派給使用者，才能讓其他人看到您所做的變更。 如需將配置範本指派給使用者的詳細資訊，請參閱[將使用者指派給配置範本](../use-layout-templates/assign-users-to-layout-template.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> 若要在系統層級執行這些步驟，您需要[！UICONTROL系統管理員]存取層級。<p>若要為群組執行這些動作，您必須是該群組的管理員。</p> <p><b>注意</b>：如果您仍然沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂[!DNL Workfront]中某個區域的左側面板：

1. 開始使用版面配置範本，如[建立和管理版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 按一下&#x200B;**[!UICONTROL 自訂使用者看到的內容]**&#x200B;下方的向下箭頭![](assets/dropdown-arrow.png)，然後按一下您要自訂的左側面板。

   >[!NOTE]
   >
   >如需此下拉式清單中[!UICONTROL 首頁]選項的相關資訊，請參閱[使用配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)自訂[!UICONTROL 首頁]和[!UICONTROL 摘要]。 如需[清單]選項的相關資訊，請參閱[使用版面配置範本自訂篩選器、檢視和群組](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

1. 在&#x200B;**[!UICONTROL 左側面板]**&#x200B;清單中，執行下列任一項作業，以決定使用者會在左側面板中看見您所選取的選項（[!DNL Workfront]區域或物件型別）的內容：

   * 顯示![](assets/add-secondary-nav-item.png)或隱藏![](assets/delete-secondary-nav-item.png)專案。 無法隱藏任何沒有![](assets/add-secondary-nav-item.png)或![](assets/delete-secondary-nav-item.png)的專案。

   * 拖曳專案![](assets/move-icon---dots.png)以變更其在左側面板上的順序。
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>選項</th> 
      <th>當使用者按一下以下時……</th> 
      <th>他們看到您從下列選項中選擇的左側面板專案：</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[！UICONTROL專案]</td> 
      <td>專案名稱</td> 
      <td>[！UICONTROL任務]， [！UICONTROL專案詳細資料]， [！UICONTROL業務案例]， [！UICONTROL更新]， [！UICONTROL檔案]， [！UICONTROL問題]， [！UICONTROL風險]， [！UICONTROL核准]， [！UICONTROL基準]， [！UICONTROL計費費率]，[！UICONTROL計費記錄]， [！UICONTROL trol費用]、[！UICONTROL小時數]、[！UICONTROL工作負載均衡器]、[！UICONTROL人員]、[！UICONTROL利用率]、[！UICONTROL隊列詳細資訊]、[！UICONTROL路由規則]、[！UICONTROL隊列主題]、[！UICONTROL主題組]、[！UICONTROL量度]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL任務]</td> 
      <td>任務的名稱</td> 
      <td> [！UICONTROL更新]， [！UICONTROL檔案]， [！UICONTROL任務詳細資訊]， [！UICONTROL子任務]， [！UICONTROL問題]， [！UICONTROL小時]， [！UICONTROL核准]， [！UICONTROL費用]， [！UICONTROL前置任務]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL問題]</td> 
      <td>問題的名稱</td> 
      <td> [！UICONTROL更新]、[！UICONTROL檔案]、[！UICONTROL問題詳細資訊]、[！UICONTROL小時]、[！UICONTROL核准]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROLPortfolio]</td> 
      <td>投資組合的名稱</td> 
      <td>[！UICONTROL專案]， [！UICONTROL計畫]， [！UICONTROLPortfolio詳細資訊]， [！UICONTROLPortfolio] [！UICONTROL最佳化]， [！UICONTROL檔案]， [！UICONTROL更新]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL Program]</td> 
      <td>方案的名稱</td> 
      <td>[！UICONTROL專案]， [！UICONTROL計畫詳細資料]， [！UICONTROL更新]， [！UICONTROL檔案]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL範本]</td> 
      <td>專案範本的名稱</td> 
      <td>[！UICONTROL範本任務]， [！UICONTROL範本詳細資料]， [！UICONTROL更新]， [！UICONTROL檔案]， [！UICONTROL風險]， [！UICONTROL費用]， [！UICONTROL人員]， [！UICONTROL核准]， [！UICONTROL計費率]， [！UICONTROL佇列詳細資料]，[！UICONTROL路由規則]， [！UICONTROL trol隊列主題]，[！UICONTROL主題組]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL範本任務]</td> 
      <td>範本任務的名稱</td> 
      <td>[！UICONTROL更新]， [！UICONTROL檔案]， [！UICONTROL範本任務詳細資訊]， [！UICONTROL子任務]， [！UICONTROL費用]， [！UICONTROL核准]， [！UICONTROL前置任務]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [！UICONTROL付費記錄]</td> 
      <td>專案的計費記錄名稱</td> 
      <td>[！UICONTROL計費記錄詳細資料]、[！UICONTROL可計費時數]、[！UICONTROL可計費費用]、[！UICONTROL固定收入]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL專案]</td> 
      <td>[！UICONTROL主功能表]中的專案<img src="assets/projects-in-main-menu.png"> <img src="assets/main-menu-icon.png"></td> 
      <td>[！UICONTROL專案]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL請求]</td> 
      <td>請求的名稱</td> 
      <td>[！UICONTROL新請求]、[！UICONTROL已提交請求]、[！UICONTROL所有請求]、[！UICONTROL草稿]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL儀表板]</td> 
      <td>控制面板的名稱</td> 
      <td>[！UICONTROL我的儀表板]、[！UICONTROL共用儀表板]、[！UICONTROL所有儀表板]<p><b>注意</b>：如果您在[!DNL Adobe Workfront Classic]中使用版面配置範本建立[！UICONTROL報告]區域的自訂標籤，它們會顯示在此清單底部。 若是使用者，註解會顯示在[！UICONTROL控制面板]區域左側面板底部。</p> </td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL Scrum團隊]</td> 
      <td>Scrum團隊的名稱</td> 
      <td><p>[！UICONTROL反複專案]、[！UICONTROL目前反複專案]、[！UICONTROL待處理專案]、[！UICONTROL工作負載平衡器]、[！UICONTROL更新]、[！UICONTROL團隊設定]</p> <p><strong>注意：</strong> <strong>[！UICONTROL目前反複專案]</strong>專案只有在反複專案上至少有一個任務或問題時，才會顯示在左側面板中。</p></td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL Kanban團隊]</td> 
      <td>Kanban團隊的名稱</td> 
      <td>[！UICONTROL工作負載平衡器]、[！UICONTROL Kanban board]、[！UICONTROL待處理專案]、[！UICONTROL更新]、[！UICONTROL團隊設定]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL Waterfall團隊]</td> 
      <td>Waterfall團隊的名稱</td> 
      <td>[！UICONTROL工作負載平衡器]、[！UICONTROL更新]、[！UICONTROL團隊請求]、[！UICONTROL團隊設定]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL反複專案]</td> 
      <td>反複專案的名稱</td> 
      <td>[！UICONTROL Stories]， [！UICONTROL Issues]， [！UICONTROL Story Board]， [！UICONTROL Overview]， [！UICONTROL Custom Forms]， [！UICONTROL Updates] </td> 
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
   >**[!UICONTROL 自訂使用者看到的專案]**&#x200B;下拉式清單（[!UICONTROL 清單]、[!UICONTROL 首頁和摘要]以及[!UICONTROL 品牌]）中的最後3個專案是用於設定左側面板以外的區域。 如需其相關資訊，請參閱下列文章：
>   >   
* [使用配置範本自訂篩選器、檢視和群組](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [使用配置範本自訂[!UICONTROL 首頁]和[!UICONTROL 摘要]](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* 使用版面配置範本的[品牌Adobe [!DNL Workfront] ](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. （選擇性）如果您想要新增連結至您組織其中一個儀表板的左側面板專案，請按一下「**[!UICONTROL 新增自訂區段]**」，為專案輸入「**[!UICONTROL 自訂區段標題]**」，然後新增儀表板。

   儀表板專案會出現在左側面板的底部。 當使用者將滑鼠游標停留在左側面板上時，他們會看到您在控制面板專案旁鍵入的自訂區段標題。

   >[!NOTE]
   >
   使用者可以將自訂儀表板專案新增到自己的左側面板。 當您在版面配置範本中新增自訂儀表板專案時，您的專案會與其合併，而不會覆寫或重設它們。 如果您將使用者指派給具有自訂儀表板專案的新配置範本，也會發生這種情況。 若要瞭解使用者如何自訂左側面板，請參閱[建立自訂標籤或區段](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)。

   如需儀表板的詳細資訊，請參閱[儀表板](../../../reports-and-dashboards/dashboards/dashboards-overview.md)。

1. 繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下&#x200B;**[!UICONTROL 儲存]**。

   >[!TIP]
   >
   您可以隨時按一下[儲存]來儲存進度，然後再繼續修改範本。
