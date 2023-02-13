---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: 配置Scrum
description: 您可以在建立團隊期間或之後，為Scrum靈活團隊設定下列選項。
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 0%

---

# 設定 [!UICONTROL Scrum]

您可以在建立團隊期間或之後，為敏捷團隊配置下列選項。 在以下位置建立敏捷小組（看板或看板） [!DNL Adobe Workfront] 如 [建立敏捷的團隊](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL工作]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請連絡您的 [!DNL Workfront] 管理員。

## 設定是以點還是小時來預估動態

>[!NOTE]
>
>如果團隊有任何當前正在進行的迭代，則無法更改此設定。

您可以設定使用點或小時來預估動態。

要配置如何為您敏捷的團隊估計故事：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!UICONTROL Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. 按一下 **[!UICONTROL 交換組]** 表徵圖，然後從下拉菜單中選擇新團隊，或在搜索欄中搜索團隊。
1. 選擇要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** ，然後選取 **[!UICONTROL 編輯]**.

   僅包含 [!UICONTROL 計畫] 或 [!UICONTROL 工作] 許可證請參閱此選項。\
   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 區段中 **[!UICONTROL 預估中的動態]** 區域中，選擇是否要使用點或小時來估計文章的大小（工作負載）。 如果選擇「點」(Points)，請指定多少小時等於1點。 （預設為1點= 8小時。） 這是新增至動態的「計畫小時數」。

   **範例：** 如果您選擇以點數估計動態，而1點等於8小時，且動態估計為3點，則會在動態中新增24個計畫小時。

1. 按一下 **[!UICONTROL 儲存變更]**.

## 在敏捷動態展示板上設定狀態欄

您可以針對指派給您團隊的所有迭代項目或指定專案，設定在敏捷動態展示板上顯示的欄。

