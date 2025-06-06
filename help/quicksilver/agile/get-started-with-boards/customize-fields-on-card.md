---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: 自訂要在卡片上顯示的欄位
description: 您可以停用欄位來自訂卡片上顯示的欄位，使其不會顯示在完整卡片或壓縮卡片檢視中，或隱藏壓縮卡片檢視中的欄位。
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# 自訂要在卡片上顯示的欄位

依預設，所有可用欄位都會顯示在卡片上，當卡片開啟時會顯示為完整檢視，並在展示板上的壓縮卡片檢視中顯示。 您可以自訂哪些欄位會以下列方式顯示：

* 停用欄位，使其不顯示在任一檢視中
* 在壓縮卡片檢視上隱藏欄位

如果欄位包含值且您停用該欄位，則稍後您再次啟用該欄位時會保留值。

區段（顯示為卡片詳細資料上的左側導覽選項）也可用於顯示和隱藏。

您也可以顯示先前建立的自訂欄位。 您不能在展示板中設計和建立新的自訂欄位。

>[!NOTE]
>
>您所做的任何欄位自訂都只適用於您正在使用的展示板。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> 
   <p>新增：[!UICONTROL Contributor]或以上</p> 
   <p>或</p>
   <p>目前： [!UICONTROL Request]或以上</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定卡片 {#configure-cards}

{{step1-to-boards}}

1. 存取展示板。 如需詳細資訊，請參閱[建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md)。
1. 按一下主機板右側的&#x200B;[!UICONTROL **[設定]**]&#x200B;以開啟[設定]面板。
1. 展開&#x200B;[!UICONTROL **卡片**]。

   預設會啟用大部分的欄位和區段。

1. 關閉欄位或區段以在兩個卡片檢視中將其停用。
1. 按一下欄位或區段旁的隱藏圖示![隱藏圖示](assets/eye-hide-icon.png)，在壓縮檢視中隱藏它。
1. 若要在兩個檢視中顯示所有欄位和區段，請按一下[將所有欄位還原為預設值]。**&#x200B;**
1. 按一下&#x200B;[!UICONTROL **隱藏設定**]&#x200B;以關閉「設定」面板。

## 新增自訂欄位到卡片

已連線的卡片上有自訂欄位可用。 它們只會在完整卡片檢視中顯示，不會顯示在展示板上的壓縮檢視中。

自訂欄位上的資料可在卡片上編輯，但某些自訂元素可能只能在原始欄位上編輯，無法在卡片上編輯。

1. 存取展示板並按一下&#x200B;[!UICONTROL **設定**]&#x200B;以開啟「設定」面板。
1. 展開&#x200B;[!UICONTROL **卡片**]。
1. 在[!UICONTROL 卡片欄位]下，按一下&#x200B;[!UICONTROL **新增自訂欄位**]。
1. 選取&#x200B;[!UICONTROL **任務**]&#x200B;或&#x200B;[!UICONTROL **問題**]。

   任務或問題的可用欄位類別隨即顯示。 展開類別以檢視所有欄位。 您也可以搜尋欄位。

   ![搜尋自訂欄位](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >下列欄位型別無法新增至卡片：Adobe XD、影像、PDF、視訊。

1. 選取欄位名稱。
1. （選擇性）按一下&#x200B;**[!UICONTROL 欄位值]**&#x200B;欄位，將此自訂欄位變更為其他欄位。
1. （選擇性）將&#x200B;**[!UICONTROL 欄位標籤]**&#x200B;變更為您想在卡片上顯示的欄位名稱。
1. 完成變更後，按一下&#x200B;[!UICONTROL **儲存欄位**]。

   ![自訂欄位值和標籤](assets/save-custom-field-value-label.png)

   自訂欄位會新增至可用欄位清單，並依預設啟用。 您可以依照上面[設定卡片](customize-fields-on-card.md#configure-cards)區段中的步驟停用自訂欄位、編輯欄位或從所有卡片中刪除它。

>[!NOTE]
>
>如果您稍後在Workfront中重新命名自訂欄位，則必須編輯「設定」面板上的欄位標籤以相符，否則該欄位將不會顯示在卡片上。

## 顯示或隱藏已封存的卡片

您必須開啟組態設定，才能在展示板上顯示封存的卡片。

1. 存取展示板並按一下&#x200B;[!UICONTROL **設定**]&#x200B;以開啟「設定」面板。
1. 展開&#x200B;[!UICONTROL **卡片**]。
1. 開啟&#x200B;[!UICONTROL **在展示板上顯示封存的卡片**]。

   現在，您可以篩選展示板以顯示任何已封存的卡片。 如需詳細資訊，請參閱[在展示板中篩選和搜尋](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)。

1. 按一下&#x200B;[!UICONTROL **隱藏設定**]&#x200B;以關閉「設定」面板。

## 設定卡片縮減

若要在一段時間後自動從展示板移除卡片，請參閱[設定卡片縮減](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md)。
