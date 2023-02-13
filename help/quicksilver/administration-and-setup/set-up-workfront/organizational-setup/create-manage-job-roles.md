---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 建立和管理作業角色
description: 作為 [!DNL Adobe Workfront] 管理員或具有「作業角色」管理訪問權限的用戶，可以建立可分配給用戶的作業角色，並刪除與組織無關的預設作業角色。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# 建立和管理作業角色

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作為 [!DNL Adobe Workfront] 管理員或具有「作業角色」管理訪問權限的用戶，可以建立可分配給用戶的作業角色，並刪除與組織無關的預設作業角色。 如需有關 [!DNL Workfront]，請參閱 [授予用戶對特定區域的管理訪問權限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>對作業角色的管理訪問</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 建立作業角色

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一&#x200B;下 **[!UICONTROL 作業角色].**
1. 按一下 **[!UICONTROL 新工作角色].**
1. 設定下列項目：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL名稱]</td> 
      <td> <p>指定作業角色的名稱。 這是中任何位置顯示的名稱 [!DNL Workfront] 其中顯示[!UICONTROL作業角色]欄位。 </p> <p>提示：作業角色的名稱最多可包含255個字元。 不過，某些區域的較長名稱可能會遭到截斷 [!DNL Workfront]. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL處於活動狀態]</span> </td> 
      <td> 
       <ul> 
        <li> <p>選擇 <b>[!UICONTROL是]</b> 如果您希望角色處於作用中狀態且可在 [!DNL Workfront] 與用戶、工作項等關聯。 </p> </li> 
        <li> <p>選擇 <b>[!UICONTROL否]</b>，如果您想要停用角色，但無法指派給使用者、工作項目等。 </p> </li> 
       </ul> <p><span>有關停用作業角色的資訊，請參閱</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">停用作業角色</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td>輸入角色的說明，以指明該角色的獨特之處。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL基本貨幣]</span> </td> 
      <td> <p><span>這是[!UICONTROL基本貨幣]，如您的Workfront管理員在[!UICONTROL設定]區域中所設定。 如需詳細資訊，請參閱</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a> .</p> <p>提示： <span>您無法在作業角色級別編輯[!UICONTROL基本貨幣]。 此欄位呈灰色，可提醒您系統的基本貨幣為何。</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL成本/小時]</td> 
      <td>這是作業角色的每小時成本率。 此值計算與職責相關的任務和問題的計畫成本和實際成本，最終計算項目的計畫成本和實際成本。 <span>使用[!UICONTROL基本貨幣]輸入匯率。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL帳單/小時] </td> 
      <td>這是作業角色的每小時計費率。 此值計算任務和與職責相關的問題的計畫收入和實際收入，最終計算項目的計畫收入和實際收入。 使用[!UICONTROL基本貨幣]輸入匯率。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL覆蓋貨幣]</span> </td> 
      <td> 
       <div> 
        <p>選擇與此作業角色關聯的貨幣。 這是 [!DNL Workfront] 用於計算與此任務角色關聯的成本和收入。 </p> 
        <p><span>這與您 [!DNL Workfront] 管理員（位於[!UICONTROL設定]區域中），並且可能與與項目關聯的貨幣不同。</span> </p> 
        <p>提示：此欄位中只有系統中[!UICONTROL匯率]區域中可用的貨幣可用。</p> 
       </div> <p><span>如需有關在 [!DNL Workfront]，請參閱</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>.</p> <p><span>如需變更專案貨幣的相關資訊，請參閱</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">更改項目幣種</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL覆蓋貨幣成本/小時]</span> </td> 
      <td> 
       <div> 
        <p>這是使用所選[!UICONTROL覆蓋幣種]的作業角色的每小時成本比率。 [!DNL Workfront] 使用此值來計算與任務職責關聯的任務和問題的計畫成本和實際成本。 </p> 
        <p><span>在上述指定的[!UICONTROL覆蓋貨幣]中輸入匯率。 這也會在使用[!UICONTROL基本貨幣]時更新此作業角色的成本/小時費率。</span> </p> 
        <p>如需如何 [!DNL Workfront] 計算成本，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> 
       </div> <p>提示：更新已與其關聯的成本/小時費率的現有作業角色時， [!DNL Workfront] 根據系統中的轉換率計算[!UICONTROL覆蓋貨幣]匯率。 如果更新[!UICONTROL改寫幣種成本/小時]，則作業角色的成本/小時也會自動更新。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL覆蓋貨幣帳單/小時]</span> </td> 
      <td> 
       <div> 
        <p>這是使用所選[!UICONTROL覆蓋幣種]的作業角色的每小時計費率。 [!DNL Workfront] 使用此值來計算與任務職責關聯的任務和問題的計畫收入和實際收入。 </p> 
        <p><span>在上述指定的[!UICONTROL覆蓋貨幣]中輸入匯率。 這也會在使用[!UICONTROL基本貨幣]時更新此作業角色的計費/小時費率。</span> </p> 
        <p>如需如何 [!DNL Workfront] 計算收入，請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單和收入概觀</a>.</p> 
       </div> <p>提示：更新已與其關聯的開單/小時費率的現有作業角色時， [!DNL Workfront] 根據系統中的轉換率計算「改寫貨幣」匯率。 如果更新「改寫幣種開單/小時」，則作業角色的「開單/小時」也會自動更新。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >工作角色是管理資源的必要部分。 要使用資源規劃工具，任務職責需要與它們關聯的成本和開單費率。 如需詳細資訊，請參閱 [開始使用資源管理](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. 按一下 **[!UICONTROL 建立作業角色]**. 現在，作業角色可以分配給任務、問題、批准，或者您可以與其共用佈局模板或其他對象。 有關中作業角色的所有使用的資訊 [!DNL Workfront]，請參閱 [工作角色概觀](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). 有關刪除作業角色的資訊，請參閱 [刪除作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
