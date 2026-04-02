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
source-git-commit: 3fe3313bd545d51be7aa0fb021dd0bb0f91b4321
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 1%

---

# 建立和管理職務角色

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

{{highlighted-preview}}

>[!IMPORTANT]
>
>在25.11版本中，工作角色的覆寫貨幣在生產環境中已過時。 （10月30日在預覽環境中棄用。） 工作角色現在可以使用一種貨幣，而不是使用基本貨幣和覆寫貨幣，而且成本和計費率會使用該貨幣來定義。

作為[!DNL Adobe Workfront]管理員或具有工作角色管理存取權的使用者，您可以建立可指派給使用者的工作角色，並刪除與您的組織無關的預設工作角色。 如需[!DNL Workfront]中管理存取權的相關資訊，請參閱[授予使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

>[!TIP]
>
>工作角色是管理資源的必要部分。 若要使用資源計畫工具，職務角色需要與其相關的成本與帳單費率。 如需詳細資訊，請參閱[開始使用資源管理](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>若要建立或編輯工作角色：任何Workfront或Workflow套件</p>
   <p>若要套用費率屬性並將自訂表單新增至工作角色：工作流程Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[！UICONTROL標準]</p>
       <p>[！UICONTROL計畫]</p></td>
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

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 工作角色]**。
1. 按一下&#x200B;**[!UICONTROL 新增工作角色]**。
<!-- 1. Click **New Job Role > Create new job role**.  -->
1. 在下列欄位中輸入資訊：

   * **名稱**：表示工作角色的名稱。 這是Workfront中顯示「工作角色」欄位的所有位置的名稱。

     >[!TIP]
     >
     >工作角色的名稱最多可包含255個字元。 不過，在Workfront的某些區域，較長的名稱可能會被截斷。

   * **描述**：輸入角色的描述，以指出其獨特性。
   * **為作用中**：如果您想要該角色為作用中，並且可在Workfront中的任何地方與使用者、工作專案等建立關聯，請選取&#x200B;**是**。 如果您想要停用該角色，且不將其指派給使用者、工作專案等，請選取&#x200B;**否**。

     如需有關停用工作角色的資訊，請參閱[停用工作角色](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)。

   * **Currency**：預設會顯示基本貨幣。 Workfront管理員會在「設定」區域中新增基本貨幣。 您可以將選取專案變更為其他可用貨幣，也可以變更有效日期時間範圍內的貨幣。

     >[!TIP]
     >
     >此欄位僅提供您系統中「匯率」區域中可用的貨幣。 如果您只設定一種貨幣，則只能使用該貨幣。

     如需有關在Workfront中設定基本貨幣的資訊，請參閱[設定匯率](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

     如需有關變更專案貨幣的資訊，請參閱[變更專案貨幣](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md)。

   * **成本費率**：這是工作角色的每小時成本費率。 此值會計算與角色相關之任務與問題的計畫成本與實際成本，以及最終的專案計畫成本與實際成本。 使用選取的幣別輸入匯率。

     若要取得日期有效成本費率，請按一下[新增費率]。**** 輸入時間期間的成本/小時值，並視需要指定「開始日期」與「結束日期」。 第一個成本費率不會有開始日期，而最後一個成本費率不會有結束日期。

     部分日期會自動新增。 例如，如果第一個成本費率沒有結束日期，而您新增了開始日期為2025年5月1日的第二個成本費率，則結束日期為2025年4月30日的成本費率會新增至第一個成本費率，這樣就不會有差距。

     如需Workfront如何計算成本的詳細資訊，請參閱[追蹤成本](/help/quicksilver/manage-work/projects/project-finances/track-costs.md)。

     >[!TIP]
     >
     >編輯現有工作角色時，您可以排序清單，以在費率清單頂端檢視最近的開始日期。

   * **收費率**：這是工作角色的每小時收費率。 此值會計算與角色相關之任務和問題的計畫和實際收入，最終是專案的計畫和實際收入。 使用選取的幣別輸入匯率。

     若要取得日期有效收費率，請按一下[新增費率]。**** 輸入時間期間的帳單/小時值，並視需要指定「開始日期」與「結束日期」。 第一個收費率不會有開始日期，而最後一個收費率則不會有結束日期。

     部分日期會自動新增。 例如，如果第一個收費率沒有結束日期，而您新增了開始日期為2025年5月1日的第二個收費率，則第一個收費率會新增2025年4月30日的結束日期，因此不會有間隙。

     如需Workfront如何計算收入的詳細資訊，請參閱[帳單與收入概觀](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)。

     >[!TIP]
     >
     >編輯現有工作角色時，您可以排序清單，以在費率清單頂端檢視最近的開始日期。

<!-- Remove or hide the billing rate and cost rate bullets on April 16 for GA -->

1. 按一下&#x200B;**[!UICONTROL 建立工作角色]**。 工作角色現在可指派給任務、問題、核准，或者您可以與其共用版面範本或其他物件。 如需[!DNL Workfront]中所有工作角色使用的相關資訊，請參閱[工作角色總覽](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)。 如需有關刪除工作角色的資訊，請參閱[刪除工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md)。

<div class="preview">

## 將費率和屬性新增至工作角色

在財務計算中使用工作角色的計費和成本費率。

在費率存在的Workfront區域中（例如工作角色和使用者），可支援費率屬性。 將屬性套用至職務角色時，其指定會自動解析為正確的費率。

如需詳細資訊，請參閱[定義費率屬性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 工作角色]**。
1. 按一下現有工作角色的名稱以進行編輯。
1. 若要更新工作角色詳細資料，請按一下左側面板中的&#x200B;**詳細資料**。
1. （選擇性）若要將自訂表單附加到工作角色，請按一下[詳細資訊]頁面右上角的&#x200B;**新增自訂表單**&#x200B;欄位，然後從顯示的清單中選取自訂表單。

   如需附加自訂表單的詳細資訊，請參閱[新增自訂表單至物件](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

1. 按一下左側面板中的&#x200B;[!UICONTROL **費率**]。
1. 按一下&#x200B;[!UICONTROL **帳單**]&#x200B;或&#x200B;[!UICONTROL **成本**]&#x200B;以選取費率型別。
1. 按一下&#x200B;[!UICONTROL **新增費率**]&#x200B;以新增費率。

   或

   選取現有的速率，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)以更新它。

   >[!NOTE]
   >
   >因為每個費率都與角色和屬性的組合相關聯，以建立唯一費率，所以當您編輯費率時，無法變更屬性。

1. 在&#x200B;**新費率**&#x200B;方塊中，選取費率屬性，例如「代理商」、「地點」或「成本中心」。

   >[!NOTE]
   >
   >這些屬性會個別定義，可能會影響收入和成本的計算。 如需詳細資訊，請參閱[定義費率屬性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)。

1. 選取匯率的&#x200B;**貨幣**。 Workfront管理員會在「設定」區域中新增基本貨幣。 您可以將選取專案變更為其他可用貨幣，也可以變更有效日期時間範圍內的貨幣。

   >[!TIP]
   >
   >此欄位僅提供您系統中「匯率」區域中可用的貨幣。 如果您只設定一種貨幣，則只能使用該貨幣。

   如需有關在Workfront中設定基本貨幣的資訊，請參閱[設定匯率](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

   如需有關變更專案貨幣的資訊，請參閱[變更專案貨幣](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md)。

1. （視條件而定）若要取得帳單費率，請輸入此工作角色的&#x200B;**帳單費率**。

   這是工作角色的每小時收費率。 此值會計算與角色相關之任務和問題的計畫和實際收入，最終是專案的計畫和實際收入。 使用選取的幣別輸入匯率。

   如果您使用屬性，則屬性和職務角色會結合以定義唯一費率。 例如，代理商A在紐約的Designer角色與代理商B在巴黎的Designer角色可能有不同的費率。

   若要取得日期有效收費率，請按一下[新增費率]。**** 輸入時間期間的帳單/小時值，並視需要指定「開始日期」與「結束日期」。 第一個收費率不會有開始日期，而最後一個收費率則不會有結束日期。

   部分日期會自動新增。 例如，如果第一個收費率沒有結束日期，而您新增了開始日期為5月1日的第二個收費率，則結束日期為4月30日會新增至第一個收費率，因此不會有間隙。

   如需Workfront如何計算收入的詳細資訊，請參閱[帳單與收入概觀](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)。

   >[!TIP]
   >
   >編輯現有工作角色時，您可以排序清單，以在費率清單頂端檢視最近的開始日期。

1. （視條件而定）若要取得成本費率，請輸入此職務角色的&#x200B;**成本費率**。

   這是工作角色的每小時成本率。 此值會計算與角色相關之任務與問題的計畫成本與實際成本，以及最終的專案計畫成本與實際成本。 使用選取的幣別輸入匯率。

   如果您使用屬性，則屬性和職務角色會結合以定義唯一費率。 例如，代理商A在紐約的Designer角色與代理商B在巴黎的Designer角色可能有不同的費率。

   若要取得日期有效成本費率，請按一下[新增費率]。**** 輸入時間期間的成本/小時值，並視需要指定「開始日期」與「結束日期」。 第一個成本費率不會有開始日期，而最後一個成本費率不會有結束日期。

   部分日期會自動新增。 例如，如果第一個成本費率沒有結束日期，而您新增了開始日期為5月1日的第二個成本費率，則結束日期為4月30日會新增至第一個成本費率，這樣就不會有差距。

   如需Workfront如何計算成本的詳細資訊，請參閱[追蹤成本](/help/quicksilver/manage-work/projects/project-finances/track-costs.md)。

   >[!TIP]
   >
   >編輯現有工作角色時，您可以排序清單，以在費率清單頂端檢視最近的開始日期。

1. 按一下「[!UICONTROL **儲存**]」。

</div>

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.

-->



