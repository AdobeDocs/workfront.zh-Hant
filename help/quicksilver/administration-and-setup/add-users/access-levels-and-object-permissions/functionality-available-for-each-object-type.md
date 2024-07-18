---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 存取，模型，漏斗，圖表，層級，許可權
navigation-topic: access-levels
title: 適用於各種存取層級之每種物件型別的功能
description: 下表列出各種存取層級中每種物件型別的可用功能。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 10%

---

# 適用於各種存取層級之每種物件型別的功能

{{highlighted-preview}}

下表列出各種存取層級中每種物件型別的可用功能。

它也會指出Workfront管理員可使用存取層級停用或啟用哪些動作。

## 專案

只有擁有計畫授權的使用者才能被授予專案的完整存取權。

| 動作 | 規劃工具 | 工作者 | 檢閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓ &#42; |   |   |   |   |
| 複製 | ✓ &#42; |   |   |   |   |
| 刪除 | ✓ &#42; |   |   |   |   |
| 共用 | ✓ &#42; | ✓ &#42; |   |   |   |
| 共用系統範圍 | ✓ &#42; |   |   |   |   |
| 檢視 | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |   |
| 新增自訂表格 | ✓ (A) |   |   |   |   |
| 更新自訂欄位 | ✓ (A) | ✓ (A) |   |   |   |
| 新增核准流程 | ✓ (A) |   |   |   |   |
| 核准專案 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 新增文件 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 新增問題 | ✓ (A) | ✓ (A) |   |   |   |
| 新增任務 | ✓ (A) | ✓ (A) |   |   |   |
| 提供更新/評論 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 變更狀態 | ✓ (A) |   |   |   |   |
| 記錄時數 | ✓ (A) | ✓ (A) |   |   |   |
| 編輯指派 | ✓ (A) | ✓ (A) |   |   |   |
| 管理基準線 | ✓ (A) |   |   |   |   |
| 管理風險 | ✓ (A) |   |   |   |   |
| 管理財務 | ✓ (A) |   |   |   |   |
| 新增/編輯費用 | ✓ (A) | ✓ (A) |   |   |   |
| 附加範本 | ✓ (A) |   |   |   |   |
| 另存為範本 | ✓ (A) |   |   |   |   |
| 新增/編輯業務案例 | ✓ (A) |   |   |   |   |
| 編輯專案詳細資料 | ✓ (A) |   |   |   |   |
| 編輯人員配置 | ✓ (A) |   |   |   |   |
| 匯出到 MS Project | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 重新計算財務/時間表 | ✓ (A) |   |   |   |   |
| 設定佇列屬性 | ✓ (A) |   |   |   |   |



&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 任務

| 動作 | 規劃工具 | 工作者 | 檢閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓ &#42; | ✓ &#42; |   |   |   |
| 刪除 | ✓ &#42; | ✓ &#42; |   |   |   |
| 共用 | ✓ &#42; | ✓ &#42; |   |   |   |
| 共用系統範圍 | ✓ &#42; |   |   |   |   |
| 檢視 | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |
| 新增前置任務 | ✓ (A) | ✓ (A) |   |   |   |
| 新增問題 | ✓ (A) | ✓ (A) |   |   |   |
| 編輯任務（不包括狀態） | ✓ (A) | ✓ (A) |   |   |   |
| 變更任務狀態 | ✓ (A) | ✓ (A) |   |   |   |
| 新增文件 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 複製任務 | ✓ (A) | ✓ (A) |   |   |   |
| 移動任務 | ✓ (A) | ✓ (A) |   |   |   |
| 記錄時數 | ✓ (A) | ✓ (A) |   |   |   |
| 接受指派 | ✓ (A) | ✓ (A) |   |   |   |
| 進行指派 | ✓ (A) | ✓ (A) | 僅限內嵌編輯 | 僅限內嵌編輯 |   |
| 附加自訂表單 | ✓ (A) | ✓ (A) |   |   |   |
| 編輯自訂欄位 | ✓ (A) | ✓ (A) |   |   |   |
| 建立核准流程 | ✓ (A) | ✓ (A) |   |   |   |
| 核准任務 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 編輯財務 | ✓ (A) |   |   |   |   |
| 新增/編輯費用 | ✓ (A) | ✓ (A) |   |   |   |
| 檢視財務 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 更新/評論 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |

