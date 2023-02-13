---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 存取，模型，漏斗，圖表，層級，權限
navigation-topic: access-levels
title: 每種物件類型皆可使用的功能
description: 下表列出了各種訪問級別中每種對象類型可用的功能。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '1457'
ht-degree: 12%

---

# 每種物件類型皆可使用的功能

下表列出了各種訪問級別中每種對象類型可用的功能。

它也會指出Workfront管理員可使用存取層級來停用或啟用的動作。

## 專案

只有具有計畫許可證的用戶才能獲得項目的完全訪問權限。

| 動作 | 計劃者 | 工作者 | 檢閱者 | 要求者 | 外部用戶 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; |   |   |   |   |
| 複製 | ✓&#42; |   |   |   |   |
| 刪除 | ✓&#42; |   |   |   |   |
| 共用 | ✓&#42; | ✓&#42; |   |   |   |
| 共用全系統 | ✓&#42; |   |   |   |   |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 新增自訂表單 | ✓ |   |   |   |   |
| 更新自訂欄位 | ✓ | ✓ |   |   |   |
| 新增核准程式 | ✓ |   |   |   |   |
| 核准專案 | ✓ | ✓ | ✓ |   |   |
| 添加文檔 | ✓ | ✓ | ✓ |   |   |
| 新增問題 | ✓ | ✓ |   |   |   |
| 新增  個任務 | ✓ | ✓ |   |   |   |
| 提供更新/評論 | ✓ | ✓ | ✓ |   |   |
| 更改狀態 | ✓ |   |   |   |   |
| 記錄時數 | ✓ | ✓ |   |   |   |
| 編輯分配 | ✓ | ✓ |   |   |   |
| 管理基線 | ✓ |   |   |   |   |
| 管理風險 | ✓ |   |   |   |   |
| 管理財務 | ✓ |   |   |   |   |
| 添加/編輯費用 | ✓ | ✓ |   |   |   |
| 附加範本 | ✓ |   |   |   |   |
| 另存為範本 | ✓ |   |   |   |   |
| 添加/編輯業務案例 | ✓ |   |   |   |   |
| 編輯專案詳細資訊 | ✓ |   |   |   |   |
| 編輯人員配置 | ✓ |   |   |   |   |
| 匯出到 MS Project | ✓ | ✓ | ✓ |   |   |
| 重新計算財務/時間表 | ✓ |   |   |   |   |
| 設定隊列屬性 | ✓ |   |   |   |   |



&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 任務

| 動作 | 計劃者 | 工作者 | 檢閱者 | 要求者 | 外部用戶 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; | ✓&#42; |   |   |   |
| 刪除 | ✓&#42; | ✓&#42; |   |   |   |
| 共用 | ✓&#42; | ✓&#42; |   |   |   |
| 共用全系統 | ✓&#42; |   |   |   |   |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 添加前置任務 | ✓ | ✓ |   |   |   |
| 新增  個問題 | ✓ | ✓ |   |   |   |
| 編輯任務（排除狀態） | ✓ | ✓ |   |   |   |
| 更改任務狀態 | ✓ | ✓ |   |   |   |
| 新增文件 | ✓ | ✓ | ✓ |   |   |
| 複製任務 | ✓ | ✓ |   |   |   |
| 移動任務 | ✓ | ✓ |   |   |   |
| 記錄時數 | ✓ | ✓ |   |   |   |
| 接受分配 | ✓ | ✓ |   |   |   |
| 進行指派 | ✓ | ✓ | 僅在行內編輯 | 僅在行內編輯 |   |
| 附加自訂表單 | ✓ | ✓ |   |   |   |
| 編輯自訂欄位 | ✓ | ✓ |   |   |   |
| 建立核准流程 | ✓ | ✓ |   |   |   |
| 核准任務 | ✓ | ✓ | ✓ |   |   |
| 編輯財務 | ✓ |   |   |   |   |
| 添加/編輯費用 | ✓ | ✓ |   |   |   |
| 查看財務 | ✓ | ✓ | ✓ |   |   |
| 更新/注釋 | ✓ | ✓ | ✓ |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 問題

