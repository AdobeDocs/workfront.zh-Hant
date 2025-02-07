---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 設定系統更新
description: Workfront會在物件的[!UICONTROL 更新]區域產生自動系統更新，以記錄使用者對物件執行的變更。 作為 [!DNL Workfront] 管理員，您可以設定哪些物件欄位和動作 [!DNL Workfront] 追蹤以記錄系統更新。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 8%

---

# 設定系統更新

[!DNL Adobe Workfront]在物件的[!UICONTROL 更新]區域產生自動系統更新，以記錄下列事件：

* 使用者在物件欄位中所做的變更
* 使用者對物件執行的動作

這些系統更新包含下列型別的資訊：

* 已進行的變更
* 進行變更的使用者名稱
* 變更的時間和日期

如需系統更新的詳細資訊，請參閱[系統追蹤的更新](../system-tracked-update-feeds/system-tracked-update-feeds.md)。

作為[!DNL Workfront]管理員，您可以設定哪些物件欄位和動作[!DNL Workfront]追蹤以記錄系統更新。

例如，您可以讓[!DNL Workfront]追蹤使用者對整個系統中的問題名稱所做的所有變更。 然後，任何問題名稱變更都會顯示為問題[!UICONTROL 更新]區域上的系統更新。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>新增：[！UICONTROL Standard]</p>
   或
   <p>目前： [！UICONTROL計畫]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 決定物件型別要追蹤哪些欄位[!DNL Workfront]

您可以決定當使用者在整個[!DNL Workfront]介面中變更與特定物件型別相關聯的資訊時，[!DNL Workfront]會追蹤哪些資訊。 若要這麼做，請新增或移除您要[!DNL Workfront]追蹤該物件型別的欄位。

>[!NOTE]
>
>* [!DNL Workfront]無法追蹤和記錄有關已計算自訂欄位的更新。
>* 您可以自訂專案、任務、問題、投資組合、計畫和使用者的系統更新。 您無法自訂範本、檔案或時程表的系統更新，但[!DNL Workfront]確實記錄這些物件的系統更新。
>



