---
product-area: reporting
navigation-topic: reporting-elements
title: 使用以使用者為基礎的萬用字元來歸納報表
description: 建置特定報表元素時，您可以使用萬用字元（而非特定資訊）來歸納報表。
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# 使用以使用者為基礎的萬用字元來歸納報表

建置特定報表元素時，您可以使用萬用字元（而非特定資訊）來歸納報表。 例如，如果要建立報告來顯示分配給特定用戶的任務，則可以在篩選器的「已分配給」欄位中使用該用戶的名稱。 不過，如果您想要建立一個報表來顯示指派給登入使用者的工作（無論該使用者是誰），您可以使用萬用字元指出當有人檢視報表時，其只會顯示與其相關的資訊。 這樣，您只需建立報表一次，但因為您在篩選器中使用萬用字元，所以每次有其他人讀取報表時，會產生不同的結果。

建置下列報表元素時，您可以使用使用者型萬用字元：

* 篩選器
* 自訂提示
* 新增欄規則時的檢視

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取，以編輯報表中的報表元素</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>管理報表權限以編輯報表中的報表元素</p> <p>管理檢視或篩選器的權限，以便編輯</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須先建立報表，才能新增萬用字元變數。

如需建立報表的指示，請參閱 [建立報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 操作步驟

若要在報表中插入使用者型萬用字元：

1. 轉至要插入基於用戶的通配符的報告。
1. 按一下 **報表動作**，然後 **編輯**.

1. 按一下 **篩選器** 標籤。
1. 按一下 **新增篩選規則**.
1. 開始鍵入要篩選的欄位名稱。\
   必須鍵入引用用戶對象或有關用戶資訊的欄位。
1. 選擇 **等於** 的下拉式選單中。

   >[!TIP]
   >
   >您必須一律選取 **等於** 在Adobe Workfront中使用萬用字元時篩選變數。

1. 在 **開始鍵入名稱……** 框，鍵入： `$$USER.ID` 或 `$$USER.name` 如果您希望報表根據登入使用者的名稱，顯示有關該使用者的資訊。 您可以插入其他萬用字元，以參考登入使用者的群組、團隊、公司或其他資訊。

   如需使用者型萬用字元的完整清單，請參閱 [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. 按一下 **儲存+關閉**.

## 其他資訊

另請參閱：

* [基本報表建立程式](https://one.workfront.com/s/basic-report-creation-program)
* [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中建立或編輯篩選器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
