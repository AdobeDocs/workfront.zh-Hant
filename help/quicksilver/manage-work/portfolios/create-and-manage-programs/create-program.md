---
product-area: programs
navigation-topic: create and manage programs
title: 建立方案
description: 方案代表共用跨專案界限的共同策略、目標或目標的專案集合。 程式不能存在於投資組合之外。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
source-git-commit: e4cd543aa9f47e6b93aa148ea3fb972fbd356c02
workflow-type: tm+mt
source-wordcount: '998'
ht-degree: 1%

---

# 建立方案

<!-- Audited: 1/2024 -->

方案代表共用跨專案界限的共同策略、目標或目標的專案集合。 程式不能存在於投資組合之外。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>新增：任何</p><p>或</p><p>目前： [！UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>新增：[！UICONTROL Standard] </p><p>或 </p><p>目前： [！UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>[！UICONTROL Edit]對Portfolio和計畫的存取權 </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>投資組合的[！UICONTROL Manage]許可權</p> <p>建立方案後，預設情況下您擁有[！UICONTROL管理]許可權。</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 建立方案

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 左上角。

1. 執行下列任一項作業。

   * 從建立方案 [!UICONTROL 計畫] 區域：

      1. 按一下 **[!UICONTROL 計畫]** 在主要功能表中。
      1. 按一下 **[!UICONTROL 新計畫]**.
      1. 在顯示的方塊中，輸入現有Portfolio的名稱 **[!UICONTROL 選取Portfolio]** 欄位。
      1. 在「 」中輸入新方案的名稱 **[!UICONTROL 名稱]** 欄位。
      1. 按一下「**[!UICONTROL 儲存]**」。
   * 從建立方案 [!UICONTROL Portfolio] 區域：

      1. 按一下 **[!UICONTROL Portfolio]** 在 [!UICONTROL 主要功能表]，然後開啟投資組合。
      1. 在左側面板中，按一下 **[!UICONTROL 計畫]**.
      1. 按一下 **[!UICONTROL 新計畫]** 下拉式功能表，然後 **[!UICONTROL 新計畫]**.


1. （視條件而定）如果您是從投資組合建立方案，請在 **[!UICONTROL 未命名的計畫]** 欄位。

   名稱最多可包含255個字元。

1. （選用）按一下 **[!UICONTROL 計畫管理員]** 在計畫的標題中進行更新。

   >[!TIP]
   >
   >作為方案的建立者，預設會將您設定為「方案管理員」。

1. 按一下 **[!UICONTROL 計畫詳細資訊]** 在左側面板中。
1. 連按兩下任何欄位以更新 **[!UICONTROL 概觀]** 區域。

您可以指定下列資訊：

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>欄位</th> 
      <th>說明</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL說明]</td> 
      <td> <p>指定程式的說明。</p> <p>說明會顯示在程式的登陸頁面上。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL計畫管理員]</td> 
      <td> <p>開始輸入您想當作「方案管理員」的使用者名稱，然後在使用者名稱出現在下拉式清單中時按一下該使用者的名稱。 這與[！UICONTROL計畫所有者]相同。 </p> <p>提示：您也可以在方案標題中更新「方案管理員」。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL群組] </td> 
      <td> <p>如果群組擁有方案或負責完成方案，請新增單一群組的名稱。 </p> <p>您可以暫留在正確的群組上，並按一下[！UICONTROL資訊]圖示，確定您選取的群組正確 <img src="assets/info-icon.png"> 隨即顯示。 這會顯示工具提示，列出群組的相關資訊，例如群組及其管理員上方的群組階層。</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性和條件性）按一下 **[!UICONTROL 新增自訂表格]** 方塊來選取投資組合的自訂表單並更新自訂欄位。

   >[!TIP]
   >
   >您必須先建立程式自訂表單，才能將其附加至程式。

1. （選擇性和條件性）如果您新增自訂表單，請按一下自訂表單上的任何欄位以更新該欄位中的資訊。
1. 按一下「**[!UICONTROL 儲存變更]**」。
1. 按一下 **[!UICONTROL 專案]** 在左側面板中，然後 **[!UICONTROL 新增專案]** 將專案新增至方案。

   如需有關將專案新增至方案的資訊，請參閱 [將專案新增至方案](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. 按一下「**[!UICONTROL 儲存變更]**」。
1. （可選）按一下 **[!UICONTROL 更多選單]** ![](assets/more-icon.png) 在程式名稱旁邊，然後按一下 **[!UICONTROL 停用計畫]**.

   停用方案時，當使用者嘗試將方案新增到專案時，方案不再顯示在方案清單中。 您仍然可以從以下位置存取該計畫： [!UICONTROL 計畫] 區域。

## 計畫標題總覽

您可以在計畫標題中找到一些有關計畫的資訊。

下列資訊會顯示在方案的標頭中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">頁首資訊</td> 
   <td> <strong>附註</strong> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">包含產品組合名稱的階層連結</td> 
   <td>您可以從方案標題存取方案所屬的投資組合。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">方案名稱</td> 
   <td>您可以在標題中編輯方案名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件型別名稱和啟動狀態</td> 
   <td>當您檢視方案時，「方案」一詞會顯示橘色圖示。 單字「[！UICONTROL已停用]」會顯示在其旁邊，如果程式未標示為[！UICONTROL作用中]，則大綱為灰色。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">計畫的動作區域 </td> 
   <td> <p>按一下下列任一項，以存取更多資訊或編輯程式的選項：</p> 
    <ul> 
     <li>星形圖示可將方案新增至您的最愛清單</li> 
     <li> <p>[！UICONTROL更多]功能表 <img src="assets/qs-more-menu.png"> 執行下列任一項作業： </p> 
      <ul> 
       <li>編輯方案</li> 
       <li>停用它。 停用方案時，您無法再將其與專案層級的專案建立關聯。 </li> 
       <li> <p>刪除它。 刪除方案不會刪除方案中的專案。 它會移除專案與方案的關聯。 </p> </li> 
       <li>與其他人共用</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL完成百分比]</td> 
   <td> <p>您無法在標題中編輯程式的[！UICONTROL完成百分比]。 此資訊會從計畫中的專案更新。 依預設，方案的完成百分比是屬於方案且處於[！UICONTROL目前]或[！UICONTROL已核准]狀態的專案之完成百分比值的平均值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL計畫管理員]</td> 
   <td> <p>您可以在標題中編輯「方案管理員」。 這與[！UICONTROL計畫所有者]相同。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL計畫完成日期]</td> 
   <td>您無法在標題中編輯方案的規劃完成日期。  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL作用中專案條件]</td> 
   <td>這是計算在計畫中有多少百分比的專案將[！UICONTROL Condition]設定為[！UICONTROL On Target]、[！UICONTROL At Risk]或[！UICONTROL In Trouble]。 這裡所代表的專案是狀態為[！UICONTROL目前]和[！UICONTROL已核准]的專案。 </td> 
  </tr> 
 </tbody> 
</table>

## 移動方案

您可以將現有方案新增至投資組合。 由於計畫不能存在於兩個不同的投資組合中，因此新增現有計畫會將其從一個投資組合永久移動到另一個投資組合。

如需詳細資訊，請參閱 [將現有方案新增至投資組合](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).
