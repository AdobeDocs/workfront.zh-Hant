---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用連結共用工作負載平衡器
description: 您可以與其他可能沒有資源區域可用的使用者共用工作負載平衡器。 如需有關使用工作負載平衡器的資訊，請參閱瀏覽工作負載平衡器。
author: Lisa
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 233e61c011cc87f49d0d4082a20b7790104c96c8
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 1%

---

# 使用連結共用工作負載平衡器

您可以與其他使用者共用工作負載平衡器，這些使用者可能沒有主功能表中可用的資源區域。 如需有關使用工作負載平衡器的資訊，請參閱[瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫，在資源區域使用工作負載平衡器時；</br>
       工作，使用團隊或專案的工作負載平衡器時</p></td>
  </tr>
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視以下專案或更高存取權：</p> 
    <ul> 
     <li>資源管理</li> 
     <li>專案</li> 
     <li>任務</li> 
     <li>問題</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>檢視專案、任務和問題的許可權或更高</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從共用連結檢視時包含在工作負載平衡器中的資訊

當您和其他使用者共用工作負載平衡器的連結時，共用連結中包含以下資訊：

* 工作負載平衡器的已指派工作區域。
* 專案、任務、使用者資訊。 這包括使用者配置資訊。
* 資訊會根據選取的篩選器顯示。

  >[!IMPORTANT]
  >
  >如果您在共用連結後刪除篩選器，則從連結檢視工作負載平衡器的使用者會收到篩選器已刪除的警告。 他們檢視指派的工作區域中的所有使用者。 這是工作負載平衡器的預設檢視。

* 先前選取的周數。

以下選項可供從共用連結檢視工作負載平衡器以更新自己的使用者使用：

* 下列時間表選取專案：

   * 今天
   * 後退和前進圖示
   * 行事曆選取專案

* 日、周和月圖示
* 「設定」圖示
* 顯示配置圖示

  如需有關使用這些選項的資訊，請參閱[瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

* 顯示角色配置圖示

  這僅適用於專案的工作負載平衡器。

接收共用連結的使用者無法在工作負載平衡器從此連結：

* 指派工作專案給使用者
* 管理使用者配置
* 建立新的篩選器或更新最初套用的篩選器

## 從共用連結檢視工作負載平衡器資訊所需的存取權

您需要以下存取權才能從共用連結檢視工作負載平衡器中的資訊：

* 具備有效的Adobe Workfront授權，且您必須登入Workfront。
* 至少要在存取層級中檢視對資源管理的存取權。 如需授與資源管理存取權的相關資訊，請參閱[授與資源管理的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)。
* 檢視顯示在工作負載平衡器中的專案、任務、問題和使用者的許可權。

## 透過連結與其他使用者共用工作負載平衡器

1. 前往工作負載平衡器

   如需有關存取工作負載平衡器的資訊，請參閱[瀏覽工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)。

1. （可選）執行下列一或多個動作：

   * 更新時段選擇。
   * 按一下&#x200B;**天、周**&#x200B;或&#x200B;**月**，檢視每日、每週或每月的資訊。

     ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * 將篩選器套用至「未指派」和「已指派」工作區域。

     如需有關在工作負載平衡器中篩選資訊的資訊，請參閱在工作負載平衡器](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)中的篩選資訊[。

1. 按一下&#x200B;**連結圖示** ![](assets/wb-shearable-link-icon-small.png)。

   這會將連結新增至剪貼簿。

1. 執行下列任一項作業，與其他人共用連結：

   * 將其貼到電子郵件、聊天訊息或任何其他應用程式中，並與其他使用者共用。
   * 將其新增到自訂區段作為外部頁面，將自訂區段新增到使用者的設定檔或版面配置範本，然後與使用者、團隊、工作角色或群組共用版面配置範本。

     如需建立外部頁面的相關資訊，請參閱[將外部網頁內嵌在儀表板中](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)。 如需將自訂區段新增至版面配置範本的相關資訊，請參閱[使用版面配置範本自訂左側面板](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)。

     >[!IMPORTANT]
     >
     >當您將工作負載平衡器新增到物件的自訂區段時，工作負載平衡器中的資訊未由物件篩選。 工作負載平衡器顯示按最初套用的篩選器篩選的資訊。
