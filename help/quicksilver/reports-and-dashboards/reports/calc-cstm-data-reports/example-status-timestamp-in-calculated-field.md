---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 「計算自訂欄位範例：在自訂表單中顯示狀態時間戳記」
description: 下列計算欄位會顯示物件狀態標示為進行中(INP)的日期。 您可以對問題、任務或專案的計算自訂欄位使用相同的資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 計算自訂欄位範例：在自訂表單中顯示狀態時間戳記

下列計算欄位會顯示物件狀態標示為進行中(INP)的日期。 您可以對問題、任務或專案的計算自訂欄位使用相同的資訊。

>[!NOTE]
>
>如果物件的狀態變更為INP，接著又變更為其他狀態，然後變回INP，Adobe Workfront只會擷取第一次變更為INP的時間戳記。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。</p> 
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
   <td><strong>存取層級設定*</strong> </td> 
   <td> <p>編輯建立報告、儀表板和行事曆的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>物件許可權</strong> </p> </td> 
   <td> <p>管理附加表單之物件的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。<br>如需儀表板許可權的詳細資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">共用報告、儀表板和行事曆</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 先決條件

若要將顯示欄位編輯歷史記錄的計算欄位新增至自訂表單，您必須先建立自訂表單。

## 在自訂表單中顯示狀態時間戳記

1. 前往您要新增欄位的自訂表單。
1. 按一下&#x200B;**計算**&#x200B;將計算自訂欄位新增至表單。
1. 輸入自訂欄位的&#x200B;**標籤**，例如&#x200B;*狀態時間戳記自訂欄位*。
1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存+關閉**。
1. 重新開啟自訂表單，然後在表單上選取新的&#x200B;**狀態時間戳記自訂欄位**。
1. 在&#x200B;**計算**&#x200B;方塊中，複製並貼上自訂欄位的下列計算：

   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >對於所有物件和所有狀態，此計算都相同。 在此計算中，您必須一律使用三個字母的索引鍵，而不是物件狀態的狀態名稱。
   >
   >如需有關狀態索引鍵的詳細資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

1. 按一下&#x200B;**儲存+關閉**。

   您現在可以針對「狀態時間戳記自訂欄位」製作報表，或將其用於其他計算、報表或自訂欄位。
