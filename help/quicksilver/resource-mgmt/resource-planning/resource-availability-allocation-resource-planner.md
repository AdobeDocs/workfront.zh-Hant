---
product-area: resource-management
navigation-topic: resource-planning
title: 使用Adobe Workfront資源計畫器複查資源可用性和分配
description: 您可以在資源計畫器中查看資源的可用性以及項目的計畫或預算工作量。 這些值以小時、FTE（相當於全職）或成本金額顯示，並按列組織。
author: Alina
feature: Resource Management
exl-id: 5b3e52a6-af9b-4e68-8d6e-43a5151a2a2c
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 4%

---

# 使用Adobe Workfront資源計畫器複查資源可用性和分配

您可以在資源計畫器中查看資源的可用性以及項目的計畫或預算工作量。 這些值以小時、FTE（相當於全職）或成本金額顯示，並按列組織。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>審核或更高版本 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視或更高存取權：</p> 
    <ul> 
     <li> <p>資源管理</p> </li> 
     <li> <p>財務資料</p> </li> 
     <li> <p>使用者</p> </li> 
     <li> <p>專案</p> </li> 
    </ul> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>在資源計畫員中查看要查看的項目的查看權限或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

<!--note from the table about the license: Review or higher: 
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (waiting on Vazgen to confirm - working differenly in classic)
      </MadCap:conditionalText>
     -->

## 必要條件

