---
content-type: overview
product-area: projects
navigation-topic: financials
title: 定義加班比率
description: 您可以定義任務的加班率，以調整任務指派的計畫收入計算。
author: Lisa
feature: Work Management
exl-id: 832d3aab-3e09-4d83-91a6-be0145ce3554
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 6%

---

# 定義加班率

將加班比率新增至任務時，會套用至任務上的所有指派。 它會乘以該任務的所有計畫時數，並且影響計畫收入計算。

同一任務內之指派的加班比率不能改變。 如果需要不同的加班乘數，您必須在父系任務下建立個別的子任務。

>[!NOTE]
>
>沒有驗證可防止將加班率新增至非加班任務。

## 計畫收入的加班計算

系統會先使用標準收費率階層來決定收費率。 如需詳細資訊，請參閱[收入與成本階層概覽](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。

如果任務存在超時比率，則計算方式為：
計畫收入=記帳費率×加班費率×計畫時數

如果加班比率為空白，則計算方式為：
計畫收入=記帳費率×計畫時數

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>標準</td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>編輯任務、專案和財務資料的存取權</td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td><p>管理包含編輯收費率之任務的許可權</p>
     <p>貢獻專案或更高的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

任務收入型別必須是使用者和角色每小時。 如需詳細資訊，請參閱[收入與成本階層概覽](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。

您的配置範本必須啟用&#x200B;**加班比率**&#x200B;欄位。

1. 在版面配置範本中，按一下&#x200B;**自訂使用者看到的內容**&#x200B;下的向下箭頭，然後按一下&#x200B;**工作**。
1. 在&#x200B;**詳細資料**&#x200B;區段中，選取&#x200B;**財務**&#x200B;區域中的&#x200B;**加班比率**&#x200B;欄位。

   如需詳細資訊，請參閱[使用配置範本自訂詳細資料檢視](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

## 定義任務的超時比率

1. 移至您要編輯的工作。

   如需詳細資訊，請參閱[在任務詳細資訊區段](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md)中管理任務財務。

1. 按一下左側面板中的&#x200B;**工作詳細資料**。
1. 在&#x200B;**財務**&#x200B;區域中，在&#x200B;**加班比率**&#x200B;欄位中輸入加班乘數。
1. 按一下「**儲存變更**」。
