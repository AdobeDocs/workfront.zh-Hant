---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 使用工作負載平衡器手動分配工作
description: 您可以使用Adobe Workfront Workload Balancer手動將工作項目指派給使用者。
author: Alina
feature: Resource Management
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 2%

---

# 使用工作負載平衡器手動分配工作

您可以使用Adobe Workfront Workload Balancer手動將工作項目指派給使用者。

有關使用工作負載平衡器為用戶分配工作的一般資訊，請參見 [工作負載平衡器中分配工作的概述](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
   <td> <p>編輯對以下項目的存取權：</p> 
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
   <td> <p>將權限或更高版本貢獻給包括「進行分配」的項目、任務和問題</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在工作負載平衡器中手動分配工作

您可以分配尚未分配給用戶的工作項，或重新分配已分配給工作負載平衡器中用戶的工作項。

1. 轉到要分配工作的工作負載平衡器。

   您可以在資源區域、項目或團隊級別使用工作負載平衡器為用戶分配工作。 有關工作負載平衡器在Workfront中的位置的詳細資訊，請參見 [找到工作負載平衡器](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. （選用）前往 **未分配的工作** 區域和套用篩選器以檢視工作或問題

   或

   前往 **已分配的工作** 區域，並展開用戶的名稱以查看分配給他們的工作項目（如果要重新分配其項目）。

1. 按一下 **更多功能表** ![](assets/qs-more-menu.png) 在工作項名稱的左側，然後按一下 **將此項指派給**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >您也可以使用下列捷徑來指派工作或問題：
   >
   >* 在Windows中：按住CTRL鍵並按一下任務或問題欄。
   >* 在Mac:按住CMD鍵並按一下任務或問題欄。


1. 執行下列任一項作業：

   * 開始鍵入要分配給以下項目的用戶、作業角色或團隊的名稱： **搜索人員、角色或團隊** 欄位，在清單中顯示時加以選取，然後按一下 **儲存**.
   >[!TIP]
   >
   >新增使用者時，請注意頭像、使用者的主要角色及其電子郵件地址，以區分名稱相同的使用者。 用戶必須至少與一個作業角色關聯，才能在添加時查看該角色。

   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > 如果您的Workfront或組管理員在您的環境中啟用了委託，請使用「指配」頁簽將用戶分配給該任務或問題。 使用「委派」頁簽查看委派給工作項的用戶。 有關委派工作的資訊，請參見 [管理任務和問題委派](../../manage-work/delegate-work/how-to-delegate-work.md).


   這將工作項指派或重新分配給指定的受分配者。

   如果僅將項目分配給一個團隊或一個工作角色，則該項目只會顯示在「未分配的工作」區域中。 必須將工作項分配給用戶，以便在工作負載平衡器的「已分配的工作」區域中顯示這些工作項。

   >[!TIP]
   >
   >您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
   >
   >
   >如果在停用前已指派使用者、工作角色或團隊，則他們仍會指派給工作項目。 在此情況下，我們建議：
   >
   >   
   >   
   >   * 將工作項重新分配給活動資源。
   >   * 將已停用團隊中的用戶與活動團隊關聯，並將工作項重新分配給活動團隊。


   * 按一下 **進階** 訪問「高級分配」。

      有關進行高級分配的詳細資訊，請參閱 [建立高級分配](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).


1. （選用）按一下 **顯示分配表徵圖** ![](assets/show-allocations-icon-small.png)，然後按一下 **更多功能表** ![](assets/qs-more-menu.png) > **編輯分配**.

   或

   按兩下每日或每週分配，以修改用戶分配給工作項的時間量。

   有關在工作負載平衡器中修改用戶分配的資訊，請參閱文章中的「修改用戶分配」部分 [在工作負載平衡器中管理用戶分配](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   有關使用工作負載平衡器從工作項中刪除分配的資訊，請參見 [在工作負載平衡器中取消分配工作](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
