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
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# 建立和管理職務角色

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

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
1. 設定下列專案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名稱]</td> 
      <td> <p>指定工作角色的名稱。 這是[!DNL Workfront]中顯示[!UICONTROL Job Role]欄位的所有位置的名稱。 </p> <p>提示：工作角色的名稱最多可包含255個字元。 但是，在[!DNL Workfront]的某些區域中，較長的名稱可能會被截斷。 </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL 說明]</td> 
      <td>輸入角色的描述，以指出其獨特性。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 作用中]</span> </td> 
      <td> 
       <ul> 
        <li> <p>如果您想要角色作用中並且在<b>中的所有位置都可供使用，以便與使用者、工作專案等建立關聯，請選取</b>[!UICONTROL 是][!DNL Workfront]。 </p> </li> 
        <li> <p>如果您想要停用角色且無法指派給使用者、工作專案等，請選取<b>[!UICONTROL 否]</b>。 </p> </li> 
       </ul> <p><span>如需停用工作角色的資訊，請參閱</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">停用工作角色</a>。 </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 基本貨幣]</span> </td> 
      <td> <p><span>這是您的Workfront管理員在[!UICONTROL 設定]區域中設定的[!UICONTROL 基本貨幣]。 如需詳細資訊，請參閱</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>。</p> <p>提示： <span>您無法編輯工作角色層級的[!UICONTROL 基本貨幣]。 此欄位會變暗，以提醒您系統的基本貨幣為何。</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 成本率]</td> 
      <td><p>這是工作角色的每小時成本率。 此值會計算與角色相關之任務與問題的計畫成本與實際成本，以及最終的專案計畫成本與實際成本。 使用[!UICONTROL 基本貨幣]輸入匯率。</p> 
      <p>如需日期有效成本費率，請按一下<strong>[!UICONTROL 新增費率]</strong>。 輸入時段的成本/小時值，並視需要指派[!UICONTROL 開始日期]和[!UICONTROL 結束日期]。 第一個成本費率不會有開始日期，而最後一個成本費率不會有結束日期。</p> <p>部分日期會自動新增。 例如，如果第一個成本費率沒有結束日期，而您新增了開始日期為2023年5月1日的第二個成本費率，則結束日期為2023年4月30日的成本費率會新增至第一個成本費率，這樣就不會有差距。</p> <p>提示：編輯現有工作角色時，您可以選取<strong>依開始日期排序</strong>，在費率清單頂端檢視最近的開始日期。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 收費率] </td> 
      <td><p>這是工作角色的每小時收費率。 此值會計算與角色相關之任務和問題的計畫和實際收入，最終是專案的計畫和實際收入。 使用[!UICONTROL 基本貨幣]輸入匯率。</p> <p>若要取得日期有效收費率，請按一下<strong>[!UICONTROL 新增費率]</strong>。 輸入時段的記帳/小時值，並視需要指派[!UICONTROL 開始日期]和[!UICONTROL 結束日期]。 第一個收費率不會有開始日期，而最後一個收費率則不會有結束日期。</p> <p>部分日期會自動新增。 例如，如果第一個收費率沒有結束日期，而您新增了開始日期為2023年5月1日的第二個收費率，則第一個收費率會新增2023年4月30日的結束日期，因此不會有間隙。</p> <p>提示：編輯現有工作角色時，您可以選取<strong>依開始日期排序</strong>，在費率清單頂端檢視最近的開始日期。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 覆寫貨幣]</span> </td> 
      <td>
        <p>選取與此工作角色關聯的貨幣。 這是[!DNL Workfront]用於計算與此工作角色相關之成本和收入的貨幣。 </p> 
        <p><span>這與[!DNL Workfront]管理員在[!UICONTROL 設定]區域中設定的[!UICONTROL 基本貨幣]不同，也可能與專案相關的貨幣不同。</span> </p> 
        <p>提示：此欄位僅提供您系統中[!UICONTROL Exchange Rates]區域中可用的貨幣。 如果您只設定一種貨幣，則此欄位不會出現。</p> 
       <p><span>如需在[!DNL Workfront]中設定[!UICONTROL 基本貨幣]的相關資訊，請參閱</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>。</p> <p><span>如需有關變更專案貨幣的資訊，請參閱</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">變更專案貨幣</a>。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 覆寫貨幣成本費率]</span> </td> 
      <td>
        <p>這是工作角色使用所選[!UICONTROL 覆寫貨幣]的每小時成本率。 [!DNL Workfront]使用此值來計算與工作角色相關之任務和問題的計畫成本與實際成本。 </p> 
        <p><span>以上述指定的[!UICONTROL Override Currency]輸入匯率。 當使用[!UICONTROL 基本貨幣]時，這也會更新此工作角色的成本率。</span> </p> 
        <p>有關[!DNL Workfront]如何計算成本的資訊，請參閱<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>。</p> 
       <p>提示：更新已有關聯成本費率的現有職務角色時，[!DNL Workfront]會根據您系統中的轉換率計算[!UICONTROL 覆寫貨幣]費率。 如果您更新[!UICONTROL 覆寫貨幣成本費率]，則職務角色的成本費率也會自動更新。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 覆寫貨幣收費率]</span> </td> 
      <td>
        <p>這是工作角色使用所選[!UICONTROL 覆寫貨幣]的每小時收費率。 [!DNL Workfront]使用此值來計算與工作角色相關之任務和問題的計畫和實際收入。 </p>
        <p><span>以上述指定的[!UICONTROL Override Currency]輸入匯率。 當使用[!UICONTROL 基本貨幣]時，這也會更新此工作角色的計費率。</span> </p>
        <p>有關[!DNL Workfront]如何計算收入的資訊，請參閱<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單與收入概觀</a>。</p>
        <p>提示：更新已有關聯收費率的現有職務角色時，[!DNL Workfront]會根據您系統中的轉換率計算覆寫貨幣率。 如果您更新「覆寫幣別帳單費率」，職務角色的「帳單費率」也會自動更新。 </p>
       </td>
     </tr> 
    </tbody> 
   </table>

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
