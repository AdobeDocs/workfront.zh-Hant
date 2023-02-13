---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: '''計算自訂欄位範例：在自訂表單中顯示狀態時間戳記'
description: 以下計算欄位顯示對象狀態被標籤為In Progress(INP)的日期。 對於問題、任務或專案的計算自訂欄位，您可以使用相同的資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 計算的自訂欄位範例：在自訂表單中顯示狀態時間戳記

以下計算欄位顯示對象狀態被標籤為In Progress(INP)的日期。 對於問題、任務或專案的計算自訂欄位，您可以使用相同的資訊。

>[!NOTE]
>
>如果物件的狀態變更為INP，然後變更為其他狀態，再回到INP,Adobe Workfront只會擷取第一次變更為INP的時間戳記。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront授權*</p> </td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>訪問級別配置*</strong> </td> 
   <td> <p>編輯建立報表、控制面板和日曆的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>物件權限</strong> </p> </td> 
   <td> <p>管理表單所附加之物件的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.<br>如需控制面板權限的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">共用報表、控制面板和日曆 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 先決條件

若要將顯示欄位編輯歷史記錄的計算欄位新增至自訂表單，您必須先建立自訂表單。

## 在自訂表單中顯示狀態時間戳記

1. 移至您要新增欄位的自訂表單。
1. 按一下 **計算** 新增計算的自訂欄位至表單。
1. 輸入 **標籤** (例如 *狀態時間戳自定義欄位*.
1. 按一下 **完成**，然後按一下 **儲存並關閉**.
1. 重新開啟自訂表單，然後選取新 **狀態時間戳自定義欄位** 在表單上。
1. 在 **計算** 方塊中，複製並貼上自訂欄位的下列計算：

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >所有對象和所有狀態的此計算都相同。 在此計算中，必須始終使用三字母鍵，而不是對象狀態的狀態名稱。
   >
   >如需狀態索引鍵的詳細資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. 按一下 **儲存並關閉**.

   您現在可以報告狀態時間戳記自訂欄位，或用於其他計算、報表或自訂欄位。
