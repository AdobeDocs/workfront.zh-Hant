---
title: Workspaces概述
description: 工作區是團隊使用的記錄型別集合，代表團隊的工作生命週期。 您可以在Adobe Workfront Planning中完全自訂工作區，以符合組織單位的工作流程。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
source-git-commit: 4692dc6f7ab840bb43f3788126471425e9f8a396
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 工作區概觀

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

工作區是組織單位使用的記錄型別集合，代表單位的工作生命週期與處理。 您可以在Adobe Workfront Planning中完全自訂工作區。

<!--update screenshot with preview-->

![工作區登陸頁面管理帳戶](assets/workspaces-landing-page-admin-account.png)

## 關於工作區的考量事項

* 您可以為組織內的特定組織單位建立工作區，以符合每個單位的獨特運作方式。
* Workfront Planning未隨附任何預先設定的工作區。 您必須根據組織的需求來建立這些範本。
* 您可以使用下列方式建立工作區：

   * 從頭開始
   * 使用範本。 範本包含預先設定的記錄型別數及其欄位。
   * 使用AI支援的Planning Designer。 此功能目前在Beta中。
   * 使用多工作區範本套裝。

  如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

* 工作區是組織單位（團隊、群組、部門或部門）進行工作的架構。 欄位無法建立關聯。 只有工作區中的記錄型別可以與欄位相關聯。

  如需詳細資訊，請參閱[記錄型別概觀](/help/quicksilver/planning/architecture/overview-of-record-types.md)。
* 根據您的Workfront授權，工作區會顯示在Planning區域的下列標籤中：

   * 對於系統管理員，工作區會顯示在下列標籤中：

      * **我所在的工作區**：顯示您建立的工作區或與您共用的工作區。
      * **其他工作區**：顯示系統中的所有其他工作區。

     <!--
      * <span class="preview">**Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.</span> (************TEST THIS WITH SYSTEM ADMINS AND STANDARD USERS**********)
      -->

   * 對於所有其他使用者，他們建立的工作區以及其他使用者共用的工作區會顯示在「工作區」區域中。

  <!--

    ******************* If Standard users can see the Sample workspaces, then replace the last bullet with this: 

   * For all other users:

        * (****************what is the name of this tab????*******) Workspaces they created and workspaces others shared with them display in the Workspaces area. 
        * <span class="preview">**Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.</span>
    
    -->

  <!--      
    >[!NOTE]
    >
    ><span class="preview">We recommend to not edit the sample workspaces, but instead to use them as a reference to create your own. Use the multi-workspace template bundle to create workspaces identical to the ones listed in the Sample workspaces tab. For information, see the section "Create multiple workspaces using a best-practice multi-workspace template bundle" in the article [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md). </span> 
    -->

* 工作區包含的記錄型別應反映工作生命週期和組織單位的概念。

  例如，如果單位的工作物件為行銷活動、產品和區域，則該單位的工作區應包含行銷活動、產品和區域的記錄型別。
* 當您建立工作區時，只有您才有權存取和管理您的工作區。 您必須與其他使用者共用，他們才能在相同空間中與您共同作業。

  如需詳細資訊，請參閱[共用工作區](/help/quicksilver/planning/access/share-workspaces.md)。

  系統管理員可以管理所有工作區，即使是他們未建立的工作區。

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* 您可以在Workfront Planning例項中建立的工作區物件數目有所限制。 如需詳細資訊，請參閱[Adobe Workfront Planning物件限制總覽](/help/quicksilver/planning/general/limitations-overview.md)。
