---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 編輯報告設定
description: 您可以編輯報表的設定，以定義它如何為其他用戶顯示，或用戶在運行報表之前可以提示哪些類型的資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 6%

---

# 編輯報告設定

您可以編輯報表的設定，以定義它如何為其他用戶顯示，或用戶在運行報表之前可以提示哪些類型的資訊。

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
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 操作步驟

1. 通過轉到 **主菜單** > **報告**，然後選擇報表的對象。

   或

   開啟現有報告，然後按一下 **報告操作** > **編輯**。

1. 按一下 **報告設定** 的子菜單。
1. 配置以下報告設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">報告標題</td> 
      <td>指定報表的標題。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>指定描述報表用途和用途的語句。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">運行此報告，其訪問權限為</td> 
      <td>選擇要在顯示給其他用戶時使用此報告的訪問權限的用戶。 有關使用其他用戶的訪問權限運行報告的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">運行並提交具有其他用戶訪問權限的報告</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">載入報表時，顯示</td> 
      <td>選擇載入報告時為所有用戶顯示的預設頁籤。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在儀表板上載入報表時，顯示……項目</td> 
      <td>指定在儀表板上載入報表時為所有用戶顯示的項目數。 預設值為15個項目，最大項目數為200。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在「詳細資訊」頁籤上顯示「資源網格」視圖</td> 
      <td> <p>（僅限用戶報告）選擇此選項可在報告的「詳細資訊」頁籤上顯示「資源網格」。</p> <p>注：在將「資源網格」視圖應用於用戶報表時，該報表僅顯示處於「當前」狀態的項目。 如果要查看處於任何其他狀態的項目，可以使用全局導航欄的「人員」區域中的「用戶利用率」頁籤，並在該區域應用「資源網格視圖」。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在「詳細資訊」頁籤上顯示特殊視圖</td> 
      <td>（僅限項目報告）指定用戶在訪問詳細資訊頁籤上的此資訊時將看到的視圖類型。 例如，可以選擇「里程碑」或「甘特圖」視圖。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">預設為以甘特圖檢視顯示此報告</td> 
      <td>（僅限項目報表和任務報表）選擇此選項可在用戶查看此報表中的「詳細資訊」標籤時自動啟用甘特圖視圖。<br>有關在項目報告和任務報告中查看甘特圖的詳細資訊，請參閱文章中的「查看項目清單甘特圖中的任務資訊」一節 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">在甘特圖中查看資訊 </a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許在報告中變更檢視</td> 
      <td>選擇此選項可允許用戶在運行報告時更改視圖。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許在報告中變更群組</td> 
      <td>選擇此選項可允許用戶在運行報告時更改組。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許在報告中變更篩選</td> 
      <td>選擇此選項可允許用戶在運行報告時更改篩選器。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **報表提示** 設定報表的任何提示。\
   有關向報表添加提示的詳細資訊，請參閱文章 [向報表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

1. 按一下&#x200B;**完成，** 按一下 **保存+關閉**。

## 其他資訊

另請參閱：

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [開始在Adobe Workfront](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [使用Adobe Workfront內置報告](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [建立自定義報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
