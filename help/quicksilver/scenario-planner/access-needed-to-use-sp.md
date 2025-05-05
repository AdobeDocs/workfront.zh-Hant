---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 使用「情境規劃工具」所需的存取權
description: Scenario Planner需要Adobe Workfront的單獨授權和額外存取權。
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 7c1bd52c6d1878b556bc92849b5d65fd0e89f51b
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# 使用[!DNL Scenario Planner]所需的存取權

<!--Audited: 04/2024-->

[!DNL Scenario Planner]有額外的授權需求。 如需[!DNL Workfront Scenario Planner]的相關資訊，請參閱[ [!DNL Scenario Planner] 概觀](../scenario-planner/scenario-planner-overview.md)。

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

若沒有正確的存取或許可權，您可能無法檢視[!DNL &#x200B; Adobe Workfront]的[!UICONTROL 案例]區域，也無法管理組織的計畫或方案。 管理計畫和方案包括建立、編輯和刪除它們。

## 需要存取權才能檢視及使用[!DNL Adobe Workfront Scenario Planner]

您必須確定符合下列所有條件，才能存取[!DNL Workfront Scenario Planner]：

1. 您的組織必須擁有下列其中一個Workfront計畫。

   視您使用新計畫或目前Workfront計畫而定，您的組織必須具備下列其中一項：

   * 針對新計畫，您的組織必須有[!UICONTROL Ultimate] [!DNL Workfront]計畫。 此情境規劃工具僅包含在[!UICONTROL Ultimate]計畫中。

   * 對於目前的Workfront計畫，您的組織必須同時具備下列兩個條件：

      * 您的組織必須購買[!DNL Workfront] [!UICONTROL 企業]或更新版本的[!DNL Workfront]計畫。

      * 您的組織除了[!DNL Workfront]授權外，還必須購買[!DNL Workfront Scenario Planner]授權。 請連絡您的[!DNL Workfront]客戶代表以瞭解[!DNL Workfront Scenario Planner]授權。

1. 您必須擁有下列其中一個Workfront授權。

   視您使用新授權或目前授權而定，您的[!DNL Workfront]管理員必須為您指派下列任何型別的授權：

   * 對於新授權：
      * [!UICONTROL 標準]
      * [!UICONTROL 亮]

   * 對於目前的授權：

      * [!UICONTROL 計畫]
      * [!UICONTROL 工作]
      * [!UICONTROL 檢閱]

   >[!NOTE]
   > 
   >* 使用新授權時，具有[!UICONTROL 貢獻者]或[!UICONTROL 外部]授權型別的使用者無法存取[!DNL Scenario Planner]。
   >
   >* 使用目前的授權時，具有「請求」或「外部」授權型別的使用者無法存取Scenario Planner。

1. 您的[!DNL Workfront]管理員必須授與您存取層級中[!DNL Scenario Planner]的[!UICONTROL 檢視]或[!UICONTROL 編輯]存取權。

   如需授與[!DNL Workfront Scenario Planner]存取權的相關資訊，請參閱[授與 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)存取權。

1. （選用且建議使用）若要檢視或更新計畫和方案的財務資訊，您的[!DNL Workfront]管理員也必須授與您存取層級中[!UICONTROL 財務資料]的存取權。 如需在存取層級中授與財務資料的相關資訊，請參閱[授與財務資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

1. （選擇性）如果您需要存取您未建立的計畫，計畫建立者必須授予您計畫正確的許可權，您才能存取計畫。 如需有關存取您未建立的計畫和方案所需的許可權資訊，請參閱本文章中的[存取計畫和方案所需的許可權](#permissions-needed-to-access-plans-and-initiatives)一節。

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## 檢視計畫和方案所需的存取權

除了您的公司取得[!DNL Workfront Scenario Planner]的正確授權外，[!DNL Workfront]管理員還必須指派下列存取權和設定給您，以便您檢視此區域中的[!DNL Workfront Scenario Planner]和資訊：

* 存取層級至少具有[!UICONTROL 檢視]對[!DNL Scenario Planner]的存取權。

  如需[!DNL Scenario Planner]的存取層級相關資訊，請參閱[授與 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)的存取權。

* 存取層級，至少具有[!UICONTROL 檢視]對[!UICONTROL 財務資料]的存取權（若您也需要檢視計畫與方案的財務資訊）。 財務資訊的一些範例為預算、成本或職務角色費率。

  如需[!UICONTROL 財務資料]存取層級的相關資訊，請參閱[授予財務資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

  >[!TIP]
  >
  >[!UICONTROL 要求者]與[!UICONTROL 外部]使用者沒有檢視[!DNL Scenario Planner]的存取權。

* 檢視計畫的許可權。 如需有關存取您未建立的計畫和方案所需的許可權資訊，請參閱本文章中的[存取計畫和方案所需的許可權](#permissions-needed-to-access-plans-and-initiatives)一節。

## 管理計畫和方案所需的存取權

您的[!DNL Workfront]管理員必須指派下列存取權給您，您才能在[!DNL Scenario Planner]中管理計畫及其資訊：

* [!UICONTROL 計畫]或[!UICONTROL 工作]授權型別，具有存取層級[!DNL Scenario Planner]的編輯存取權。

  所有其他授權型別沒有管理計畫的存取權。

  如需有關從存取層級授與[!DNL Scenario Planner]存取權的資訊，請參閱[授與 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)的存取權。

* 若您還需要更新計畫的財務資訊，則在存取層級中具有[!UICONTROL 編輯]存取[!UICONTROL 財務資料]的[!UICONTROL 計畫]授權型別。

  您可以編輯的財務資訊範例包括[!UICONTROL 預算]、[!UICONTROL 計畫收益]和[!UICONTROL 固定成本]。

  >[!TIP]
  >
  >只有[!UICONTROL 計畫]授權持有人有[!UICONTROL 編輯]存取[!UICONTROL 財務資料]的許可權。

  如需[!UICONTROL 財務資料]存取層級的相關資訊，請參閱[授予財務資料的存取權](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

* 管理您未建立之計畫的許可權。 如需有關存取您未建立的計畫和方案所需的許可權資訊，請參閱本文章中的[存取計畫和方案所需的許可權](#permissions-needed-to-access-plans-and-initiatives)一節。

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