| 動作 | 計劃者 | 工作者 | 檢閱者 | 要求者 | 外部用戶 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 編輯 | ✓ | ✓ | ✓ | ✓ |   |
| 刪除 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 共用 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 共用全系統 | ✓&#42; |   |   |   |   |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 附加自訂表單 | ✓ | ✓ | ✓ | ✓ |   |
| 編輯自訂欄位 | ✓ | ✓ | ✓ | ✓ |   |
| 核准問題 | ✓ | ✓ | ✓ | ✓ |   |
| 新增核准程式 | ✓ | ✓ | ✓ | ✓ |   |
| 新增文件 | ✓ | ✓ | ✓ | ✓ |   |
| 複製問題 | ✓ | ✓ | ✓ | ✓ |   |
| 移動問題 | ✓ | ✓ | ✓ | ✓ |   |
| 記錄時數 | ✓ | ✓ |   |   |   |
| 將問題轉換為專案 | ✓ | ✓ |   |   |   |
| 將問題轉換為任務 | ✓ |   |   |   |   |
| 接受分配 | ✓ | ✓ |   |   |   |
| 進行分配 | ✓ | ✓ |   |   |   |
| 添加更新和注釋 | ✓ | ✓ | ✓ | ✓ |   |



&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 專案組合

只有具有計畫許可證的用戶才能完全訪問產品組合。

| 動作 | 計劃者 | 工作者 | 檢閱者 | 要求者 | 外部用戶 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; |   |   |   |   |
| 刪除 | ✓&#42; |   |   |   |   |
| 共用 | ✓&#42; |   |   |   |   |
| 共用全系統 | ✓&#42; |   |   |   |   |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 編輯詳細資訊 | ✓ |   |   |   |   |
| 附加自訂表單 | ✓ |   |   |   |   |
| 編輯自訂欄位 | ✓ |   |   |   |   |
| 新增和移除專案 | ✓ |   |   |   |   |
| 核准專案 | ✓ |   |   |   |   |
| Portfolio最佳化 | ✓ |   |   |   |   |
| 新增文件 | ✓ | ✓ | ✓ |   |   |
| 添加更新和注釋 | ✓ | ✓ | ✓ |   |   |



&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 計劃

只有具有計畫許可證的用戶才能完全訪問計畫。

| 動作 | 計劃者 | 工作者 | 檢閱者 | 要求者 | 外部用戶 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; |   |   |   |   |
| 刪除 | ✓&#42; |   |   |   |   |
| 共用 | ✓&#42; |   |   |   |   |
| 共用全系統 | ✓&#42; |   |   |   |   |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 編輯詳細資訊 | ✓ |   |   |   |   |
| 附加自訂表單 | ✓ |   |   |   |   |
| 編輯自訂欄位 | ✓ |   |   |   |   |
| 新增和移除專案 | ✓ |   |   |   |   |
| 核准專案 | ✓ |   |   |   |   |
| 投資組合最佳化 | ✓ |   |   |   |   |
| 新增文件 | ✓ | ✓ | ✓ |   |   |
| 添加更新和注釋 | ✓ | ✓ | ✓ |   |   |



&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 報表、控制面板和日曆

擁有計畫許可證的用戶可以完全訪問報告。 所有其他存取層級都可檢視報表的存取權。

| 動作 | 計劃者 | 工作者 | 檢閱者 | 請求 | 外部用戶 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; |   |   |   |   |
| 刪除 | ✓&#42; |   |   |   |   |
| 檢視內建報表 | ✓&#42; |   |   |   |   |
| 共用 | ✓&#42; | ✓ | ✓ |   |   |
| 公開共用日曆和報表 | ✓&#42; |   |   |   |   |
| 共用全系統 | ✓&#42; |   |   |   |   |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| 編輯 | ✓ |   |   |   |   |
| 複製 | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

>[!NOTE]
>
>請求者只能檢視已與其共用的報表

