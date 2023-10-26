---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 建立和管理職位角色
description: 作為 [!DNL Adobe Workfront] 管理員或具有職位角色管理存取權的使用者，您可以建立可指派給使用者的職位角色，並刪除與您的組織無關的預設職位角色。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 0%

---

# 建立和管理職位角色

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作為 [!DNL Adobe Workfront] 管理員或具有職位角色管理存取權的使用者，您可以建立可指派給使用者的職位角色，並刪除與您的組織無關的預設職位角色。 有關中管理存取許可權的資訊 [!DNL Workfront]，請參閱 [授予使用者管理特定區域的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

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
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>職位角色的管理存取權</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 建立職位角色

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下&#x200B;。 **[!UICONTROL 職位角色].**
1. 按一下 **[!UICONTROL 新增工作角色].**
1. 設定下列專案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL名稱]</td> 
      <td> <p>指定工作角色的名稱。 此名稱會顯示「 」中的所有位置 [!DNL Workfront] 其中顯示[！UICONTROL Job Role]欄位。 </p> <p>提示：工作角色的名稱最多可包含255個字元。 不過，較長名稱在下列特定區域可能會遭到截斷： [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[！UICONTROL說明]</td> 
      <td>輸入角色的描述，以指出其獨特性。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[！UICONTROL作用中]</span> </td> 
      <td> 
       <ul> 
        <li> <p>選取 <b>[！UICONTROL是]</b> 如果您希望角色在中任何地方都可使用且為作用中 [!DNL Workfront] 以與使用者、工作專案等建立關聯。 </p> </li> 
        <li> <p>選取 <b>[！UICONTROL否]</b>，如果您想要停用角色，且無法將其指派給使用者、工作專案等。 </p> </li> 
       </ul> <p><span>如需有關停用工作角色的資訊，請參閱</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">停用職位角色</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[！UICONTROL基本貨幣]</span> </td> 
      <td> <p><span>這是您的Workfront管理員在[！UICONTROL設定]區域中設定的[！UICONTROL基本貨幣]。 如需詳細資訊，請參閱</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a> .</p> <p>秘訣： <span>您無法在工作角色層級編輯[！UICONTROL基本貨幣]。 此欄位會變暗，以提醒您系統的基本貨幣為何。</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL成本率]</td> 
      <td><p>這是工作角色的每小時成本率。 此值會計算與角色相關之任務與問題的計畫成本與實際成本，以及最終的專案計畫成本與實際成本。 使用[！UICONTROL基本貨幣]輸入匯率。</p> 
      <p>若要取得日期有效成本率，請按一下 <strong>[！UICONTROL加入率]</strong>. 輸入時段的成本/小時值，並視需要指派[！UICONTROL開始日期]和[！UICONTROL結束日期]。 第一個成本費率不會有開始日期，而最後一個成本費率不會有結束日期。</p> <p>部分日期會自動新增。 例如，如果第一個成本費率沒有結束日期，而您新增了開始日期為2023年5月1日的第二個成本費率，則結束日期為2023年4月30日的成本費率會新增至第一個成本費率，這樣就不會有差距。</p> <p>提示：編輯現有工作角色時，您可以選取 <strong>依開始日期排序</strong> 若要在費率清單頂端檢視最近的開始日期。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL收費率] </td> 
      <td><p>這是工作角色的每小時收費率。 此值會計算與角色相關之任務和問題的計畫和實際收入，最終是專案的計畫和實際收入。 使用[！UICONTROL基本貨幣]輸入匯率。</p> <p>如需日期有效收費率，請按一下 <strong>[！UICONTROL加入率]</strong>. 輸入時段的記帳/小時值，並視需要指派[！UICONTROL開始日期]和[！UICONTROL結束日期]。 第一個收費率不會有開始日期，而最後一個收費率則不會有結束日期。</p> <p>部分日期會自動新增。 例如，如果第一個收費率沒有結束日期，而您新增了開始日期為2023年5月1日的第二個收費率，則第一個收費率會新增2023年4月30日的結束日期，因此不會有間隙。</p> <p>提示：編輯現有工作角色時，您可以選取 <strong>依開始日期排序</strong> 若要在費率清單頂端檢視最近的開始日期。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[！UICONTROL覆寫貨幣]</span> </td> 
      <td>
        <p>選取與此工作角色關聯的貨幣。 這是具有以下特性的貨幣 [!DNL Workfront] 會使用來計算與此職務角色相關聯的成本和收入。 </p> 
        <p><span>與您設定的[！UICONTROL基本貨幣]不同 [!DNL Workfront] 管理員（位於[！UICONTROL設定]區域），且可能與專案相關的貨幣不同。</span> </p> 
        <p>提示：此欄位僅提供您系統中[！UICONTROL Exchange Rates]區域中可用的貨幣。</p> 
       <p><span>如需有關在中設定[！UICONTROL基本貨幣]的資訊 [!DNL Workfront]，請參閱</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>.</p> <p><span>如需有關變更專案貨幣的資訊，請參閱</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">變更專案貨幣</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[！UICONTROL覆寫貨幣成本率]</span> </td> 
      <td>
        <p>這是工作角色使用所選[！UICONTROL覆寫貨幣]的每小時成本率。 [!DNL Workfront] 使用此值來計算與工作角色相關之任務和問題的計畫成本與實際成本。 </p> 
        <p><span>以上述指定的[！UICONTROL覆寫貨幣]輸入匯率。 當使用[！UICONTROL基本貨幣]時，這也會更新此職務角色的成本率。</span> </p> 
        <p>如需如何操作的詳細資訊 [!DNL Workfront] 計算成本，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> 
       <p>提示：更新已具有相關成本率的現有職務角色時， [!DNL Workfront] 根據您系統中的轉換率計算[！UICONTROL覆寫貨幣]匯率。 如果您更新[！UICONTROL覆寫貨幣成本費率]，則職務角色的成本費率也會自動更新。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[！UICONTROL覆寫貨幣收費率]</span> </td> 
      <td>
        <p>這是工作角色使用所選[！UICONTROL覆寫貨幣]的每小時收費率。 [!DNL Workfront] 使用此值來計算與工作角色相關之任務和問題的計畫和實際收入。 </p>
        <p><span>以上述指定的[！UICONTROL覆寫貨幣]輸入匯率。 當使用[！UICONTROL基本貨幣]時，這也會更新此職務角色的計費率。</span> </p>
        <p>如需如何操作的詳細資訊 [!DNL Workfront] 計算收入，請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單與收入概要</a>.</p>
        <p>提示：更新已具有相關聯收費率的現有職務角色時， [!DNL Workfront] 根據您系統中的兌換率計算「覆寫幣別」匯率。 如果您更新「覆寫幣別帳單費率」，職務角色的「帳單費率」也會自動更新。 </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >工作角色是管理資源的必要部分。 若要使用資源計畫工具，職務角色需要與其相關的成本與帳單費率。 如需詳細資訊，請參閱 [開始使用資源管理](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. 按一下 **[!UICONTROL 建立工作角色]**. 工作角色現在可指派給任務、問題、核准，或者您可以與其共用版面範本或其他物件。 有關中工作角色的所有使用的資訊 [!DNL Workfront]，請參閱 [工作角色總覽](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). 有關刪除工作角色的資訊，請參閱 [刪除職位角色](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
