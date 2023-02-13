---
product-area: projects
navigation-topic: use-lists
title: 內嵌編輯清單中的項目，位於 [!DNL Adobe Workfront]
description: 您可以在對象顯示在清單或報表中時內嵌編輯對象。 當您編輯清單或報表中顯示的對象的資訊時，對象會立即更新。
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# 內嵌編輯清單中的項目，位於 [!DNL Adobe Workfront]

您可以在對象顯示在清單或報表中時內嵌編輯對象。 當您編輯清單或報表中顯示的對象的資訊時，對象會立即更新。

內嵌編輯未附加至物件的自訂表單中所包含欄位時，自訂表單會自動新增至物件。 如果欄位存在於多個自訂表單中，則最近更新的自訂表單會附加至物件。

如需清單的詳細資訊，請參閱 [開始使用 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

清單或報表中顯示的大多數對象都是內嵌可編輯的 [!DNL Adobe Workfront]，有一些限制，包括：

* 您無法編輯計算欄位或 [!DNL Workfront] 計算的內建欄位。
* 您只能編輯與清單中的對象直接關聯的欄位。 不能編輯屬於與清單中的對象關聯的對象的欄位。\
   例如，您可以在「任務」報表中編輯任務的狀態，但無法編輯任務在同一報表中關聯的項目的名稱。 您只能在「專案」報表中編輯專案名稱。
* 清單檢視未顯示預設貨幣時，您無法內嵌編輯欄位。\
   如需顯示預設貨幣的資訊，請參閱區段 [編輯具有不重複貨幣的報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) 在文章中 [使用獨特的匯率建立財務資料報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

* 您無法編輯清單中顯示的標幟和圖示。

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
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>[!UICONTROL編輯]對清單所在區域的訪問</p> <p>例如，若要內嵌編輯專案中的工作，您需要[!UICONTROL編輯]的專案存取權。</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。<br>若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>[!UICONTROL管理]</p> <p>您也必須擁有編輯特定欄位的權限，例如自訂欄位、狀態等。</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 內嵌編輯物件

1. 轉到要內嵌編輯的對象清單。

   清單應顯示屬於清單中與對象關聯的對象的對象或對象的欄位。

1. 找到您要編輯的物件，然後在清單中的任何欄位內按一下。

   >[!TIP]
   >
   >如果您有多個頁面，則可使用：
   >
   >   
   >   
   >   * **分頁**:按一下向後和向前箭頭，在頁面之間導覽。\
      >     位於清單的右下角， [!UICONTROL 分頁] 當您捲動清單時，區域仍會保持黏著狀態。
   >   * **快速篩選**:按一下篩選表徵圖或鍵入Alt+F以開啟快速篩選，然後輸入文本以僅顯示包含輸入文本的項。\
      >     快速過濾器位於清單工具欄中。 如需詳細資訊，請參閱 [將快速篩選器應用於清單](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).



   如果欄位可以編輯，這會將欄位和清單中顯示的所有其他欄位轉換為可編輯的儲存格。

   ![](assets/nwe-editable-cells-350x131.png)

1. 編輯此儲存格內的資訊，然後按 [!UICONTROL 輸入].

   >[!NOTE]
   >
   >如果自訂欄位已設定為允許格式化，您可以在內嵌編輯更新清單中的欄位時，使用粗體、斜體或底線文字。\
   >如需為自訂欄位設定格式的詳細資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).\
   >如需更新清單的詳細資訊，請參閱文章中的「更新清單與舊版清單的差異」一節 [開始使用 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Press [!UICONTROL 標籤] 移至下一個可編輯的儲存格。
1. （條件性）如果您無法儲存編輯內容，且儲存格以紅色外框，請按一下欄位內的，以檢閱儲存格旁顯示的驗證訊息，並進行適當的更新。

   最常發生的情況是，使用錯誤格式或將必填欄位留空時。

1. 完成所有單元格的修改後，按 [!UICONTROL 輸入] 來儲存變更。