## 篩選器、檢視和群組

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>動作</p> </th> 
   <th> <p>計劃者</p> </th> 
   <th> <p>工作者</p> </th> 
   <th> <p>檢閱者</p> </th> 
   <th> <p>要求者</p> </th> 
   <th>外部用戶<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>建立</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>共用</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>共用全系統</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 文件

| 動作 | 計劃者 | 工作者 | 檢閱者 | 要求者 | 外部用戶 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 刪除（文檔和資料夾） | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 共用 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| 公開共用（外部） | ✓&#42; |   |   |   |   |
| 共用全系統 | ✓&#42; | ✓&#42; |   |   |   |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| 編輯詳細資訊 | ✓ | ✓ | ✓ | ✓ |   |
| 下載 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 結帳 | ✓ | ✓ | ✓ | ✓ |   |
| 添加批准者 | ✓ | ✓ | ✓ | ✓ |   |
| 核准檔案 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 附加自訂表單 | ✓ | ✓ | ✓ | ✓ |   |
| 編輯自訂欄位 | ✓ | ✓ | ✓ | ✓ |   |
| 移至（物件） | ✓ | ✓ | ✓ | ✓ |   |
| 傳送至（整合） | ✓ | ✓ | ✓ | ✓ |   |
| 添加更新和注釋 | ✓ | ✓ | ✓ | ✓ |   |
| 上傳新版本 | ✓ | ✓ | ✓ | ✓ |   |
| 刪除版本 | ✓ | ✓ | ✓ | ✓ |   |
| 預覽 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 校訂 | ✓ | ✓ | ✓ | ✓ |   |
| 生成校樣 | ✓ | ✓ |   |   |   |
| 移除校樣 | ✓ | ✓ | ✓ | ✓ |   |
| 添加/刪除&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| 重新命名&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| 連結（與整合） | ✓ | ✓ | ✓ | ✓ |   |
| 取消連結（整合） | ✓ | ✓ | ✓ | ✓ |   |

{style=&quot;table-layout:auto&quot;}

&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;僅適用於文檔資料夾，不適用於文檔

## 使用者

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>動作</p> </th> 
   <th> <p>計劃者</p> </th> 
   <th>工作者</th> 
   <th> <p>檢閱者</p> </th> 
   <th> <p>要求者</p> </th> 
   <th> <p>外部用戶**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>建立</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯、刪除、停用、登入或重設任何使用者的密碼</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯、刪除、停用、登入或重設其所管理之群組中任何使用者的密碼</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視使用者</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>查看聯繫資訊</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;外部用戶只能搜索其他用戶

## 團隊

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>動作</p> </th> 
   <th> <p>計劃者</p> </th> 
   <th>工作者</th> 
   <th> <p>檢閱者</p> </th> 
   <th> <p>要求者</p> </th> 
   <th> <p>外部用戶*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>建立</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯他們所在的團隊</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>在管理的群組中編輯團隊</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視所有團隊</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>查看與其組關聯的團隊</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 範本

| 動作 | 計劃者 | 工作者 | 檢閱者 | 要求者 | 外部用戶 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; |   |   |   |   |
| 刪除 | ✓&#42; |   |   |   |   |
| 共用 | ✓&#42; |   |   |   |   |
| 共用全系統 | ✓&#42; |   |   |   |   |
| 檢視 | ✓&#42; |   |   |   |   |
| 複製 | ✓ |   |   |   |   |
| 編輯範本詳細資訊 | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## 財務資料

只有具有計畫許可證的用戶才能完全訪問財務資料。

此處不包含請求和外部用戶許可證類型，因為它們無權訪問 [選擇對象或區域].

| 動作 | 計劃者 | 工作者 | 檢閱者 |
|---|---|---|---|
| 編輯職責開單和成本費率 | ✓&#42; |   |   |
| 編輯用戶開單和成本費率 | ✓&#42; |   |   |
| 查看職責開單和成本費率 | ✓&#42; |   |   |
| 查看用戶開單和成本費率 | ✓&#42; |   |   |
| 管理計費記錄 | ✓ |   |   |
| 管理費用 | ✓ | ✓ |   |
| 查看財務資料 | ✓&#42; | ✓&#42; | ✓&#42; |
| 在資源計畫工具中按成本查看資訊 | ✓ |   |   |
| 資源規劃工具中的預算資源&#42;&#42; | ✓ |   |   |
| 在資源計畫工具中查看資源分配&#42; | ✓ | ✓ | ✓ |
| 為項目創造風險 | ✓ |   |   |
| 查看項目風險 | ✓ | ✓ | ✓ |

