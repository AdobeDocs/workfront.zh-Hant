---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: 自訂卡片上顯示的欄位
description: 您可以停用欄位來自訂卡片上顯示的欄位，使其不會顯示在完整卡片或壓縮檢視中，或隱藏壓縮卡片檢視中的欄位。
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 80e0a053f39991d3ed8d9bd2a11a8da2d5de588e
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# 自訂卡片上顯示的欄位

依預設，所有可用欄位都會顯示在卡片上，包括卡片開啟時的完整檢視，以及展示板上的壓縮卡片檢視。 您可以自訂要顯示哪些欄位，方法是：

* 停用欄位，使其不顯示在任一檢視中
* 隱藏壓縮卡片檢視上的欄位

如果欄位包含值，而您停用該欄位，則如果您稍後再次啟用該欄位，則會保留該值。

區段（顯示為卡片詳細資料上的左側導覽選項）也可用於顯示和隱藏。

您也可以顯示先前建立的自訂欄位。 您不能在展示板中設計和建立新的自訂欄位。

>[!NOTE]
>
>您所做的任何欄位自訂都只適用於您正在使用的展示板。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr>
   </tbody> 
</table>

&#42;若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 設定卡片 {#configure-cards}

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 右上角的 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 展示板]**.
1. 存取展示板。 如需詳細資訊，請參閱 [建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 按一下 [!UICONTROL **設定**] 以開啟「設定」面板。
1. 展開 [!UICONTROL **卡片**].

   預設會啟用大部分的欄位和區段。

1. 關閉欄位或區段以在兩個卡片檢視中將其停用。
1. 按一下隱藏圖示 ![隱藏圖示](assets/eye-hide-icon.png) 在欄位或區段旁邊，將其隱藏在壓縮檢視上。
1. 若要在兩個檢視中顯示所有欄位和區段，請按一下 [!UICONTROL **將所有欄位還原為預設值**].
1. 按一下 [!UICONTROL **隱藏設定**] 以關閉「設定」面板。

## 新增自訂欄位到卡片

已連線的卡片上有自訂欄位可用。 它們只會在完整卡片檢視中顯示，不會顯示在主機板上的縮短檢視中。

>[!NOTE]
>
>當您將自訂欄位新增到卡片時，卡片上的資料是唯讀的。

1. 存取展示板並按一下 [!UICONTROL **設定**] 以開啟「設定」面板。
1. 展開 [!UICONTROL **卡片**].
1. 下 [!UICONTROL 卡片欄位]，按一下 [!UICONTROL **新增自訂欄位**].
1. 選取 [!UICONTROL **任務**] 或 [!UICONTROL **問題**].

   任務或問題的可用欄位類別隨即顯示。 展開類別以檢視所有欄位。 您也可以搜尋欄位。

   ![搜尋自訂欄位](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >下列欄位型別無法新增至卡片：Adobe XD、影像、PDF、影片。

1. 選取欄位名稱。
1. （選用）按一下 **[!UICONTROL 欄位值]** 欄位，以將此自訂欄位變更為其他欄位。
1. （可選）變更 **[!UICONTROL 欄位標籤]** 至您要顯示在卡片上的欄位名稱。
1. 完成變更後，按一下 [!UICONTROL **儲存欄位**].

   ![自訂欄位值和標籤](assets/save-custom-field-value-label.png)

   自訂欄位會新增至可用欄位清單，並依預設啟用。 您可以依照以下說明中的步驟停用自訂欄位： [設定卡片](customize-fields-on-card.md#configure-cards) 編輯欄位，或從所有卡片中刪除它。
