---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: 設定Kanban
description: 您在中建立Kanban或Scrum敏捷團隊 [!DNL Adobe Workfront].
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 1%

---

# 設定 [!UICONTROL Kanban]

您可以在中建立敏捷團隊 [!DNL Adobe Workfront] 如所述 [建立敏捷團隊](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md). 建立敏捷團隊時，您可以選擇團隊用來完成其工作的方法。 您可以從下列選項中選擇：

* Scrum
* Kanban

本文會說明如何設定Kanban團隊的設定。 建立敏捷團隊並選擇Kanban方法之後，您可以參閱本文章以更新以下設定：

* 劇本是以點還是小時為單位進行預估
* 敏捷故事板上的狀態列
* 要在敏捷故事板上顯示在故事卡上的其他欄位
* 進行中的工作(WIP)限制
* 如何自動從待處理專案新增劇本
* 卡片在Kanban板上停留多久

如需有關設定Scrum群組的資訊，請參閱 [設定Scrum](../get-started-with-agile-in-workfront/configure-scrum.md).

## 存取需求

<!--Audited: 12/2023-->

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>新增：[！UICONTROL Standard]</p> 
   或
   <p>目前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">存取層級</td> 
   <td> <p>編輯團隊的存取權</p>  </td> 
  </tr>

</tbody> 
</table>

*若要瞭解您擁有的計畫或授權型別，請連絡 [!DNL Workfront] 管理員。

## 設定是否要以點或小時為單位估計劇本

您可以設定劇本以使用點數或小時進行預估。

若要設定如何估計敏捷團隊的故事：

{{step1-to-team}}

