---
navigation-topic: use-lists
title: 修改清單的顯示方式
description: 在 [!DNL Adobe Workfront]，您可以自訂清單的顯示方式。 其他檢視清單的使用者看不到您的變更。
feature: Get Started with Workfront
author: Lisa
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# 修改清單的顯示方式

在 [!DNL Adobe Workfront]，您可以自訂清單的顯示方式。 其他檢視清單的使用者看不到您的變更。

您可以進行下列自訂：

* 顯示的項目數
* 欄寬或順序
* 群組是否展開或收合

>[!NOTE]
>
>當您登出時，會還原您所做的上述顯示變更 [!DNL Workfront] 或關閉瀏覽器。 這些變更也可能會在8小時後還原。

除了上述的臨時自定義外，您還可以調整清單排序依據的欄，哪些欄 [!DNL Workfront] 即使在您登出或關閉瀏覽器後仍會保留。 不過，如果某人編輯清單檢視中的排序選項，則不會保留先前的排序選項。

有關修改清單中顯示的資訊的資訊，請參閱 [報表元素：篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

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
   <td> <p>[!UICONTROL Request]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>[!UICONTROL視圖]對清單所在區域的訪問</p> <p>例如，若要修改專案的檢視，您需要[!UICONTROL檢視]的專案存取權。</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。<br>若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>[!UICONTROL視圖]或更高權限，適用於應用於清單的視圖</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 修改清單的顯示方式

1. 前往 [!DNL Workfront] 修改。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. （可選和條件性）如果清單中的群組已收合，且您想要檢視詳細資訊，請按一下所需的群組，以展開清單並顯示清單中列出的資訊。

   或

   要展開所有分組，請按一下列標題中複選框右側的箭頭。

   ![expand_grogns__1_.png](assets/expand-groupings--1--350x227.png)

1. （選用和條件性）如果您想在畫面上顯示特定數量的項目，請按一下 **[!UICONTROL 顯示]** 下拉式功能表（位於畫面右下角），然後選取「 」以顯示 **100**, **250**, **500**, **[!UICONTROL 全部]**，或 **2000年** 項目。

   ![](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >依預設，更新清單會顯示2,000個項目，舊版清單會顯示100個項目。 如果清單包含超過2,000個項目，則無法在一個頁面上顯示所有項目。
   >
   >
   >為在對象包含格式化文本欄位的大型清單中獲得最佳效能，建議將此數字限制為250。
   >
   >
   >如需2種清單類型的詳細資訊，請參閱區段 [更新後的清單與舊版清單之間的差異](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) 在文章中 [開始使用 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   清單的結果會經過編頁，以顯示每頁所選的項目數。 您可以按一下向後和向前箭頭，或選取特定頁面，以存取其他頁面上的結果。

1. 要調整列寬度，請將滑鼠移到分隔2列的行上，然後按一下將其拖動到所需寬度。

   欄會調整大小，直到您在瀏覽器上清除快取，或直到您再次手動調整其大小為止。

1. 若要重新排序清單中的欄，請將滑鼠移至欄標題以顯示手形工具，然後按一下以拖曳欄至您要其顯示的位置。

   欄的位置會儲存，直到您重新整理頁面為止。\
   如需自訂清單中欄的寬度和順序的詳細資訊，請參閱文章 [修改欄寬和順序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

1. 若要調整清單的排序順序，請按一下欄標題以選取它，然後按住CMD鍵(開啟 [!DNL Mac])或CTRL鍵(開啟 [!DNL Windows])，並選取最多2個額外的欄標題以依其排序。

   清單會依您選取的順序，依每個選取的欄排序。

   您對清單所做的所有修改都會立即儲存。

   >[!NOTE]
   >
   >如果您要排序 [!UICONTROL 群組] 區域 [!UICONTROL 設定]，在更改清單排序方式時，組及其子組的層次結構視圖不會被拆分 — 子組將與其父組保持一致。 清單會先依頂層群組排序。 然後，在每個父組下，同一級別的子組清單將一起排序。
