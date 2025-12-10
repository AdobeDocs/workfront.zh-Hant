---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 存取，模型，funnel，圖表，層級，許可權
navigation-topic: access-levels
title: 各種存取層級中每種物件型別的可用功能
description: 下表列出各種存取層級中每種物件型別的可用功能。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 14%

---

# 適用於各種存取層級之每種物件型別的功能

{{highlighted-preview}}

>[!NOTE]
>
>本文資訊參考舊版存取層級。 如需有關目前存取層級的資訊，請參閱[新存取層級概觀](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)。

下表列出各種存取層級中每種物件型別的可用功能。

它也會指出Workfront管理員可使用存取層級停用或啟用哪些動作。

>[!NOTE]
>
>本文說明在目前的Workfront套件模型中可用於存取層級的功能。 若要檢視新封裝模型中可用的功能，請參閱[新存取層級中每個物件型別可用的功能](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md)。

## 專案

只有擁有計畫授權的使用者才能被授予專案的完整存取權。

| 動作 | 規劃者 | 工作者 | 審閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; |  |  |  |  |
| 複製 | ✓&#42; |  |  |  |  |
| 刪除 | ✓&#42; |  |  |  |  |
| 共用 | ✓&#42; | ✓&#42; |  |  |  |
| 共用系統範圍 | ✓&#42; |  |  |  |  |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| 新增自訂表格 | ✓ |  |  |  |  |
| 更新自訂欄位 | ✓ | ✓ |  |  |  |
| 新增核准流程 | ✓ |  |  |  |  |
| 核准專案 | ✓ | ✓ | ✓ |  |  |
| 新增文件 | ✓ | ✓ | ✓ |  |  |
| 新增問題 | ✓ | ✓ |  |  |  |
| 新增任務 | ✓ | ✓ |  |  |  |
| 提供更新/評論 | ✓ | ✓ | ✓ |  |  |
| 變更狀態 | ✓ |  |  |  |  |
| 記錄時數 | ✓ | ✓ |  |  |  |
| 編輯指派 | ✓ | ✓ |  |  |  |
| 管理基準線 | ✓ |  |  |  |  |
| 管理風險 | ✓ |  |  |  |  |
| 管理財務 | ✓ |  |  |  |  |
| 新增/編輯費用 | ✓ | ✓ |  |  |  |
| 附加範本 | ✓ |  |  |  |  |
| 另存為範本 | ✓ |  |  |  |  |
| 新增/編輯業務案例 | ✓ |  |  |  |  |
| 編輯專案詳細資料 | ✓ |  |  |  |  |
| 編輯人員配置 | ✓ |  |  |  |  |
| 匯出到 MS Project | ✓ | ✓ | ✓ |  |  |
| 重新計算財務/時間表 | ✓ |  |  |  |  |
| 設定佇列屬性 | ✓ |  |  |  |  |



&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 任務

| 動作 | 規劃者 | 工作者 | 審閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; | ✓&#42; |  |  |  |
| 刪除 | ✓&#42; | ✓&#42; |  |  |  |
| 共用 | ✓&#42; | ✓&#42; |  |  |  |
| 共用系統範圍 | ✓&#42; |  |  |  |  |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| 新增前置任務 | ✓ | ✓ |  |  |  |
| 新增問題 | ✓ | ✓ |  |  |  |
| 編輯任務（不包括狀態） | ✓ | ✓ |  |  |  |
| 變更任務狀態 | ✓ | ✓ |  |  |  |
| 新增文件 | ✓ | ✓ | ✓ |  |  |
| 複製任務 | ✓ | ✓ |  |  |  |
| 移動任務 | ✓ | ✓ |  |  |  |
| 記錄時數 | ✓ | ✓ |  |  |  |
| 接受指派 | ✓ | ✓ |  |  |  |
| 進行指派 | ✓ | ✓ | 僅限內嵌編輯 | 僅限內嵌編輯 |  |
| 附加自訂表單 | ✓ | ✓ |  |  |  |
| 編輯自訂欄位 | ✓ | ✓ |  |  |  |
| 建立核准流程 | ✓ | ✓ |  |  |  |
| 核准任務 | ✓ | ✓ | ✓ |  |  |
| 編輯財務 | ✓ |  |  |  |  |
| 新增/編輯費用 | ✓ | ✓ |  |  |  |
| 檢視財務 | ✓ | ✓ | ✓ |  |  |
| 更新/評論 | ✓ | ✓ | ✓ |  |  |

