---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用連結共用工作負載平衡器
description: 您可以與其他用戶共用工作負載平衡器，這些用戶可能沒有可供他們使用的資源區域。 有關使用工作負載平衡器的資訊，請參閱導航工作負載平衡器。
author: Alina
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---

# 使用連結共用工作負載平衡器

您可以與其他用戶共用工作負載平衡器，這些用戶可能沒有可供他們使用的資源區域。 有關使用工作負載平衡器的資訊，請參見 [導航工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何計畫</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>在資源區中使用工作負載平衡器時進行計畫</p>
   <p>使用團隊或項目的工作負載平衡器時工作</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視或更高存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>任務</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案、工作和問題的權限或更高權限 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 從共用連結查看時，工作負載平衡器中包含的資訊

當與其他用戶共用指向工作負載平衡器的連結時，共用連結將包括以下資訊：

* 工作負載平衡器的「已分配工作」區域。
* 項目、任務、用戶資訊。 這包括使用者配置資訊。
* 資訊會根據選取的篩選器顯示。

   >[!IMPORTANT]
   >
   >如果在共用連結後刪除篩選器，則從連結中查看工作負載平衡器的用戶會收到刪除篩選器的警告。 它們在「已分配的工作」區域中查看所有用戶。 這是工作負載平衡器的預設視圖。

* 先前選取的周數。

從共用連結查看工作負載平衡器的用戶可以使用以下選項來更新自己：

* 以下時間軸選擇：

   * 今天
   * 後轉表徵圖
   * 日曆選擇

* 「日」、「周」和「月」圖示
* 設定圖示
* 顯示分配表徵圖

   如需使用這些選項的詳細資訊，請參閱 [導航工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* 顯示角色分配表徵圖

   這僅適用於項目的工作負載平衡器。

接收共用連結的用戶無法在工作負載平衡器中通過此連結執行以下操作：

* 將工作項目指派給使用者
* 管理用戶分配
* 建立新的或更新原本套用的篩選器

## 從共用連結查看工作負載平衡器中資訊所需的訪問

要從共用連結查看工作負載平衡器中的資訊，您需要以下訪問權限：

* 有效的Adobe Workfront授權，且您必須登入Workfront。
* 至少在訪問級別中查看對資源管理的訪問。 有關授予資源管理訪問權限的資訊，請參閱 [授予資源管理的訪問權限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* 查看工作負載平衡器中顯示的項目、任務、問題和用戶的權限。

## 通過連結與其他用戶共用工作負載平衡器

1. 轉到工作負載平衡器

   有關訪問工作負載平衡器的資訊，請參見 [導航工作負載平衡器](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. （選用）執行下列一或多個動作：

   * 更新時段選項。
   * 按一下 **日、周**，或 **月** 檢視每日、每週或每月資訊。

      ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * 將篩選器應用於「未分配」和「已分配」工作區。

      有關在工作負載平衡器中篩選資訊的資訊，請參見 [篩選工作負載平衡器中的資訊](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. 按一下 **連結圖示** ![](assets/wb-shearable-link-icon-small.png).

   這會將連結新增至剪貼簿。

1. 執行下列其中一項操作以與其他人共用連結：

   * 將其貼到電子郵件、聊天消息或任何其他應用程式中，並與其他用戶共用。
   * 將其新增至自訂區段作為外部頁面、將自訂區段新增至使用者的設定檔或配置範本，然後與使用者、團隊、工作角色或群組共用配置範本。

      如需建立外部頁面的相關資訊，請參閱 [在控制面板中內嵌外部網頁](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). 如需將自訂區段新增至版面範本的相關資訊，請參閱 [使用版面範本自訂左側面板](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

      >[!IMPORTANT]
      >
      >將工作負載平衡器添加到對象的自定義部分時，該對象不篩選工作負載平衡器中的資訊。 工作負載平衡器顯示由最初應用的篩選器篩選的資訊。
