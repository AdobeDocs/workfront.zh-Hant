---
title: 稽核記錄
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作為Adobe Workfront管理員，您可以使用稽核記錄來追蹤過去90天期間在系統中觸發的使用者變更。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '1464'
ht-degree: 3%

---

# 稽核記錄

<!--Audited: 01/2024-->

身為Adobe Workfront管理員，您可以使用下述稽核記錄追蹤過去90天內系統中觸發的使用者變更。

如需有關檢視和篩選您想要在這些稽核記錄中檢視內容的指示，請參閱[檢視和匯出稽核記錄](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)。

## 您可以在稽核記錄檔中找到的資訊

下列欄位會記錄在每個稽核記錄專案中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">日期與時間</td> 
   <td>動作發生的時間。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">記錄類型</td> 
   <td>稽核記錄的型別，例如「存取層級」或「自訂表格」。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">使用者名稱</td> 
   <td> <p>執行動作之使用者的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> 使用者執行的動作，例如「變更」、「建立」和「刪除」。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件</td> 
   <td> 受動作影響的物件名稱。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">詳细資料</td> 
   <td>此動作的其他詳細資料。 將滑鼠移到文字上以讀取完整訊息。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP 位址</td> 
   <td> <p>執行動作時執行動作之使用者的IP位址。</p> <p>某些系統動作無法使用IP位址。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 稽核記錄型別和觸發它們的動作

