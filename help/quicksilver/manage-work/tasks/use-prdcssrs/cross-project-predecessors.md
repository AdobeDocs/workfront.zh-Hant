---
product-area: projects
navigation-topic: use-predecessors
title: 建立跨專案前置任務
description: 跨專案前置任務是指另一個專案中另一個任務（稱為後續任務）所依賴的任務。 前置任務是優先於相依（後置任務）任務的任務。 例如，您可以建立相依性，要求在相依性任務開始之前，前置任務必須標籤為「完成」。
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# 建立跨專案前置任務

<!--Audited: 12/2024-->

跨專案前置任務是指另一個專案中另一個任務（稱為後續任務）所依賴的任務。 前置任務是優先於相依（後置任務）任務的任務。 例如，您可以建立相依性，要求在相依性任務開始之前，前置任務必須標籤為「完成」。

Adobe Workfront允許任務相依於其他專案中的任務，就像它允許單一專案中的前置任務一樣。

>[!INFO]
>
>例如，一家挖掘公司只有一個挖掘機，而兩個專案具有需要使用挖掘機的任務。 專案經理可讓第一個專案中的任務成為第二個專案中任務的前置任務。 這顯示第二個專案可在第一個專案使用完畢後開始使用反鏟工作台。

透過跨專案前置任務連結專案時，主要專案（具有前置任務者）的日期將影響次要專案（具有後續任務者）。

>[!TIP]
>
>您必須重新計算專案的時間表，才能檢視次要專案的更新日期。 如需重新計算時間表的相關詳細資訊，請參閱[設定專案的時間表重新計算](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)。

如需前置任務關係的詳細資訊，請參閱[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

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
   <td><p>標準</p> 
   <p>規劃</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務與專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務和專案的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard </p> 
  
   <p>Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 建立跨專案前置任務

>[!TIP]
>
>雖然建立範本任務前置任務與建立專案任務前置任務類似，但您無法為範本任務建立跨範本前置任務。


1. 移至將成為您後續任務的工作（相依任務）。
1. 按一下左側面板中的&#x200B;**前置任務**。

   >[!TIP]
   >
   >   您的Workfront或群組管理員可以從左側面板中移除&#x200B;**前置任務**&#x200B;區段或其他區段。

1. 按一下&#x200B;**新增前置任務。**
1. 在&#x200B;**父專案**&#x200B;欄位中，開始輸入專案名稱，該專案包含您想要成為目前任務的前置任務之任務。
1. 當名稱出現在下拉式清單中時，按一下該名稱。
1. 在&#x200B;**任務**&#x200B;欄位中，開始輸入您想要當做目前任務的前置任務之任務的名稱。
1. 指定下列資訊以定義前置任務與相依任務之間的關係：


   * **相依性型別：**&#x200B;選取您要前置任務與相依任務之間的關係。 預設關係為「完成 — 開始」，這表示前置任務必須先完成，相依任務才能開始。 如需各種相依性型別的詳細資訊，請參閱[工作相依性型別的概觀](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。

   * **延遲：**&#x200B;指定在強制前置任務完成後必須經過的時間長度，直到相依任務可以開始為止。 如需各種延遲型別的詳細資訊，請參閱[延遲型別概觀](../../../manage-work/tasks/use-prdcssrs/lag-types.md)。

   * **強制：**&#x200B;選取此選項時，使用者無法提早開始工作，以迴避兩個工作之間的相依關係。 例如，如果您強制任務A和任務B之間的關係，則任務B要等到任務A完成之後才能開始。 如需強制前置任務的詳細資訊，請參閱[強制前置任務](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md)。

     未選取此選項時，相依性會被視為對使用者的建議。 例如，使用者可以在任務A完成之前啟動任務B。

1. 按一下「**儲存**」。

   具有跨專案前置任務的任務會在任務清單的「前置任務」欄中顯示前置任務所屬專案的參考編號，以及任務編號（以冒號分隔）。

   ![跨專案前置任務](assets/cross-project-predecessor-in-list-view.png)

   前置任務被標示為完成時，前置任務圖示會變成綠色。 這表示相依任務已準備好工作。

   將滑鼠指標暫留在此值上，即可取得前置任務、專案和日期的詳細資訊。 按一下詳細資訊方塊中的跨專案前置任務以開啟任務。

   按一下游標停留視窗頂端附近的，檢視有關前置任務專案的詳細資訊。

   按一下&#x200B;**檢視專案**&#x200B;以開啟前置任務的專案。

   ![跨專案前置任務詳細資料](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   **檢視專案**&#x200B;選項僅在檢視跨專案前置任務時顯示。

