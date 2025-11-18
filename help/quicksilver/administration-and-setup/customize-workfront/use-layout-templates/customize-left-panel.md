---
title: 使用版面配置範本自訂左側面板
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 在版面配置範本中，您可以自訂使用者在整個Adobe Workfront的左側面板區域中看到的內容。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: 96028446d76f32daf512adf77d3b1c53021821ec
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 1%

---

# 使用版面配置範本自訂左側面板

{{preview-fast-release-general}}

<!--Audited: 10/2024-->

在版面配置範本中，您可以自訂使用者在整個[!DNL Adobe Workfront]的左側面板區域中看到的內容。

例如，您可以決定使用者在檢視專案時，會在左側面板中看見下列哪些專案：

![專案的左側面板](assets/left-panel-in-project.png)

>[!IMPORTANT]
>
>對順序和可見性所做的變更會反映在行動應用程式中。

如需有關建立版面配置範本的資訊，請參閱[建立和管理版面配置範本](../use-layout-templates/create-and-manage-layout-templates.md)。

如需有關群組配置範本的資訊，請參閱[建立和修改群組的配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置版面範本後，您必須將其指派給使用者，才能讓其他人看到您所做的變更。 如需將配置範本指派給使用者的詳細資訊，請參閱[將使用者指派給配置範本](../use-layout-templates/assign-users-to-layout-template.md)。

## 存取需求

+++ 展開以查看此文章中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 套件</td> 
   <td><p>任何</p>
       <p>將自訂應用程式新增至主功能表僅適用於授權Adobe App Builder的組織。</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。</p>
        <p>若要為群組執行這些動作，您必須是該群組的管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自訂[!DNL Workfront]中某個區域的左側面板：

1. 開始使用版面配置範本，如[建立和管理版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 按一下![自訂使用者看到的內容](assets/dropdown-arrow.png)底下的向下箭頭&#x200B;**[!UICONTROL 向下箭頭]**，然後按一下您要自訂其左側面板的物件型別或[!DNL Workfront]區域的名稱。

   下表列出您可以自訂其左側面板的物件型別和[!DNL Workfront]區域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>物件型別或[!DNL Workfront]區域</th> 
      <th>當使用者按一下以下時……</th> 
      <th>在版面配置範本中顯示區段後，使用者會看到的左側面板區段：</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL 專案]</td> 
      <td>專案名稱</td> 
      <td>[!UICONTROL 任務]， [!UICONTROL 專案詳細資料]， [!UICONTROL 業務案例]， [!UICONTROL 更新]， [!UICONTROL 檔案]， [!UICONTROL 問題]， [!UICONTROL 風險]， [!UICONTROL 核准]， [!UICONTROL 基準]， [!UICONTROL 計費費率]，[!UICONTROL 計費記錄]， [!UICONTROL uicontrol支出]、[!UICONTROL 小時數]、[!UICONTROL 工作負載均衡器]、[!UICONTROL 人員]、[!UICONTROL 利用率]、[!UICONTROL 隊列詳細資訊]、[!UICONTROL 路由規則]、[!UICONTROL 隊列主題]、[!UICONTROL 主題組]、[!UICONTROL 量度]、[!UICONTROL 規劃]*、[!UICONTROL 自定義應用程式]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 任務]</td> 
      <td>任務的名稱</td> 
      <td> [!UICONTROL 更新]， [!UICONTROL 檔案]， [!UICONTROL 任務詳細資訊]， [!UICONTROL 子任務]， [!UICONTROL 問題]， [!UICONTROL 小時]， [!UICONTROL 核准]， [!UICONTROL 費用]， [!UICONTROL 前置任務]， [!UICONTROL 自訂應用程式]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 問題]</td> 
      <td>問題的名稱</td> 
      <td> [!UICONTROL 更新]、[!UICONTROL 檔案]、[!UICONTROL 問題詳細資訊]、[!UICONTROL 小時]、[!UICONTROL 核准]、[!UICONTROL 自訂應用程式]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>投資組合的名稱</td> 
      <td>[!UICONTROL 專案]， [!UICONTROL 計畫]， [!UICONTROL Portfolio詳細資料]， [!UICONTROL Portfolio] [!UICONTROL 最佳化]， [!UICONTROL 檔案]， [!UICONTROL 更新]， [!UICONTROL 規劃]*， [!UICONTROL 自訂應用程式]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>方案的名稱</td> 
      <td>[!UICONTROL 專案]、[!UICONTROL 計畫詳細資料]、[!UICONTROL 更新]、[!UICONTROL 檔案]、[!UICONTROL 計畫]*、[!UICONTROL 自訂應用程式]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 範本]</td> 
      <td>專案範本的名稱</td> 
      <td>[!UICONTROL 範本任務]， [!UICONTROL 範本詳細資料]， [!UICONTROL 更新]， [!UICONTROL 檔案]， [!UICONTROL 風險]， [!UICONTROL 費用]， [!UICONTROL 人員]， [!UICONTROL 核准]， [!UICONTROL 計費率]， [!UICONTROL 佇列詳細資料]， [!UICONTROL 路由規則]， [!UICONTROL uicontrol隊列主題]，[!UICONTROL 主題組]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 範本任務]</td> 
      <td>範本任務的名稱</td> 
      <td>[!UICONTROL 更新]， [!UICONTROL 檔案]， [!UICONTROL 範本任務詳細資訊]， [!UICONTROL 子任務]， [!UICONTROL 費用]， [!UICONTROL 核准]， [!UICONTROL 前置任務]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL 付費記錄]</td> 
      <td>專案的計費記錄名稱</td> 
      <td>[!UICONTROL 計費記錄詳細資料]、[!UICONTROL 可計費時數]、[!UICONTROL 可計費費用]、[!UICONTROL 固定收入]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 專案]</td> 
      <td>[!UICONTROL 主功能表]中的專案<img src="assets/projects-in-main-menu.png"> <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL 專案]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 請求]</td> 
      <td>請求的名稱</td> 
      <td>[!UICONTROL 新請求]、[!UICONTROL 已提交請求]、[!UICONTROL 所有請求]、[!UICONTROL 草稿]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 儀表板]</td> 
      <td>控制面板的名稱</td> 
      <td>[!UICONTROL 我的儀表板]、[!UICONTROL 共用儀表板]、[!UICONTROL 所有儀表板]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum團隊]</td> 
      <td>Scrum團隊的名稱</td> 
      <td><p>[!UICONTROL 反複專案]、[!UICONTROL 目前反複專案]、[!UICONTROL 待處理專案]、[!UICONTROL 工作負載平衡器]、[!UICONTROL 更新]、[!UICONTROL 團隊設定]</p> <p><strong>注意：</strong> <strong>[!UICONTROL 目前反複專案]</strong>專案只有在反複專案上至少有一個任務或問題時，才會顯示在左側面板中。</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban團隊]</td> 
      <td>Kanban團隊的名稱</td> 
      <td>[!UICONTROL 工作負載平衡器]、[!UICONTROL Kanban board]、[!UICONTROL 待處理專案]、[!UICONTROL 更新]、[!UICONTROL 團隊設定]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfall團隊]</td> 
      <td>Waterfall團隊的名稱</td> 
      <td>[!UICONTROL 工作負載平衡器]、[!UICONTROL 更新]、[!UICONTROL 團隊請求]、[!UICONTROL 團隊設定]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL 反複專案]</td> 
      <td>反複專案的名稱</td> 
      <td>[!UICONTROL Stories]， [!UICONTROL Issues]， [!UICONTROL Story Board]， [!UICONTROL Overview]， [!UICONTROL Custom Forms]， [!UICONTROL Updates] </td> 
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

   *貴公司必須購買Workfront Planning的額外授權，才能將此區域新增至專案、產品組合和計畫的左側面板。 如需詳細資訊，請參閱[開始使用Adobe Workfront計畫](/help/quicksilver/planning/general/planning-overview.md)

   **自訂應用程式必須個別建立，才能作為主功能表選項使用。 如需詳細資訊，請參閱[使用Adobe App Builder建立Workfront的自訂應用程式](/help/quicksilver/app-builder/app-builder.md)。


