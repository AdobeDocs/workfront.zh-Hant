---
product-area: projects
navigation-topic: use-predecessors
title: 建立跨專案的前置項目
description: 跨項目前置任務是另一個項目中的另一個任務（稱為後繼任務）所依賴的任務。 前置任務是優先順序高於相依（後置任務）任務的任務。 例如，您可以建立一個依賴項，該依賴項要求在相依任務啟動之前將前置任務標籤為「完成」。
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# 建立跨專案的前置項目

跨項目前置任務是另一個項目中的另一個任務（稱為後置任務）所依賴的任務。 前置任務是優先順序高於相依（後置任務）任務的任務。 例如，您可以建立一個依賴項，該依賴項要求在相依任務啟動之前將前置任務標籤為「完成」。

與單一專案中的前置作業一樣，Adobe Workfront也允許工作與其他專案中的工作相依。

**範例**

如果挖掘公司只有一個挖掘機，並且兩個併發的項目都有需要使用挖掘機的任務，則項目經理可以使第一個項目中的任務依賴於第二個項目中的任務，以說明挖掘可以在上一個項目放棄挖掘時開始。
通過跨項目前置任務連結項目時，主項目（具有前置任務的項目）的日期將影響輔助項目（具有後置任務的項目）。

>[!TIP]
>
>必須重新計算項目的時間表，才能查看輔助項目的更新日期。 有關重新計算時間表的詳細資訊，請參見 [設定專案的時間軸重新計算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

如需先前關係的詳細資訊，請參閱 [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 存取需求

<!--drafted - replace table for P&P:

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
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>編輯對任務和項目的訪問</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理任務和專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立跨專案前置項目

1. 轉到將作為您的繼任者的任務。
1. 按一下 **前置任務** 中。
1. 按一下 **添加前置項。**
1. 在 **上層專案** 欄位中，開始鍵入包含要與當前任務相關的任務的項目名稱。
1. 出現在下拉式清單中時，按一下名稱。
1. 在 **工作** 欄位，開始鍵入要與當前任務相依的任務的名稱。
1. 指定以下資訊以定義前置任務和從屬任務之間的關係：

   * **相依類型：** 選擇希望任務與相依任務的關係。 預設關係為「完成 — 開始」，這意味著前置任務必須在從屬任務開始之前完成。 如需各種相依性類型的詳細資訊，請參閱 [任務相關性類型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)

   * **延遲：** 指定在強制前置任務完成之後必須經過的時間長度，直到從屬任務開始為止。 如需各種延遲類型的詳細資訊，請參閱 [延遲類型概觀](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **強制：** 選取此選項時，使用者無法提早開始工作來規避這兩個工作之間的相依關係。 例如，如果強制執行任務A和任務B之間的關係，則任務B在任務A完成之前無法啟動。 有關強制執行前置任務的詳細資訊，請參閱 [強制前置作業](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

      未選取此選項時，相依性會視為對使用者的建議。 例如，用戶可以在任務A完成之前啟動任務B。

1. 按一下&#x200B;**儲存**。

   具有跨項目前置項的任務將顯示前置項所屬的項目的參考編號和任務編號，在任務清單的「前置項」列中用冒號分隔。

   ![跨專案前身](assets/cross-project-predecessor-in-list-view.png)

   前置任務標籤為完成時，前置任務表徵圖將變為綠色。 這表示相依任務已準備就緒可供使用。

   將滑鼠指標暫留在此值上，可取得前置項目、日期的詳細資訊。 在「詳細資訊」(details)框中按一下跨項目前置項以開啟任務。 按一下 **請參閱專案** 來開啟跨專案。

   ![跨專案前置項目詳細資訊](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   此 **請參閱專案** 選項僅在檢視跨專案前置項目時顯示。

