---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 設定系統更新
description: Workfront會在物件的中產生自動系統更新 [!UICONTROL 更新] 區域來記錄使用者對物件執行的變更。 作為 [!DNL Workfront] 管理員，您可以設定哪些物件欄位和動作 [!DNL Workfront] 追蹤以記錄系統更新。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 7%

---

# 設定系統更新

[!DNL Adobe Workfront] 在物件的中產生自動系統更新 [!UICONTROL 更新] 區域以記錄下列事件：

* 使用者在物件欄位中所做的變更
* 使用者對物件執行的動作

這些系統更新包含下列型別的資訊：

* 已進行的變更
* 進行變更的使用者名稱
* 變更的時間和日期

如需有關系統更新的詳細資訊，請參閱 [系統追蹤更新](../system-tracked-update-feeds/system-tracked-update-feeds.md).

作為 [!DNL Workfront] 管理員，您可以設定哪些物件欄位和動作 [!DNL Workfront] 追蹤以記錄系統更新。

例如，您可以 [!DNL Workfront] 追蹤使用者對整個系統中的問題名稱所做的所有變更。 然後，任何問題名稱變更將作為系統更新出現在問題的上 [!UICONTROL 更新] 區域。

## 存取需求

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
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 決定哪些欄位 [!DNL Workfront] 追蹤物件型別

您可以決定哪些資訊 [!DNL Workfront] 追蹤使用者何時在整個過程中變更與特定物件型別相關的資訊 [!DNL Workfront] 介面。 您可以新增或移除想要的欄位來執行此操作 [!DNL Workfront] 以追蹤該物件型別。

>[!NOTE]
>
>* [!DNL Workfront] 無法追蹤和記錄有關計算自訂欄位的更新。
>* 您可以自訂專案、任務、問題、投資組合、計畫和使用者的系統更新。 您無法自訂範本、檔案或時程表的系統更新，但是 [!DNL Workfront] 會記錄這些物件的系統更新。
>



* [新增您想要的欄位 [!DNL Workfront] 要追蹤的](#add-fields-you-want-workfront-to-track)
* [移除不想追蹤的欄位](#remove-fields-that-you-don-t-want-tracked)

### 新增您想要的欄位 [!DNL Workfront] 要追蹤的 {#add-fields-you-want-workfront-to-track}

您可以新增想要的欄位 [!DNL Workfront] 以追蹤整個過程中的特定物件型別 [!DNL Workfront] 介面。 當使用者變更該欄位中的資訊時， [!DNL Workfront] 將有關變更的資訊記錄為中的系統更新 [!UICONTROL 更新] 物件的區域。

>[!NOTE]
>
>您可以在更新摘要中追蹤最多300個內建和自訂欄位。 如果您要追蹤最大欄位數，並想追蹤未顯示在 [!UICONTROL 所有欄位] 子索引標籤中，您必須先移除部分已追蹤的欄位，才能追蹤新欄位。 如需有關從更新欄位中移除欄位的詳細資訊，請參閱 [移除不想追蹤的欄位](#remove-fields-that-you-don-t-want-tracked).

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側的面板中，按一下 **[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**.

1. 按&#x200B;一下 **[!UICONTROL 新增欄位]**，然後按一下您要追蹤的物件。

1. 在&#x200B; **[!UICONTROL 更新摘要]** 在出現的方塊中，開始輸入物件的內建（標準）欄位或自訂欄位，然後按一下以在物件出現在清單中時選取它。

   如果 [!DNL Workfront] 已在追蹤欄位，您無法從清單中再次新增該欄位。

1. 新增所有您想要的欄位後 [!DNL Workfront] 若要追蹤，請按一下 **[!UICONTROL 新增欄位]**.

   您新增的內建欄位會顯示在 **[!UICONTROL 內建欄位]** 子標籤。

   您新增的自訂欄位會顯示在 **[!UICONTROL 自訂欄位]** 子標籤。

   此 **[!UICONTROL 所有欄位]** 子標籤會顯示正在追蹤的內建和自訂欄位。

### 移除不想追蹤的欄位 {#remove-fields-that-you-don-t-want-tracked}

您可以移除不希望系統追蹤整個過程中特定物件型別的欄位 [!DNL Workfront] 介面。

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**.

1. 在 **[!UICONTROL 已追蹤的欄位]** 索引標籤中，選取 **[!UICONTROL 所有欄位]** 子標籤。

   這會顯示目前追蹤的內建和自訂欄位。

1. 選取您要停止追蹤的欄位，然後按一下 **[!UICONTROL 移除]**.

1. 在 **[!UICONTROL 移除欄位]** 方塊中，按一下 **[!UICONTROL 是的，請移除]** 以確認。

有關先前追蹤欄位的任何更新都會保留在 [!UICONTROL 更新] 錄製區域。

## 決定哪些動作 [!DNL Workfront] 追蹤物件型別

您可以 [!DNL Workfront] 在整個中追蹤使用者可在物件上執行的下列動作 [!DNL Workfront] 介面。

例如，您可以 [!DNL Workfront] 每次使用者變更任務或問題時記錄更新。 然後，變更會以系統更新的形式出現在 [!UICONTROL 更新] 任務或問題的區域。

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

設定您要執行的動作 [!DNL Workfront] 要追蹤的：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**.

1. 按一下 **[!UICONTROL 動作]** 標籤。

1. 選取要啟用的動作，或取消選取要停用的動作。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

當您停用動作時，先前就該動作所錄製的任何更新都會保留在 [!UICONTROL 更新] 錄製區域。
