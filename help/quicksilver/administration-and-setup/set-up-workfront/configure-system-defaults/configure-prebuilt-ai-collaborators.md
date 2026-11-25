---
user-type: administrator
product-area: system-administration;setup
title: 設定預先建立的AI共同作業人員
description: 身為Adobe Workfront管理員，您可以從Adobe將預先建立的AI共同作業人員（例如錄取協調員）設定為工作代理程式，以便使用者指派給任務和問題。
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c95c5a71a2706d4ddbf3e53a579b348bd072a04e
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 4%
---
# 設定預先建立的AI共同作業人員

## 概觀

預先建立的AI共同作業人員是來自Adobe的現成工作代理程式，這些工作代理程式設定用於執行特定工作，例如檢查遺失資訊的請求。 它們能作為Adobe原生工作代理程式使用，因此您不需要在外部平台中設定代理程式或提供外部平台認證。

當您設定工作代理程式時，您會選取預先建立的共同作業人員作為代理程式的來源。 然後，您可以命名「工作代理程式」、設定其存取層級，並選擇它可以採取的動作。 使用者會以指派任何其他工作代理程式的相同方式，將已設定的工作代理程式指派給任務或問題。 使用者不需要知道代理程式是預先建立的共同作業人員。

如需工作代理程式和其他AI共同作業人員型別的詳細資訊，請參閱[設定AI共同作業人員](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>Select、Prime或Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[!UICONTROL 標準]</p></td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]或群組管理員</td> 
  </tr> 
  </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

貴組織必須啟用Adobe CX Coworker。 如需詳細資訊，請參閱[Workfront中的CX Enterprise Coworker概觀](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)。

## 設定預先建立的AI共同作業人員

您可以在設定工作代理時設定預先建立的AI共同作業人員。 在&#x200B;**選擇代理程式來源**&#x200B;區域中，選取&#x200B;**Adobe Native**，然後從下列清單中選取您要使用的預先建立Collaborator。

如需完整步驟，請參閱[在Workfront中設定工作代理程式](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent-in-workfront)。

設定Collaborator後，使用者可以將其指派給任務或問題。 如需詳細資訊，請參閱[使用工作代理](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)。

## 可用的預先建立AI共同作業人員

### CX Enterprise Coworker {#cx-enterprise-coworker}

由Adobe Agent Orchestrator提供支援的CX Enterprise Coworker代理程式。

如需詳細資訊，請參閱[Workfront中的CX Enterprise Coworker概觀](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)。

### 輸入協調器 {#intake-coordinator}

Intract Coordinator會檢查要求的詳細資料、自訂表單及附件，以找出遺失、不清楚或不一致的資訊。 它會發佈意見回饋，或在使用者核准後進行變更。

>[!NOTE]
>
>建立規則時，您可以將「匯入協調器」指派給路由規則，但稍後無法再指派。

<!--
### Context Carrier {#context-carrier}

The Context Carrier keeps brief information flowing downstream so that context doesn't get scattered. It helps campaign managers and project managers keep the project team current without writing reports.

Requirements: A Workfront project and a Workfront Planning project must be connected to a Planning record. The Context Carrier must be triggered to run.

Steps to be added.

### Production Specialist {#production-specialist}

The Production Specialist produces images in every size you need, so designers don't have to resize them manually.

Requirement: Users must assign the Production Specialist to a task or issue.

Steps to be added.

### Version Comparer {#version-comparer}

The Version Comparer compares versions of a document so project teams can move content faster instead of spotting differences by hand.

Requirement: The document must have more than one version.

Steps to be added.

### Metadata Manager {#metadata-manager}

The Metadata Manager helps marketing teams find, tag, and label documents while work is in progress instead of later in the process.

Requirement: The Metadata Manager is available when you upload a document. Users must trigger it from the toolbar.

Steps to be added.

### Resource PTO Detector {#resource-pto-detector}

The Resource PTO Detector helps project teams make sure delivery isn't affected by time off, by identifying tasks assigned to people who are out of office.

Requirements: Tasks must be assigned, and PTO must be logged in Workfront.

Steps to be added.

### Campaign Summarizer {#campaign-summarizer}

Description and steps to be added.
-->
