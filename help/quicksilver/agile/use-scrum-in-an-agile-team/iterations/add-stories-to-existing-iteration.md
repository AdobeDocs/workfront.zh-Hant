---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 將動態添加到現有小版本
description: 您可以以多種方式將動態添加到小版本。
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 將動態添加到現有小版本

您可以通過以下任何方式將文章添加到小版本：

* 從建立小版本後的積壓，如 [將動態從積壓工作移至小版本或 [!UICONTROL 看板] 展示板](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) 區段 [管理敏捷積壓](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* 從 [!UICONTROL 詳細資料] 個別任務或問題的頁面
* 從任務或問題清單
* 從報表
* 從控制面板

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL工作]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>[!UICONTROL管理]對文章所在項目的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 了解新增動態如何影響工作日期

預設情況下，將現有任務添加到小版本時，該任務的 [!UICONTROL 計劃開始日期] 和 [!UICONTROL 計畫完成日期] 設定如下：

### 任務 [!UICONTROL 計劃開始日期]

* 在以下情況下，任務將使用小版本的開始日期：

   * 專案沒有 [!UICONTROL 計劃開始日期] 設定。
   * 專案的 [!UICONTROL 計劃開始日期] is *befor* 或 *on* 迭代的開始日期。

* 任務使用項目的 [!UICONTROL 計劃開始日期] 時間：

   * 專案的 [!UICONTROL 計劃開始日期] is *after* 迭代的開始日期。

### 任務 [!UICONTROL 計畫完成日期]

* 在下列情況下，任務將使用小版本的「結束日期」(End Date):

   * 專案沒有 [!UICONTROL 計畫完成日期] 設定。
   * 專案的 [!UICONTROL 計劃開始日期] is *在之前或在* 小版本的開始日期或項目的 [!UICONTROL 計畫完成日期] is *在之前或在* 迭代的結束日期。

* 任務使用項目的 [!UICONTROL 計畫完成日期] 時間：

   * 專案的 [!UICONTROL 計劃開始日期] is *after* 小版本的「開始日期」和項目的 [!UICONTROL 計畫完成日期] is *after* 迭代的結束日期。

您可以設定個別Scrum團隊，依預設使用專案日期，而非迭代日期。 如需詳細資訊，請參閱 [配置將工作項添加到小版本時如何應用日期](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 在文章中 [配置Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## 將文章添加到現有小版本

要直接從任務或問題向小版本添加動態，請執行以下操作：

>[!IMPORTANT]
>
>任務移動到小版本後，無法更新 [!UICONTROL 持續時間類型] 或 [!UICONTROL 任務約束]. [!UICONTROL 持續時間類型] 設為 [!UICONTROL 簡單] 和 [!UICONTROL 任務約束] 設為 [!UICONTROL 固定日期] 使任務時間軸與迭代的時間軸一致。

### 從任務或問題頁簽

如果您對項目具有「管理」訪問權限，則可以將任何任務或問題添加到任何小版本。 將任務或問題移至小版本時，請牢記以下事項：

* 如果添加多個團隊，則任務或問題只能顯示在一個團隊的小版本上。 這是您在下面的步驟3中選擇的小版本。
* 如果將任務或問題分配給敏捷團隊，並移至另一個團隊的小版本，則團隊分配不會更改。
* 如果未將任務或問題分配給小組，則將任務或問題分配給擁有小版本的小組。
* 不能向小版本添加父任務。 如果添加任何子任務，則父任務將作為游泳道顯示在Scrum板上。

1. 轉到包含要添加到小版本的任務或問題的項目、報告或控制面板。
1. 選取一或多個工作或問題。
1. 按一下 **[!UICONTROL 更多]** ![](assets/more-icon.png) > **[!UICONTROL 添加到小版本]**.\
   您無法指派指派指派給非敏捷團隊的任務或問題。

1. 在 **[!UICONTROL 新增動態]** 框中，鍵入小版本的名稱。

   >[!NOTE]
   >
   >您可以將文章從現有小版本移動到新小版本。

1. 如果要添加任務，請按一下 **[!UICONTROL 新增動態]**.\
   或\
   如果您新增問題，請按一下 **[!UICONTROL 新增問題]**.