{style="table-layout:auto"}

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 問題

| 動作 | 規劃者 | 工作者 | 審閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| 編輯 | ✓ | ✓ | ✓ | ✓ |  |
| 刪除 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| 共用 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| 共用系統範圍 | ✓&#42; |  |  |  |  |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| 附加自訂表單 | ✓ | ✓ | ✓ | ✓ |  |
| 編輯自訂欄位 | ✓ | ✓ | ✓ | ✓ |  |
| 核准問題 | ✓ | ✓ | ✓ | ✓ |  |
| 新增核准流程 | ✓ | ✓ | ✓ | ✓ |  |
| 新增文件 | ✓ | ✓ | ✓ | ✓ |  |
| 複製問題 | ✓ | ✓ | ✓ | ✓ |  |
| 移動問題 | ✓ | ✓ | ✓ | ✓ |  |
| 記錄時數 | ✓ | ✓ |  |  |  |
| 將問題轉換為專案 | ✓ | ✓ |  |  |  |
| 將問題轉換為任務 | ✓ |  |  |  |  |
| 接受指派 | ✓ | ✓ |  |  |  |
| 進行指派 | ✓ | ✓ |  |  |  |
| 新增更新和註解 | ✓ | ✓ | ✓ | ✓ |  |



&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 專案組合

只有擁有計畫授權的使用者才能完整存取產品組合。

| 動作 | 規劃者 | 工作者 | 審閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; |  |  |  |  |
| 刪除 | ✓&#42; |  |  |  |  |
| 共用 | ✓&#42; |  |  |  |  |
| 共用系統範圍 | ✓&#42; |  |  |  |  |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| 編輯詳細資料 | ✓ |  |  |  |  |
| 附加自訂表單 | ✓ |  |  |  |  |
| 編輯自訂欄位 | ✓ |  |  |  |  |
| 新增和移除專案 | ✓ |  |  |  |  |
| 核准專案 | ✓ |  |  |  |  |
| Portfolio最佳化 | ✓ |  |  |  |  |
| 新增文件 | ✓ | ✓ | ✓ |  |  |
| 新增更新和註解 | ✓ | ✓ | ✓ |  |  |



&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 計劃

只有擁有計畫授權的使用者才能完整存取計畫。

| 動作 | 規劃者 | 工作者 | 審閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; |  |  |  |  |
| 刪除 | ✓&#42; |  |  |  |  |
| 共用 | ✓&#42; |  |  |  |  |
| 共用系統範圍 | ✓&#42; |  |  |  |  |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| 編輯詳細資料 | ✓ |  |  |  |  |
| 附加自訂表單 | ✓ |  |  |  |  |
| 編輯自訂欄位 | ✓ |  |  |  |  |
| 新增和移除專案 | ✓ |  |  |  |  |
| 核准專案 | ✓ |  |  |  |  |
| 投資組合最佳化 | ✓ |  |  |  |  |
| 新增文件 | ✓ | ✓ | ✓ |  |  |
| 新增更新與註解 | ✓ | ✓ | ✓ |  |  |



&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 報告、儀表板和行事曆

擁有Plan授權的使用者可以完全存取報告。 所有其他存取層級都擁有報表的檢視存取權。

| 動作 | 規劃者 | 工作者 | 審閱者 | 請求 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; |  |  |  |  |
| 刪除 | ✓&#42; |  |  |  |  |
| 檢視內建報告 | ✓&#42; |  |  |  |  |
| 共用 | ✓&#42; | ✓ | ✓ |  |  |
| 公開共用行事曆和報告 | ✓&#42; |  |  |  |  |
| 共用系統範圍 | ✓&#42; |  |  |  |  |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| 編輯 | ✓ |  |  |  |  |
| 複製 | ✓ |  |  |  |  |

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
   <th> <p>規劃者</p> </th> 
   <th> <p>工作者</p> </th> 
   <th> <p>審閱者</p> </th> 
   <th> <p>請求者</p> </th> 
   <th>外部使用者<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>建立</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>共用</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>共用系統範圍</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 文件

