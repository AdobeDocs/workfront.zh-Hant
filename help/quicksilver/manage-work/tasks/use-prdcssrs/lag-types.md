---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 延遲類型概觀
description: 滯後是指在強制的前置任務完成之後必須經過的時間量，直到相依任務開始（正滯後），或相依任務在前置任務開始之前可能開始的時間量（負滯後）。
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1385'
ht-degree: 0%

---

# 延遲類型概觀

滯後是指在強制的前置任務完成之後必須經過的時間量，直到相依任務開始（正滯後），或相依任務在前置任務開始之前可能開始的時間量（負滯後）。

計算後續任務的計畫日期、預計日期和預計日期時，會考慮前置任務的延遲日期和計畫日期、預計日期和預計開始日期（完成日期）。

## 存取需求

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

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

## 指示任務上的延遲和延遲類型

在定義其前置關係時，可以指明任務的延遲類型。

* [在任務的前置任務部分中指定延遲類型](#indicate-lag-types-in-the-predecessors-section-of-a-task)
* [在任務清單中指定延遲類型](#indicate-lag-types-in-a-task-list)

### 在任務的前置任務部分中指定延遲類型 {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. 轉到要定義前置任務和滯後類型的任務。
1. 按一下 **前置任務** 中。 您可能必須按一下 **顯示更多**，然後 **前置任務**.
1. 按一下 **添加前置任務**.
1. （選用）如果您想要新增跨專案前置項目，請取代 **上層專案** 以其他專案命名。
1. 開始鍵入前置任務的名稱，然後在其出現在清單中時選擇它。
1. 選取 **相依類型**.

   如需先前相依性類型的詳細資訊，請參閱 [任務相關性類型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. 指定 **延遲** 使用數值的金額。 您可以指定負數來表示負延遲。
1. 從下列選項中選取，以識別您要為前身指出的延遲類型：

   * **天**
   * **行事曆日**
   * **百分比**
   * **星期**
   * **星期（非零）**

      如需這些延遲類型及其計算方式的詳細資訊，請參閱區段 [延遲類型概觀](#lag-types-overview) 這篇文章。

1. 按一下&#x200B;**儲存**。

### 在任務清單中指定延遲類型  {#indicate-lag-types-in-a-task-list}

1. 轉到任務清單，然後選擇 **標準** 從 **檢視** 下拉式功能表。

1. 按一下內部 **前置任務** 與要為其指定前置任務和延遲量的任務對應的列。
1. 輸入以下內容，不含空格：

   * 要指示為所選任務的前置任務的任務數
   * 要在任務之間指示的依賴關係類型的縮寫

      如需「相依類型」縮寫的詳細資訊，請參閱 [任務相關性類型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * a **+** 正滯後或 **-** 負滯後

   * 延遲量
   * 要使用的Lag Type的縮寫。

      如需Lag Types縮寫的詳細資訊，請參閱區段 [延遲類型概觀](#lag-types-overview) 這篇文章。
   例如，要指示任務具有前置任務和2天的正滯後，請輸入

   ```
   1fs+2d
   ```

   （在前置項列中）。

1. 按一下鍵盤上的Enter以保存對任務所做的更改。

## 延遲類型概觀 {#lag-types-overview}

需要一段時間的任務的一個示例可能是將樹木鋸成木材。 如果新切的木頭必須先乾燥一段時間才能切割，那麼在切樹和鋸成木材之間就會有一段時間的滯後。

下表說明「延遲類型」以及如何指示每個類型的時間量：

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>值</strong> </p> </td> 
   <td> <p><strong>說明</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>天(d)</p> </td> 
   <td> <p>由相依性連結的兩個任務之間的延遲是以工作天數衡量。 這是預設的滯後類型。 </p> <p>例如，如果某個完成 — 開始相關性有2個工作日延遲，而前置任務在星期五完成，則相依任務從星期三開始。 週末天數不會計為延遲的一部分。 </p> <p>注意：天的最大延遲限制為366。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>日曆天數(c)</p> </td> 
   <td> <p>兩個任務之間的延遲以日曆天數（包括節假日和週末）計算。 </p> <p>注意：雖然此延遲類型會將非工作日計為延遲的一部分，但相依任務絕不能從非工作日開始。 如果此延遲類型使相依任務在非工作日開始，則相依任務的計畫起始日期將安排在下一個工作日。 </p> <p>例如，如果某個完成 — 開始相關性有2個日曆日延遲，而前一任務在星期四完成，則相依任務從星期一開始，而不是星期日。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>百分比（p或pe）</p> </td> 
   <td> <p>延遲以完成前置任務的估計時間的百分比表示。 </p> <p>例如，如果在10天的前置任務上存在20%延遲的終止 — 開始依賴項，則系統將計算多少天是前置任務持續時間的20%，並將其用作延遲。 在此情況下，工作完成後2天。 </p> <p>注意：百分比的最大延遲限制為2000%。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>星期(w) </p> </td> 
   <td> <p>兩個任務之間的延遲通過指示包含前一任務的計畫完成日期的一週中的天數來衡量。</p> <p>對於此延遲類型，一週中的每一天都與一個數字相關聯：</p> 
    <ul> 
     <li>星期日=1</li> 
     <li>星期一=2</li> 
     <li>星期二=3</li> 
     <li>星期三=4</li> 
     <li>星期四=5</li> 
     <li>星期五=6</li> 
     <li>星期六=7</li> 
    </ul> <p>如果要指明繼承者的計畫起始日期應為當周的星期二，並且星期二早於前一個的計畫完成日期，則您將使用以下公式為您的繼承者編碼： </p> <p><code style="font-style: normal;">4fs-3w</code> </p> <p>注意：如果星期二是前一任務的計畫完成日期的一週，則後續任務的計畫起始日期是該周的第一個可用工作日。 </p> <p>如果您想要指出延遲應落在當周的星期六，而星期六晚於前一個的計畫完成日期，您將使用下列公式為您的繼任者編碼：</p> <p><code style="font-style: normal;">4fs+7w</code> </p> <p>如果星期六是非工作日，則選擇星期六之後的下一個可用日（以表示正滯後）作為後續的計畫起始日期。 </p> <p>若要指出過去或未來的周數，您可以在延遲類型的日數前面新增數字。 </p> <p>例如，若要指出10週前的星期一，您可以使用此程式碼來指出您繼任者的前身：</p> <p><code>4fs-102w</code> </p> <p>10表示10週前，2是指派給星期一的數字。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>星期非零(k)</p> </td> 
   <td> <p>兩個任務之間的延遲的測量方式與「周」延遲類型的「天」(Day of the Week)相同，但前身的時間結束於指定的一週的同一天。 然後，將延遲時間計算到相鄰的周(+/-)。 </p> <p>在此情況下，延遲時間永遠不能為0。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 負延遲概觀

您可以使用負滯值來表示任務在前置任務結束之前開始的必要性或能力。

使用負滯後時，請考量下列規則：

* 負滯後不能強制任務的開始/完成日期在項目的計劃開始/完成日期之前或之後。 這些項目的「排程起始」欄位中會指定這些日期。

   在此情況下，請考量下列事項：

   * 計畫項目的完成日期。
   * 項目上的最後一個任務應使用「必須完成任務約束」。 建議為任務指定足夠的持續時間，以說明項目上的所有任務。 其餘任務可以與「盡快」約束一起使用。

* 與任務使用「完成 — 開始」前置項關係可能會生成錯誤消息。

   在此情況下，請考量下列事項：

   * 在任務之間設定「完成 — 完成」前置關係。
   * 後續任務的持續時間應等於或超過任務之間的預期延遲天數。