* [配置小版本的狀態列](#configure-status-columns-for-iterations)
* [設定專案的狀態欄](#configure-status-columns-for-projects)

### 配置小版本的狀態列 {#configure-status-columns-for-iterations}

您可以為敏捷團隊定義動態板上存在的狀態。 這些是顯示在動態板上的唯一狀態。

要定義與敏捷團隊關聯的故事板可用的狀態：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. 按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊，或在搜尋列中搜尋團隊。

1. 選擇要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** ，然後選取 **[!UICONTROL 編輯]**.

   僅包含 [!UICONTROL 計畫] 或 [!UICONTROL 工作] 許可證請參閱此選項。

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 區段，找到 **[!UICONTROL 展示板]** 的上界。

1. （選用）按一下 **[!UICONTROL 添加列]** 新增其他狀態欄至動態板。
1. （可選）使用拖放指示器拖曳任何狀態欄，以重新排序動態展示板上的狀態欄。 無法移動第一列，並且不能拖動第一列前面的另一列。

   ![拖放](assets/agile-story-card-drag-and-drop.png)

1. 選擇任務和問題狀態。 任務狀態會顯示為動態板上各欄的欄標題。 您選擇的問題狀態映射至任務狀態。 這表示當您將問題移至動態展示板的其他欄時，問題狀態會變更為此處顯示的問題狀態，而非動態展示板上的欄名稱（反映任務狀態）。

   >[!IMPORTANT]
   >
   >只有鎖定的全系統狀態可供選擇；您無法選取群組特定狀態。 此外，第一欄的狀態一律對應至 **[!UICONTROL 新增]**.

   若您的 [!DNL Workfront] 管理員已配置它們；自訂狀態可依 [建立或編輯狀態](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >選擇問題狀態時，第三欄一律預設為 [!UICONTROL 已關閉]. 如果有三個以上的欄，請確定您手動更新欄以反映正確的狀態。

1. 按一下 **[!UICONTROL 儲存變更]**.

### 設定專案的狀態欄 {#configure-status-columns-for-projects}

如需如何設定專案狀態欄的相關資訊，請參閱區段 [建立或自訂 [!UICONTROL 敏捷] 檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) 在文章中 [在中建立或編輯視圖 [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## 設定其他欄位，以顯示在敏捷動態展示板上的動態資訊卡上

將欄位新增至動態卡片時，欄位是僅供檢視，填入欄位時則僅供顯示。

根據預設，任務和問題的動態卡片上會顯示以下類型的資料：

* 與任務或問題直接連結的動態名稱
* 具有直接連結至專案的專案名稱
* 此連結只會針對動態顯示，不會針對子工作顯示
* 任務或問題說明
* 當前承諾
* 通過調整完成百分比本身或通過調整完成的點數或小時數來查看和編輯完成百分比
* 已指派的使用者

您可以在動態卡片上顯示其他資料（包括自訂資料）。 基於任何原因，您可能想在動態卡上顯示其他欄位。 例如，如果正在迭代內為多個客戶處理動態，或想顯示「項目開始日期」或「項目完成日期」，則可能想要顯示「客戶ID」。

>[!NOTE]
>
>如果您在動態卡片上使用自訂欄位，名稱中不能包含句點/點。

要配置分配給敏捷團隊的動態資訊卡，以顯示其他欄位：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!UICONTROL Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. 按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊，或在搜尋列中搜尋團隊。

1. 選擇要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** ，然後選取 **[!UICONTROL 編輯]**.\
   僅包含 [!UICONTROL 計畫] 或 [!UICONTROL 工作] 許可證請參閱此選項。

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 **[!UICONTROL 敏捷]** 區段，輸入欄位名稱以找到它。

   ![其他欄位](assets/agile-additional-fields-scrum.png)

1. 選取您要新增的欄位名稱。
1. 輸入 **[!UICONTROL 顯示名稱]** 讓欄位顯示在動態或發卡上。
1. 按一下 **[!UICONTROL 儲存變更]**.

## 設定如何在敏捷動態展示板上為動態使用顏色指標

依預設，敏捷小版本中的文章展示板圖磚會根據文章關聯的專案進行色彩編碼。 每個專案在展示板上都會任意指定顏色。 您可以變更每個敏捷團隊的預設行為。 敏捷故事的色彩可以與故事優先順序、擁有者等相關聯。

若要變更為敏捷團隊的動態指派顏色的行為：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. 按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新團隊，或在搜尋列中搜尋團隊。

1. 選擇要管理的敏捷團隊。
1. 按一下 **[!UICONTROL 更多]** ，然後選取 **[!UICONTROL 編輯]**.

   僅包含 [!UICONTROL 計畫] 或 [!UICONTROL 工作] 許可證請參閱此選項。

   ![編輯團隊](assets/edit-team-settings-350x205.png)

1. 在 [!UICONTROL 敏捷] 區段中 [!UICONTROL 將卡片顏色關聯至] ，請從以下選項中選擇：

   * **[!UICONTROL 專案]**:顏色與文章所系結的專案相關聯。 (文章建立時，必須與專案相關聯，如 [建立敏捷故事](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). 同一項目中的所有任務都以相同的顏色顯示。
   * **[!UICONTROL 自由格式]**:在使用者手動變更顏色之前，所有卡片預設會顯示為藍色，如 [[!UICONTROL 依顏色分類動態] 在Scrum板上](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL 優先順序]**:顏色與文章優先順序相關聯，如下所示：

      * 高=紅色
      * 中=黃色
      * 低=綠色\

         如果系統管理員已為 [!DNL Workfront] 系統中，最高優先順序為紅色，第二最高為黃色，第三最高為綠色。
   * **[!UICONTROL 任務所有者]**:所有與相同主要受託人的動態顏色相同。 主要受託人是第一次分配給任務的用戶。


1. 按一下 **[!UICONTROL 儲存變更]**.

## 配置將工作項添加到小版本時如何應用日期

預設情況下，在將工作項添加到Scrum小版本時，將修改工作項上的計畫起始日期和計畫完成日期，以匹配小版本的起始日期和終止日期。 您可以選擇保留團隊所有工作項的原始日期。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 團隊]**.
1. （選用）按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊，或在搜尋列中搜尋團隊。
1. 按一下 **[!UICONTROL 更多]** ，然後選取 **[!UICONTROL 編輯]**.\
   僅包含 [!UICONTROL 計畫] 或 [!UICONTROL 工作] 許可證請參閱此選項。
1. 在 [!UICONTROL 敏捷] 區段中 [!UICONTROL 將工作項添加到小版本時] ，請從以下選項中選擇：

   * **[!UICONTROL 修改計畫起始日期和計畫完成日期以匹配小版本起始日期和終止日期]**:將工作項添加到小版本時，工作項日期將更改為小版本日期。

      如需如何修改日期的詳細資訊，請參閱區段 [了解新增動態如何影響工作日期](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understa) 在文章中 [將動態添加到現有小版本](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL 不要修改計畫起始日期和計畫完成日期以匹配小版本起始日期和終止日期]**:將工作項添加到小版本時，工作項將保留其原始日期。

   如果更改日期選項，則不會調整小版本上已在工作項的日期。

   這些選項會影響團隊將工作項目指派給彼此迭代的日期。 例如，團隊A將工作項日期修改為小版本日期，而團隊B不修改工作項日期。 如果B組將工作項分配給A組的小版本，則工作項日期將更改。 但是，如果A組將工作項分配給B組的小版本，則日期不會更改。

1. 按一下 **[!UICONTROL 儲存變更]**.