* [新增您要 [!DNL Workfront] 追蹤的欄位](#add-fields-you-want-workfront-to-track)
* [移除不想追蹤的欄位](#remove-fields-that-you-don-t-want-tracked)

### 新增您要[!DNL Workfront]追蹤的欄位 {#add-fields-you-want-workfront-to-track}

您可以新增要[!DNL Workfront]在整個[!DNL Workfront]介面中追蹤特定物件型別的欄位。 當使用者在該欄位中變更資訊時，[!DNL Workfront]會將有關變更的資訊記錄為物件的[!UICONTROL 更新]區域中的系統更新。

>[!NOTE]
>
>您可以在更新摘要中追蹤最多300個內建和自訂欄位。 若您正在追蹤最大欄位數，且想要追蹤未顯示在[!UICONTROL 所有欄位]子標籤中的其他欄位，您必須先移除部分已追蹤的欄位，才能追蹤新欄位。 如需有關從更新欄位移除欄位的詳細資訊，請參閱[移除您不想追蹤的欄位](#remove-fields-that-you-don-t-want-tracked)。

1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![齒輪設定圖示](assets/gear-icon-settings.png)。

1. 在左側的面板中，按一下&#x200B;**[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**。

1. 按&#x200B;一下&#x200B;**[!UICONTROL 新增欄位]**，然後按一下您要追蹤的物件。

1. 在出現的&#x200B;**[!UICONTROL 更新摘要]**&#x200B;方塊中，開始輸入物件的內建（標準）欄位或自訂欄位，然後按一下以在物件出現在清單中時選取它。

   如果[!DNL Workfront]已在追蹤欄位，您無法從清單中再次新增該欄位。

1. 新增所有您要[!DNL Workfront]追蹤的欄位後，請按一下&#x200B;**[!UICONTROL 新增欄位]**。

   您新增的內建欄位會顯示在&#x200B;**[!UICONTROL 內建欄位]**&#x200B;子標籤下。

   您新增的自訂欄位會顯示在&#x200B;**[!UICONTROL 自訂欄位]**&#x200B;子標籤下。

   **[!UICONTROL 所有欄位]**&#x200B;子標籤同時顯示正在追蹤的內建和自訂欄位。

### 移除不想追蹤的欄位 {#remove-fields-that-you-don-t-want-tracked}

您可以移除不希望系統透過[!DNL Workfront]介面追蹤特定物件型別的欄位。

1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![齒輪設定圖示](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**。

1. 在&#x200B;**[!UICONTROL 追蹤的欄位]**&#x200B;標籤上，選取&#x200B;**[!UICONTROL 所有欄位]**&#x200B;子標籤。

   這會顯示目前追蹤的內建和自訂欄位。

1. 選取您要停止追蹤的欄位，然後按一下[移除]。****

1. 在出現的&#x200B;**[!UICONTROL 移除欄位]**&#x200B;方塊中，按一下&#x200B;**[!UICONTROL 是，移除它]**&#x200B;以進行確認。

有關先前追蹤的欄位的任何更新會保留在記錄它們的[!UICONTROL 更新]區域中。

## 決定物件型別要追蹤哪些動作[!DNL Workfront]

您可以讓[!DNL Workfront]在整個[!DNL Workfront]介面中追蹤使用者可以在物件上執行的下列動作。

例如，每次使用者將指派變更至任務或問題時，您都可以讓[!DNL Workfront]記錄更新。 然後，變更會以系統更新的形式出現在任務或問題的[!UICONTROL 更新]區域中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>動作</strong> </th> 
   <th><strong>物件</strong> </th> 
   <th><strong>預設狀態</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>指派已變更</td> 
   <td>任務、問題</td> 
   <td> <p>已啟用</p> </td> 
  </tr> 
  <tr> 
   <td>基準線已刪除</td> 
   <td>專案</td> 
   <td> <p>已停用</p> </td> 
  </tr> 
  <tr> 
   <td>記賬記錄已建立或已刪除</td> 
   <td>專案</td> 
   <td> <p>已啟用</p> </td> 
  </tr> 
  <tr> 
   <td>文件已建立或已刪除</td> 
   <td>專案、任務、問題、投資組合、項目計劃等</td> 
   <td> <p>已啟用</p> </td> 
  </tr> 
  <tr> 
   <td>費用已建立或已刪除</td> 
   <td>專案、任務</td> 
   <td> <p>已啟用</p> </td> 
  </tr> 
  <tr> 
   <td>小時已記錄或已刪除</td> 
   <td>專案、任務、問題</td> 
   <td> <p>已啟用</p> </td> 
  </tr> 
  <tr> 
   <td>問題已刪除</td> 
   <td>專案</td> 
   <td> <p>已啟用</p> </td> 
  </tr> 
  <tr> 
   <td>任務已刪除</td> 
   <td>專案</td> 
   <td> <p>已啟用</p> </td> 
  </tr> 
  <tr> 
   <td>某人的存取權限已變更</td> 
   <td>專案、任務、問題、文件、投資組合、計劃</td> 
   <td> <p>已啟用</p> </td> 
  </tr> 
  <tr> 
   <td>訂閱註解物件</td> 
   <td>專案、任務、問題</td> 
   <td> <p>已啟用</p> </td> 
  </tr> 
 </tbody> 
</table>

若要設定您要[!DNL Workfront]追蹤的動作：

1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![齒輪設定圖示](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**。

1. 按一下&#x200B;**[!UICONTROL 動作]**&#x200B;標籤。

1. 選取要啟用的動作，或取消選取要停用的動作。
1. 按一下「**[!UICONTROL 儲存]**」。

當您停用動作時，先前記錄的有關該動作的任何更新都會保留在記錄該動作的[!UICONTROL 更新]區域中。
