---
product-area: reporting
navigation-topic: reporting-elements
title: 使用基於日期的通配符來概括報告
description: 在構建某些報告元素時，可以使用通配符而不是特定資訊來概括報告。
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# 使用基於日期的通配符來概括報告

在構建某些報告元素時，可以使用通配符而不是特定資訊來概括報告。

例如，如果要建立顯示具有特定計畫起始日期的任務的報表，則可以在篩選器中使用日曆日期選擇器選擇特定日期。 但是，如果要建立一個報告，該報告顯示在訪問報告之日起的某個時間範圍內具有計畫起始日期的任務，則可以使用通配符來指示某人在查看報告時顯示與查看報告時的時間段相關的資訊。

比如說過去一週，過去一年，接下來的兩週等等。 這樣，您只需構建一次報告，但由於您在篩選器中使用通配符，因此每次有人讀取報告時，報告都會生成不同的結果，因為它會適應運行報告的日期。

在構建以下報告元素時，可以使用基於日期的通配符：

* 篩選器
* 自定義提示
* 添加列規則時的視圖

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront許可證*</strong></td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、視圖、分組的訪問</p> <p>編輯對報表、儀表板、日曆的訪問以編輯報表中的報表元素</p> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>對象權限</strong></td> 
   <td> <p>管理對報表的權限以編輯報表中的報表元素</p> <p>管理對視圖或篩選器的權限以編輯它們</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 先決條件

必須先建立報表，然後才能向其添加通配符變數。

有關建立報告的資訊，請參見 [建立報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

## 操作步驟

要在報表中插入基於日期的通配符：

1. 轉到要插入基於日期的通配符的報表。
1. 按一下 **報告操作**，則 **編輯**。

1. 按一下 **篩選器** 頁籤。
1. 按一下 **添加篩選器規則**。
1. 開始鍵入要篩選依據的欄位的名稱。\
   必須鍵入引用日期的欄位。
1. 選擇 **等於** 的子菜單。

   >[!TIP]
   >
   >必須始終選擇 **等於** 在Adobe Workfront使用通配符時使用filter變數。

1. 在 **開始鍵入名稱……** 框中，鍵入： `$$TODAY` ，也請參見Wiki頁。

   或

   類型 `$$NOW` 的子菜單。

   此日期始終不同，因為它隨用戶實際查看報告的日期而改變。 所以報告裡的資訊是日復一日的。

1. （可選）如果要顯示在報告運行日期之後的時間範圍內發生的資訊，請鍵入 `$$TODAY+1w` 顯示下週的資訊，或 `$$TODAY+2m` 來顯示未來兩個月的資訊。 您還可以指明季度、小時、天或年的時限。
1. （可選）如果要顯示有關在運行報告之日之前某個時間範圍內發生的事件的資訊，請鍵入 `$$TODAY-1w` 顯示上週的資訊，或 `$$TODAY-2m` 顯示前兩個月的資訊。 您還可以指明季度、小時、天或年的時限。

   有關可在基於日期的通配符中使用的屬性、限定詞和運算子的完整清單，請參閱文章 [通配符篩選器變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. 按一下 **保存+關閉**。

## 其他資訊

另請參閱：

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [通配符篩選器變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront建立或編輯篩選器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [向報表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在視圖中使用條件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
