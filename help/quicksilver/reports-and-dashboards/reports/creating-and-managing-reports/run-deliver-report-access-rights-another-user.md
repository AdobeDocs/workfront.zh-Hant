---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 運行並提交具有其他用戶訪問權限的報告
description: 預設情況下，用戶只能查看他們有權查看的報告中的對象。
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: e68e470da3b03e418584898c4098f0be302c68ec
workflow-type: tm+mt
source-wordcount: '1206'
ht-degree: 0%

---

# 運行並提交具有其他用戶訪問權限的報告

預設情況下，用戶只能查看他們有權查看的報告中的對象。

您可以允許所有用戶在報告中看到與其他用戶相同的結果，而不管他們對報告內對象的訪問權限級別或權限級別如何。

如果您運行的報告具有其他具有較高訪問權限的用戶的訪問權限(例如，Adobe Workfront管理員的訪問權限)，則所有具有查看報告權限的用戶都可以以報告生成器中指定的用戶身份查看報告中的資訊。 您可以為用戶在Workfront介面中找到的兩個報告或作為電子郵件附件發送給用戶的報告設定此設定。

>[!TIP]
>
>您應替換 **使用以下權限運行此報告：** 僅當希望報告以該用戶的訪問權限顯示時，才顯示該活動用戶的欄位。 例如，工作許可證用戶可能無權查看由計畫許可證用戶或系統管理員構建的報告中的所有項目，除非報告顯示時具有計畫員或系統管理員的訪問權限。\
如果報告與具有與中指定的用戶相似訪問權限的用戶共用 **使用以下權限運行此報告：** 欄位，可將此欄位留空。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問</p> <p>編輯對篩選器、視圖、分組的訪問</p> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>查看對報告的權限（查看已交付的報告）</p> <p>管理對報告的權限（以運行報告）</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 顯示具有其他用戶訪問權限的報告

填充 **使用以下權限運行此報表：** 欄位確保報告包含相同的資料，而不管哪個用戶正在訪問該報告。 該報告將像指定用戶一樣顯示。

訪問報告的用戶必須至少對報告具有「查看」權限才能查看報告。 如果中列出的用戶 **使用以下權限運行此報表：** 欄位已停用，報告將不再顯示給與報告共用的其他用戶。

要運行具有其他用戶訪問權限的報告，請執行以下操作：

1. 按一下 **主菜單** 表徵圖 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **報告**。

1. 選擇要顯示的報告，並具有其他用戶的訪問權限。
1. 按一下 **報告操作**，然後按一下 **編輯**。

1. 按一下 **報告設定**。

1. 在 **使用以下權限運行此報告：** 欄位中，開始鍵入希望報告顯示為的用戶的名稱，然後在清單中看到報告時選擇它。\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   訪問級別較低且允許生成報告的用戶沒有能力為 **使用以下權限運行此報表：** 的子菜單。

1. 按一下 **完成**。
1. 按一下 **保存+關閉**。\
   現在，將為與報告共用的所有用戶顯示該報告，如同在中指定的用戶查看了該報告一樣 **使用以下權限運行此報告：** 的子菜單。

>[!IMPORTANT]
輸入登錄用戶以外的用戶 **使用以下權限運行此報告：** 如果報表包含引用登錄用戶的通配符的篩選器，則欄位會影響報表中顯示的資訊。 根據在 **使用以下權限運行此報告：** 欄位，而不是通配符篩選器中定義的內容。
有關用戶欄位的通配符的詳細資訊，請參閱中的「基於用戶的變數」部分 [通配符篩選器變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)。

## 提交具有其他用戶訪問權限的報告

您可以設定要作為電子郵件附件傳送的報告。 您可以設定這些已傳送的報告以在它們顯示時顯示給訪問級別較高的用戶，以便所有用戶都可以在已傳送的報告中看到相同的資訊。 要查看通過電子郵件發送的報告的用戶必須添加到報告發送內收件人的「發送到」清單中。 有關設定要交付的報表的詳細資訊，請參閱文章 [報告交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

要提交具有其他用戶訪問權限的報告，請執行以下操作：

1. 按一下 **主菜單** 表徵圖 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **報告**。

1. 選擇要提交且具有其他用戶訪問權限的報告。
1. 按一下報告的名稱以選擇它。
1. 按一下 **報告操作**。
1. 按一下 **發送報告**。

1. 在 **提交此報告，其訪問權限為：** 欄位中，開始鍵入希望報告在通過電子郵件發送時顯示的用戶名稱，然後在清單中看到報告時選擇它。 預設值是生成報告的用戶的名稱。\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   訪問級別較低且允許生成報告的用戶沒有能力為 **以下列權限提交此報告：** 的子菜單。

1. 選擇 **格式** 您希望報告在電子郵件中顯示：

   * HTML
   * PDF
   * MS Excel
   * MS Excel(.xlsx)
   * TSV

1. 按一下 **立即發送** 立即發送。\
   或\
   按一下 **重複傳遞** 計畫報表的定期交貨。\
   有關報表交貨的詳細資訊，請參閱文章 [報告交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

## 具有源列的報表的限制

以下報表顯示「源」列，在該列中可以查看有關父對象的資訊：

* 發佈報告
* 工時報告
* 文檔報表

如果用戶對問題、小時或文檔的父對象沒有權限，則即使將報告配置為顯示或以其他用戶的訪問權限傳遞，報告的「源」列也將顯示為空。

為了在報告中顯示有關父對象的資訊，我們建議為父對象添加一列，在列中可以顯示父對象的名稱。

例如，可以將下列任何一項添加到具有「源」列的報表中：

* 文檔或小時報表的「項目名稱」(Project Name)、「任務名稱」(Task Name)或「發行名稱」(Issue Name)列。
* 發佈報告的「項目名稱」或「任務名稱」列。
* 使用引用所有三個對象的文本模式表達式的列。 以下是小時報告的示例：

   `displayname=Custom Source`

   `linkedname=opTask`

   `namekey=view.relatedcolumn`

   `namekeyargkey.0=opTask`

   `namekeyargkey.1=name`

   `textmode=true`

   `valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))`

   `valueformat=HTML`

   有關文本模式視圖的資訊，請參見 [使用文本模式編輯視圖](../text-mode/edit-text-mode-in-view.md)。