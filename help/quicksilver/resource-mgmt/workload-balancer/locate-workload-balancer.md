---
product-area: resource-management
keywords: 工作，團隊，員工，資源
navigation-topic: the-workload-balancer
title: 找到工作負載平衡器
description: 您可以使用工作負載平衡器來排程工作資源，或檢閱其使用狀態和目前配置。
author: Lisa
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# 找到工作負載平衡器


您可以使用工作負載平衡器來排程工作資源，或檢閱其使用狀態和目前配置。

您可以透過以下方式存取「工作負載平衡器」：

* 從Adobe Workfront預先定義的數個區域
* 將其新增到自訂區段

本文會說明您可在其中存取工作負載平衡器的區域。

>[!NOTE]
>
>無論您使用何種方法存取工作負載平衡器，導覽它和管理資源都是相同的。
>
>如需有關工作負載平衡器以及如何使用它來管理和排程您的工作資源的資訊，請參閱以下文章：
>
>* [工作負載平衡器總覽](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [在工作負載平衡器](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)中指派工作的總覽
>* [在工作負載平衡器](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)中管理使用者配置
>

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計畫，在資源區域使用工作負載平衡器</p>
   <p>工作，使用團隊或專案的工作負載平衡器時</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>檢視以下專案或更高存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>任務</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p><b> 附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案、任務和問題的許可權或更高 </p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 在預先定義的區域中存取工作負載平衡器

以下章節說明您可以在何處存取Workfront中的工作負載平衡器。

### 存取工作負載平衡器資源區域中的多個專案

1. 按一下&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**資源**。
1. 按一下左側面板中的&#x200B;**工作負載平衡器**。

   ![](assets/nwe-balancer-global.png)

   依預設，工作負載平衡器會依資源區域中的資訊顯示以下內容：

   * **未指派的工作**：沒有未指派的工作專案。
   * **已指派的工作**：系統中的所有作用中使用者。

     在「已指派的工作」區域顯示使用者時，我們建議使用篩選器。 如需詳細資訊，請參閱工作負載平衡器](../workload-balancer/filter-information-workload-balancer.md)中的[篩選器資訊。

### 存取團隊的工作負載平衡器

1. 按一下&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下[團隊]。
您的主團隊頁面隨即顯示。

   預設會顯示團隊的工作負載平衡器。

   ![](assets/nwe-balancer-team-350x172.png)

   依預設，團隊的工作負載平衡器顯示以下資訊：

   * **未指派的工作**：指派給團隊且未指派給使用者的專案。
   * **已指派的工作**：團隊的所有成員及其所有指派。

     >[!TIP]
     >
     >團隊成員可能被指派給同時被指派給團隊或指派給其他團隊或角色的工作。



### 存取專案的工作負載平衡器

1. 按一下&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**專案**。
1. 按一下專案名稱以開啟專案頁面。
1. 按一下左側面板中的&#x200B;**工作負載平衡器**。 您可能需要按一下&#x200B;**顯示更多**，然後按一下&#x200B;**工作負載平衡器**。

   專案的工作負載平衡器顯示。

   ![](assets/nwe-balancer-project-350x152.png)

   依預設，專案的工作負載平衡器會依資訊顯示以下內容：

   * **未指派的工作**：專案中已指派給工作角色或團隊的專案，但未指派給使用者。
   * **指派的工作**：指派給專案專案的使用者。

     >[!TIP]
     >
     >您可以透過啟用「顯示所有使用者」選項來顯示系統中的所有使用者，而不是僅顯示專案上的使用者（在指派的工作區域中）。 如需詳細資訊，請參閱[瀏覽工作負載平衡器](../workload-balancer/navigate-the-workload-balancer.md)。


## 將工作負載平衡器新增到自訂區段

您可以將工作負載平衡器新增到任何自訂區段。

將工作負載平衡器新增到自訂區段時，會保留您已經套用至該工作負載平衡器的大部分自訂。

1. 請前往下列任一區域存取工作負載平衡器：

   * 資源區域
   * 團隊
   * 專案

1. 取得可共用的連結，並將其複製到剪貼簿，如[使用連結共用工作負載平衡器](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)中所述。
1. 建立具有外部頁面的儀表板，如[在儀表板中內嵌外部網頁](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)中所述。 針對外部頁面使用您在步驟2取得的分享連結。

   <!--
      (NOTE: ensure this stays correct)
      -->

1. 依照[建立自訂標籤或區段](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)中的說明建立自訂區段，以將儀表板放在自訂標籤上。

   從自訂區段存取工作負載平衡器時，您可以檢視它，就像您直接從步驟1中列出的其中一個原始區域存取它一樣。

   <!--
      (NOTE: ensure this stays correct)
     -->

1. （選擇性）共用版面配置範本中的自訂標籤，如[使用版面配置範本自訂左側面板](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)中所述。


<!--
For a team:

* From the Workload Balancer section of a team.

  You can adjust allocations and review or assign work from multiple projects to individual team members.

For a project:

  You can do the following when you use the Workload Balancer within a project:

   * Assign work on the project to users already assigned other work on the project.
   * Assign work to any user that might not be on the project.

   * View additional work that users are assigned to on other projects.
   * Adjust user allocations to work items.-->