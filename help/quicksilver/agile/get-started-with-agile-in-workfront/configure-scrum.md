---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: 設定Scrum
description: 您可以在團隊建立期間或之後，為Scrum敏捷團隊設定以下選項。
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 3c5bcb85080a882a8b69bffcd01563a0479f98a5
workflow-type: tm+mt
source-wordcount: '1793'
ht-degree: 0%

---

# 設定 [!UICONTROL Scrum]

您可以在中建立敏捷團隊 [!DNL Adobe Workfront] 如所述 [建立敏捷團隊](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md). 建立敏捷團隊時，您可以選擇團隊用來完成其工作的方法。 您可以從下列選項中選擇：

* Scrum
* Kanban

本文會說明如何設定Scrum群組的設定。 建立敏捷團隊並選擇Scrum方法之後，您可以參閱本文章以更新以下設定：

* 劇本是以點還是小時為單位進行預估
* 敏捷故事板上的狀態列，用於疊代和專案
* 要在敏捷故事板上顯示在故事卡上的其他欄位
* 如何在敏捷故事板上為故事使用顏色指示器
* 將工作專案新增至疊代時如何套用日期

如需有關設定Kanban團隊的資訊，請參閱 [設定Kanban](/help/quicksilver/agile/get-started-with-agile-in-workfront/configure-kanban.md).

## 存取需求

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

>[!NOTE]
>
>如果團隊有任何目前正在進行中的反複專案，則無法變更此設定。

您可以設定劇本以使用點數或小時進行預估。

若要設定如何估計敏捷團隊的故事：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!UICONTROL Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. 按一下 **[!UICONTROL 切換群組]** 圖示，然後從下拉式選單中選取新專案團隊或在搜尋列中搜尋專案團隊。
1. 選取您要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表，然後選取 **[!UICONTROL 編輯]**.

   僅限擁有下列任一專案的團隊成員： [!UICONTROL 計畫] 或 [!UICONTROL 工作] 授權請參閱此選項。\
   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 區段，在 **[!UICONTROL 預估劇本在]** 區域，選取您是否要使用點或小時來預估內文的大小（工作負載）。 如果您選取「點」，請指定多少小時等於1點。 （預設值為1點= 8小時。） 這是新增到劇本的計畫時數。

   **範例：** 如果您已選取以點為單位來預估劇本，而1點等於8小時，則預估劇本為3點，則系統會將24個計畫小時新增至劇本。

1. 按一下 **[!UICONTROL 儲存變更]**.

## 在敏捷故事板上設定狀態列

您可以針對指派給團隊的所有反複專案或特定專案，設定要在敏捷故事板上顯示哪些欄。

