---
title: 稽核記錄
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 身為Adobe Workfront管理員，您可以使用稽核記錄來追蹤過去90天內在系統中觸發的使用者變更。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 4%

---

# 稽核記錄

身為Adobe Workfront管理員，您可以使用以下所述的稽核記錄，追蹤系統在過去90天中觸發的使用者變更。

如需檢視和篩選您要在這些稽核記錄中查看之內容的指示，請參閱 [查看和導出審核日誌](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## 可在稽核記錄中找到的資訊

每個審核日誌條目都記錄以下欄位：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">日期與時間</td> 
   <td>動作發生時。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">記錄類型</td> 
   <td>稽核記錄的類型，例如存取層級或自訂表單。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">使用者名稱</td> 
   <td> <p>執行動作的使用者名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">動作</td> 
   <td> 由用戶執行的操作，如更改、建立和刪除。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件</td> 
   <td> 因動作而受影響的物件名稱。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">詳细資訊</td> 
   <td>動作的其他詳細資訊。 將滑鼠移到文字上以閱讀完整訊息。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP位址</td> 
   <td> <p>在動作執行時執行動作的使用者的IP位址。</p> <p>IP地址不可用於某些系統操作。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 稽核記錄類型及觸發這些類型的動作

* [存取層級](#access-level)
* [公司](#company)
* [狀況](#condition)
* [自訂欄位](#custom-field)
* [自訂表單](#custom-forms)
* [自訂區段](#custom-section)
* [匯率](#exchange-rate)
* [群組](#group)
* [職務角色](#job-roles)
* [登入嘗試](#login-attempt)
* [優先順序](#priority)
* [專案偏好設定](#project-preferences)
* [嚴重程度](#severity)
* [狀態](#status)
* [任務和問題偏好設定](#tasks-issues-preferences)
* [使用者](#user)

### 存取層級 {#access-level}

當用戶執行以下操作之一時，系統將生成訪問級別日誌條目：

* 建立存取層級
* 刪除訪問級別
* 更改訪問級別：

   * 修改許可證類型
   * 變更專案、工作、問題、Portfolio、方案、報表、檔案、使用者或範本的權限

      >[!NOTE]
      >
      >系統不會記錄對Financial Data或以下訪問類型的任何權限更改：檢視和編輯。
      >
      >例如，如果用戶將計畫員訪問類型從「視圖」更改為「編輯」，則系統將不會顯示「微調設定」下拉菜單中包含的資訊。

### 公司 {#company}

當用戶執行以下操作之一時，系統將生成一個公司審核日誌條目：

* 建立公司
* 變更公司：

   * 重新命名
   * 添加或刪除成員
   * 在其「組」欄位中添加、編輯或刪除值
   * 添加或編輯工作角色的公司帳單費率
   * 刪除職務角色的公司開單率
   * 將其設定為組織的主要公司
   * 附加或移除自訂表單

* 刪除公司

如需狀態的詳細資訊，請參閱 [狀態概觀](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### 狀況 {#condition}

當使用者執行下列其中一項動作時，系統會產生條件稽核記錄項目：

* 建立條件
* 變更條件：

   * 變更名稱
   * 變更顏色
   * 將其設為預設值
   * 變更或移除條件的說明
   * 隱藏或顯示條件

* 刪除條件

有關配置作業角色的詳細資訊，請參閱 [建立或編輯自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### 自訂欄位 {#custom-field}

當用戶執行以下操作之一時，系統將生成自定義欄位審計日誌條目：

* 建立自訂欄位
* 變更自訂欄位：

   * 變更名稱、標籤、指示或格式
   * 更改顯示類型

      只有當欄位為下列其中一種類型時，才可使用：單行，段落，下拉式清單，核取方塊，選項按鈕

   * 變更欄位大小

      只有當欄位為下列其中一種類型時，才可使用：單行，段落，帶格式的文本

   * 新增、移除或隱藏欄位選項
   * 編輯欄位選擇標籤或值
   * 配置預設要選擇或未選擇的欄位選項
   * 配置下拉欄位以允許多個選擇或單個選擇
   * 設定日期欄位以顯示或不顯示當天時間
   * 編輯超連結或更改描述性文本欄位中的值

* 刪除自訂欄位
* 共用自訂欄位

### 自訂表單 {#custom-forms}

當使用者執行下列其中一項動作時，系統會產生自訂Forms稽核記錄項目：

* 建立自訂表單
* 變更自訂表單：

   * 變更名稱或說明
   * 啟用或停用是啟用
   * 新增或移除欄位或區段
   * 對於自訂區段，會變更「其他設定」下的設定
   * 將欄位變更為必要或非必要
   * 變更自訂欄位中的計算
   * 隱藏或顯示「指示」暫留文字中與計算欄位關聯的公式
   * 啟用或禁用更新以前的計算
   * 新增或變更略過邏輯或顯示邏輯

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* 刪除自訂表單
* 共用自訂表單

### 自訂區段 {#custom-section}

當使用者以自訂表單執行下列其中一項動作時，系統會產生自訂區段稽核記錄項目：

* 建立自訂區段
* 變更自訂區段的名稱或說明
* 刪除自訂區段

如需自訂表單中自訂區段的相關資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### 匯率 {#exchange-rate}

當用戶執行以下操作之一時，系統將生成一個匯率審核日誌條目：

* 建立匯率
* 更改匯率：

   * 新增貨幣
   * 更改幣種的匯率
   * 將該幣種設定為整個系統中所有項目和報告的基本（預設）幣種

* 刪除匯率

有關配置匯率的詳細資訊，請參見 [設定匯率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### 群組 {#group}

當用戶執行以下操作之一時，系統將生成組審核日誌條目：

* 建立群組
* 刪除群組
* 變更群組：

   * 新增或移除使用者
   * 添加或刪除子組

### 職務角色 {#job-roles}

當用戶執行以下操作之一時，系統將生成作業角色審核日誌條目：

* 建立作業角色
* 更改作業角色：

   * 變更名稱
   * 添加、更改或刪除說明
   * 添加、更改或刪除每小時成本（成本/小時）
   * 添加、更改或刪除開單費率（開單/小時）

* 刪除工作角色

有關配置作業角色的詳細資訊，請參閱 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### 登入嘗試 {#login-attempt}

當用戶執行以下操作之一時，系統將生成「登錄嘗試」審核日誌條目：

* 在Workfront（瀏覽器和行動應用程式中）登入、登出或失敗登入嘗試
* 在任何Workfront整合(例如Workfront for Slack和Workfront for Salesforce)中登入、登出或失敗登入嘗試
* 登入或登出Workfront API

當Workfront管理員使用「登入方式」功能時，不會記錄登入嘗試記錄。

>[!NOTE]
>
>如果您的組織已上線至Adobe Admin Console，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

### 優先順序 {#priority}

當用戶執行以下操作之一時，系統將生成優先順序審核日誌條目：

* 建立優先順序
* 變更優先順序：

   * 變更名稱
   * 變更顏色
   * 將其設為預設值
   * 添加、更改或刪除優先順序的說明
   * 隱藏或顯示優先順序

* 刪除優先順序

如需設定優先順序的詳細資訊，請參閱 [建立和自訂優先順序](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### 專案偏好設定 {#project-preferences}

當用戶執行以下操作之一時，系統將生成「項目首選項」審核日誌條目：

* 建立自訂季度
* 變更專案偏好設定：

   * 鎖定或解除鎖定
   * 變更其中一項設定
   * 啟用、停用或編輯
   * 編輯時間軸計算

* 刪除自訂季度

如需專案偏好設定的詳細資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### 嚴重程度 {#severity}

當用戶執行以下操作之一時，系統將生成嚴重性審核日誌條目：

* 建立問題嚴重性
* 更改問題嚴重性：

   * 變更名稱
   * 變更顏色
   * 將其設為預設值
   * 更改或刪除嚴重性的描述
   * 隱藏或顯示嚴重性

* 刪除問題嚴重性

有關配置作業角色的詳細資訊，請參閱 [建立或自訂問題嚴重性](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### 狀態 {#status}

當用戶執行以下操作之一時，系統會生成狀態審核日誌條目：

* 在系統或組級別建立狀態
* 更改系統或組級別的狀態：

   * 重新命名
   * 設為預設狀態
   * 鎖定或解除鎖定
   * 隱藏或取消隱藏
   * 變更顏色或說明

* 刪除系統或組級別上的狀態

如需狀態的詳細資訊，請參閱 [狀態概觀](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### 任務和問題偏好設定 {#tasks-issues-preferences}

當用戶以下列方式之一更改「任務和問題」首選項時，系統將生成「任務和問題首選項」審核日誌條目：

* 鎖定或解除對首選項的鎖定
* 更改首選項的設定
* 更改任務、問題或請求的訪問設定

有關任務和問題首選項的詳細資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### 使用者 {#user}

當用戶執行以下操作之一時，系統將生成用戶審核日誌條目：

* 建立使用者

   <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

   >[!NOTE]
   >
   >如果您的組織已上線至Adobe Admin Console，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。

* 刪除使用者
* 變更使用者的存取層級、公司、團隊或群組
* 啟用使用者
* 停用使用者
