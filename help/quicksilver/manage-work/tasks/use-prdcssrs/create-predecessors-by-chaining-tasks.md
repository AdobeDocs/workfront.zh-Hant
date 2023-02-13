---
product-area: projects
navigation-topic: use-predecessors
title: 通過連結任務建立前置任務關係
description: 您可以在Adobe Workfront中以多種方式建立前置關係。 一種方法是通過連結任務。
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 1%

---

# 通過連結任務建立前置任務關係

您可以在Adobe Workfront中以多種方式建立前置關係。 一種方法是通過連結任務。

有關前置任務的資訊，請參見 [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

通過連結任務，您可以允許系統在選定任務上自動建立前置任務關係，而不是自行為每個任務手動建立關係。 任務之間仍可使用不同的前置關係類型。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和項目的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理任務和專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立前置關係的鏈任務

1. 轉至包含要連結的任務的項目。
1. 按一下 **工作** 中。
1. （條件性）選取 **自動儲存** 在任務清單的右上角，選擇要鏈結的任務。

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >手動保存對任務的更改或使用時間軸計畫模式保存任務時，無法在任務清單中連結任務。

1. 以滑鼠右鍵按一下選取的任務，然後按一下 **鏈**.
1. 從下列相依性類型中選取：

   * **完成-開始**
   * **完成-完成**
   * **開始-開始**
   * **開始-完成**

   如需先前相依性類型的詳細資訊，請參閱 [任務相關性類型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. （選用）按一下 **取消鏈** 如果某些任務之前已被連結。

   >[!CAUTION]
   >
   >批量編輯任務時，只使用「取消鏈」選項刪除循序前置任務。

   您的選定任務現在由前身關係連結。
