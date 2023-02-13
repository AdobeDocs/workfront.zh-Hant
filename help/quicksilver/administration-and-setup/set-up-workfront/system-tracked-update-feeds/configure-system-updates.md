---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 配置系統更新
description: Workfront會在物件的中產生自動系統更新 [!UICONTROL 更新] 區域，記錄用戶對對象執行的更改。 As a [!DNL Workfront] 管理員，可以配置哪些對象欄位和操作 [!DNL Workfront] 記錄系統更新的跟蹤。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 7%

---

# 配置系統更新

[!DNL Adobe Workfront] 在對象中生成自動系統更新 [!UICONTROL 更新] 區域來記錄下列事件：

* 使用者在物件欄位中所做的變更
* 使用者對物件執行的動作

這些系統更新包括所進行的更改、進行更改的用戶的名稱、更改的時間和日期。

As a [!DNL Workfront] 管理員，可以配置哪些對象欄位和操作 [!DNL Workfront] 記錄系統更新的跟蹤。

例如，您可以 [!DNL Workfront] 追蹤使用者對整個系統問題名稱所做的所有變更。 任何問題名稱的更改將作為問題的系統更新顯示 [!UICONTROL 更新] 的上界。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 決定哪些欄位 [!DNL Workfront] 對象類型的跟蹤

您可以決定哪些資訊 [!DNL Workfront] 跟蹤用戶在整個過程中更改與特定對象類型關聯的資訊的時間 [!DNL Workfront] 介面。 若要這麼做，請新增或移除您想要的欄位 [!DNL Workfront] 來追蹤該物件類型。

>[!NOTE]
>
>* [!DNL Workfront] 無法追蹤及記錄有關計算自訂欄位的更新。
>* 您可以自訂專案、工作、問題、產品組合、方案和使用者的系統更新。 不能自定義模板、文檔或時間表的系統更新，但 [!DNL Workfront] 會記錄這些對象的系統更新。
>




* [新增您想要的欄位 [!DNL Workfront] 追蹤](#add-fields-you-want-workfront-to-track)
* [移除您不想追蹤的欄位](#remove-fields-that-you-don-t-want-tracked)

### 新增您想要的欄位 [!DNL Workfront] 追蹤 {#add-fields-you-want-workfront-to-track}

您可以新增所需欄位 [!DNL Workfront] 在 [!DNL Workfront] 介面。 當用戶更改該欄位中的資訊時， [!DNL Workfront] 在 [!UICONTROL 更新] 區域。

>[!NOTE]
>
>您可以在更新摘要中追蹤最多300個內建和自訂欄位。 如果您要追蹤欄位數上限，且想要追蹤未顯示在 [!UICONTROL 所有欄位] 子索引標籤中，您必須先移除部分追蹤欄位，才能追蹤新欄位。 有關從更新欄位中刪除欄位的詳細資訊，請參閱 [移除您不想追蹤的欄位](#remove-fields-that-you-don-t-want-tracked).

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側的面板中，按一下 **[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**.

1. &#x200B;按一下 **[!UICONTROL 新增欄位]**，然後按一下您要追蹤的物件。

1. 在 **[!UICONTROL 更新摘要]** 框中，開始鍵入對象的內置（標準）欄位或自定義欄位，然後按一下以在清單中顯示時選擇它。

   若 [!DNL Workfront] 已在追蹤欄位，則無法從清單中再次新增欄位。

1. 新增您想要的所有欄位後 [!DNL Workfront] 若要追蹤，請按一下 **[!UICONTROL 新增欄位]**.

   新增的內建欄位會顯示在 **[!UICONTROL 內建欄位]** 頁簽。

   新增的自訂欄位會顯示在 **[!UICONTROL 自訂欄位]** 頁簽。

   此 **[!UICONTROL 所有欄位]** 子索引標籤會顯示正在追蹤的內建和自訂欄位。

### 移除您不想追蹤的欄位 {#remove-fields-that-you-don-t-want-tracked}

您可以在 [!DNL Workfront] 介面。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**.

1. 在 **[!UICONTROL 追蹤的欄位]** 頁簽，選擇 **[!UICONTROL 所有欄位]** 頁簽。

   這會顯示目前追蹤的內建和自訂欄位。

1. 選取您要停止追蹤的欄位，然後按一下 **[!UICONTROL 移除]**.

1. 在 **[!UICONTROL 刪除欄位]** 框，按一下 **[!UICONTROL 是，刪除它]** 確認。

先前追蹤欄位的任何更新都會保留在 [!UICONTROL 更新] 記錄的區域。

## 決定哪些動作 [!DNL Workfront] 對象類型的跟蹤

您可以 [!DNL Workfront] 追蹤使用者可在 [!DNL Workfront] 介面。

例如，您可以 [!DNL Workfront] 每次用戶將分配更改為任務或問題時都記錄更新。 然後，變更會以系統更新的形式顯示於 [!UICONTROL 更新] 區域。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>動作</strong> </th> 
   <th><strong>物件</strong> </th> 
   <th><strong>主要狀態</strong> </th> 
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
   <td>已建立或刪除計費記錄</td> 
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

設定您要執行的動作 [!DNL Workfront] 若要追蹤：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**.

1. 按一下 **[!UICONTROL 動作]** 標籤。

1. 選取要啟用的動作，或取消選取要停用的動作。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

當您停用動作時，先前記錄的關於該動作的任何更新都會保留在 [!UICONTROL 更新] 記錄的區域。
