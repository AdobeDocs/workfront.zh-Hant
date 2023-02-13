---
product-area: resource-management
keywords: 工作，團隊，人員，資源
navigation-topic: the-workload-balancer
title: 找到工作負載平衡器
description: 您可以使用工作負載平衡器來調度資源以進行工作或查看其可用性和當前分配。
author: Alina
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: 87f02f3908c86575ca2dfacd7d88146b9967a804
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 1%

---

# 找到工作負載平衡器


您可以使用工作負載平衡器來調度資源以進行工作或查看其可用性和當前分配。

您可以通過以下方式訪問工作負載平衡器：

* 從Adobe Workfront預先定義的數個區域
* 將其新增至自訂區段

本文介紹了可以訪問Workload Balancer的區域。

>[!NOTE]
>
>無論您使用何種方法來訪問工作負載平衡器，進行導航和管理資源都是相同的。
>
>有關工作負載平衡器以及如何使用它來管理和調度工作資源的資訊，請參閱以下文章：
>
>* [工作負載平衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [導航工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [工作負載平衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [在工作負載平衡器中管理用戶分配](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)
>


## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>在使用團隊或「資源配置」區域中的工作負載平衡器時進行計畫 </p>
   <p>使用項目的工作負載平衡器時工作 </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>檢視或更高存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>任務</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p><b> 附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案、工作和問題的權限或更高權限 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在預定義區域中訪問工作負載平衡器

以下各節將說明您可以在何處訪問Workfront中的工作負載平衡器。

### 訪問資源區中多個項目的工作負載平衡器

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)，然後按一下 **資源**.
1. 按一下 **工作負載平衡器** 中。

   ![](assets/nwe-balancer-global.png)

   預設情況下， Workload Balancer將按「資源」區域中的資訊顯示以下內容：

   * **未分配的工作**:沒有未分配的工作項。
   * **已分配的工作**:系統中所有活動用戶。

      在「已指派的工作」區域中顯示使用者時，建議使用篩選器。 如需詳細資訊，請參閱 [篩選工作負載平衡器中的資訊](../workload-balancer/filter-information-workload-balancer.md).

### 訪問團隊的工作負載平衡器

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)，然後按一下「團隊」。
顯示您的首頁。

   預設情況下，將顯示該團隊的工作負載平衡器。

   ![](assets/nwe-balancer-team-350x172.png)

   組的工作負載平衡器預設顯示以下資訊：

   * **未分配的工作**:指派給團隊且未指派給使用者的項目。
   * **已分配的工作**:團隊的所有成員及其所有任務。

      >[!TIP]
      >
      >可將團隊成員指派給也分配給團隊的工作，或指派給其他團隊或角色的工作。



### 訪問項目的工作負載平衡器

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)，然後按一下 **專案**.
1. 按一下專案名稱以開啟專案頁面。
1. 按一下 **工作負載平衡器** 中。 您可能必須按一下 **顯示更多**，然後 **工作負載平衡器**.

   項目的工作負載平衡器隨即顯示。

   ![](assets/nwe-balancer-project-350x152.png)

   項目的工作負載平衡器預設顯示以下資訊：

   * **未分配的工作**:已指派給工作角色或團隊且未指派給使用者之專案中的項目。
   * **已分配的工作**:指派給專案項目的使用者。

      >[!TIP]
      >
      >通過啟用「顯示所有用戶」選項，您可以顯示系統中的所有用戶，而不只顯示項目上的用戶（在「已分配的工作」區域中）。 如需詳細資訊，請參閱 [導航工作負載平衡器](../workload-balancer/navigate-the-workload-balancer.md).


## 將工作負載平衡器添加到自定義部分

您可以將工作負載平衡器添加到任何自定義部分。

已將您已應用到工作負載平衡器的大多數自定義內容添加到自定義部分時，將保留它。

1. 通過轉到以下任一區域訪問工作負載平衡器：

   * 資源區
   * 團隊
   * 專案

1. 取得可分享的連結，並將其複製到剪貼簿，如 [使用連結共用工作負載平衡器](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
1. 使用外部頁面建立控制面板，如 [在控制面板中內嵌外部網頁](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). 將您在步驟2取得的分享連結用於外部頁面。

   <!--
      (NOTE: ensure this stays correct)
      -->

1. 建立自訂區段，如 [建立自訂標籤或區段](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) 將控制面板置於自訂標籤上。

   從自定義部分訪問工作負載平衡器時，您可以像直接從步驟1中列出的其中一個原始區域訪問它一樣來查看它。

   <!--
      (NOTE: ensure this stays correct)
     -->

1. （選用）在「配置範本」中共用自訂索引標籤，如  [使用版面範本自訂左側面板](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md) .


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