{style="table-layout:auto"}

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 問題

| 動作 | 規劃工具 | 工作者 | 檢閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |
| 編輯 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 刪除 | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |
| 共用 | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |
| 共用系統範圍 | ✓ &#42; |   |   |   |   |
| 檢視 | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |
| 附加自訂表單 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 編輯自訂欄位 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 核准問題 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 新增核准流程 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 新增文件 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 複製問題 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 移動問題 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 記錄時數 | ✓ (A) | ✓ (A) |   |   |   |
| 將問題轉換為專案 | ✓ (A) | ✓ (A) |   |   |   |
| 將問題轉換為任務 | ✓ (A) |   |   |   |   |
| 接受指派 | ✓ (A) | ✓ (A) |   |   |   |
| 進行指派 | ✓ (A) | ✓ (A) |   |   |   |
| 新增更新和註解 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |



&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 專案組合

只有擁有計畫授權的使用者才能完整存取產品組合。

| 動作 | 規劃工具 | 工作者 | 檢閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓ &#42; |   |   |   |   |
| 刪除 | ✓ &#42; |   |   |   |   |
| 共用 | ✓ &#42; |   |   |   |   |
| 共用系統範圍 | ✓ &#42; |   |   |   |   |
| 檢視 | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |   |
| 編輯詳細資料 | ✓ (A) |   |   |   |   |
| 附加自訂表單 | ✓ (A) |   |   |   |   |
| 編輯自訂欄位 | ✓ (A) |   |   |   |   |
| 新增和移除專案 | ✓ (A) |   |   |   |   |
| 核准專案 | ✓ (A) |   |   |   |   |
| Portfolio最佳化 | ✓ (A) |   |   |   |   |
| 新增文件 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 新增更新和註解 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |



&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 計劃

只有擁有計畫授權的使用者才能完整存取計畫。

| 動作 | 規劃工具 | 工作者 | 檢閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓ &#42; |   |   |   |   |
| 刪除 | ✓ &#42; |   |   |   |   |
| 共用 | ✓ &#42; |   |   |   |   |
| 共用系統範圍 | ✓ &#42; |   |   |   |   |
| 檢視 | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |   |
| 編輯詳細資料 | ✓ (A) |   |   |   |   |
| 附加自訂表單 | ✓ (A) |   |   |   |   |
| 編輯自訂欄位 | ✓ (A) |   |   |   |   |
| 新增和移除專案 | ✓ (A) |   |   |   |   |
| 核准專案 | ✓ (A) |   |   |   |   |
| 投資組合最佳化 | ✓ (A) |   |   |   |   |
| 新增文件 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 新增更新與註解 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |



&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 報告、儀表板和行事曆

擁有Plan授權的使用者可以完全存取報告。 所有其他存取層級都擁有報表的檢視存取權。

| 動作 | 規劃工具 | 工作者 | 檢閱者 | 請求 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓ &#42; |   |   |   |   |
| 刪除 | ✓ &#42; |   |   |   |   |
| 檢視內建報告 | ✓ &#42; |   |   |   |   |
| 共用 | ✓ &#42; | ✓ (A) | ✓ (A) |   |   |
| 公開共用行事曆和報告 | ✓ &#42; |   |   |   |   |
| 共用系統範圍 | ✓ &#42; |   |   |   |   |
| 檢視 | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; |
| 編輯 | ✓ (A) |   |   |   |   |
| 複製 | ✓ (A) |   |   |   |   |

{style="table-layout:auto"}

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

>[!NOTE]
>
>請求者只能檢視已與他們共用的報告

## 篩選器、視圖和分組

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
   <th> <p>規劃工具</p> </th> 
   <th> <p>工作者</p> </th> 
   <th> <p>檢閱者</p> </th> 
   <th> <p>請求者</p> </th> 
   <th>外部使用者<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>建立</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>共用</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>共用系統範圍</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 文件

