---
product-area: projects
navigation-topic: use-lists
title: 在的清單中內聯編輯專案 [!DNL Adobe Workfront]
description: 當物件顯示在清單或報表中時，您可以內嵌編輯物件。 當您編輯清單或報表中顯示的物件資訊時，物件會立即更新。
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: f0912e4ef29d682ae3e6dd0e543b8e77fb7f29b6
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# 在的清單中內聯編輯專案 [!DNL Adobe Workfront]

當物件顯示在清單或報表中時，您可以內嵌編輯物件。 當您編輯清單或報表中顯示的物件資訊時，物件會立即更新。

當您內聯編輯未附加至物件的自訂表單中包含的欄位時，自訂表單會自動新增至物件。 如果欄位存在於多個自訂表單中，則最近更新的自訂表單會附加到物件。

如需清單的詳細資訊，請參閱 [開始使用中的清單 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

雖然清單或報表中顯示的物件大多可在中內嵌編輯 [!DNL Adobe Workfront]，有一些限制，包括：

* 您無法編輯計算欄位或 [!DNL Workfront] 作為計算的內建欄位。
* 您只能編輯與清單中物件直接關聯的欄位。 您無法編輯屬於與清單中物件相關聯之物件的欄位。\
   例如，您可以在「任務」報告中編輯任務的狀態，但無法在同一報告中編輯與任務相關聯的專案名稱。 您只能在專案報告中編輯專案名稱。
* 當清單的檢視未顯示預設貨幣時，您無法內聯編輯欄位。\
   如需顯示預設貨幣的詳細資訊，請參閱區段 [編輯具有唯一貨幣的報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) 在文章中 [建立具有唯一匯率的財務資料報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).
* 您無法編輯清單中顯示的旗標和圖示。
* 您無法內聯編輯源自其他報表的報表欄位。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>[！UICONTROL Edit]清單所在區域的存取權</p> <p>例如，若要內聯編輯專案中的任務，您需要[！UICONTROL Edit]專案存取權。</p> <p>注意：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。<br>如需瞭解如何 [!DNL Workfront] 管理員可以變更您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>[！UICONTROL管理]</p> <p>您也必須有權編輯特定欄位，例如自訂欄位、狀態等。</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 編輯內嵌物件

1. 移至您要內嵌編輯的物件清單。

   清單應顯示屬於物件的欄位，或屬於與清單中的物件相關聯的物件的欄位。

1. 找到您要編輯的物件，然後在清單中的任何欄位中按一下。

   >[!TIP]
   >
   >如果您有多個頁面，則可以使用以下方式找出物件：
   >
   >   
   >   
   >   * **分頁**：按一下向後和向前箭頭，在頁面之間導覽。\
   >     位於清單右下角的 [!UICONTROL 分頁] 當您捲動清單時，區域會保持粘性。
   >   * **快速篩選**：按一下篩選圖示或輸入Alt+F開啟快速篩選，然後輸入文字以僅顯示包含輸入文字的專案。\
   >     快速篩選位於清單工具列中。 如需詳細資訊，請參閱 [將快速篩選套用至清單](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).


   如果欄位可以編輯，這會將該欄位和清單中顯示的所有其他欄位轉換為可編輯的儲存格。

   ![](assets/nwe-editable-cells-350x131.png)

1. 編輯此儲存格內的資訊，然後按 [!UICONTROL 輸入].

   >[!NOTE]
   >
   >如果自訂欄位已設定為允許格式化，則可在內聯編輯更新清單中的欄位時以粗體、斜體或底線文字顯示。\
   >如需設定自訂欄位格式的相關資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).\
   >如需更新清單的詳細資訊，請參閱文章中的「更新清單和舊版清單的差異」一節 [開始使用中的清單 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. 按下 [!UICONTROL 標籤] 移至下一個可編輯的儲存格。
1. （視條件而定）如果您無法儲存編輯，且儲存格外框為紅色，請按一下欄位內部以檢閱儲存格旁顯示的驗證訊息，並進行適當的更新。

   最常見的情況是，使用錯誤格式或必填欄位留空時。

1. 修改完所有儲存格後，按下 [!UICONTROL 輸入] 以儲存變更。
