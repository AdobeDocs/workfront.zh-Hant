---
navigation-topic: use-lists
title: 修改清單的顯示方式
description: 在 [!DNL Adobe Workfront]中，您可以自訂清單的顯示方式。 其他檢視清單的使用者看不到您的變更。
feature: Get Started with Workfront
author: Nolan
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: f0b3b8aa64fa0b03a196bbcc2bdd037eeeb0f89e
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# 修改清單的顯示方式

<!--Audited: 11/2024-->

在[!DNL Adobe Workfront]中，您可以自訂清單的顯示方式。 其他檢視清單的使用者看不到您的變更。

您可以進行下列自訂：

* 顯示的專案數
* 欄寬或順序
* 群組是展開還是收合

>[!NOTE]
>
>當您登出[!DNL Workfront]或關閉瀏覽器時，您所做的上述顯示變更將會還原。 這些變更也可能會在8小時後回覆。

除了上述的暫時自訂功能之外，您也可以調整清單排序所依據的欄，即使在您登出或關閉瀏覽器之後，[!DNL Workfront]仍會保留這些欄。 但是，如果有人編輯清單檢視中的排序選項，則不會保留先前的排序選取範圍。

如需修改清單中所顯示資訊的詳細資訊，請參閱[報告元素：篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>投稿人或以上 </p>
   <p>要求或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>[！UICONTROL檢視]清單所在區域的存取權</p> <p>例如，若要修改專案的檢視，您需要[！UICONTROL檢視]專案的存取權。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>[！UICONTROL檢視]或套用至清單之檢視的更高許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 修改清單

1. 移至[!DNL Workfront]中您要修改的清單。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. （選擇性和條件性）如果清單中的群組已收合且您想要檢視更多資訊，請按一下所需的群組以展開清單並顯示其中列出的資訊。

   或

   若要展開所有群組，請按一下欄標題中核取方塊右側的箭頭。

   ![expand_groupings__1_.png](assets/expand-groupings--1--350x227.png)

1. （選擇性和條件性）如果您想要在熒幕上顯示特定數量的專案，請按一下熒幕右下角的&#x200B;**[!UICONTROL Showing]**&#x200B;下拉式功能表，然後選取以顯示&#x200B;**100**、**250**、**500**、**[!UICONTROL All]**&#x200B;或&#x200B;**2000**&#x200B;專案。

   第![頁上的](assets/list-number-page-350x119.png)清單編號

   >[!TIP]
   >
   >依預設，有2,000個專案會顯示在更新的清單中，有100個專案會顯示在舊版清單中。 如果清單包含超過2,000個專案，您無法在單一頁面上顯示所有專案。
   >
   >
   >為了在物件包含格式化文字欄位的大型清單中取得最佳效能，建議將此數字限製為250。
   >
   >
   >如需有關2種清單型別的詳細資訊，請參閱文章[開始使用](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated)中的清單[更新清單和舊版清單的差異 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)一節。

   清單的結果會以分頁方式顯示，以顯示每頁選取的專案數。 您可以按一下向後和向前箭頭，或選取特定頁面，來存取其他頁面上的結果。

1. 若要調整欄寬，請將滑鼠移至分隔兩欄的線條上，然後按一下以將欄拖曳至所需的寬度。

   欄會重新調整大小，直到您在瀏覽器上清除快取或手動重新調整它的大小為止。

1. 若要重新排序清單中的欄，請將滑鼠移至欄標題上以顯示手形工具，然後按一下以將欄拖曳到您要顯示的位置。

   會儲存欄的位置，直到您重新整理頁面為止。

   如需自訂清單中欄寬和順序的詳細資訊，請參閱文章[修改欄寬和順序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)。

1. 若要調整清單的排序順序，請按一下欄標題加以選取，然後在鍵盤上按住CMD鍵（在[!DNL Mac]上）或CTRL鍵（在[!DNL Windows]上），並選取最多2個要依其排序的其他欄標題。

   清單會依您選取的順序依每個選取的欄排序。

   您對清單所做的所有修改都會立即儲存。

   >[!NOTE]
   >
   >如果您在[!UICONTROL 設定]的[!UICONTROL 群組]區域中排序群組，則當您變更清單的排序方式時，群組及其子群組的階層檢視不會中斷，子群組會與其父群組一起保留。 清單會先依頂層群組排序。 然後，在每個父群組下，位於相同層級的子群組清單會一起排序。
