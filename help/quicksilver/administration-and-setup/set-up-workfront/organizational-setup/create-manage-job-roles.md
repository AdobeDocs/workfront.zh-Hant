---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 建立和管理職位角色
description: 作為 [!DNL Adobe Workfront] 管理員或具有「工作角色」管理存取許可權的使用者，您可以建立可指派給使用者的工作角色，並刪除與您的組織無關的預設工作角色。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: e5416fab4f4ad1f2c31edf962554ddd6a4c2f1e5
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# 建立和管理職務角色

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>在25.11版中，工作角色的覆寫貨幣將在生產環境中被取代。 （10月30日在預覽環境中將停止使用。） 工作角色將可以使用一種貨幣，而不使用基本貨幣和覆寫貨幣，並將使用該貨幣定義成本和計費率。

作為[!DNL Adobe Workfront]管理員或具有工作角色管理存取權的使用者，您可以建立可指派給使用者的工作角色，並刪除與您的組織無關的預設工作角色。 如需[!DNL Workfront]中管理存取權的相關資訊，請參閱[授予使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[!UICONTROL 標準]</p>
       <p>[!UICONTROL 計畫]</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>工作角色的管理存取權</td>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立職位角色

若要建立工作角色，請執行下列動作：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 工作角色].**
1. 按一下&#x200B;**[!UICONTROL 新增工作角色].**
1. 設定下列欄位：

   * **名稱**：表示工作角色的名稱。 這是Workfront中顯示「工作角色」欄位的所有位置的名稱。

     >[!TIP]
     >
     >工作角色的名稱最多可包含255個字元。 不過，在Workfront的某些區域，較長的名稱可能會被截斷。

   * **描述**：輸入角色的描述，以指出其獨特性。
   * **為作用中**：如果您想要該角色為作用中，並且可在Workfront中的任何地方與使用者、工作專案等建立關聯，請選取&#x200B;**是**。 如果您想要停用該角色，且不將其指派給使用者、工作專案等，請選取&#x200B;**否**。

     如需有關停用工作角色的資訊，請參閱[停用工作角色](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)。

   * **基本貨幣**：這是基本貨幣，如您的Workfront管理員在設定區域中設定。 如需詳細資訊，請參閱[設定匯率](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

     >[!TIP]
     >
     >您無法在工作角色層級編輯基本貨幣。 此欄位會變暗，以提醒您系統的基本貨幣為何。

   * **成本費率**：這是工作角色的每小時成本費率。 此值會計算與角色相關之任務與問題的計畫成本與實際成本，以及最終的專案計畫成本與實際成本。 使用「基本貨幣」輸入匯率。

     若要取得日期有效成本費率，請按一下[新增費率]。**&#x200B;** 輸入時間期間的成本/小時值，並視需要指定「開始日期」與「結束日期」。 第一個成本費率不會有開始日期，而最後一個成本費率不會有結束日期。

     部分日期會自動新增。 例如，如果第一個成本費率沒有結束日期，而您新增了開始日期為2025年5月1日的第二個成本費率，則結束日期為2025年4月30日的成本費率會新增至第一個成本費率，這樣就不會有差距。

     >[!TIP]
     >
     >編輯現有工作角色時，您可以選取&#x200B;**依開始日期排序**，在費率清單頂端檢視最近的開始日期。

   * **收費率**：這是工作角色的每小時收費率。 此值會計算與角色相關之任務和問題的計畫和實際收入，最終是專案的計畫和實際收入。 使用「基本貨幣」輸入匯率。

     若要取得日期有效收費率，請按一下[新增費率]。**&#x200B;** 輸入時間期間的帳單/小時值，並視需要指定「開始日期」與「結束日期」。 第一個收費率不會有開始日期，而最後一個收費率則不會有結束日期。

     部分日期會自動新增。 例如，如果第一個收費率沒有結束日期，而您新增了開始日期為2025年5月1日的第二個收費率，則第一個收費率會新增2025年4月30日的結束日期，因此不會有間隙。

     >[!TIP]
     >
     >編輯現有工作角色時，您可以選取&#x200B;**依開始日期排序**，在費率清單頂端檢視最近的開始日期。

   * **覆寫貨幣**：選取與此工作角色關聯的貨幣。 這是Workfront用於計算與此職務角色相關之成本和收入的貨幣。

     這與Workfront管理員在設定區域中設定的基本貨幣不同，也可能會與專案相關的貨幣不同。

     >[!TIP]
     >
     >此欄位僅提供您系統中「匯率」區域中可用的貨幣。 如果您只設定一種貨幣，則此欄位不會出現。

     如需有關在Workfront中設定基本貨幣的資訊，請參閱[設定匯率](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

     如需有關變更專案貨幣的資訊，請參閱[變更專案貨幣](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md)。

   * **覆寫貨幣成本費率**：這是使用所選覆寫貨幣的工作角色的每小時成本費率。 Workfront使用此值來計算與工作角色相關之任務和問題的計畫成本與實際成本。

     以上述指定的「修訂幣別」輸入匯率。 當使用基本貨幣時，這也會更新此職務角色的成本率。

     如需Workfront如何計算成本的詳細資訊，請參閱[追蹤成本](/help/quicksilver/manage-work/projects/project-finances/track-costs.md)。

     >[!TIP]
     >
     >在更新已具有相關成本費率的現有職務角色時，Workfront會根據您系統中的兌換率計算「修訂幣別」費率。 如果您更新「修訂幣別成本費率」，職務角色的成本費率也會自動更新。

   * **覆寫貨幣收費率**：這是使用所選覆寫貨幣的工作角色的每小時收費率。 Workfront使用此值來計算與工作角色相關之任務和問題的計畫和實際收入。

     以上述指定的「修訂幣別」輸入匯率。 使用基本貨幣時，這也會更新此職務角色的計費率。

     如需Workfront如何計算收入的詳細資訊，請參閱[帳單與收入概觀](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)。

     >[!TIP]
     >
     >在更新已有關聯收費率的現有職務角色時，Workfront會根據您系統中的轉換率計算「覆寫貨幣」費率。 如果您更新「覆寫幣別帳單費率」，職務角色的帳單費率也會自動更新。

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicate a name for the job role. This is the name that displays everywhere in [!DNL Workfront] where the [!UICONTROL Job Role] field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Enter a description for the role that indicates what is unique about it. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <b>[!UICONTROL Yes]</b> if you want the role to be active and available everywhere in [!DNL Workfront] to be associated with users, work items, etc. </p> </li> 
        <li> <p>Select <b>[!UICONTROL No]</b>, if you want the role to be deactivated and not available to assign to users, work items, etc. </p> </li> 
       </ul> <p><span>For information about deactivating job roles, see</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>This is the [!UICONTROL Base Currency], as set in the [!UICONTROL Setup] area by your Workfront administrator. For information, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span>You cannot edit the [!UICONTROL Base Currency] at the job role level. This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> 
      <p>For date effective cost rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the cost/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first cost rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> <p>For date effective billing rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the billing/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first billing rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Select a currency associated with this job role. This is the currency that [!DNL Workfront] uses for calculating costs and revenue associated with this job role. </p> 
        <p><span>This is different than the [!UICONTROL Base Currency] set up by your [!DNL Workfront] administrator in the [!UICONTROL Setup] area, and can be different than the currency associated with a project.</span> </p> 
        <p>Tip: Only currencies available in the [!UICONTROL Exchange Rates] area in your system are available in this field. If you only have one currency set up, this field is does not appear.</p> 
       <p><span>For information about setting up the [!UICONTROL Base Currency] in [!DNL Workfront], see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span>For information about changing the currency of a project, see</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>This is the cost per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Cost Rate for this job role when using the [!UICONTROL Base Currency].</span> </p> 
        <p>For information about how [!DNL Workfront] calculates cost, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> 
       <p>Tip: When updating an existing job role that already has a Cost Rate associated with it, [!DNL Workfront] calculates the [!UICONTROL Override Currency] rate based on the conversion rate in your system. If you update the [!UICONTROL Override Currency Cost Rate], the Cost Rate of the job role also updates automatically.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>This is the billing per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p>
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Billing Rateate for this job role when using the [!UICONTROL Base Currency].</span> </p>
        <p>For information about how [!DNL Workfront] calculates revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p>
        <p>Tip: When updating an existing job role that already has a Billing Rate associated with it, [!DNL Workfront] calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the Billing Rate of the job role also updates automatically. </p>
       </td>
     </tr> 
    </tbody> 
   </table>
-->

>[!TIP]
>
>工作角色是管理資源的必要部分。 若要使用資源計畫工具，職務角色需要與其相關的成本與帳單費率。 如需詳細資訊，請參閱[開始使用資源管理](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)。

1. 按一下&#x200B;**[!UICONTROL 建立工作角色]**。 工作角色現在可指派給任務、問題、核准，或者您可以與其共用版面範本或其他物件。 如需[!DNL Workfront]中所有工作角色使用的相關資訊，請參閱[工作角色總覽](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)。 如需有關刪除工作角色的資訊，請參閱[刪除工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md)。

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
