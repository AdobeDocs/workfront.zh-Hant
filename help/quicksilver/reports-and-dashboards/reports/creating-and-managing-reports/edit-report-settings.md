---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 編輯報表設定
description: 您可以編輯報表的設定，以定義其他使用者如何顯示報表，或使用者在執行報表前可提示輸入哪些資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 6%

---

# 編輯報表設定

您可以編輯報表的設定，以定義其他使用者如何顯示報表，或使用者在執行報表前可提示輸入哪些資訊。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 操作步驟

1. 前往 **主菜單** > **報表**，然後選取報表的物件。

   或

   開啟現有報表，然後按一下 **報表動作** > **編輯**.

1. 按一下 **報表設定** 在報告建立工具的右上角。
1. 設定下列報表設定：

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
      <td>指定說明報表用途和用途的陳述式。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">使用以下權限運行此報表：</td> 
      <td>選擇在顯示給其他用戶時希望此報表使用的訪問權限的用戶。 如需使用其他使用者的存取權限執行報表的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">使用其他使用者的存取權限執行並傳送報表</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報表載入時，顯示</td> 
      <td>選取報表載入時針對所有使用者顯示的預設索引標籤。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報表在控制面板上載入時，顯示……項目</td> 
      <td>指定報表在控制面板上載入時顯示給所有使用者的項目數。 預設為15個項目，項目數上限為200。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在「詳細資訊」頁簽上顯示資源網格視圖</td> 
      <td> <p>（僅限用戶報告）選擇此選項以在報告的「詳細資訊」頁簽上顯示資源網格。</p> <p>注意：將「資源網格」視圖應用到用戶報表時，該報表只顯示處於「當前」狀態的項目。 如果要查看處於任何其他狀態的項目，可以使用全局導航欄的「人員」區域中的「用戶利用率」頁簽，然後在該處應用資源網格視圖。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在「詳細資訊」標籤上顯示特殊檢視</td> 
      <td>（僅限專案報表）指定使用者在「詳細資訊」標籤上存取此資訊時會看到的檢視類型。 例如，您可以選取「里程碑」(Milestone)或「甘特」(Gantt)視圖。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">預設為以甘特圖檢視顯示此報告</td> 
      <td>（僅限項目報告和任務報告）選擇此選項，在用戶查看此報告中的「詳細資訊」頁簽時自動啟用甘特視圖。<br>有關在項目報告和任務報告中查看甘特圖的詳細資訊，請參閱文章中的「在項目清單中查看任務資訊甘特圖」部分 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">在甘特圖中查看資訊 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許在報告中變更檢視</td> 
      <td>選擇此選項可讓使用者在執行報表時變更檢視。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許在報告中變更群組</td> 
      <td>選取此選項，可讓使用者在執行報表時變更群組。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許在報告中變更篩選</td> 
      <td>選取此選項，可讓使用者在執行報表時變更篩選。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **報表提示** 設定報表的任何提示。\
   有關向報表添加提示的詳細資訊，請參閱文章 [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. 按一下&#x200B;**完成，** 然後按一下 **儲存+關閉**.

## 其他資訊

另請參閱：

* [新Workfront體驗的基本報表建立計畫](https://one.workfront.com/s/basic-report-creation-program)
* [開始使用Adobe Workfront中的報表](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [使用Adobe Workfront內建報表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
