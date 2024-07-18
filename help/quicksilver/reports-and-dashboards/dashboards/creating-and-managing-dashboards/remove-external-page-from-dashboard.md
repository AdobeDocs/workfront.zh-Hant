---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 從儀表板移除外部頁面
description: 如果不再需要外部頁面，您可以從控制面板中將其移除。
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# 從儀表板移除外部頁面

如果不再需要外部頁面，您可以從控制面板中將其移除。

但是，在Adobe Workfront中建立外部頁面後，您無法刪除該頁面。 您只能使用API刪除外部頁面。 如需Workfront API的相關資訊，請參閱[API基本知識](../../../wf-api/general/api-basics.md)。 如需有關建立外部頁面的資訊，請參閱[將外部網頁內嵌在儀表板中](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>管理儀表板的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 從儀表板移除外部頁面

1. 按一下&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**儀表板**。
1. 選取您要移除外部頁面的儀表板，然後按一下[編輯]。**** ![](assets/edit-icon.png)

   ![選取[編輯]圖示。](assets/nwe-editdashboard2021-350x188.png)

1. 在畫面右側，找到您要移除的外部頁面，然後按一下&#x200B;**刪除**&#x200B;圖示![](assets/delete.png)。

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. 按一下左下角的&#x200B;**儲存+關閉**。

   這會從選取的控制面板移除外部頁面。 外部頁面仍保留在Workfront中，並可從報表存取。 如需相關資訊，請參閱[在儀表板中內嵌外部網頁](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)一文中的「在報表中檢視外部頁面」一節。
