---
product-area: reporting
navigation-topic: reporting-elements
title: 使用里程碑檢視
description: 您可以將里程碑檢視套用至專案清單或報表。
author: Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: dcdcf21903d0fceb3c05039689bb87ae4c834d07
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 1%

---

# 使用里程碑檢視

您可以將里程碑檢視套用至專案清單或報表。

您必須先設定里程碑，將里程碑路徑新增至專案，並將里程碑與任務建立關聯，如文章所述 [建立里程碑路徑](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) 和 [將里程碑與任務關聯](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

檢視專案清單或專案報表時，可使用「里程碑」檢視。 以下幾節將說明如何檢視和使用里程碑檢視。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>工作或更高 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>檢視或更高存取報表、控制面板、日曆</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>檢視專案報表的權限，以將「里程碑」檢視套用至報表</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 切換至里程碑檢視 {#switch-to-the-milestone-view}

1. 前往專案清單，或前往包含您要檢視里程碑的專案報表。
1. 按一下 **檢視** 下拉式功能表，然後按一下 **里程碑**.

   清單或報表會顯示在「里程碑」檢視中。

   如需里程碑檢視的相關資訊，請參閱區段 [里程碑檢視概述](#milestone-view-overview) 這篇文章。

## 里程碑檢視概述 {#milestone-view-overview}

「里程碑」視圖可用於項目清單和項目報告。 此檢視可讓您快速檢視與您檢視之專案內之任務相關聯的所有里程碑。


>[!NOTE]
>
>「里程碑」視圖不適用於以下區域：
>* 時間表，在添加項目時在項目清單中。



如需如何切換至「里程碑」檢視的詳細資訊，請參閱區段 [切換至里程碑檢視](#switch-to-the-milestone-view) 這篇文章。

![具有里程碑檢視的專案](assets/project-with-milestone-view-with-complete.png)

### 里程碑檢視區段

將「里程碑」視圖應用到項目清單時，項目將顯示在以下部分：

* 與「里程碑路徑」關聯的專案會先顯示，並列在其各自的「里程碑路徑」名稱下。

   Workfront會依下列條件，依此順序排序第一節中的專案：

   1. 里程碑路徑 ID. 您可以在「里程碑路徑」報表中檢視「里程碑路徑ID」。

   2. 在您選擇「里程碑」視圖之前，在以前應用於項目清單的視圖中，作為項目清單的第一個排序欄位選擇的欄位。

* 未與里程碑路徑關聯的項目隨即顯示在「未分配」部分。 Workfront會在您選取「里程碑」檢視之前，先根據在先前套用至專案清單的檢視中，為專案清單選取的第一個排序欄位，對「未指派」區段中的專案進行排序。

### 「里程碑」視圖中的項目資訊

在「里程碑」檢視中檢視專案清單或專案報表時，可使用下列資訊：

* **計畫日期或預計日期：** 指定您要在「里程碑」視圖中顯示「計畫日期」還是「預計日期」。\
   會顯示「開始」和「完成」的日期，以及「里程碑路徑」內每個「里程碑」的日期。\
   如果您正在查看計畫日期，並且您也擁有項目的「管理」訪問權限，則可以直接從「里程碑」視圖編輯以下日期：（如果您正在查看「預計日期」，則無法編輯日期，因為計算了「預計日期」，並且無法人工更改。）

   * **專案開始日期：** 如果從「開始日期」計畫了項目，則可以人工更改項目的「開始日期」，然後計算「完成日期」。
   * **項目完成日期：** 如果從完成日期開始計畫項目，則可以人工更改項目的完成日期，然後計算起始日期。
   * **任務完成日期：** 您可以直接從「里程碑」檢視手動更新任務的「完成」。

* **完成百分比：** 顯示每個任務和項目的完成百分比。\
   您可以停用不顯示完成百分比，如區段所述 [配置顯示在「里程碑」視圖中的資訊](#configure-what-information-displays-in-the-milestone-view) 這篇文章。\
   您可以直接從「里程碑」檢視調整完成百分比，如區段所述 [在「里程碑」視圖中調整任務的完成百分比](#adjust-percent-complete-for-tasks-in-the-milestone-view) 這篇文章。

* **任務狀態表徵圖：** 在「里程碑」視圖中，每個項目和任務旁將顯示一個狀態表徵圖。

   * 準時\
      ![](assets/gantt-ontime.png)

   * 滞後\
      ![](assets/gantt-behind.png)

   * 有風險\
      ![](assets/gantt-atrisk.png)

   * 延遲\
      ![](assets/gantt-late.png)
   您可以停用這些狀態圖示的顯示，如區段所述 [配置顯示在「里程碑」視圖中的資訊](#configure-what-information-displays-in-the-milestone-view) 這篇文章。\
   如需每個狀態類型的詳細資訊，請參閱文章 [任務進度狀態概述](../../../manage-work/tasks/task-information/task-progress-status.md).

* **已完成任務的任務狀態底紋**:將任務標籤為「完成」後，任務的背景將在「里程碑」視圖中著色，以指示任務是按時完成還是延遲完成：

   * **任務列的紅色底紋**:進度狀態為時，任務的背景為紅色 **延遲**.

   * **任務列的綠色底紋**:進度狀態為時，任務的背景為綠色 **準時**.

* **「項目開始」和「完成」列的項目狀態底紋**:

   * **專案開始欄**:只有在填入「實際開始日期」時，「項目開始」列的背景才會是紅色或綠色：

      * **「項目開始」列的紅色底紋**:項目的「進度狀態」為紅色時，「項目開始」列的背景為紅色 **延遲**.

      * **「項目開始」列的綠色底紋**:當項目的「進度狀態」為 **準時**.
   * **項目完成列**:只有在填入「實際完成日期」時，「項目完成」列的背景才會為紅色或綠色：

      * **項目完成列的紅色底紋**:當項目的「進度狀態」為「 **延遲**.

      * **項目完成列的綠色底紋**:當項目的「進度狀態」為 **準時**.
   * 當任務的「進度狀態」為「風險」或「滯後」時，不會為「開始」和「完成」列分配顏色底紋。

   ![帶底紋的里程碑視圖](assets/milestone-view-with-shading.png)

* **專案名稱**:專案名稱會隨專案連結一起顯示。
* **專案條件圖示**:專案名稱旁會顯示圖示，指出專案的條件。

## 配置顯示在「里程碑」視圖中的資訊 {#configure-what-information-displays-in-the-milestone-view}

您可以設定下列元素是否顯示在「里程碑」檢視中：

* 進度狀態表徵圖
* 項目和任務完成百分比

依預設，會顯示專案狀態圖示和專案完成百分比。

您對這些選項所做的任何變更都只適用於您；其他使用者則不受影響。 您所做的變更會在您下次登入Adobe Workfront時保留。

要配置是否顯示項目狀態表徵圖和項目完成百分比：

1. 前往專案清單，或前往包含您要檢視里程碑的專案報表。
1. 按一下 **檢視** 下拉式功能表，然後按一下 **里程碑**.\
   如果您檢視的是Portfolio或方案內的專案清單，請選取 **里程碑** 子標籤。

1. 按一下 **選項** 在「里程碑」檢視的右上角。\
   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

1. 從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">進度狀態</td> 
      <td> <p>選擇此選項可顯示每個項目和任務旁邊的進度狀態表徵圖。</p> <p>預設會啟用此選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>選擇此選項可顯示每個項目和任務旁邊的完成百分比。</p> <p>預設會啟用此選項。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 在「里程碑」視圖中調整任務的完成百分比 {#adjust-percent-complete-for-tasks-in-the-milestone-view}

您可以在「里程碑」檢視中調整任務的「完成百分比」。 不能調整父任務（包含子任務的任務）的「完成百分比」。

要調整「里程碑」視圖中任務的完成百分比：

1. 前往專案清單，或前往包含您要檢視里程碑的專案報表。
1. 按一下 **檢視** 下拉式功能表，然後按一下 **里程碑**.

1. （條件性）如果「里程碑」檢視中未顯示完成百分比，請按一下 **選項** 在「里程碑」檢視的右上角，然後確定 **完成百分比** 啟用。

1. 按一下任務下方的完成百分比，指定新百分比，然後按Enter鍵。