* [設定反複專案的狀態列](#configure-status-columns-for-iterations)
* [設定專案的狀態列](#configure-status-columns-for-projects)

### 設定反複專案的狀態列 {#configure-status-columns-for-iterations}

您可以為敏捷團隊定義故事板上的狀態。 這是唯一會顯示在故事板上的狀態。

若要定義與敏捷團隊相關劇本面板可用的狀態：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. 按一下 **[!UICONTROL 切換群組]** 圖示 ![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊或在搜尋列中搜尋團隊。

1. 選取您要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表，然後選取 **[!UICONTROL 編輯]**.

   僅限擁有下列任一專案的團隊成員： [!UICONTROL 計畫] 或 [!UICONTROL 工作] 授權請參閱此選項。

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 區段，找出 **[!UICONTROL 劇本面板]** 區域。

1. （選用）按一下 **[!UICONTROL 新增欄]** 將額外的狀態列新增到劇本面板。
1. （選擇性）使用拖放指示器拖曳任何狀態列，以重新排序內文板上的狀態列。 第一欄無法移動，而且您無法將另一欄拖到第一欄的前面。

   ![拖放](assets/agile-story-card-drag-and-drop.png)

1. 選取任務和問題狀態。 工作狀態會顯示為內文面板上每個欄的欄標題。 問題狀態您選擇對應到任務狀態。 這表示當您將問題移至故事板的另一個欄時，問題狀態會變更為此處顯示的問題狀態，而不是變成故事板上的欄名稱（反映任務狀態）。

   >[!IMPORTANT]
   >
   >只有鎖定的系統範圍狀態可供選取；您無法選取群組特定的狀態。 此外，第一欄的狀態一律與 **[!UICONTROL 新增]**.

   您可以新增自訂狀態，如果 [!DNL Workfront] 管理員已設定這些狀態；自訂狀態可依照中的說明進行設定 [建立或編輯狀態](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >選取問題狀態時，第三欄一律預設為 [!UICONTROL 已關閉]. 如果您有超過三欄，請確定您手動更新欄以反映適當的狀態。

1. 按一下 **[!UICONTROL 儲存變更]**.

### 設定專案的狀態列 {#configure-status-columns-for-projects}

如需如何設定專案之狀態列的詳細資訊，請參閱區段 [建立或自訂 [!UICONTROL 敏捷] 檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) 在文章中 [在中建立或編輯檢視 [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## 設定要在敏捷故事板上顯示在故事卡上的其他欄位

當您新增欄位到內文卡時，欄位在填入欄位時為僅限檢視和僅限顯示。

預設情況下，以下型別的資料會顯示在任務與問題的劇本卡片上：

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
>如果您在內文卡上使用自訂欄位，則名稱中不能包含句號/點。

若要設定指派給敏捷團隊的內文卡以顯示其他欄位：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!UICONTROL Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. 按一下 **[!UICONTROL 切換群組]** 圖示 ![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊或在搜尋列中搜尋團隊。

1. 選取您要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表，然後選取 **[!UICONTROL 編輯]**.\
   僅限擁有下列任一專案的團隊成員： [!UICONTROL 計畫] 或 [!UICONTROL 工作] 授權請參閱此選項。

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 區段，輸入欄位名稱以尋找該區段。

   ![其他欄位](assets/agile-additional-fields-scrum.png)

1. 選取您要新增的欄位名稱。
1. 輸入 **[!UICONTROL 顯示名稱]** ，以便在本文或問題卡上顯示的欄位。
1. 按一下 **[!UICONTROL 儲存變更]**.

## 設定如何使用顏色指標用於敏捷故事板上的故事

依預設，敏捷疊代中的內文板圖磚會根據內文關聯的專案進行色彩編碼。 每個專案都會任意指定故事板上的顏色。 您可以為每個敏捷團隊變更此預設行為。 敏捷內文的顏色可以與內文優先順序、所有者等繫結。

若要變更將顏色指派給敏捷團隊內文的行為：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. 按一下 **[!UICONTROL 切換群組]** 圖示 ![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊或在搜尋列中搜尋團隊。

1. 選取您要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表，然後選取 **[!UICONTROL 編輯]**.

   僅限擁有下列任一專案的團隊成員： [!UICONTROL 計畫] 或 [!UICONTROL 工作] 授權請參閱此選項。

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 [!UICONTROL 敏捷] 區段，在 [!UICONTROL 將卡片顏色關聯至] 區域，選取下列選項：

   * **[!UICONTROL 專案]**：顏色與內文繫結的專案相關聯。 (建立內文時，必須關聯至專案，如所述 [建立敏捷劇本](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). 來自相同專案的所有任務都會以相同顏色顯示。
   * **[!UICONTROL 自由格式]**：所有卡片預設都會顯示為藍色，直到使用者手動變更顏色為止，如所述 [[!UICONTROL 依色彩分類劇本] 在Scrum展示板上](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL 優先順序]**：顏色與內文優先順序相關聯，如下所示：

      * 高=紅色
      * 中=黃色
      * 低=綠色\

        如果您的系統管理員已設定您的自訂優先順序 [!DNL Workfront] 系統，最高優先順序為紅色，第二高為黃色，第三高為綠色。
   * **[!UICONTROL 任務擁有者]**：所有具有相同主要受指派人的劇本都是相同的色彩。 主要受指派人是首次受指派工作的使用者。


1. 按一下 **[!UICONTROL 儲存變更]**.

## 設定將工作專案新增至疊代時日期的套用方式

根據預設，當您將工作專案新增到Scrum反複專案時，會修改工作專案上的計劃開始日期和計畫完成日期，以符合反複專案的開始和結束日期。 您可以選擇保留團隊所有工作專案的原始日期。

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 團隊]**.
1. （可選）按一下 **[!UICONTROL 切換群組]** 圖示 ![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊或在搜尋列中搜尋團隊。
1. 按一下 **[!UICONTROL 更多]** 功能表，然後選取 **[!UICONTROL 編輯]**.\
   僅限擁有下列任一專案的團隊成員： [!UICONTROL 計畫] 或 [!UICONTROL 工作] 授權請參閱此選項。
1. 在 [!UICONTROL 敏捷] 區段，在 [!UICONTROL 當工作專案新增到疊代時] 區域，選取下列選項：

   * **[!UICONTROL 修改計劃開始日期和計畫完成日期以符合反複專案的開始和結束日期]**：當工作專案新增到疊代時，工作專案日期會變更為疊代日期。\

     如需日期修改方式的詳細資訊，請參閱區段 [瞭解新增劇本如何影響任務日期](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understa) 在文章中 [將劇本新增至現有反複專案](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL 請勿修改規劃開始日期和規劃完成日期以符合反複專案的開始和結束日期]**：將工作專案新增至疊代時，工作專案會保留其原始日期。

   如果您變更日期選項，則不會調整已在反複專案上的工作專案日期。

   這些選項會影響團隊將工作專案指派給彼此版序的日期。 例如，團隊A會將工作專案日期修改為版序日期，而團隊B不會修改工作專案日期。 如果專案團隊B指派工作專案給專案團隊A的疊代，則工作專案日期將會變更。 但是，如果專案團隊A指派工作專案給專案團隊B的疊代，日期將不會變更。

1. 按一下 **[!UICONTROL 儲存變更]**.
