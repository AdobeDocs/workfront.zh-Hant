---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 從儀表板移除外部頁面
description: 如果不再需要外部頁面，您可以從控制面板中將其移除。
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# 從儀表板移除外部頁面

<!-- Audited: 1/2025 -->

如果不再需要外部頁面，您可以從控制面板中將其移除。

但是，在Adobe Workfront中建立外部頁面後，您無法刪除該頁面。 您只能使用API刪除外部頁面。 如需Workfront API的相關資訊，請參閱[API基本知識](../../../wf-api/general/api-basics.md)。 如需有關建立外部頁面的資訊，請參閱[將外部網頁內嵌在儀表板中](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權</strong></td> 
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>規劃</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>管理儀表板的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從儀表板移除外部頁面

1. 移至包含您要刪除之外部頁面的儀表板。

1. 按一下&#x200B;**儀表板動作**，然後按一下&#x200B;**編輯**。

   ![編輯儀表板](assets/unshimmed-edit-dashboard.png)

1. 在熒幕右側，找到您要移除的外部頁面，然後按一下&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete.png)。

   ![刪除儀表板內的外部頁面圖示](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. 按一下左下角的&#x200B;**儲存+關閉**。

   這會從選取的控制面板移除外部頁面。 外部頁面仍保留在Workfront中，並可從報表存取。 如需相關資訊，請參閱[在儀表板中內嵌外部網頁](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)一文中的「在報表中檢視外部頁面」一節。
