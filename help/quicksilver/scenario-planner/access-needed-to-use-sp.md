---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 使用方案計畫員所需的訪問權限
description: 方案規劃器需要與Adobe Workfront單獨的許可證和附加訪問。
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# 使用 [!DNL Scenario Planner]

此 [!DNL Scenario Planner] 需要額外的授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 [此 [!DNL Scenario Planner] 概述](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

若沒有正確的存取權或權限，您可能無法檢視 [!UICONTROL 藍本] 區域[!DNL  Adobe Workfront] 也無法管理貴組織的計畫或計畫。 管理計畫和方案包括建立、編輯和刪除計畫和方案。

>[!IMPORTANT]
>
>存取 [!UICONTROL 藍本]，則您只能檢視和管理您建立的計畫。 如果要允許其他用戶查看或管理您建立的計畫，必須執行以下操作：
>
>* 將連結傳送給其他使用者
>* 與其他使用者共用計畫
>
>  如需共用計畫的相關資訊，請參閱 [在 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>停用使用者時，其計畫沒有擁有者，除非先前已與連結共用，否則無法存取。

## 檢視和使用 [!DNL Adobe Workfront Scenario Planner]

您必須先確定符合下列所有條件，才能存取 [!DNL Workfront Scenario Planner]:

<!--drafted for P&P:

* Depending on whether you use the current or the legacy Workfront plans, your organization must have the following:

  * For the current plans:  

    * The [!UICONTROL Ultimate] [!DNL Workfront] plan.

      Or
  
    * The [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] plan, in addition to purchasing a separate [!DNL Scenario Planner] license.

  * For the legacy plans: (indent the bullets below, before the NOTE)

-->

* 貴組織必須購買 [!DNL Workfront] [!UICONTROL 企業] 或更高 [!DNL Workfront] 計畫。 如需 [!DNL Workfront] 計畫，請參閱 [Workfront計畫](http://workfront.com/plans).
* 貴組織必須購買 [!DNL Workfront Scenario Planner] 除 [!DNL Workfront] 授權。 請連絡您的 [!DNL Workfront] 客戶代表以了解 [!DNL Workfront Scenario Planner] 授權。

<!--drafted for P&P: 

* Depending on whether you use the current or legacy licenses, your [!DNL Workfront] administrator must assign you a license of any of the following types: 

  * For the current licenses: 
    * [!UICONTROL Standard]
    * [!UICONTROL Light]

  * For the legacy licenses: (re-indent the licenses below and reword the sentence)

-->



* 您的 [!DNL Workfront] 管理員必須為您分配以下任何許可 [!DNL Workfront] 類型：

   * [!UICONTROL 計劃]
   * [!UICONTROL 工作]
   * [!UICONTROL 檢閱]

   >[!NOTE]
   >
   >具有 [!UICONTROL 要求] 或 [!UICONTROL 外部] 許可證類型無法訪問 [!DNL Workfront Scenario Planner].

<!--drafted - replace the note above with this at P&P release: 
  * When using the current licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
  * When using the legacy licenses, users with a Request or External license type cannot access the Scenario Planner. -->

* 您的 [!DNL Workfront] 管理員必須 [!UICONTROL 檢視] 或 [!UICONTROL 編輯] 存取 [!DNL Scenario Planner] 在您的存取層級。

   有關授予 [!DNL Workfront Scenario Planner]，請參閱 [授予的存取權 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* （可選和建議）要查看或更新計畫和計畫的財務資訊，請 [!DNL Workfront] 管理員還必須授予您訪問權限 [!UICONTROL 財務資料] 在您的存取層級。 有關在訪問級別授予財務資料的資訊，請參見 [授予金融資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   <!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

* 如果您需要訪問您未建立的計畫，計畫建立者必須為您授予其計畫訪問計畫的正確權限。 如需存取您未建立的計畫和計畫所需權限的相關資訊，請參閱 [存取計畫和計畫所需的權限](#permissions-needed-to-access-plans-and-initiatives) 一節。

## 查看計畫和計畫所需的訪問權

除了貴公司取得 [!DNL Workfront Scenario Planner]，您的 [!DNL Workfront] 管理員還必須為您分配以下訪問權限和設定，以便您可以查看 [!DNL Workfront Scenario Planner] 以及這方面的資訊：

* 至少具有 [!UICONTROL 檢視] 存取 [!DNL Scenario Planner].

   如需以下項目的存取層級相關資訊： [!DNL Scenario Planner]，請參閱 [授予的存取權 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* 至少具有 [!UICONTROL 檢視] 存取 [!UICONTROL 財務資料] 如果您還需要查看有關計畫和計畫的財務資訊。 財務資訊的一些示例是預算、成本或職務職責費率。

   如需 [!UICONTROL 財務資料] 存取層級，請參閱 [授予金融資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   >[!TIP]
   >
   >[!UICONTROL 請求者] 和 [!UICONTROL 外部] 使用者無權檢視 [!DNL Scenario Planner].

* 檢視計畫的權限。 如需存取您未建立的計畫和計畫所需權限的相關資訊，請參閱 [存取計畫和計畫所需的權限](#permissions-needed-to-access-plans-and-initiatives) 一節。

## 管理計畫和計畫所需的訪問

您的 [!DNL Workfront] 管理員必須指派下列存取權，才能在 [!DNL Scenario Planner]:

* A [!UICONTROL 計畫] 或 [!UICONTROL 工作] 許可類型，可編輯 [!DNL Scenario Planner] 在您的存取層級。

   所有其他許可證類型都無權管理計畫。

   有關授予 [!DNL Scenario Planner] 從存取層級，請參閱 [授予的存取權 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL 計畫] 許可證類型 [!UICONTROL 編輯] 存取 [!UICONTROL 財務資料] 在您的訪問級別中，如果您還需要更新有關計畫的財務資訊。

   您可以編輯的財務資訊的一些範例包括 [!UICONTROL 預算], [!UICONTROL 計畫福利]，和 [!UICONTROL 固定成本].

   >[!TIP]
   >
   >僅 [!UICONTROL 計畫] 授權擁有者 [!UICONTROL 編輯] 存取 [!UICONTROL 財務資料].

   如需 [!UICONTROL 財務資料] 存取層級，請參閱 [授予金融資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* 管理您未建立之計畫的權限。 如需存取您未建立的計畫和計畫所需權限的相關資訊，請參閱 [存取計畫和計畫所需的權限](#permissions-needed-to-access-plans-and-initiatives) 一節。

## 存取計畫和計畫所需的權限

存取層級可與 [!DNL Workfront] 讓您了解您未建立的計畫和計畫。 除了具有正確的訪問級別以訪問 [!DNL Scenario Planner]，如果您不是這些計畫的建立者，您也必須擁有您要檢視或管理的計畫的正確權限。

依預設，您只能存取您建立的計畫。 要查看其他用戶建立的計畫，他們必須與您共用其計畫。 如需共用計畫的相關資訊，請參閱 [在 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

如果使用者共用計畫的連結而不共用計畫，您可以請求計畫的權限。 如需請求計畫權限的相關資訊，請參閱 [在 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

