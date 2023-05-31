---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 協調專案與方案之間的資源配置概要
description: 協調專案與方案之間的資源配置概要
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# 協調專案與方案之間的資源配置概要

>[!IMPORTANT]
>
>您的組織必須購買額外的授權 [!DNL Adobe Workfront Scenario Planner] 以便您檢視專案的方案資訊。 如需關於取得 [!DNL Workfront Scenario Planner]，請參閱 [使用「情境規劃工具」所需的存取權](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

您可以將專案與行動方案連線起來，以確保您的策略性計畫與實際工作同步。 當您在中概述您的策略性計畫和方案時 [!DNL Scenario Planner] 而且您可以規劃專案中的實際工作，可以確保專案和方案上的資源彼此相符，因此您不會過度配置或利用不足。

## 必要條件

開始之前，您必須具備下列條件：

* 中的計畫 [!DNL Scenario Planner] 具有連線到專案的方案。
* 方案所需的職務角色分配。
* 專案中具有計畫時數且已指派給下列其中一項的任務或問題：

   * 工作角色
   * 與工作角色相關聯的使用者

## 連線專案和方案

>[!NOTE]
>
>只有貴組織已為購買額外授權，您才能建立行動方案並將其連結至專案。 [!DNL Workfront Scenario Planner].

您可以執行下列任一項作業，將專案與行動方案連結：

* 將專案匯入計畫（作為新方案）

   如需詳細資訊，請參閱 [將專案匯入至中的計畫 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* 將方案發佈至專案

   如需詳細資訊，請參閱 [透過發佈中的方案來更新或建立專案 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

這兩個程式都會在專案與其對應的方案之間建立連線。 在連線它們之後，您可以透過比較它們並確保它們相符來管理它們的資源配置。

## 有關協調連結專案和行動方案上的資源的考量事項

>[!NOTE]
>
>只有貴組織已為購買額外授權，您才能檢視方案、將其連線至專案，以及檢視其在專案上的資源配置。 [!DNL Workfront Scenario Planner].

* 您可以將使用者、團隊和工作角色指派給專案上的工作專案，也可以將工作角色指派給方案。 因此，您只能調解專案與方案之間的職位角色。

   >[!TIP]
   >
   >若要協調使用者在專案上的時間與行動方案上的角色分配，您必須將使用者與工作角色相關聯。

* 您可以在專案的下列區域中，檢視連結專案上的方案工作角色配置：

   * [!DNL Scenario Planner] 部分 [!UICONTROL 專案詳細資訊] 專案區域。 如需詳細資訊，請參閱下列文章：

      * [透過發佈中的方案來更新或建立專案 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [管理專案中的資訊 [!UICONTROL 概觀] 區域](../manage-work/projects/manage-projects/understand-project-overview-area.md)

      >[!TIP]
      >
      >您無法在中看到專案和行動方案並排顯示的工作角色資訊 [!DNL Scenario Planner] 部分 [!UICONTROL 專案詳細資訊].

   * 此 [!UICONTROL 角色分配] 面板的下列區域：

      * [!UICONTROL 工作負載平衡器] 專案的

         如需有關如何檢視及協調行動方案與連結專案之間角色分配的資訊，請參閱 [!UICONTROL 工作負載平衡器]，請參閱 [在中顯示專案和方案的角色分配 [!UICONTROL 工作負載平衡器]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL 任務] 區段

         有關如何協調行動方案和連結專案之間角色分配的資訊，請參閱 [!UICONTROL 任務] 區段，請參閱 [在任務清單中顯示專案和方案的角色分配](../scenario-planner/show-role-allocation-task-list-nwe.md).
      >[!TIP]
      >
      >您可以在中並排檢視專案和行動方案中的職務角色資訊 [!UICONTROL 角色分配] 面板。



* 您無法檢視已連結方案上專案的工作角色配置。 如需詳細資訊，請參閱 [將專案匯入至中的計畫 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