1. 在&#x200B;**[!UICONTROL 左側面板]**&#x200B;清單中，執行下列任一項作業，以決定使用者會在左側面板中看見您所選取的[!DNL Workfront]區域或物件型別：

   * 按一下&#x200B;**顯示** ![顯示圖示](assets/add-secondary-nav-item.png)或&#x200B;**隱藏** ![隱藏圖示](assets/delete-secondary-nav-item.png)圖示，以顯示或隱藏左側面板中的區段。 您無法隱藏沒有&#x200B;**顯示**&#x200B;或&#x200B;**隱藏**&#x200B;圖示的專案。

   * 拖曳專案![移動圖示](assets/move-icon---dots.png)以變更其在左側面板上的順序。

   >[!NOTE]
   >
   >**[!UICONTROL 自訂使用者看到的內容]**&#x200B;下拉式清單中的下列專案，參照的是左側面板以外的區域：
   >* [!UICONTROL 清單]
   >* [!UICONTROL 摘要面板]
   >* [!UICONTROL 首頁]
   >* [!UICONTROL 品牌]
   > 
   >如需有關如何自訂其他區域的資訊，請參閱下列文章：
   >
   >* [使用配置範本自訂篩選器、檢視和群組](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >* [使用配置範本自訂[!UICONTROL 摘要面板]](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   >* [使用配置範本自訂首頁](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   >* 使用版面配置範本的[品牌Adobe [!DNL Workfront] &#x200B;](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. （選擇性）如果您想要新增連結至貴組織其中一個儀表板的左側面板專案，請按一下&#x200B;**[!UICONTROL 新增儀表板]**，輸入專案的&#x200B;**[!UICONTROL 快速連結名稱]**，然後選擇儀表板。

   您必須先建置儀表板，儀表板才會出現在清單中。

   儀表板專案會出現在左側面板的底部。

   >[!NOTE]
   >
   >使用者可以將自訂儀表板專案新增到自己的左側面板。 當您在版面配置範本中新增自訂儀表板專案時，除了它們新增的專案外，還會顯示您的專案，而不會覆寫或重設它們。 如果您將使用者指派給具有自訂儀表板專案的新配置範本，也會發生這種情況。 若要瞭解使用者如何自訂左側面板，請參閱[在Workfront物件或區域的左側面板中新增儀表板](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)。
   >
   >如需儀表板的詳細資訊，請參閱[儀表板](../../../reports-and-dashboards/dashboards/dashboards-overview.md)。

1. <span class="preview">在預覽環境中：繼續自訂版面範本。 您可以隨時按一下&#x200B;**套用**&#x200B;以儲存進度。</span>

   <span class="preview">或</span>

   <span class="preview">如果您已完成自訂，請按一下&#x200B;**儲存並關閉**。</span>

1. 在生產環境中：繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下&#x200B;**儲存**。

   >[!TIP]
   >
   >您可以隨時按一下[儲存]來儲存進度，然後再繼續修改範本。**&#x200B;**