您必須滿足使用資源計畫員所需的所有先決條件。 如需詳細資訊，請參閱 [資源計畫員概覽](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

>[!IMPORTANT]
>
>如果缺少資源規劃器正確功能所需的任何先決條件，則某些數字可能為零，或預算小時數可能變灰。

## 資源的可用性和分配

顯示資源可用性和分配的列會根據您應用於資源計畫員的視圖而變化。 有關按項目、角色或用戶在資源計畫器中顯示資訊的資訊，請參閱 [資源計畫員導航概覽](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

將視圖更改為資源計畫員時，請考慮以下事項：

* 當您套用 **依專案檢視** 或&#x200B;**按角色查看** 檢視，您可以看到下列欄：

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: Alina: (some of the information in this area is also covered in Calculating Costs in the RP - https://workfront.zendesk.com/hc/en-us/articles/115004186433 - update this article also, when changes here occur)
  </MadCap:conditionalText>
  -->



   * 可用小時數、FTE或成本
   * 計畫小時數、FTE或成本
   * 預算小時數、FTE或成本
   * 小時數、FTE或成本差異
   * 淨小時數、FTE或成本

* 當您套用 **按用戶查看** 檢視，您可以看到下列欄：

   * 可用小時數或FTE
   * 計畫小時數或FTE
   * 小時或FTE差異
   * 計畫時數分配百分比

>[!TIP]
>
>在應用 **按用戶查看** 查看資源計畫員。
>
>有關每列顯示內容的詳細資訊，請將滑鼠移到顯示數字的列的名稱上。\
>![Net_hours_res_planner_mouse_over.png](assets/net-hours-res-planner-mouse-over-350x95.png)
>
>如需各欄所顯示資料的詳細資訊，請參閱下列文章：
>
>* [資源計畫員的「項目」和「職責」視圖中的小時數、FTE和成本資訊概覽](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)
>* [使用「用戶」視圖時，查看資源計畫員中的可用小時數、計畫小時數和實際小時數或FTE](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)
>


## 按小時、FTE或成本查看資訊

1. 轉至資源計畫器。

   預設情況下，資訊按小時數顯示在資源計畫器中。

1. 展開下拉式功能表。\
   ![Hours_fte_or_cost_dropdown.png](assets/hours-fte-or-cost-dropdown.png)

1. 從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">時數</td> 
      <td>以小時顯示可用性和分配資訊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">FTE</td> 
      <td> <p>以FTE顯示可用性和分配資訊。</p> <p>有關在資源計畫員中如何計算FTE的詳細資訊，請參閱 <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">在資源計畫員中計算用戶和角色的小時數和FTE的概覽</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">成本</td> 
      <td> <p>如果在「項目」或「職責」視圖中查看「資源計畫員」，則按成本顯示可用性和分配資訊。 資訊會以您系統的貨幣顯示值。 您的Workfront管理員會定義系統貨幣。 如需在Workfront中設定系統貨幣的詳細資訊，請參閱 <a href="../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>.</p> <p><b>附註</b>

   您必須將用戶和任務職責與「每小時成本」費率關聯，以便在資源計畫員中顯示「成本」資訊。<br style="font-style: italic;">有關將「每小時成本」費率與任務職責關聯的詳細資訊，請參閱 <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a>.<br style="font-style: italic;">有關將「每小時成本」費率與用戶關聯的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>.<br style="font-style: italic;">有關如何在資源計畫器中計算成本的詳細資訊，請參閱 <a href="../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md" class="MCXref xref">在資源計畫器中計算成本 </a>.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">自訂</td> 
      <td>建立顯示在資源規劃器中的列的自定義視圖。 選擇要在資源計畫器中顯示的選項，如以下步驟所述。 </td> 
     </tr> 
    </tbody> 
   </table>

1. （條件性）如果您選取 **自訂**，表示 **自訂顯示的量度** 方塊來設定自訂檢視。

   ![](assets/planner-customize-view-box-350x114.png)

1. 在 **檢視類型** 欄中，選取下列其中一個檢視：

   * 專案
   * 角色
   * 使用者

1. 在 **顯示所選項目** 節，選擇要在選定視圖的列中顯示的資訊類型。 下表顯示每個檢視中可用的選項：

   | **選項** | 使用者檢視 | 專案檢視 | 角色視圖 |
   |---|---|---|---|
   | 可用 | ✔ | ✔ | ✔ |
   | 計畫 | ✔ | ✔ | ✔ |
   | 已編列預算 |   | ✔ | ✔ |
   | 差額 |   | ✔ | ✔ |
   | 淨餘 |   | ✔ | ✔ |
   | 實際 | ✔ |   |   |
   | 差異 | ✔ |   |   |
   | 百分比 | ✔ |   |   |

1. 選擇 **在NET計算中使用計畫值(PLN)** 在「項目」和「職責」視圖中計算「淨值」時，使用「計畫」資訊，而不是「預算」資訊。

   選取此選項時，Workfront會使用下列公式計算淨值：

   ```
   Net = Available - Planned
   ```

   >[!TIP]
   >
   >**只有當您選取至少一個選項來自訂「顯示選取的項目」區段中的檢視時，才會套用此選項。**

1. 按一下&#x200B;**儲存**。

   隨即顯示包含您所選欄的自訂檢視。

   「資源規劃器」在「小時」下拉菜單中將自定義視圖列為「自定義」。

   >[!NOTE]
   >
   >您只能有一個自訂檢視。

   ![](assets/planner-hours-drop-down-with-custom-and-customize-option-183x281.png)

## 查看用戶分配圖表

您可以根據使用者在圖表中的可用性，顯示使用者的「計劃分配」。

要在圖表中顯示用戶分配，請執行以下操作：

1. 轉至資源計畫器。

   有關訪問資源計畫員的詳細資訊，請參閱 [查找資源計畫員](../../resource-mgmt/resource-planning/get-started-resource-planner.md#accessing-the-resource-planner) 文章一節 [資源計畫員概覽](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

1. 選擇 **按用戶查看**.

   >[!TIP]
   >
   >您只能在「使用者檢視」中檢視「使用者配置」圖表。

1. 按一下 **用戶分配圖表** 圖示 ![RP_user_allocation_chart.png](assets/rp-user-allocation-chart.png) 顯示下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">所有使用者皆未過度配置的可用性 %</td> 
      <td>這是某個時段內所有使用者都可工作的時間量，以其可用時間總數的百分比顯示。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有使用者的過度配置 % </td> 
      <td> <p>這是一個時段內使用者被過度分配的時間量，以可用時間總數的百分比顯示。</p> <p><b>附註</b>

   當計畫小時數高於可用小時數時，會發生超額分配。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">所有使用者的使用量過低 %</td> 
      <td> <p>這是用戶在一個時間段內未充分利用的時間量，以佔總可用時間的百分比顯示。</p> <p><b>附註</b>

   當計畫小時數低於可用小時數時，會出現利用率不足。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">此時間期間內有至少一位使用者過度配置</td> 
      <td>這表示一個時段內至少有一個使用者有超額分配，不過該時段內並未過度分配所有使用者的總時間量。<br>您必須捲動瀏覽使用者清單，而過分配之使用者的小時數會以紅色強調顯示。</td> 
     </tr> 
    </tbody> 
   </table>

   ![RP__user_allocation_chart_Dec._7__2017.png](assets/rp--user-allocation-chart-dec.-7--2017-350x148.png)

1. （選用）按一下 **所有用戶的超額分配%** 框中。\
   所有被過度分配的用戶都會以紅色突出顯示。
1. （選用）按一下 **所有用戶的利用率不足%** 框中。\
   所有未充分利用的用戶都以藍色突出顯示。

1. （選用）按一下指標圖示 ![one_user_overallocation_marker.png](assets/one-user-overallocation-marker.png) 這會顯示您至少有一個使用者被過度配置的位置。\
   被過度分配的用戶將以紅色突出顯示。

1. （選用）重新整理頁面以折疊圖表。
