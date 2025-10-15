---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 使用「情境規劃工具」所需的存取權
description: Scenario Planner需要Adobe Workfront的單獨授權和額外存取權。
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 1b06589a705cf218239ff1273b865c05e4ceb96f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 使用[!DNL Scenario Planner]所需的存取權

<!--Audited: 04/2024-->

<!--The [!DNL Scenario Planner] has additional license requirements. For information about the [!DNL Workfront Scenario Planner], see [The [!DNL Scenario Planner] overview](../scenario-planner/scenario-planner-overview.md).-->

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

若沒有正確的存取或許可權，您可能無法檢視[!UICONTROL 的]案例[!DNL &#x200B; Adobe Workfront]區域，也無法管理組織的計畫或方案。 管理計畫和方案包括建立、編輯和刪除它們。

## 需要存取權才能檢視及使用[!DNL Adobe Workfront Scenario Planner]

您必須確定符合下列所有條件，才能存取[!DNL Workfront Scenario Planner]：

1. 貴組織必須有Workfront Ultimate套件。

   Scenario Planner不適用於Workfront Workflow套件。

   如果您目前正在更新Workfront，而且想要保留Scenario Planner，請洽詢Workfront客戶代表。

   如果您是新客戶，Scenario Planner將無法再購買。

   <!--Old: 
    Depending on whether you use the new or the current Workfront plan, your organization must have one of the following:
    * For the new plans, your organization must have the  [!UICONTROL Ultimate] [!DNL Workfront] plan. The Scenario Planner is included only in the [!UICONTROL Ultimate] plan. 
    * For the current Workfront plans, your organization must have both of the following: 
      * Your organization must purchase a [!DNL Workfront] [!UICONTROL Business] or higher [!DNL Workfront] plan. 
      
      * Your organization must purchase a [!DNL Workfront Scenario Planner] license, in addition to a [!DNL Workfront] license. Contact your [!DNL Workfront] Account Representative to learn about [!DNL Workfront Scenario Planner] licenses. -->

1. 您必須具備下列其中一個Workfront授權：

   * [!UICONTROL 輕]或更高
   * [!UICONTROL 檢閱者]或更新版本

   <!--Old: 
      * For the current licenses: 
        * [!UICONTROL Plan]
        * [!UICONTROL Work]
        * [!UICONTROL Review]-->
   <!--Old: 
      >[!NOTE]
      > 
      >* When using the new licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
      >
      >* When using the current licenses, users with a Request or External license type cannot access the Scenario Planner. -->

1. 您的[!DNL Workfront]管理員必須授與您存取層級中[!UICONTROL 的]檢視[!UICONTROL 或]編輯[!DNL Scenario Planner]存取權。

   如需授與[!DNL Workfront Scenario Planner]存取權的相關資訊，請參閱[授與 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)存取權。

1. （選用且建議使用）若要檢視或更新計畫和方案的財務資訊，您的[!DNL Workfront]管理員也必須授與您存取層級中[!UICONTROL 財務資料]的存取權。 如需在存取層級中授與財務資料的相關資訊，請參閱[授與財務資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。


<!--1. (Optional) If you need to access plans you didn't create, a plan creator must give you the correct permissions to their plan to access it. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.-->

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

<!--Repetitive from above?? 

## Access needed to view plans and initiatives

In addition to your company acquiring the correct license for the [!DNL Workfront Scenario Planner], your [!DNL Workfront] administrator must also assign you the following access and setup so you can view the [!DNL Workfront Scenario Planner] and the information in this area:

* An access level with at least [!UICONTROL View] access to [!DNL Scenario Planner].

  For information about the access level to [!DNL Scenario Planner], see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* An access level with at least [!UICONTROL View] access to [!UICONTROL Financial Data] if you need to also view financial information about the plan and the initiatives. Some examples of financial information are budgets, costs, or job role rates.

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Requestors] and [!UICONTROL External] Users do not have access to view the [!DNL Scenario Planner].

* View permissions to the plan. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

## Access needed to manage plans and initiatives

Your [!DNL Workfront] administrator must assign you the following access so you can manage plans and their information in the [!DNL Scenario Planner]:

* A [!UICONTROL Plan] or [!UICONTROL Work] license type with Edit access to the [!DNL Scenario Planner] in your access level.

  All other license types do not have access to manage plans.

  For information about granting access to [!DNL Scenario Planner] from the Access Level, see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plan] license type with [!UICONTROL Edit] access to [!UICONTROL Financial Data] in your access level, if you need to also update financial information about the plan.

  Some examples of financial information that you can edit are [!UICONTROL Budget], [!UICONTROL Planned Benefit], and [!UICONTROL Fixed Costs].

  >[!TIP]
  >
  >Only [!UICONTROL Plan] license holders have [!UICONTROL Edit] access to [!UICONTROL Financial Data].

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Manage permissions to a plan that you didn't create. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

-->

## 存取計畫和方案所需的許可權

存取層級與[!DNL Workfront]中的許可權搭配使用，可讓您檢視未建立的計畫和方案。 除了擁有存取[!DNL Scenario Planner]的正確存取層級之外，如果您不是計畫的建立者，您還必須擁有您要檢視或管理的計畫的正確許可權。

所有使用者（包括系統管理員）都只能存取他們建立的計畫。

若要檢視其他使用者建立的計畫，他們必須透過下列方式與您共用其計畫：

* 與您共用計畫

  如需共用計畫的詳細資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md)中共用計畫。

* 傳送其所建立計畫的連結

  如果使用者在不共用計畫的情況下共用計畫的連結，您可以要求計畫的許可權。 如需有關向計畫要求許可權的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md)中要求計畫的存取權。

>[!NOTE]
>
>停用使用者時，其計畫沒有擁有者，除非先前與連結共用，否則無法存取。