| 動作 | 規劃者 | 工作者 | 審閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| 刪除（檔案和資料夾） | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| 共用 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| 公開（外部）共用 | ✓&#42; |  |  |  |  |
| 共用系統範圍 | ✓&#42; | ✓&#42; |  |  |  |
| 檢視 | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| 編輯詳細資料 | ✓ | ✓ | ✓ | ✓ |  |
| 下載 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 簽出 | ✓ | ✓ | ✓ | ✓ |  |
| 新增核准者 | ✓ | ✓ | ✓ | ✓ |  |
| 核准檔案 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 附加自訂表單 | ✓ | ✓ | ✓ | ✓ |  |
| 編輯自訂欄位 | ✓ | ✓ | ✓ | ✓ |  |
| 移動至（物件） | ✓ | ✓ | ✓ | ✓ |  |
| 傳送至（整合） | ✓ | ✓ | ✓ | ✓ |  |
| 新增更新和註解 | ✓ | ✓ | ✓ | ✓ |  |
| 上傳新版本 | ✓ | ✓ | ✓ | ✓ |  |
| 刪除版本 | ✓ | ✓ | ✓ | ✓ |  |
| 預覽 | ✓ | ✓ | ✓ | ✓ | ✓ |
| 校樣 | ✓ | ✓ | ✓ | ✓ |  |
| 產生校訂 | ✓ | ✓ |  |  |  |
| 移除校訂 | ✓ | ✓ | ✓ | ✓ |  |
| 新增/移除&#42;&#42; | ✓ | ✓ | ✓ | ✓ |  |
| 重新命名&#42;&#42; | ✓ | ✓ | ✓ | ✓ |  |
| 連結（與整合） | ✓ | ✓ | ✓ | ✓ |  |
| 取消連結（與整合） | ✓ | ✓ | ✓ | ✓ |  |

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
   <th> <p>規劃者</p> </th> 
   <th>工作者</th> 
   <th> <p>審閱者</p> </th> 
   <th> <p>請求者</p> </th> 
   <th> <p>外部使用者**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>建立</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯、刪除、停用、登入身份或重設任何使用者的密碼</td> 
   <td>✓*<p><b>注意</b>：您無法作為系統管理員的任何使用者登入。</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯、刪除、停用、登入身份或重設其管理的群組之任何使用者的密碼</td> 
   <td>✓*<p><b>注意</b>：您無法作為系統管理員的任何使用者登入。</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視使用者</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視聯絡資訊</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
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
   <th> <p>規劃者</p> </th> 
   <th>工作者</th> 
   <th> <p>審閱者</p> </th> 
   <th> <p>請求者</p> </th> 
   <th> <p>外部使用者*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>建立</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>刪除</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>編輯他們所在的團隊</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>在團隊管理的群組中編輯團隊</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視所有團隊</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視與其群組相關聯的團隊</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 範本

| 動作 | 規劃者 | 工作者 | 審閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立 | ✓&#42; |  |  |  |  |
| 刪除 | ✓&#42; |  |  |  |  |
| 共用 | ✓&#42; |  |  |  |  |
| 共用系統範圍 | ✓&#42; |  |  |  |  |
| 檢視 | ✓&#42; |  |  |  |  |
| 複製 | ✓ |  |  |  |  |
| 編輯範本詳細資料 | ✓ |  |  |  |  |

{style="table-layout:auto"}

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

## 財務資料

只有擁有Plan授權的使用者才能完整存取財務資料。

此處不包含請求和外部使用者授權型別，因為它們無權存取這些物件和區域。

| 動作 | 規劃者 | 工作者 | 審閱者 |
|---|---|---|---|
| 編輯角色帳單和成本費率 | ✓&#42; |  |  |
| 編輯使用者帳單和成本費率 | ✓&#42; |  |  |
| 檢視角色帳單與成本費率 | ✓&#42; |  |  |
| 檢視使用者帳單和成本費率 | ✓&#42; |  |  |
| 管理計費記錄 | ✓ |  |  |
| 管理費用 | ✓ | ✓ |  |
| 檢視財務資料 | ✓&#42; | ✓&#42; | ✓&#42; |
| <span class="preview">管理費率卡</span> | ✓ |  |  |
| 在資源計畫工具中依成本檢視資訊 | ✓ |  |  |
| 資源規劃工具中的預算資源&#42;&#42; | ✓ |  |  |
| 檢視資源規劃工具中的資源配置&#42; | ✓ | ✓ | ✓ |
| 建立專案風險 | ✓ |  |  |
| 檢視專案風險 | ✓ | ✓ | ✓ |