{style=&quot;table-layout:auto&quot;}

&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;需要對資源管理的其他訪問。

## 資源管理

只有具有計畫許可證的用戶才能完全訪問 [選擇對象或區域]. 其他授權類型可能對Workfront中的資源管理有限或無法存取。

| 動作 | 計劃者 | 工作者 | 檢閱者 | 要求者 | 外部用戶 |
|---|---|---|---|---|---|
| 在規劃工具中編輯優先順序和預算 | ✓&#42; |   |   |   |   |
| 建立、編輯、刪除資源池&#42;&#42; | ✓&#42; |   |   |   |   |
| `Update Planned Hours in the Workload Balancer`&#42;&#42;&#42; | `✓*` |   |   |   |   |
| 在資源計畫器中查看項目優先順序 | ✓&#42; |   |   |   |   |
| 在資源計畫工具中查看資源分配 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 查看資源池 | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| 資源規劃工具中的預算資源&#42;&#42; | ✓ |   |   |   |   |
| 將資源池附加到項目、模板和用戶 | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; 使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;需要對Financial Data的額外訪問權限，並需要對項目財務的權限。 如果您將資源管理訪問權限授予無權訪問財務資料的計畫員用戶，則用戶仍然可以在資源計畫員中查看每小時分配，但無法切換到「成本」視圖或查看業務案例。 如需詳細資訊，請參閱 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) 和 [共用物件的財務權限](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;需要對對象進行貢獻的權限，並在「高級設定」下啟用「進行分配」。 如需詳細資訊，請參閱 [了解繼承的權限和對象的層次結構](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) 在文章中 [對象共用權限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## 方案計畫員區域

| 動作 | 計劃者 | 工作者 | 檢閱者 | 要求者 | 外部用戶 |
|---|---|---|---|---|---|
| 建立/編輯現有計畫和方案 | ✓ | ✓ | ✓ |   |   |
| 添加或編輯有關計畫和方案的職務角色資訊&#42; | ✓ | ✓ | ✓ |   |   |
| 添加或編輯計畫和方案的成本資訊&#42; | ✓ | ✓ | ✓ |   |   |
| 刪除計畫和方案 | ✓ | ✓ | ✓ |   |   |
| 在主菜單中查看方案 ![](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ |  |   |
| 查看用戶建立的計畫和方案&#42; | ✓ | ✓ | ✓ |   |   |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>只有當共用到計畫的連結時，用戶才能查看其他用戶建立的計畫。

&#42; 為了讓使用者在計畫或計畫中檢視財務資料，他們需要存取財務資料。 如需詳細資訊，請參閱 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Workfront目標區

| 動作 | 檢視 | 編輯 |
|---|---|---|
| 建立 |   | ✓ |
| 編輯/刪除所有目標 |   | ✓ |
| 在主功能表中檢視目標 | ✓ | ✓ |
| 從共用連結檢視「目標」區域 | ✓ | ✓ |
| 查看系統中的所有目標 | ✓ | ✓ |
| 啟用/停用/關閉所有目標 |   | ✓ |
| 建立/編輯/刪除活動 |   | ✓ |
| 建立/編輯/刪除結果 |   | ✓ |
| 新增對齊的目標 |   | ✓ |
| 更新結果或活動的進度 |   | ✓ |
| 擁有目標、結果或活動 | ✓ | ✓ |
| 對目標的註解 | ✓ | ✓ |
| 複製目標 |   | ✓ |
| 檢視左側面板中的「目標清單」區段 | ✓ | ✓ |
| 檢視左側面板中的「圖形」區段 | ✓ | ✓ |
| 在左側面板中檢視「目標對齊方式」區段 | ✓ | ✓ |

