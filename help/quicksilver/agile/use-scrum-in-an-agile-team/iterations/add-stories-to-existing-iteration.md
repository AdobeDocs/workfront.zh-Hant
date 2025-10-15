---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 新增劇本至現有反複專案
description: 您可以透過多種方式將劇本新增至反複專案。
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# 將劇本新增至現有反複專案

您可以透過下列任何方式將劇本新增至反複專案：

* 在建立疊代後，從待處理專案，如[管理敏捷待處理專案[!UICONTROL 中的]將劇本從待處理專案移至疊代，或](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board)看板[面板](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)區段所述

* 從個別任務或問題的[!UICONTROL 詳細資料]頁面
* 從任務或問題清單
* 從報表
* 從控制面板

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> 
   <p>工作或更高</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>管理內文所在專案的存取權 </td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 瞭解新增劇本如何影響任務日期

根據預設，當您新增現有任務至疊代時，任務的[!UICONTROL 計劃開始日期]和[!UICONTROL 計畫完成日期]設定如下：

### 任務[!UICONTROL 計劃開始日期]

* 在以下情況下，任務會使用反複專案的「開始日期」：

   * 專案未設定[!UICONTROL 計劃開始日期]。
   * 專案的[!UICONTROL 計劃開始日期]是&#x200B;**&#x200B;之前，或&#x200B;**&#x200B;反複專案的開始日期。

* 任務在下列情況下使用專案的[!UICONTROL 計劃開始日期]：

   * 專案的[!UICONTROL 計劃開始日期]是&#x200B;*晚於*&#x200B;反複專案的開始日期。

### 任務[!UICONTROL 計畫完成日期]

* 在以下情況下，任務會使用反複專案的「結束日期」：

   * 專案未設定[!UICONTROL 計畫完成日期]。
   * 專案的[!UICONTROL 計劃開始日期]是&#x200B;*在或是*&#x200B;反複專案的開始日期或專案的[!UICONTROL 計畫完成日期]是&#x200B;*在或是*&#x200B;反複專案的結束日期。

* 任務在下列情況下使用專案的[!UICONTROL 計畫完成日期]：

   * 專案的[!UICONTROL 計劃開始日期]是&#x200B;*在*&#x200B;反複專案的開始日期之後，專案的[!UICONTROL 計畫完成日期]是&#x200B;*在*&#x200B;反複專案的結束日期之後。

您可以設定個別Scrum團隊以預設使用專案日期，而不是反複專案日期。 如需詳細資訊，請參閱[設定Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration)一文中的[設定將工作專案新增至疊代](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)時如何套用日期一節。

## 將劇本新增至現有反複專案

如果您擁有專案的管理存取權，您可以將任何任務或問題新增到任何反複專案。 將任務或問題移動至疊代時，請記住下列事項：

* 如果您新增多個團隊，任務或問題只能顯示在一個團隊的疊代上。 這是您在步驟3中選擇的版序。
* 如果任務或問題指派給敏捷團隊並移動到另一個團隊的疊代，則團隊指派不會改變。
* 如果任務或問題未指派給團隊，則會將任務或問題指派給擁有疊代的團隊。
* 您無法將父系任務新增至疊代。 如果您新增任何子系任務，父系任務就會在Scrum展示板上顯示為泳道。

>[!IMPORTANT]
>
>任務移至疊代後，您無法更新[!UICONTROL 期間型別]或[!UICONTROL 任務限制]。 [!UICONTROL 期間型別]設定為[!UICONTROL 簡單]，而[!UICONTROL 任務限制]設定為[!UICONTROL 固定日期]，以保持任務時間表與反複專案的時間表一致。

1. 開啟您要新增至疊代的任務或問題。
或
前往專案、報告或儀表板，其中包含您要新增至疊代的任務或問題。 然後，選取一或多個任務或問題。

1. 按一下&#x200B;**[!UICONTROL 更多]** ![更多圖示](assets/more-icon.png) > **[!UICONTROL 新增到反複專案]**。
您無法將任務或問題指派給非敏捷團隊。

1. 在&#x200B;**[!UICONTROL 新增至]**&#x200B;方塊中，開始輸入反複專案的名稱，並在它出現在清單中時選取它。

   >[!NOTE]
   >
   >您可以將內文從現有的反複專案移至新的反複專案。

1. 按一下&#x200B;**[!UICONTROL 新增]**。
