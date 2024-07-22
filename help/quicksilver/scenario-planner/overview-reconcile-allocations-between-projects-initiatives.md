---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 協調專案與方案之間資源配置的概要
description: 協調專案與方案之間資源配置的概要
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# 協調專案與方案之間資源配置的概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

您可以將專案與方案連線起來，以確保您的策略性計畫與實際工作同步。 當您在[!DNL Scenario Planner]中概述您的策略性計畫和方案，並計畫專案中的實際工作時，您可以確保專案和方案上的資源相符，這樣您就不會過度配置或利用它們。

## 先決條件

開始之前，您必須具備下列條件：

* [!DNL Scenario Planner]中計畫具有連線到專案的方案。
* 方案所需的職務角色分配。
* 專案中已規劃時數並指派給以下其中一項的任務或問題：

   * 職務角色
   * 與工作角色相關聯的使用者

## 連線專案和方案

>[!NOTE]
>
>只有貴組織已為[!DNL Workfront Scenario Planner]購買額外授權，您才能建立方案並將它們連結至專案。

您可以執行下列任一項作業，將專案與行動方案連結：

* 將專案匯入計畫，作為新方案

  如需詳細資訊，請參閱[將專案匯入 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)中的計畫。

* Publish方案至專案

  如需詳細資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中發佈行動方案以更新或建立專案。

這兩個程式都會在專案與其對應的方案之間建立連線。 在連線它們之後，您可以透過比較它們並確保它們相符來管理它們的資源配置。

## 有關協調連結專案和方案上資源的考量事項

>[!NOTE]
>
>只有貴組織已為[!DNL Workfront Scenario Planner]購買額外授權時，您才能檢視方案、將其連線至專案，以及檢視其在專案上的資源配置。

* 您可以將使用者、團隊和工作角色指派給專案上的工作專案，也可以將工作角色指派給方案。 因此，您只能調解專案與方案之間的職務角色。

  >[!TIP]
  >
  >若要將使用者在專案上的時間與方案上的角色分配進行調解，您必須將使用者與工作角色相關聯。

* 您可以在專案的下列區域中，檢視連結專案上的方案工作角色分配：

   * 專案上[!UICONTROL 專案詳細資料]區域的[!DNL Scenario Planner]區段。 如需詳細資訊，請參閱下列文章：

      * [在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中發佈行動方案以更新或建立專案
      * [管理專案[!UICONTROL 概觀]區域中的資訊](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >您無法在[!UICONTROL 專案詳細資料]的[!DNL Scenario Planner]區段中，從專案與行動方案並排看到工作角色資訊。

   * [!UICONTROL 角色配置]面板位於下列區域：

      * 專案的[!UICONTROL 工作負載平衡器]

        如需有關如何在[!UICONTROL 工作負載平衡器]中檢視及調解方案與連結專案之間角色配置的資訊，請參閱[在[!UICONTROL 工作負載平衡器]](../scenario-planner/show-role-allocation-workload-balancer.md)中顯示專案與方案的角色配置。

      * [!UICONTROL 任務]區段

        如需有關如何在[!UICONTROL 任務]區段中協調方案與連結專案之間角色分配的資訊，請參閱[顯示任務清單中專案與方案的角色分配](../scenario-planner/show-role-allocation-task-list-nwe.md)。

     >[!TIP]
     >
     >您可以在[!UICONTROL 角色配置]面板中並排檢視專案和行動方案中的工作角色資訊。

* 您無法檢視已連結方案上專案的工作角色配置。 如需詳細資訊，請參閱[將專案匯入 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)中的計畫。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
