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
source-git-commit: f7cb314067d105d5534f4be356024aea8e8f9a28
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 8%

---

# 設定系統更新

<!-- Audited: 6/2025 -->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div> -->

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
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

*如需此表格中資訊的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 決定物件型別要追蹤哪些欄位[!DNL Workfront]

您可以決定當使用者在整個[!DNL Workfront]介面中變更與特定物件型別相關聯的資訊時，[!DNL Workfront]會追蹤哪些資訊。 若要這麼做，請新增或移除您要[!DNL Workfront]追蹤該物件型別的欄位。

>[!NOTE]
>
>* [!DNL Workfront]無法追蹤和記錄有關已計算自訂欄位的更新。
>* 您可以自訂專案、任務、問題、投資組合、計畫和使用者的系統更新。 您無法自訂範本、檔案或時程表的系統更新，但[!DNL Workfront]確實記錄這些物件的系統更新。
>


### 新增您要[!DNL Workfront]追蹤的欄位 {#add-fields-you-want-workfront-to-track}

您可以新增要[!DNL Workfront]在整個[!DNL Workfront]介面中追蹤特定物件型別的欄位。 當使用者在該欄位中變更資訊時，[!DNL Workfront]會將有關變更的資訊記錄為物件的[!UICONTROL 更新]區域中的系統更新。

>[!NOTE]
>
>您可以在更新摘要中追蹤最多300個內建和自訂欄位。 若您正在追蹤最大欄位數，且想要追蹤未顯示在[!UICONTROL 所有欄位]子標籤中的其他欄位，您必須先移除部分已追蹤的欄位，才能追蹤新欄位。 如需有關從更新欄位移除欄位的詳細資訊，請參閱[移除您不想追蹤的欄位](#remove-fields-you-don-t-want-tracked)。

{{step-1-to-setup}}

1. 在左側的面板中，按一下&#x200B;**[!UICONTROL 介面]**，然後按&#x200B;**[!UICONTROL 更新摘要]**。
1. （選擇性）在&#x200B;**追蹤的欄位**&#x200B;索引標籤中，根據您要在更新摘要中追蹤的欄位型別，按一下下列其中一個子索引標籤：

   * **內建欄位**：顯示內建欄位清單。
   * **自訂欄位**：顯示自訂欄位清單。 您必須先建立自訂欄位，清單才能顯示這些欄位。
   * **所有欄位**：顯示內建和自訂欄位的清單。

1. 按一下&#x200B;**[!UICONTROL 新增欄位]**，然後從下拉式清單中選取您要追蹤的物件。

   手動選取欄位並非適用於具有「更新」區域的所有物件。

   從欄位中選取下列物件：

   * 專案
   * 任務
   * 問題
   * 專案組合
   * 方案
   * 使用者

   針對每個選取的物件，**新增欄位**&#x200B;方塊會開啟。
1. 在&#x200B;**新增欄位**&#x200B;方塊中，開始輸入物件的內建（標準）欄位或自訂欄位，然後當物件出現在清單中時選取它。

   >[!NOTE]
   >
   >如果[!DNL Workfront]已在追蹤欄位，您無法從清單中再次新增該欄位。

1. 新增所有您要[!DNL Workfront]追蹤的欄位後，請按一下&#x200B;**[!UICONTROL 新增欄位]**。
您新增的內建欄位會顯示在**[!UICONTROL 內建欄位]**&#x200B;子標籤下，而自訂欄位會顯示在&#x200B;**[!UICONTROL 自訂欄位]**子標籤下。
**[!UICONTROL 所有欄位]**&#x200B;子標籤會顯示[!DNL Workfront]追蹤的內建和自訂欄位。

<!-- replace the above when releasing to Preview: 

1. In the panel on the left, click **[!UICONTROL Interface]**, then **[!UICONTROL Update Feeds]**.
1. (Optional) In the <span class="preview">**Tracked fields** tab</span>, click one of the following subtabs, depending on which types of fields you want to track in the update feed:

   * <span class="preview">**Built-in fields**</span>: Displays a list of built-in fields.
   * <span class="preview">**Custom fields**</span>: Displays a list of custom fields. You must create the custom fields before they are available in the list. 
   * <span class="preview">**All fields**</span>: Displays a list of both built-in and custom fields. 

1. Click <span class="preview">**[!UICONTROL Add fields]**,</span> then select the object that you want to be tracked from the drop-down. 

   Manually selecting fields is not available for all the objects that have an Updates area.

   Select from fields for the following objects:

      * Project
      * Task
      * Issue
      * Portfolio
      * Program
      * User

   The <span class="preview">**Add fields** </span> box opens, for each object selected.
1. In the <span class="preview">**Add fields** </span> box, start typing either a built-in (standard) field or a custom field for the object, then select it when it appears in the list.

   >[!NOTE]
   >
   >If [!DNL Workfront] is already tracking the field, you can't add it a second time from the list.

1. After adding all the fields you want [!DNL Workfront] to track, <span class="preview"> click **[!UICONTROL Add]**.
   The built-in fields that you added show under the **[!UICONTROL Built-in fields]** subtab, and the custom fields show under the **[!UICONTROL Custom fields]** subtab.
   The **[!UICONTROL All fields]** subtab shows both the built-in and the custom fields that [!DNL Workfront] tracks.</span>

-->

### 移除您不想要追蹤的欄位 {#remove-fields-you-don-t-want-tracked}

您可以移除不希望系統透過[!DNL Workfront]介面追蹤特定物件型別的欄位。

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 介面]**，然後按&#x200B;**[!UICONTROL 更新摘要]**。

1. 在&#x200B;**[!UICONTROL 追蹤的欄位]**&#x200B;標籤上，選取&#x200B;**[!UICONTROL 所有欄位]**&#x200B;子標籤。 目前追蹤的內建和自訂欄位都會顯示。

1. 選取您要停止追蹤的欄位，然後按一下&#x200B;**[!UICONTROL 移除]**。


<!--replace above at Preview release with this:

1. On the <span class="preview">**[!UICONTROL Tracked fields]** tab</span>, select the **[!UICONTROL All fields]** subtab. Both the built-in and custom fields that are currently being tracked display.

1. Select the field you want to stop tracking, then click the <span class="preview">**[!UICONTROL Remove]** icon ![Remove icon](assets/remove-icon.png).</span>

-->

1. 在出現的&#x200B;**[!UICONTROL 移除欄位]**&#x200B;方塊中，按一下&#x200B;**[!UICONTROL 是，移除它]**&#x200B;以進行確認。

   有關先前追蹤的欄位的任何更新會保留在記錄它們的[!UICONTROL 更新]區域中。

## 決定物件型別要追蹤哪些動作[!DNL Workfront]

您可以讓使用者在[!DNL Workfront]介面中的物件上執行[!DNL Workfront]個追蹤動作。

例如，每次使用者將指派變更至任務或問題時，您都可以讓[!DNL Workfront]記錄更新。

然後，變更會以系統更新的形式出現在任務或問題的[!UICONTROL 更新]區域中。

下表說明您可以在[!DNL Workfront]中追蹤的物件動作：

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

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 介面]**，然後按&#x200B;**[!UICONTROL 更新摘要]**。

1. 按一下&#x200B;**[!UICONTROL 動作]**&#x200B;標籤。

1. 選取動作的核取方塊以啟用動作，或取消選取動作以停用動作。
1. 按一下「**[!UICONTROL 儲存]**」。

   當您停用動作時，先前記錄的有關該動作的任何更新都會保留在記錄該動作的[!UICONTROL 更新]區域中。 [!DNL Workfront]停止記錄已停用動作的任何新更新。
