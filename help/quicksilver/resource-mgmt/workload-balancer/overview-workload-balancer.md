---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: 工作負載平衡器總覽
description: 在專案經理透過建立任務來計畫專案工作之後，以及資源經理將工作角色資源配置給資源規劃工具中的專案之後，專案所有者和專案團隊經理可以使用工作負載平衡器將工作專案指派給使用者。
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1194'
ht-degree: 1%

---

# 工作負載平衡器概觀 {#workload-balancer-overview}

>[!CONTEXTUALHELP]
>id="wf-resourcing-workload-balancer"
>title="工作負載平衡器"
>abstract="專案擁有者和團隊經理可以使用工作負載平衡器將工作項目指派給使用者。"

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

在專案經理透過建立任務來計畫專案工作之後，以及資源經理將工作角色資源配置給資源規劃工具中的專案之後，專案所有者和專案團隊經理可以使用工作負載平衡器將工作專案指派給使用者。

>[!IMPORTANT]
>
>您可以使用工作負載平衡器將實際工作（任務和問題）指派給使用者。
>
>您必須使用資源規劃工具，而不是工作負載平衡器，以高層級評估您專案的工作角色分配。 如需資源規劃工具的詳細資訊，請參閱[資源規劃工具概觀](../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

本文說明工作負載平衡器的一般用途，以及如何設定您的專案和資源以成功使用它的一些最佳實務。

若要檢閱工作負載平衡器的影片教學課程，請前往[Workfront教學課程](https://experienceleague.adobe.com/zh-hant/docs/workfront-learn/tutorials-workfront/home)頁面。 在左側功能表中，選取&#x200B;**管理資源** > **工作負載平衡器**，然後選擇教學課程。

## 找到工作負載平衡器

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

我們建議在以下區域使用工作負載平衡器來排程資源：

* 在系統層級的「資源」區域中。
* 在專案層級，在工作負載平衡器區段。
* 在團隊層級，在團隊的工作負載平衡器區段。

如需尋找工作負載平衡器的詳細資訊，請參閱[尋找工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。

## 工作負載平衡器的優點

使用工作負載平衡器時請考慮以下優點：

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* 存取資源過度配置和利用不足的清晰視覺化對應，這對所有利害關係人都透明。
* 身為人員經理，您可以保護您的人員免於倦怠，並賦予他們更好的專注、品質和參與度來完成最佳工作。 您可以確保充分發揮其使用率、打破獨立單位，並啟用跨團隊的工作協調一致。
* 當您在任務或問題層級指派工作時，您不會看到使用者可能有多忙。 使用工作負載平衡器時，您可以檢視哪些使用者在其工作負荷中有可用性，以準時完成任務或問題。 這包括他們的休假和排程例外詳細資料。

  如需詳細資訊，請參閱[在工作負載平衡器](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)中指派工作的總覽。

  您也可以大量指派工作專案，如此將能更輕鬆地一次在多個專案中分配多個工作專案。 如需詳細資訊，請參閱[使用工作負載平衡器](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md)大量指派工作。

* 高階主管可以透過透明度來決定組織內部人員使用方式，進而及時決定人員配置。
* 團隊成員受益於更好的共同作業，因為他們可以在任何指定時間檢視同事正在工作的內容。 如需有關在工作負載平衡器中檢視或管理資源所需存取權的資訊，請參閱[在工作負載平衡器中管理資源所需的存取權](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md)。
* 將連結嵌入自訂標籤中，與主要功能表中沒有資源的人共用。 如需詳細資訊，請參閱[使用連結](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)共用工作負載平衡器。
* 視您的角色而定，在全球、專案或團隊層級的單一檢視中，以視覺化方式呈現和管理人員的工作負荷和需求。 在管理專案時，這不僅包括專案的資源配置，還包括從Adobe Workfront案例規劃工具視覺化資源配置。 人員經理使用Workfront情境規劃工具來管理整個組織的工作技能。 「情境規劃工具」僅適用於新的Adobe Workfront體驗。

  >[!NOTE]
  >
  >  Scenario Planner需要額外的授權。 如需Workfront Scenario Planner的相關資訊，請參閱[Scenario Planner概觀](../../scenario-planner/scenario-planner-overview.md)。


## 使用工作負載平衡器的最佳實務

我們建議在使用工作負載平衡器開始排程您的資源之前，使用下列最佳實務來計畫專案、設定使用者和使用篩選器。

* [在工作負載平衡器](#best-practices-for-displaying-information-in-the-workload-balancer)中顯示資訊的最佳實務
* [設定使用者的最佳實務](#best-practices-for-setting-up-users)
* [設定任務和問題的最佳實務](#best-practices-for-setting-up-tasks-and-issues)

### 在工作負載平衡器顯示資訊的最佳做法 {#best-practices-for-displaying-information-in-the-workload-balancer}

建議您使用篩選器，以便只顯示與您相關的未指派和已指派工作專案資訊。

如需有關在工作負載平衡器中建立和使用篩選器的資訊，請參閱工作負載平衡器中[篩選資訊](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)。

### 設定使用者的最佳實務

* 作為為他人排程工作的使用者，您必須擁有正確的存取權和許可權來排程工作的資源。

  如需有關在工作負載平衡器中管理資源的工作負載所需的存取資訊，請參閱[在工作負載平衡器中管理資源所需的存取許可權](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md)。

* 您要管理其工作負載的使用者必須符合下列條件，以便有關其使用狀態和技能的資訊是準確的：

   * 擁有與其設定檔相關聯的排程和工作角色。

     如需將排程和工作角色與使用者產生關聯的詳細資訊，請參閱[新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * 若使用者未與排程建立關聯，為了進行資源管理，您的Workfront系統的「預設排程」預設會與使用者建立關聯。
   * 在其排程中更新「排程例外」。

     如需建立排程的詳細資訊，請參閱[建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * 在設定檔中更新其休假行事曆。

     如需有關更新使用者休假行事曆的資訊，請參閱[設定個人休假](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md)。

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* Workfront管理員必須決定Workfront計算使用者可用性的方式。 他們可以決定Workfront是否使用系統預設排程，或使用者的排程，透過調整Workfront設定區域中的資源管理偏好設定來計算使用者可使用的時間。

  如需詳細資訊，請參閱[設定資源管理喜好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

### 設定任務和問題的最佳實務 {#best-practices-for-setting-up-tasks-and-issues}

開始將工作指派給工作負載平衡器中的使用者之前，請確定以下任務和問題設定存在：

* 父系任務未指派給使用者或角色。 父系任務未顯示在工作負載平衡器中。
* 任務和問題的計畫時數值大於零。

* 任務和問題的持續時間值大於零。
* 問題的計畫日期在專案的時間表內。

## 開始使用工作負載平衡器之前

* 開始使用工作負載平衡器之前請檢閱下列文章：

   * 本文會逐步說明如何導覽工作負載平衡器以執行這些動作： [導覽工作負載平衡器](../workload-balancer/navigate-the-workload-balancer.md)。

   * 以下文章將逐步引導您瞭解如何指派工作和管理使用者分配：

      * [在工作負載平衡器](../workload-balancer/assign-work-in-workload-balancer.md)中指派工作的概觀。
      * [在工作負載平衡器](../workload-balancer/manage-user-allocations-workload-balancer.md)中管理使用者配置。

* 工作負載平衡器可以在Workfront的多個不同區域找到。 如需您可以在何處找到工作負載平衡器的相關資訊，請參閱[尋找工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。

## 使用工作負載平衡器所需的存取權

您必須擁有對特定專案的正確Workfront存取權和許可權，才能在Workfront中檢視和使用工作負載平衡器。 如需有關使用工作負載平衡器所需存取權的資訊，請參閱文章[管理工作負載平衡器中的資源所需的存取權](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md)。
