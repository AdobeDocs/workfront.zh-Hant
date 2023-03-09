---
title: 使用舊版表單產生器將顯示邏輯新增及略過邏輯至自訂表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以根據使用者在填寫自訂表單時所做的選擇，決定應顯示或略過自訂表單的哪些區段。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: 7835b5f9b5903e19b03cb7e25bfae37c9739f064
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# 使用舊版表單產生器將顯示邏輯新增及略過邏輯至自訂表單

您可以根據使用者在填寫自訂表單時所做的選擇，決定應顯示或略過自訂表單的哪些區段。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>管理對自訂表單的存取</p> <p>如需Workfront管理員如何授予此存取權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取層級設定，請聯絡您的Workfront管理員。

## 使用顯示邏輯和略過邏輯的考量事項

* 若要在自訂欄位、介面工具集或區段插播上新增顯示邏輯，表單上至少必須先放置一個多選欄位（選項按鈕、下拉式清單或核取方塊）。

   如需自訂表單中自訂欄位和小工具的相關資訊，請參閱 [使用舊版表單產生器將自訂欄位新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [使用舊版表單產生器在自訂表單中新增或編輯資產介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* 您無法將略過邏輯新增至介面工具集或區段插播。 您只能將其新增至多個選擇欄位（選項按鈕、下拉式清單或核取方塊）。

* 您可以將顯示邏輯和略過邏輯新增至自訂欄位，而自訂欄位的下列所有內容皆為true:

   * 它是多選欄位（選項按鈕、下拉式清單或核取方塊）
   * 前面有多選欄位
   * 後面接著另一個自訂欄位

* 使用顯示邏輯或略過邏輯複製表單時，邏輯會複製到新的自訂表單。
* 為自訂表單建立顯示邏輯規則時，請謹記下列事項

   * 顯示邏輯陳述式中未包含的自訂欄位依預設會顯示在自訂表單上。
   * 您可以建立多欄位顯示邏輯陳述式。

* 批量編輯對象時，所有自定義欄位都顯示在「編輯對象」框中，包括跳過或隱藏的欄位。

## 建立具有顯示和略過邏輯的自訂表單範例

若要了解如何將顯示和略過邏輯新增至自訂表單，最佳方式是透過以下兩節中說明的實用範例：

* [顯示邏輯](#display-logic)
* [略過邏輯](#skip-logic)

### 顯示邏輯 {#display-logic}

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **自訂Forms** ![](assets/custom-forms-icon.png).

1. 建立範例自訂表單：

   1. 按一下 **新自訂表單**，然後按一下 **專案** 中。

   1. 在 **表單標題** 框，類型 **自訂表單範例 — 學習顯示邏輯和略過邏輯**.

   1. 按一下 **新增欄位** 在左上角。
   1. 新增下拉式欄位，稱為 *問題欄位* 按一下 **下拉式清單**，然後輸入 **問題欄位** 在 **標籤** 框。

   1. 在 **選擇**，在文本框中添加以下選項：

      需要的研究

      不再進行研究

   1. 按一下 **儲存+關閉** 左下角。

1. 選取新 **自訂表單範例 — 學習顯示邏輯和略過邏輯** 自訂表單，然後按一下 **編輯**.

1. 新增名為的單行文字欄位 *其他研究* 按一下 **單行文本欄位**，然後輸入 **其他研究** 在 **標籤** 框。

1. 按一下 **新增邏輯** 靠近 **編輯自訂表單** 螢幕。

1. 在出現的方塊中，搭配 **顯示邏輯** 索引標籤開啟，設定 **其他研究** 欄位，按一下 **問題欄位** 在第一個下拉式清單中， **需要的研究** 在第二個下拉式清單中， **已選取** 第三個下拉式清單中。
1. 按一下 **儲存** 關閉 **欄位邏輯** ，然後按一下 **完成** 在 **欄位設定** 的上界。

   現在，當某人選取 **需要的研究** 在 **問題欄位** 下拉式清單， **其他研究** 欄位。

1. 按一下 **預覽** 以確保邏輯以您希望的方式顯示在表單上。
1. 按一下 **結束預覽** 當您發現邏輯如預期般運作時。
1. 按一下 **儲存+關閉** 在 **編輯自訂表單** 窗口以保存表單，然後繼續 [略過邏輯](#skip-logic) 下方。

### 略過邏輯 {#skip-logic}

略過邏輯函式與顯示邏輯類似，但作用相反：您可以根據使用者的選擇決定應跳過哪些欄位，而不是根據特定選擇來顯示特定的自訂多選項欄位。

若要了解相關資訊，請繼續處理您在區段中建立的自訂表單範例 [顯示邏輯](#display-logic) 在本文中：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms**.
1. 選取表單 **自訂表單範例 — 學習顯示邏輯和略過邏輯** 在上述步驟中建立，然後按一下 **編輯**.

1. 選取您建立的下拉式欄位，名稱為 *問題欄位*.
1. 按一下 **新增邏輯** 按鈕 **欄位設定** 邊欄。

1. 在 **欄位邏輯** 框，確定 **略過邏輯** 頁簽。

1. 將第一個下拉式清單設為 **不再進行研究** 第二個下拉式清單 **已選取**.

1. 在 **然後跳到** 下拉式清單，選取 **表單結尾。**

   現在，當某人選取 **不再進行研究** 在 **問題欄位** 下拉式欄位中，表單將直接略過至表單結尾，而不顯示 **其他研究** 欄位。

1. 按一下&#x200B;**儲存**。
1. 按一下 **預覽**  以確保邏輯能如您所願套用。
1. 按一下 **完成** 在表單的左下側。
