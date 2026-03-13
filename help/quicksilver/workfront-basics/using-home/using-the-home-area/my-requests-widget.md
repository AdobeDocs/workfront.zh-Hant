---
product-area: projects
navigation-topic: use-the-home-area
title: 使用「我的請求」小部件
description: 您可以在「我的請求」構件中提交請求。 還可以使用篩選器和列自定義小部件。
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 3893a57fb7ae31a1649b20beccc1f0b79f2421fb
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 3%

---

# 使用「我的請求」小部件

>[!IMPORTANT]
>
>本文介紹新的「我的請求」小部件。 必須啟用新的請求體驗才能查看新小部件。
>您可以在「請求」區域啟用新的請求體驗。

「我的請求」小部件顯示您已提交的請求。 您可以篩選請求、搜索特定請求或調整列順序和可見性。 您也可以從「我的請求」小部件建立新請求。

>[!NOTE]
>
>* 載入「我的請求」小部件時，它最多顯示50個請求。 要顯示更多請求，請向下滾動清單。

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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 許可證</strong></td> 
   <td> <p>貢獻者或更高</p>
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
   <td> <p>[！UICONTROL檢視]對您在對話中被標籤或需要解決核准的專案、任務、問題和檔案的許可權或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立請求

您可以直接從「我的請求」構件建立請求。

有關說明，請參閱文章[從「首頁」區域](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request)建立工作項和項目[建立請求](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)部分。

## 複製請求

您可以在「我的請求」小部件中複製請求，對其進行編輯，然後將其作為新請求提交。

有關說明，請參閱[複製和提交請求](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md)。

## 篩選請求

「我的請求」小部件具有可自定義的篩選器，可讓您控制小部件中顯示的請求。 您可以為不同的欄位和值配置此篩選器，並可以使用AND和OR運算子來堆疊條件。

要在「我的請求」小部件中配置篩選器，請執行以下操作：

1. 按一下右上角的&#x200B;**[!UICONTROL 主菜單]** ![主菜單表徵圖](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （視條件而定）將&#x200B;**我的請求** Widget新增至您的主畫面。 按一下&#x200B;**自訂**，找到&#x200B;**我的要求**，然後按一下它以將其新增到&#x200B;**首頁**。
1. 在&#x200B;**我的請求** Widget中，按一下&#x200B;**篩選器**。
1. 選擇要篩選依據的欄位。 可選擇下列選項：

   * 工作區
   * 物件類型
   * 輸入日期
   * 請求表單
   * 狀態
   * 輸入者
   * 請求或建立物件的自訂欄位

1. 在下一個欄位中，選擇要用於此篩選條件的運算子。 可用運算子取決於所選欄位。
1. （條件）如果運算子右側出現欄位，請選擇要篩選的值。
1. （可選）要添加其他篩選條件，請按一下&#x200B;**添加條件**，然後重複步驟4-6。
1. （可選和條件）如果您有多個條件，請通過按一下條件左側的&#x200B;**和**&#x200B;或&#x200B;**或**&#x200B;來切換和或值。

過濾器會自動保存。

>[!TIP]
>
>如果您的組織除了購買Adobe Workfront之外還購買了Workfront規劃，「我的請求」小部件將同時包括Workfront和Workfront規劃請求。
> 
>* 若要僅篩選Workfront請求，請將篩選設定為&#x200B;**物件型別** > **具有任何** > **問題**。
>* 若要僅篩選Workfront Planning請求，請將篩選設定為&#x200B;**物件型別** > **沒有** > **問題**。

## 調整或添加列

您可以選擇「我的請求」構件上顯示哪些可用列，並設定其順序。

可用列包括：

* 主旨
* 已建立的物件
* 物件類型
* 狀態
* 請求表單
* 輸入日期
* 輸入者

要調整「我的請求」小部件上的列，請執行以下操作：

1. 按一下右上角的&#x200B;**[!UICONTROL 主菜單]** ![主菜單表徵圖](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （條件）將&#x200B;**我的請求**&#x200B;小部件添加到您的主螢幕。 按一下&#x200B;**自定義**，找到&#x200B;**我的請求**，然後按一下將其添加到&#x200B;**首頁**。
1. 在&#x200B;**我的請求**&#x200B;小部件中，按一下&#x200B;**列**。
1. （可選）要重新排序列，請按一下要移動的列的拖動句柄![拖動句柄](assets/drag-handle.png)，並將其拖動到所需位置。 清單頂部的列作為第一列顯示在「我的請求」構件中。
1. （可選）使用切換可隱藏或顯示請求清單中的列。
1. 若要將自定義欄位添加為列，請按一下清單右上角的&#x200B;**添加列**&#x200B;表徵圖![添加列](assets/add-column.png)，然後按一下要作為列添加到小部件的自定義欄位旁邊的加號表徵圖。

   清單中附加到對象的表單上的自定義欄位可作為列添加。

欄偏好設定會自動儲存。

## 建立檢視

您可以在「我的請求」小部件中建立視圖，以更改資訊在請求清單中的顯示方式。

在「我的請求」小部件中處理視圖時，請考慮以下事項：

* 「我的請求」小部件中的視圖包含應用於該視圖的列和篩選器。
* 您可以建立視圖，並與他人共用它們。 在您共用檢視之前，您為檢視選取的篩選器和欄會包含在您共用的檢視中。
* 下列是您無法編輯、共用或刪除的系統檢視：

   * Widget整合請求預設檢視
* 在「我的請求」Widget中建立和編輯檢視類似於增強型清單。 如需詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

## 搜尋請求

要在「我的請求」構件中搜索特定請求，請執行以下操作：

1. 按一下右上角的&#x200B;**[!UICONTROL 主菜單]** ![主菜單表徵圖](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （條件）將&#x200B;**我的請求**&#x200B;小部件添加到您的主螢幕。 按一下&#x200B;**自定義**，找到&#x200B;**我的請求**，然後按一下將其添加到&#x200B;**首頁**。
1. 在「我的請求」小部件右上角的搜索欄中，輸入要搜索的術語。

   包含辭彙的請求會以橘色醒目提示。

1. （可選）要跳轉到突出顯示的請求，請按一下搜索欄中的上箭頭或下箭頭。

## 轉到由請求建立的對象

您可以在「我的請求」小部件中查找由請求建立的對象。

>[!NOTE]
>
>在新請求體驗中，僅對Planning請求提供指向已建立對象的連結，在請求本身已建立對象的情況下。 如果將Workfront請求轉換為項目或其他對象，則到該轉換對象的連結在新請求體驗中的請求清單中不可用。

1. 按一下右上角的&#x200B;**[!UICONTROL 主菜單]** ![主菜單表徵圖](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （視條件而定）將&#x200B;**我的請求** Widget新增至您的主畫面。 按一下&#x200B;**自訂**，找到&#x200B;**我的要求**，然後按一下它以將其新增到&#x200B;**首頁**。
1. 找到建立對象的請求。
1. 按一下該請求的&#x200B;**已建立對象**&#x200B;列中的對象名稱。

   對象的頁面隨即開啟。

