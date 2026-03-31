---
product-area: projects
navigation-topic: use-the-home-area
title: 使用我的請求Widget
description: 您可以在「我的請求」Widget中提交請求。 您也可以使用篩選器和欄來自訂Widget。
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 2%

---

# 使用我的請求Widget

>[!IMPORTANT]
>
>本文會說明新的「我的請求」Widget。 您必須啟用新的請求體驗才能檢視新的Widget。
>您可以在請求區域中啟用新的請求體驗。

「我的請求」Widget會顯示您已提交的請求。 您可以篩選請求、搜尋特定請求，或調整欄順序和可見度。 您也可以從「我的請求」Widget建立新請求。

>[!NOTE]
>
>* 當「我的請求」Widget載入時，最多會顯示50個請求。 若要顯示更多請求，請向下捲動清單。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任何Workfront或Workflow套件</p>
   <p>用於存取Workfront Planning請求及其建立物件的任何Workfront Planning套件</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權</strong></td> 
   <td> <p>投稿人或以上</p>
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>檢視或更高的存取權以存取您在對話中被標籤或需要解決核准的任何物件（專案、任務、問題、檔案）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>[!UICONTROL 檢視]對您在對話中被標籤或需要解決核准的專案、任務、問題和檔案的許可權或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立請求

您可以直接從「我的請求」Widget建立請求。

如需指示，請參閱文章[從首頁區域建立工作專案和專案](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request)中的[建立請求](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)一節。

## 複製請求

您可以複製我的請求Widget中的請求、編輯請求，然後將其作為新請求提交。

如需指示，請參閱[複製並提交要求](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md)。

## 管理我的請求Widget中請求清單的資訊

<!--
The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR operators.

To configure the filter in the My Requests widget:
-->

1. 按一下左上角的&#x200B;**[!UICONTROL 主功能表]** ![主功能表圖示](assets/lines-main-menu.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （視條件而定）將&#x200B;**我的請求** Widget新增至您的主畫面。 按一下&#x200B;**自訂**，找到&#x200B;**我的要求**，然後按一下它以將其新增到&#x200B;**首頁**。
1. （選擇性）若要管理資訊在請求清單中的顯示方式，請更新清單的下列檢視元素：

   * 檢視
   * 篩選器
   * 欄

   <!--
   <div class="preview">
      * Group
   * Format cells
   * Row height
      </div>
   -->

   如需管理請求清單中資訊的詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。


<!-- Removed all these sections because this is common to ALL the Glists/ enhanced lists. So, we will update that article with all the specific steps: 
1. Select the field that you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by
   * Custom fields from the request or from the created object   

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.


The filter is saved automatically.

-->

>[!TIP]
>
>如果貴組織除了Adobe Workfront外也購買了Workfront Planning，「我的請求」Widget將會同時包含Workfront和Workfront Planning請求。
> 
>* 若要僅篩選Workfront請求，請將篩選設定為&#x200B;**物件型別** > **具有任何** > **問題**。
>* 若要僅篩選Workfront Planning請求，請將篩選設定為&#x200B;**物件型別** > **沒有** > **問題**。

<!--

## Adjust or add columns

You can choose which of the available columns appear on the My Requests widget, and set their order.

Available columns include:

* Subject
* Created object
* Object type
* Status
* Request form
* Entry date
* Entered by

To adjust the columns on the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Columns**.
1. (Optional) To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the first column.
1. (Optional) Use the toggle to hide or show the column in the requests list.
1. To add a custom field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list, and click the plus icon next to the custom field that you want to add as a column to the widget.

   Custom fields on forms attached to the object in the list are available to add as columns.

Column preferences are saved automatically.

-->

<!--

## Create a view

You can create views in the My Requests widget to change the way the information displays in the request list. 

Consider the following when working with views in the My Requests widget:

* A view in the My Requests widget contains the columns and filters applied to the view.
* You can create views and share them with others. The filters and columns you select for the view before you share it are included in the views you share. 
* The following is a system view which you cannot edit, share, or delete: 

   * Widget Unified Requests Default View
* Creating and editing a view in the My Requests widget is similar to enhanced lists. For information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). 

-->

## 搜尋請求

若要在「我的請求」小工具中搜尋特定請求：

1. 按一下右上角的&#x200B;**[!UICONTROL 主功能表]** ![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （視條件而定）將&#x200B;**我的請求** Widget新增至您的主畫面。 按一下&#x200B;**自訂**，找到&#x200B;**我的要求**，然後按一下它以將其新增到&#x200B;**首頁**。
1. 在「我的請求」Widget右上角附近的搜尋列中，輸入您要搜尋的字詞。

   包含辭彙的請求會以橘色醒目提示。

1. （可選）若要跳至醒目提示的請求，請按一下搜尋列中的向上或向下箭頭。

## 移至請求建立的物件

您可以在「我的請求」Widget中找到請求建立的物件。

>[!NOTE]
>
>建立物件的連結僅適用於Planning請求的新請求體驗，當請求本身建立了物件時。 如果Workfront請求轉換為專案或其他物件，則指向該轉換物件的連結在新請求體驗的請求清單中無法使用。

1. 按一下右上角的&#x200B;**[!UICONTROL 主功能表]** ![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （視條件而定）將&#x200B;**我的請求** Widget新增至您的主畫面。 按一下&#x200B;**自訂**，找到&#x200B;**我的要求**，然後按一下它以將其新增到&#x200B;**首頁**。
1. 找出建立物件的請求。
1. 按一下該要求的&#x200B;**已建立物件**&#x200B;欄中的物件名稱。

   物件的頁面隨即開啟。

