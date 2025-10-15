---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 篩選器：個人任務
description: 此任務篩選器會傳回傳送給使用者的臨時工作請求，或使用者在其首頁區域中新增的待辦事項。 個人任務未連線至專案，但如果需要，可將其移至專案。
author: Nolan
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 篩選器：個人任務

<!--Audited: 10/2024-->

此任務篩選器會傳回傳送給使用者的臨時工作請求，或使用者在首頁區域的待辦事項Widget中新增的待辦事項。

臨時工作請求和待辦事項會儲存到Adobe Workfront作為個人任務。

個人任務未連線至專案，但如果需要，可將其移至專案。 如需詳細資訊，請參閱[建立個人工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md)。

![個人工作報告](assets/personal-tasks-report.png)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>修改篩選器的貢獻者或請求 </p>
   <p>要修改報告的標準或計畫</p>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 篩選個人任務

若要建立此篩選：

1. 前往工作清單或工作報告。
1. 從&#x200B;**篩選器**&#x200B;下拉式功能表，按一下&#x200B;**新增篩選器**。
1. （視條件而定）按一下&#x200B;**新增篩選器規則**，您正在從報表存取篩選器；或者，如果您正在從清單存取篩選器，請在第一個欄位中開始選取您的篩選器條件。
1. （視條件而定）選取下列篩選條件：

   * 從清單篩選器： **工作** > **個人** **為True**
   * 從報告篩選器： **任務** > **個人** > **相等（區分大小寫）** > **真**。
1. 儲存篩選。

   此清單只會顯示不在任何專案中的個人任務。