| 動作 | 規劃工具 | 工作者 | 檢閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |
| 刪除（檔案和資料夾） | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |
| 共用 | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |
| 公開（外部）共用 | ✓ &#42; |   |   |   |   |
| 共用系統範圍 | ✓ &#42; | ✓ &#42; |   |   |   |
| 檢視 | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; | ✓ &#42; |
| 編輯詳細資料 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 下載 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |
| 簽出 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 新增核准者 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 核准檔案 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |
| 附加自訂表單 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 編輯自訂欄位 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 移動至（物件） | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 傳送至（整合） | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 新增更新和註解 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 上傳新版本 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 刪除版本 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 預覽 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |
| 校樣 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 產生校訂 | ✓ (A) | ✓ (A) |   |   |   |
| 移除校訂 | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 新增/移除&#42;&#42; | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 重新命名&#42;&#42; | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 連結（與整合） | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |
| 取消連結（與整合） | ✓ (A) | ✓ (A) | ✓ (A) | ✓ (A) |   |

{style="table-layout:auto"}

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

&#42;&#42;僅適用於檔案資料夾，不適用於檔案

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
   <th> <p>規劃工具</p> </th> 
   <th>工作者</th> 
   <th> <p>檢閱者</p> </th> 
   <th> <p>請求者</p> </th> 
   <th> <p>外部使用者**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>建立</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯、刪除、停用、登入身份或重設任何使用者的密碼</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯、刪除、停用、登入身份或重設其管理的群組之任何使用者的密碼</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視使用者</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視聯絡資訊</td> 
   <td>✓ (A)</td> 
   <td> ✓ (A)</td> 
   <td>✓ (A) </td> 
   <td> ✓ (A)</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

&#42;&#42;外部使用者只能搜尋其他使用者

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
   <th> <p>規劃工具</p> </th> 
   <th>工作者</th> 
   <th> <p>檢閱者</p> </th> 
   <th> <p>請求者</p> </th> 
   <th> <p>外部使用者*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>建立</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯他們所在的團隊</td> 
   <td>✓ (R)*</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>在團隊管理的群組中編輯團隊</td> 
   <td>✓ (R)*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視所有團隊</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視與其群組相關聯的團隊</td> 
   <td>✓ (A)</td> 
   <td> ✓ (A)</td> 
   <td>✓ (A) </td> 
   <td> ✓ (A)</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 範本

| 動作 | 規劃工具 | 工作者 | 檢閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓ &#42; |   |   |   |   |
| 刪除 | ✓ &#42; |   |   |   |   |
| 共用 | ✓ &#42; |   |   |   |   |
| 共用系統範圍 | ✓ &#42; |   |   |   |   |
| 檢視 | ✓ &#42; |   |   |   |   |
| 複製 | ✓ (A) |   |   |   |   |
| 編輯範本詳細資料 | ✓ (A) |   |   |   |   |

{style="table-layout:auto"}

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 財務資料

只有擁有Plan授權的使用者才能完整存取財務資料。

此處不包含請求和外部使用者授權型別，因為它們無權存取這些物件和區域。

| 動作 | 規劃工具 | 工作者 | 檢閱者 |
|---|---|---|---|
| 編輯角色帳單和成本費率 | ✓ &#42; |   |   |
| 編輯使用者帳單和成本費率 | ✓ &#42; |   |   |
| 檢視角色帳單與成本費率 | ✓ &#42; |   |   |
| 檢視使用者帳單和成本費率 | ✓ &#42; |   |   |
| 管理計費記錄 | ✓ (A) |   |   |
| 管理費用 | ✓ (A) | ✓ (A) |   |
| 檢視財務資料 | ✓ &#42; | ✓ &#42; | ✓ &#42; |
| <span class="preview">管理費率卡</span> | ✓ (A) |   |   |
| 在資源計畫工具中依成本檢視資訊 | ✓ (A) |   |   |
| 資源規劃工具中的預算資源&#42;&#42; | ✓ (A) |   |   |
| 檢視資源規劃工具中的資源配置&#42; | ✓ (A) | ✓ (A) | ✓ (A) |
| 建立專案風險 | ✓ (A) |   |   |
| 檢視專案風險 | ✓ (A) | ✓ (A) | ✓ (A) |

