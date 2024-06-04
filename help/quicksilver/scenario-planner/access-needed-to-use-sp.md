---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 使用「情境規劃工具」所需的存取權
description: Scenario Planner需要Adobe Workfront的單獨授權和額外存取權。
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: f0f6c2bee98c6cebf8ea9e18bf34262f3c1d6e3a
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# 使用所需的存取權 [!DNL Scenario Planner]

此 [!DNL Scenario Planner] 需要額外的授權。 如需關於的資訊， [!DNL Workfront Scenario Planner]，請參閱 [此 [!DNL Scenario Planner] 概述](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

沒有正確的存取權或許可權，您可能無法檢視 [!UICONTROL 情境] 區域[!DNL  Adobe Workfront] 也不會管理組織的計畫或方案。 管理計畫和方案包括建立、編輯和刪除它們。

>[!IMPORTANT]
>
>存取時 [!UICONTROL 情境]，您只能檢視及管理您建立的計畫。 如果要允許其他使用者檢視或管理您建立的計畫，您必須執行下列動作：
>
>* 傳送您計畫的連結給其他使用者
>* 與其他使用者共用計畫
>
>  如需共用計畫的詳細資訊，請參閱 [在中共用計畫 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>停用使用者時，其計畫沒有擁有者，除非先前與連結共用，否則無法存取。

## 檢視和使用 [!DNL Adobe Workfront Scenario Planner]

您必須確定符合下列所有條件，才能存取 [!DNL Workfront Scenario Planner]：

1. 您的組織必須擁有下列其中一個Workfront計畫。

   視您使用新計畫或目前Workfront計畫而定，您的組織必須具備下列其中一項：

   * 對於新計畫，您的組織必須具備下列其中一項：

      * 此 [!UICONTROL Ultimate] [!DNL Workfront] 計畫。 「情境規劃工具」包含在「最終計畫」中。

        或

      * 此 [!UICONTROL 選取] 或 [!UICONTROL Prime] [!DNL Workfront] 計畫，除了另外購買 [!DNL Scenario Planner] 授權。

   * 針對目前的Workfront計畫，您的組織必須具備下列兩個條件：

      * 貴組織必須購買 [!DNL Workfront] [!UICONTROL 企業] 或更高 [!DNL Workfront] 計畫。 如需關於的資訊， [!DNL Workfront] 計畫，請參閱 [Workfront計畫](https://workfront.com/plans).

      * 貴組織必須購買 [!DNL Workfront Scenario Planner] 除了授權之外， [!DNL Workfront] 授權。 連絡您的 [!DNL Workfront] 要瞭解的帳戶代表 [!DNL Workfront Scenario Planner] 授權。

1. 您必須擁有下列其中一個Workfront授權。

   視您使用新授權或目前授權而定，您的 [!DNL Workfront] 管理員必須指派下列任何型別的授權給您：

   * 對於新授權：
      * [!UICONTROL 標準]
      * [!UICONTROL 淺色]

   * 對於目前的授權：

      * [!UICONTROL 計畫]
      * [!UICONTROL 工作]
      * [!UICONTROL 檢閱]

   >[!NOTE]
   > 
   >* 使用新授權時，使用者具有 [!UICONTROL 投稿人] 或 [!UICONTROL 外部] 授權型別無法存取 [!DNL Scenario Planner].
   >
   >* 使用目前的授權時，具有「請求」或「外部」授權型別的使用者無法存取Scenario Planner。

1. 您的 [!DNL Workfront] 管理員必須提供您 [!UICONTROL 檢視] 或 [!UICONTROL 編輯] 存取目標 [!DNL Scenario Planner] 在存取層級中。

   如需有關授與存取權的資訊， [!DNL Workfront Scenario Planner]，請參閱 [授予存取許可權 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. （選用且建議使用）若要檢視或更新計畫與方案的財務資訊，請 [!DNL Workfront] 管理員也必須授予您存取許可權 [!UICONTROL 財務資料] 在存取層級中。 如需在存取層級中授與財務資料的相關資訊，請參閱 [授予財務資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

1. （選擇性）如果您需要存取您未建立的計畫，計畫建立者必須授予您計畫正確的許可權，您才能存取計畫。 如需有關存取您未建立之計畫和方案所需的許可權資訊，請參閱 [存取計畫和方案所需的許可權](#permissions-needed-to-access-plans-and-initiatives) 一節。

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## 檢視計畫和方案所需的存取權

除了貴公司取得「 」的正確授權外， [!DNL Workfront Scenario Planner]，您的 [!DNL Workfront] 管理員還必須為您指派以下存取權和設定，以便您檢視 [!DNL Workfront Scenario Planner] 以及此區域中的資訊：

* 存取層級，至少包括 [!UICONTROL 檢視] 存取目標 [!DNL Scenario Planner].

  如需的存取層級相關資訊， [!DNL Scenario Planner]，請參閱 [授予存取許可權 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* 存取層級，至少包括 [!UICONTROL 檢視] 存取目標 [!UICONTROL 財務資料] 如果您也需要檢視有關計畫和方案的財務資訊。 財務資訊的一些範例為預算、成本或職務角色費率。

  如需關於的資訊， [!UICONTROL 財務資料] 存取層級，請參閱 [授予財務資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL 請求者] 和 [!UICONTROL 外部] 使用者無權檢視 [!DNL Scenario Planner].

* 檢視計畫的許可權。 如需有關存取您未建立之計畫和方案所需的許可權資訊，請參閱 [存取計畫和方案所需的許可權](#permissions-needed-to-access-plans-and-initiatives) 一節。

## 管理計畫和方案所需的存取權

您的 [!DNL Workfront] 管理員必須為您指派下列存取權，以便您能夠在 [!DNL Scenario Planner]：

* A [!UICONTROL 計畫] 或 [!UICONTROL 工作] 授權型別，具有的編輯存取權 [!DNL Scenario Planner] 在存取層級中。

  所有其他授權型別沒有管理計畫的存取權。

  如需授與存取權的相關資訊， [!DNL Scenario Planner] 從「存取層級」，請參閱 [授予存取許可權 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL 計畫] 授權型別，具有 [!UICONTROL 編輯] 存取目標 [!UICONTROL 財務資料] 若您還需要更新計畫的財務資訊，請使用存取層級。

  您可以編輯的財務資訊範例包括 [!UICONTROL 預算]， [!UICONTROL 計畫收益]、和 [!UICONTROL 固定成本].

  >[!TIP]
  >
  >僅限 [!UICONTROL 計畫] 授權持有者擁有 [!UICONTROL 編輯] 存取目標 [!UICONTROL 財務資料].

  如需關於的資訊， [!UICONTROL 財務資料] 存取層級，請參閱 [授予財務資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* 管理您未建立之計畫的許可權。 如需有關存取您未建立之計畫和方案所需的許可權資訊，請參閱 [存取計畫和方案所需的許可權](#permissions-needed-to-access-plans-and-initiatives) 一節。

## 存取計畫和方案所需的許可權

存取層級與中的許可權搭配使用 [!DNL Workfront] 可讓您檢視您未建立的計畫和方案。 除了具有正確的存取層級以存取 [!DNL Scenario Planner]，您也必須擁有想要檢視或管理之計畫的正確許可權（如果您不是這些計畫的建立者）。

依預設，您只能存取您建立的計畫。 若要檢視其他使用者建立的計畫，他們必須與您共用他們的計畫。 如需共用計畫的詳細資訊，請參閱 [在中共用計畫 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

如果使用者在不共用計畫的情況下共用計畫的連結，您可以要求計畫的許可權。 如需有關向計畫要求許可權的資訊，請參閱 [請求對中的計畫的存取權 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