1. 按一下 **[!UICONTROL 切換群組]** 圖示 ![](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊或在搜尋方塊中搜尋團隊。
1. 選取您要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![](assets/more-menu.png) ，然後選取 **[!UICONTROL 編輯]**.

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 區段，在 **[!UICONTROL 預估劇本在]** 區域，選取您是否要使用點或小時來預估內文的大小（工作負載）。 如果您選取「點」，請指定多少小時等於1點。 （預設值為1點= 8小時。） 這是新增到劇本的計畫時數。

   **範例：** 如果您已選取以點為單位來預估劇本，而1點等於8小時，則預估劇本為3點，則系統會將24個計畫小時新增至劇本。

1. 按一下「**[!UICONTROL 儲存變更]**」。

## 在敏捷故事板上設定狀態列

您可以為敏捷團隊定義故事板上的狀態。 這是唯一會顯示在故事板上的狀態。

若要定義與敏捷團隊相關劇本面板可用的狀態：

{{step1-to-team}}

1. 按一下 **[!UICONTROL 切換群組]** 圖示 ![切換團隊圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊或在搜尋列中搜尋團隊。

1. 選取您要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表，然後選取 **[!UICONTROL 編輯]**.

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 區段，找出 **[!UICONTROL 劇本面板]** 區域。

1. （選用）按一下 **[!UICONTROL 新增欄]** 將額外的狀態列新增到劇本面板。
1. （選擇性）使用拖放指示器拖曳任何狀態列，以重新排序內文板上的狀態列。 第一欄無法移動，而且您無法將另一欄拖到第一欄的前面。

   ![拖放](assets/agile-story-card-drag-and-drop.png)

1. 選取工作狀態。

   >[!IMPORTANT]
   >
   >只有鎖定的系統範圍狀態可供選取。 您無法選取群組特定的狀態。 第一欄的狀態一律對應至 **[!UICONTROL 新增]**.

   您可以新增自訂狀態，如果 [!DNL Workfront] 管理員已設定它們。 如需詳細資訊，請參閱 [建立或編輯狀態](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. 按一下「**[!UICONTROL 儲存變更]**」。

## 設定要在敏捷故事板上顯示在故事卡上的其他欄位

當您新增欄位到內文卡時，欄位是僅供檢視的，並且只有在填入欄位時才顯示。

預設情況下，以下型別的資料會顯示在任務和問題的劇本卡片上：

* 內文名稱，內有直接指向任務或問題的連結
* 含有直接連結至專案的專案名稱
* 此連結僅針對內文顯示，不針對子任務顯示
* 任務或問題說明
* 目前承諾
* 檢視並編輯完成百分比，方法是調整完成百分比本身，或調整完成點數或時數
* 已指派的使用者

您可以在故事卡上顯示其他資料（包括自訂資料）。 基於各種原因，您可能會想要在內文卡上顯示額外的欄位。 例如，如果您正在疊代內為多個客戶撰寫內文，或想要顯示專案開始日期或專案完成日期，您可能會想要顯示客戶ID。

>[!NOTE]
>
>如果您在內文卡上使用自訂欄位，則名稱中不能包含句點（或點）。

若要設定指派給敏捷團隊的內文卡以顯示其他欄位：

{{step1-to-team}}

1. 按一下 **[!UICONTROL 切換群組]** 圖示 ![切換團隊圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊或在搜尋列中搜尋團隊。

1. 選取您要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表，然後選取 **[!UICONTROL 編輯]**.\

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 區段，輸入欄位名稱以尋找該區段。

   ![其他欄位](assets/agile-additional-fields-kanban.png)

1. 選取您要新增的欄位名稱。
1. 輸入 **[!UICONTROL 顯示名稱]** ，以便在本文或問題卡上顯示的欄位。
1. 按一下「**[!UICONTROL 儲存變更]**」。

## 設定進行中的工作(WIP)限制

當您定義Kanban小組的WIP限制時，您可以藉由限制可在 [!UICONTROL 新增] 或 [!UICONTROL 進行中] 上的欄 [!UICONTROL Kanban] 展示板。

設定Kanban團隊的在製品限制後，您可以檢視在製品限制，並從 [!UICONTROL Kanban] 敏捷故事板，如中所述 [管理上的進行中工作(WIP)限制 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

若要限制看板團隊的在製品，請執行下列步驟：

{{step1-to-team}}

1. 按一下 **[!UICONTROL 切換群組]** 圖示 ![切換團隊圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊或在搜尋列中搜尋團隊。

1. 選取您要管理的Kanban團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![](assets/more-menu.png)，然後選取 **[!UICONTROL 編輯]**.

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 區段，在 **[!UICONTROL 方法]** 區段，確定已選取Kanban。

1. 在 **[!UICONTROL 劇本面板]** 區段，在 **[!UICONTROL 在製品限制]** 欄位中，指定每個欄位允許的專案數上限。 [!UICONTROL Kanban] 敏捷故事板。 您可以為每個欄設定不同的限制。 您可以為每個欄設定的最大限製為100。\
   設定後，在製品限制會在 [!UICONTROL Kanban] 敏捷故事板任何時候超過故事板任何欄的限制。 此警告訊息只會在第一次超過WIP限制時顯示。 此警告訊息不會顯示在任何具有相等狀態的欄上 [!UICONTROL 完成].\
   WIP限制只是視覺上的警告，不會限制您的團隊在單一欄中有超過您設定的限制以上的專案。

   ![WIP限制](assets/wip-limit-350x193.png)

1. 按一下「**儲存變更**」。

## 設定從待處理專案自動新增劇本

<!-- this functionality needs to be verified-->

您可以設定待處理專案中的劇本，以自動新增至 [!UICONTROL Kanban] 在專案從該欄移動之後立即顯示板。

{{step1-to-team}}

1. 按一下 **[!UICONTROL 切換群組]** 圖示 ![切換團隊圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊或在搜尋列中搜尋團隊。

1. 選取您要管理的Kanban團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![](assets/more-menu.png)，然後選取 **[!UICONTROL 編輯]**.

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 選取 **[!UICONTROL 自動從待處理專案新增下一個劇本]** 設定待處理專案中的下一個專案自動新增至 **[!UICONTROL 新增]** 欄(當專案移出 **[!UICONTROL 進行中]** 欄。

   使用者必須啟用 **顯示待處理專案** 設定 [!UICONTROL Kanban] 讓此功能生效。 當使用者啟用 [!UICONTROL 顯示待處理專案] 設定 [!UICONTROL Kanban面板]，接著會發生下列功能：

   任何時候將劇本從 [!UICONTROL 進行中] 欄放入故事板上的欄，代表 [!UICONTROL 完成] 狀態（或相等的狀態） [!UICONTROL 完成])，待處理專案欄中的劇本會自動移至 [!UICONTROL 新增] 的欄 [!UICONTROL Kanban面板].
從待處理專案新增時，具有最高優先順序的內文會新增到內文板中。

1. 按一下「**[!UICONTROL 儲存變更]**」。

## 設定卡片在網站上停留的時間 [!UICONTROL Kanban] 展示板

您可以選擇完成的卡片在網站上停留的時間 [!UICONTROL Kanban] 展示板。 脫離的任務 [!UICONTROL Kanban] 展示板仍可在原始專案中存取。

{{step1-to-team}}

1. （可選）按一下 **[!UICONTROL 切換群組]** 圖示 ![切換團隊圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Kanban團隊或在搜尋列中搜尋團隊。
1. 選取Kanban團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![](assets/more-menu.png) ，然後選取 **[!UICONTROL 編輯]**.

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 已完成天數卡會保留在Kanban板上]** 從下拉式選單中選取一個值。

   您可以選擇1到30天之間的數字。
1. 按一下「**[!UICONTROL 儲存變更]**」。