{style="table-layout:auto"}

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

&#42;&#42;需要資源管理的額外存取許可權。

## 資源管理

只有擁有計畫授權的使用者才能擁有[選取物件或區域]的完整存取權。 其他授權型別對Workfront中的資源管理可能有限制或沒有存取權。

| 動作 | 規劃工具 | 工作者 | 檢閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 在規劃工具中編輯優先順序和預算 | ✓ &#42; |   |   |   |   |
| 建立、編輯、刪除資源集區&#42;&#42; | ✓ &#42; |   |   |   |   |
| `Update Planned Hours in the Workload Balancer`&#42;&#42;&#42; | `✓*` |   |   |   |   |
| 在資源規劃工具中檢視專案優先順序 | ✓ &#42; |   |   |   |   |
| 檢視資源計畫工具中的資源配置 | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |   |
| 檢視資源集區 | ✓ &#42; | ✓ &#42; | ✓ &#42; |   |   |
| 資源規劃工具中的預算資源&#42;&#42; | ✓ (A) |   |   |   |   |
| 將資源集區附加至專案、範本和使用者 | ✓ (A) |   |   |   |   |

{style="table-layout:auto"}

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

&#42;&#42;需要其他財務資料存取權以及專案財務的許可權。 如果您將「資源管理」存取權授與沒有「財務資料」存取權的「供需規劃員」使用者，該使用者仍可在「資源供需規劃員」中看到每小時配置，但無法切換至「成本」檢視或檢視「業務案例」。 如需詳細資訊，請參閱[授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)以及[共用物件的財務許可權](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md)。

&#42;&#42;&#42;需要Contribute存取物件的許可權，且在[進階設定]下啟用[指派工作]。 如需相關資訊，請參閱文章[物件許可權共用概觀](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)中的[瞭解繼承許可權和物件階層](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object)一節。

## 情境規劃工具區域

| 動作 | 規劃工具 | 工作者 | 檢閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立/編輯現有計畫和方案 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 新增或編輯計畫和方案的工作角色資訊&#42; | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 新增或編輯計畫和方案&#42;的成本資訊 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 刪除計畫和方案 | ✓ (A) | ✓ (A) | ✓ (A) |   |   |
| 在主要功能表![](assets/esp-icon-in-main-menu.png)中檢視情境 | ✓ (A) | ✓ (A) | ✓ (A) | |   |
| 檢視使用者建立的計畫和方案&#42; | ✓ (A) | ✓ (A) | ✓ (A) |   |   |

{style="table-layout:auto"}

>[!NOTE]
>
>只有當計畫的連結與其共用時，使用者才能檢視其他使用者建立的計畫。

&#42;若要讓使用者檢視計畫或方案中的財務資料，他們需要財務資料的存取權。 如需詳細資訊，請參閱[授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

## Workfront目標區域

| 動作 | 檢視 | 編輯 |
|---|---|---|
| 建立 |   | ✓ (A) |
| 編輯/刪除所有目標 |   | ✓ (A) |
| 在主要功能表中檢視目標 | ✓ (A) | ✓ (A) |
| 從共用連結檢視目標區域 | ✓ (A) | ✓ (A) |
| 檢視系統中的所有目標 | ✓ (A) | ✓ (A) |
| 啟用/停用/關閉所有目標 |   | ✓ (A) |
| 建立/編輯/刪除活動 |   | ✓ (A) |
| 建立/編輯/刪除結果 |   | ✓ (A) |
| 新增對齊的目標 |   | ✓ (A) |
| 更新結果或活動的進度 |   | ✓ (A) |
| 擁有目標、結果或活動 | ✓ (A) | ✓ (A) |
| 目標上的註解 | ✓ (A) | ✓ (A) |
| 複製目標 |   | ✓ (A) |
| 檢視左側面板中的「目標清單」區段 | ✓ (A) | ✓ (A) |
| 檢視左側面板中的圖形區段 | ✓ (A) | ✓ (A) |
| 檢視左側面板中的「目標校準」區段 | ✓ (A) | ✓ (A) |