{style="table-layout:auto"}

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

&#42;&#42;需要資源管理的額外存取許可權。

## 資源管理

只有擁有計畫授權的使用者才能擁有[選取物件或區域]的完整存取權。 其他授權型別對Workfront中的資源管理可能有限制或沒有存取權。

| 動作 | 規劃者 | 工作者 | 審閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 在規劃工具中編輯優先順序和預算 | ✓&#42; |  |  |  |  |
| 建立、編輯、刪除資源集區&#42;&#42; | ✓&#42; |  |  |  |  |
| 更新工作負載平衡器&#42;&#42;&#42;中的計畫時數 | ✓* |  |  |  |  |
| 在資源規劃工具中檢視專案優先順序 | ✓&#42; |  |  |  |  |
| 檢視資源計畫工具中的資源配置 | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| 檢視資源集區 | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| 資源規劃工具中的預算資源&#42;&#42; | ✓ |  |  |  |  |
| 將資源集區附加至專案、範本和使用者 | ✓ |  |  |  |  |

{style="table-layout:auto"}

&#42;使用存取層級，Workfront管理員可以停用或啟用此功能。 如需詳細資訊，請參閱[每個物件型別](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)可設定的功能存取權。

&#42;&#42;需要其他財務資料存取權以及專案財務的許可權。 如果您將「資源管理」存取權授與沒有「財務資料」存取權的「供需規劃員」使用者，該使用者仍可在「資源供需規劃員」中看到每小時配置，但無法切換至「成本」檢視或檢視「業務案例」。 如需詳細資訊，請參閱[授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)以及[共用物件的財務許可權](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md)。

&#42;&#42;&#42;需要許可權才能貢獻至物件，且在[進階設定]下啟用[指派工作]。 如需相關資訊，請參閱文章[物件許可權共用概觀](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object)中的[瞭解繼承許可權和物件階層](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)一節。

## 情境規劃工具區域

| 動作 | 規劃者 | 工作者 | 審閱者 | 請求者 | 外部使用者 |
|---|---|---|---|---|---|
| 建立/編輯現有計畫和方案 | ✓ | ✓ | ✓ |  |  |
| 新增或編輯計畫和方案的工作角色資訊&#42; | ✓ | ✓ | ✓ |  |  |
| 新增或編輯計畫和方案&#42;的成本資訊 | ✓ | ✓ | ✓ |  |  |
| 刪除計畫和方案 | ✓ | ✓ | ✓ |  |  |
| 在主要功能表中檢視案例![案例規劃工具圖示](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ | |  |
| 檢視使用者建立的計畫和方案&#42; | ✓ | ✓ | ✓ |  |  |

{style="table-layout:auto"}

>[!NOTE]
>
>只有當計畫的連結與其共用時，使用者才能檢視其他使用者建立的計畫。

&#42;若要讓使用者檢視計畫或方案中的財務資料，他們需要財務資料的存取權。 如需詳細資訊，請參閱[授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

## Workfront目標區域

| 動作 | 檢視 | 編輯 |
|---|---|---|
| 建立 |  | ✓ |
| 編輯/刪除所有目標 |  | ✓ |
| 在主要功能表中檢視目標 | ✓ | ✓ |
| 從共用連結檢視目標區域 | ✓ | ✓ |
| 檢視系統中的所有目標 | ✓ | ✓ |
| 啟用/停用/關閉所有目標 |  | ✓ |
| 建立/編輯/刪除活動 |  | ✓ |
| 建立/編輯/刪除結果 |  | ✓ |
| 新增對齊的目標 |  | ✓ |
| 更新結果或活動的進度 |  | ✓ |
| 擁有目標、結果或活動 | ✓ | ✓ |
| 目標上的註解 | ✓ | ✓ |
| 複製目標 |  | ✓ |
| 檢視左側面板中的「目標清單」區段 | ✓ | ✓ |
| 檢視左側面板中的圖形區段 | ✓ | ✓ |
| 檢視左側面板中的「目標校準」區段 | ✓ | ✓ |


