---
product-area: programs
navigation-topic: create and manage programs
title: 建立方案
description: 方案代表一組專案，這些專案共用超越專案界限的共同策略、目標或目標。 程式不能存在於產品組合之外。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
source-git-commit: 93c36a87667097729e89a61f68cc17e9c861d547
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# 建立方案

方案代表一組專案，這些專案共用超越專案界限的共同策略、目標或目標。 程式不能存在於產品組合之外。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>[!UICONTROL編輯]對Portfolio和程式的訪問 </p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>產品組合的[!UICONTROL管理]權限</p> <p>建立程式後，依預設，您會擁有該程式的[!UICONTROL管理]權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 建立方案

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 執行下列任一操作。

   * 從 [!UICONTROL 方案] 區域：

      1. 按一下 **[!UICONTROL 方案]** 的下限。
      1. 按一下 **[!UICONTROL 新計畫]**.
      1. 在顯示的方塊中，在 **[!UICONTROL 選擇Portfolio]** 欄位。
      1. 在 **[!UICONTROL 名稱]** 欄位。
      1. 按一下&#x200B;**[!UICONTROL 儲存]**。
   * 從 [!UICONTROL Portfolio] 區域：

      1. 按一下 **[!UICONTROL Portfolio]** 在 [!UICONTROL 主菜單]，然後按一下產品組合。
      1. 在左側面板中，按一下 **[!UICONTROL 方案]**.
      1. 按一下 **[!UICONTROL 新計畫]** 下拉式功能表，然後 **[!UICONTROL 新計畫]**.


1. 指定 **[!UICONTROL 無標題程式]** 欄位。

   名稱最多可包含255個字元。

1. （選用）按一下 **[!UICONTROL 計畫經理]** （在程式的標題中）以更新它。

   >[!TIP]
   >
   >作為程式的建立者，預設情況下將您設定為程式管理器。

1. 按一下 **[!UICONTROL 方案詳細資訊]** 中。
1. 按兩下任何欄位以更新 **[!UICONTROL 概述]** 的上界。
1. 指定下列資訊：

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
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td> <p>指定程式的說明。</p> <p>說明會顯示在方案的登陸頁面上。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL程式管理器]</td> 
      <td> <p>開始鍵入要作為程式管理器的用戶的名稱，然後在下拉清單中顯示該用戶的名稱時按一下該用戶的名稱。 這與[!UICONTROL程式所有者]相同。 </p> <p>提示：您也可以更新方案標題中的方案管理員。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL組] </td> 
      <td> <p>如果組擁有程式或有責任完成程式，則添加單個組的名稱。 </p> <p>您可以將游標移至群組上並按一下[!UICONTROL資訊]圖示，以確定您選取的是正確的群組 <img src="assets/info-icon.png"> 顯示於其旁。 此工具提示會列出群組的相關資訊，例如上方的群組階層及其管理員。</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選用和條件式）按一下 **[!UICONTROL 新增自訂表單]** 方塊來選取產品組合的自訂表單並更新自訂欄位。

   >[!TIP]
   >
   >必須先建立程式自定義表單，然後才能將其附加到程式。

1. （可選）按兩下任何欄位以更新自訂表單的資訊。
1. 按一下 **[!UICONTROL 專案]** 在左側面板中，然後 **[!UICONTROL 新增專案]** 將項目添加到方案。

   有關將項目添加到方案的資訊，請參閱 [將專案新增至方案](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. 按一下 **[!UICONTROL 儲存變更]**.
1. （選用）按一下 **[!UICONTROL 更多功能表]** ![](assets/more-icon.png) 在方案名稱旁，按一下 **[!UICONTROL 停用程式]**.

   當您停用方案時，當使用者嘗試將其新增至專案時，該方案不再顯示在方案清單中。 您仍可從 [!UICONTROL 方案] 的上界。

## 方案標題概述

您可以在其標題中找到有關該方案的有限資訊。

以下資訊會顯示在方案的標題中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">標題資訊</td> 
   <td> <p><strong>附註</strong> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">包含產品組合名稱的階層連結</td> 
   <td>您可以從方案的標題中存取方案所屬的產品組合。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">方案名稱</td> 
   <td>您可以編輯標題中的方案名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">對象類型的名稱和激活狀態</td> 
   <td>查看程式時，「程式」一詞將顯示在綠色大綱中。 「[!UICONTROL Devarited]」一字會顯示在旁邊，如果程式未標籤為[!UICONTROL Active]，則大綱將顯示為灰色。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">方案的行動領域 </td> 
   <td> <p>按一下以下任一選項，以訪問程式的更多資訊或編輯選項：</p> 
    <ul> 
     <li>將程式添加到收藏夾清單的星形表徵圖</li> 
     <li> <p>[!UICONTROL更多]菜單 <img src="assets/qs-more-menu.png"> 執行下列任一操作： </p> 
      <ul> 
       <li>編輯方案</li> 
       <li>停用它。 方案停用後，您無法再將其與專案層級的專案建立關聯。 </li> 
       <li> <p>刪除它。 刪除方案不會刪除方案中的專案。 它會移除專案與方案的關聯。 </p> </li> 
       <li>與其他人共用</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL百分比完成]</td> 
   <td> <p>您無法編輯標題中方案的[!UICONTROL完成百分比]。 此資訊會從方案中的專案更新。 預設情況下，方案的完成百分比是屬於方案的[!UICONTROL當前]和[!UICONTROL已批准]狀態中項目的完成百分比值的平均值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL程式管理器]</td> 
   <td> <p>您可以編輯標題中的方案管理員。 這與[!UICONTROL程式所有者]相同。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL計畫完成日期]</td> 
   <td>您無法編輯標題中方案的完成百分比。 方案完成百分比是標題中專案完成百分比的平均值。 此處表示的項目為狀態為[!UICONTROL Current]和[!UICONTROL Approved]的項目。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL活動項目條件]</td> 
   <td>這是計算程式中項目的百分比，將[!UICONTROL條件]設定為[!UICONTROL On Target]、[!UICONTROL At Risk]或[!UICONTROL In Faule]。 此處表示的項目為狀態為[!UICONTROL Current]和[!UICONTROL Approved]的項目。 </td> 
  </tr> 
 </tbody> 
</table>

## 移動程式

您可以將現有程式新增至產品組合。 因為程式不能存在於兩個不同的產品組合中，所以添加現有程式會將其從一個產品組合永久移到另一個組合。

如需詳細資訊，請參閱 [將現有程式添加到產品組合](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).
