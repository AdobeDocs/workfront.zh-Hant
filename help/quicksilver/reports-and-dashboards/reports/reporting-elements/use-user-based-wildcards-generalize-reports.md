---
product-area: reporting
navigation-topic: reporting-elements
title: 使用以使用者為基礎的萬用字元來歸納報表
description: 您可以在建立特定報表元素時，使用萬用字元而非特定資訊來泛化報表。
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 1%

---

# 使用以使用者為基礎的萬用字元來歸納報表

<!-- Audited: 11/2024 -->

您可以在建立特定報表元素時，使用萬用字元而非特定資訊來泛化報表。 例如，如果您想建立一個報告來顯示指派給特定使用者的任務，您可以在篩選器的「指派給」欄位中使用使用者的名稱。 但是，如果您想要建立一份報表來顯示指派給登入使用者的任務（無論該使用者是誰），您可以使用萬用字元來表示當有人檢視報表時，報表只會顯示與他們相關的資訊。 這樣的話，報表只需建置一次，但由於您在篩選器中使用萬用字元，因此每次有人閱讀時都會產生不同的結果。

建置下列報表元素時，您可以使用以使用者為基礎的萬用字元：

* 篩選器
* 自訂提示
* 為欄新增規則時的檢視

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>計劃</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯報告、儀表板、行事曆的存取權，以編輯報告中的報告元素</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>管理報表的許可權，以編輯報表中的報表元素</p> <p>管理檢視或篩選的許可權以編輯它們</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須先建立報表，才能在其中新增萬用字元變數。

如需建立報表的指示，請參閱[建立報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

## 操作步驟

若要在報表中插入以使用者為基礎的萬用字元：

1. 移至您要插入使用者型萬用字元的報表。
1. 按一下&#x200B;**報告動作**，然後按一下&#x200B;**編輯**。

1. 按一下&#x200B;**篩選器**&#x200B;索引標籤。
1. 按一下&#x200B;**新增篩選規則**。
1. 開始輸入您要作為篩選依據的欄位名稱。\
   您必須輸入參考使用者物件或使用者相關資訊的欄位。
1. 在篩選變數的下拉式選單中選取&#x200B;**等於**。

   >[!TIP]
   >
   >在Adobe Workfront中使用萬用字元時，您必須一律選取&#x200B;**等於**&#x200B;篩選器變數。

1. 在&#x200B;**開始輸入名稱……**&#x200B;方塊中，輸入： `$$USER.ID`或`$$USER.name` （如果您希望報告顯示登入的使用者資訊，根據其名稱）。 您可以插入參考登入使用者群組、團隊、公司或其他資訊的其他萬用字元。

   如需使用者型萬用字元的完整清單，請參閱[萬用字元篩選變數概觀](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。

1. 按一下「**儲存並關閉**」。

## 其他資訊

另請參閱：

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [萬用字元篩選器變數總覽](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中建立或編輯篩選器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [篩選器總覽](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