* [存取層級](#access-level)
* [公司](#company)
* [狀況](#condition)
* [自訂欄位](#custom-field)
* [自訂表單](#custom-forms)
* [自訂節](#custom-section)
* [匯率](#exchange-rate)
* [群組](#group)
* [工作角色](#job-roles)
* [登入嘗試](#login-attempt)
* [優先順序](#priority)
* [專案喜好設定](#project-preference)
* [嚴重性](#severity)
* [狀態](#status)
* [任務和問題偏好設定](#tasks-issues-preferences)
* [使用者](#user)

### 存取層級 {#access-level}

當使用者執行下列其中一項動作時，系統會產生「存取層級」記錄專案：

* 建立存取層級
* 刪除存取層級
* 變更存取層級：

   * 修改授權型別
   * 變更專案、任務、問題、Portfolio、方案、報告、檔案、使用者或範本的許可權

     >[!NOTE]
     >
     >系統不會記錄對財務資料或以下存取型別的任何許可權變更：檢視和編輯。
     >
     >例如，如果使用者將「規劃工具」存取型別從「檢視」變更為「編輯」，則系統不會顯示「微調您的設定」下拉式選單中所包含的資訊。

### 公司 {#company}

當使用者執行下列其中一項作業時，系統會產生「公司」稽核記錄專案：

* 建立公司
* 變更公司：

   * 重新命名
   * 新增或移除成員
   * 在其群組欄位中新增、編輯或刪除值
   * 新增或編輯工作角色的公司收費率
   * 移除工作角色的公司收費率
   * 將其設為組織的主要公司
   * 附加或移除自訂表單

* 刪除公司

如需有關狀態的詳細資訊，請參閱[狀態概觀](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md)。

### 狀況 {#condition}

當使用者執行下列其中一個動作時，系統會產生「條件」稽核記錄專案：

* 建立條件
* 變更條件：

   * 變更名稱
   * 變更顏色
   * 設為預設值
   * 變更或移除條件的說明
   * 隱藏或顯示條件

* 刪除條件

如需設定工作角色的詳細資訊，請參閱[建立或編輯自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)。

### 自訂欄位 {#custom-field}

當使用者執行下列其中一個動作時，系統會產生「自訂欄位」稽核記錄專案：

* 建立自訂欄位
* 變更自訂欄位：

   * 變更名稱、標籤、指示或格式
   * 變更顯示型別

     僅當欄位是以下型別之一時，此選項才可用：單行、段落、下拉式清單、核取方塊、選項按鈕

   * 變更欄位大小

     只有當欄位是以下其中一種型別時，才可使用此選項：單行、段落、含格式的文字

   * 新增、移除或隱藏欄位選擇
   * 編輯欄位選擇標籤或值
   * 設定預設為選取或未選取的欄位選擇
   * 設定下拉式欄位以允許多個選取專案或單一選取專案
   * 設定日期欄位以顯示或不顯示當日時間
   * 編輯超連結或變更描述性文字欄位中的值

* 刪除自訂欄位
* 共用自訂欄位

### 自訂表單 {#custom-forms}

當使用者執行下列其中一項動作時，系統會產生自訂Forms稽核記錄專案：

* 建立自訂表單
* 變更自訂表格：

   * 變更名稱或說明
   * 啟用或停用作用中
   * 新增或移除欄位或區段
   * 對於自訂區段，會變更「其他設定」底下的設定
   * 將欄位變更為必要或非必要
   * 變更自訂欄位中的計算
   * 隱藏或顯示「指示」暫留文字中與計算欄位相關聯的公式
   * 啟用或停用更新先前的計算
   * 新增或變更跳過邏輯或顯示邏輯

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* 刪除自訂表單
* 共用自訂表單

### 自訂區段 {#custom-section}

當使用者在自訂表單中執行以下動作之一時，系統會產生「自訂區段」稽核記錄專案：

* 建立自訂區段
* 變更自訂區段的名稱或說明
* 刪除自訂部分

如需自訂表單中自訂區段的資訊，請參閱[建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)。

### 匯率 {#exchange-rate}

當使用者執行下列其中一個動作時，系統會產生「匯率」稽核記錄專案：

* 建立匯率
* 變更匯率：

   * 新增貨幣
   * 變更貨幣的匯率
   * 將貨幣設定為整個系統的所有專案和報表的基礎（預設）貨幣

* 刪除匯率

如需設定匯率的詳細資訊，請參閱[設定匯率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

### 群組 {#group}

當使用者執行下列其中一個動作時，系統會產生「群組」稽核記錄專案：

* 建立群組
* 刪除群組
* 變更群組：

   * 新增或移除使用者
   * 新增或移除子群組

### 職務角色 {#job-roles}

當使用者執行下列其中一個動作時，系統會產生「工作角色」稽核記錄專案：

* 建立工作角色
* 變更工作角色：

   * 變更名稱
   * 新增、變更或移除說明
   * 新增、變更或移除每小時成本（成本/小時）
   * 新增、變更或移除帳單費率（計費/小時）

* 刪除工作角色

如需設定工作角色的詳細資訊，請參閱[建立和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

### 登入嘗試 {#login-attempt}

當使用者執行下列其中一個動作時，系統會產生「登入嘗試」稽核記錄專案：

* 在Workfront中登入、登出或登入嘗試失敗（在瀏覽器和行動應用程式中）
* 在任何Workfront整合中登入、登出或登入嘗試失敗(例如適用於Slack的Workfront和適用於Salesforce的Workfront)
* 登入或登出Workfront API

Workfront管理員使用「登入身份」功能時，不會記錄登入嘗試記錄檔。

>[!NOTE]
>
>如果您的組織已上線Adobe Admin Console，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

### 優先順序 {#priority}

當使用者執行下列其中一個動作時，系統會產生「優先順序」稽核記錄專案：

* 建立優先順序
* 變更優先順序：

   * 變更名稱
   * 變更顏色
   * 設為預設值
   * 新增、變更或移除優先順序的說明
   * 隱藏或顯示優先順序

* 刪除優先順序

如需設定優先順序的詳細資訊，請參閱[建立及自訂優先順序](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md)。

### 專案偏好設定 {#project-preference}

當使用者執行下列其中一個動作時，系統會產生「專案偏好設定」稽核記錄專案：

* 建立自訂季度
* 變更專案偏好設定：

   * 鎖定或解除鎖定
   * 變更其中一個設定
   * 啟用、停用或編輯它
   * 編輯時間表計算

* 刪除自訂季度

如需有關專案偏好設定的詳細資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

### 嚴重程度 {#severity}

當使用者執行下列其中一個動作時，系統會產生「嚴重程度」稽核記錄專案：

* 建立問題嚴重程度
* 變更問題嚴重性：

   * 變更名稱
   * 變更顏色
   * 設為預設值
   * 變更或移除嚴重程度的說明
   * 隱藏或顯示嚴重性

* 刪除問題嚴重程度

如需設定職位角色的詳細資訊，請參閱[建立或自訂問題嚴重程度](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md)。

### 狀態 {#status}

當使用者執行下列其中一個動作時，系統會產生「狀態」稽核記錄專案：

* 在系統或群組層級上建立狀態
* 變更系統或群組層級的狀態：

   * 重新命名
   * 設為預設狀態
   * 鎖定或解除鎖定
   * 隱藏或取消隱藏它
   * 變更顏色或說明

* 刪除系統或群組層級的狀態

如需有關狀態的詳細資訊，請參閱[狀態概觀](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md)。

### 任務和問題偏好設定 {#tasks-issues-preferences}

當使用者以下列方式之一變更任務與問題偏好設定時，系統會產生「任務與問題偏好設定」稽核記錄專案：

* 鎖定或解除鎖定偏好設定
* 變更偏好設定的設定
* 變更任務、問題或請求的存取設定

如需有關任務和問題偏好設定的詳細資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

### 使用者 {#user}

當使用者執行下列其中一個動作時，系統會產生「使用者」稽核記錄專案：

* 建立使用者

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >如果您的組織已上線Adobe Admin Console，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

* 刪除使用者
* 變更使用者的存取層級、公司、團隊或群組
* 啟動使用者
* 停用使用者
