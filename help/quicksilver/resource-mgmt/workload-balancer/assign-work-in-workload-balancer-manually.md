---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用工作負載平衡器手動指派工作
description: 您可以使用Adobe Workfront工作負載平衡器手動指派工作專案給使用者。
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 1%

---

# 使用工作負載平衡器手動指派工作

您可以使用Adobe Workfront工作負載平衡器手動指派工作專案給使用者。

如需使用工作負載平衡器指派工作給使用者的一般資訊，請參閱在工作負載平衡器](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)中指派工作的總覽。[

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
   <td> <p>編輯下列專案的存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>專案</p> </li> 
     <li> <p>任務</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>Contribute許可權或以上至專案、任務和問題，包括進行指派</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 在工作負載平衡器中手動指派工作

您可以在工作負載平衡器中指派尚未指派給使用者的工作專案，或重新指派已指派給使用者的專案。

1. 前往您要指派工作的工作負載平衡器。

   您可以使用資源區域、專案或團隊層級的工作負載平衡器將工作指派給使用者。 如需有關工作負載平衡器在Workfront中的位置的詳細資訊，請參閱[找到工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)。

1. （選擇性）移至&#x200B;**未指派的工作**&#x200B;區域並套用篩選器以檢視任務或問題

   或

   移至&#x200B;**指派的工作**&#x200B;區域，並展開使用者的名稱以檢視指派給他們的工作專案（如果您要重新指派其專案）。

1. 按一下工作專案名稱左側的&#x200B;**其他功能表** ![](assets/qs-more-menu.png)，然後按一下&#x200B;**將此指派給**。

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >您也可以使用下列捷徑來指派任務或問題：
   >
   >* 在Windows中：按住CTRL鍵並按一下任務列或問題列。
   >* 在Mac中： CMD按一下任務或問題列。

1. 執行下列其中一項：

   * 開始輸入您要指派給&#x200B;**搜尋人員、角色或團隊**&#x200B;欄位中的專案的使用者、工作角色或團隊名稱，當它顯示在清單中時選取它，然後按一下&#x200B;**儲存**。

   >[!TIP]
   >
   >新增使用者時，請注意顯示圖片、使用者的主要角色及其電子郵件地址，以區分具有相同名稱的使用者。
   >
   >使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。
   >
   > 您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱[授予使用者存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。


   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > 如果您的Workfront或群組管理員在您的環境中啟用了委派，請使用「工作總攬」標籤將使用者指派給任務或問題。 使用「委派」標籤可檢視委派給工作專案的使用者。 如需委派工作的相關資訊，請參閱[管理任務和問題委派](../../manage-work/delegate-work/how-to-delegate-work.md)。


   這會將工作專案指派或重新指派給指定的受指派人。

   如果您只將專案指派給團隊或工作角色，該專案只會顯示在「未指派的工作」區域中。 您必須將工作專案指派給使用者，才能在工作負載平衡器的已指派工作區域顯示它們。

   >[!TIP]
   >
   >您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
   >
   >
   >如果使用者、工作角色或團隊在停用之前已被指派，則他們仍被指派給工作專案。 在此情況下，我們建議採取下列步驟：
   >
   >   
   >   
   >   * 將工作專案重新指派給作用中的資源。
   >   * 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。
   >   
   >

   * 按一下&#x200B;**進階**&#x200B;以存取進階指派。

     如需進行進階指派的詳細資訊，請參閱[建立進階指派](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)。

1. （選擇性）按一下&#x200B;**顯示配置圖示** ![](assets/show-allocations-icon-small.png)，然後按一下&#x200B;**更多功能表** ![](assets/qs-more-menu.png) > **編輯配置**。

   或

   按兩下每日或每週配置，以修改將使用者配置給工作專案的時間量。

   如需有關在工作負載平衡器中修改使用者配置的資訊，請參閱在工作負載平衡器](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)中管理使用者配置一文[中的「修改使用者配置」一節。

   如需有關使用工作負載平衡器從工作專案移除指派的資訊，請參閱在工作負載平衡器](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md)中取消指派工作。[

    
