---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 編輯報表設定
description: 您可以編輯報表的設定，以定義對其他使用者的顯示方式，或使用者在執行報表之前可提示輸入何種資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 7%

---

# 編輯報表設定

<!-- Audited: 11/2024 -->

您可以編輯報表的設定，以定義對其他使用者的顯示方式，或使用者在執行報表之前可提示輸入何種資訊。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
      <p>標準</p>
      <p>規劃</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
 <td> <p>管理報表的許可權</p></td>  
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 操作步驟

1. 前往&#x200B;**主要功能表** > **報表**，開始建立報表，然後選取報表的物件。

   或

   開啟現有的報表，然後按一下&#x200B;**報表動作** > **編輯**。

1. 按一下Report Builder右上角的&#x200B;**報表設定**。
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
      <td>指定說明報表用途和使用的陳述式。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">透過以下存取許可權運行此報告：</td> 
      <td>選取您希望此報告在顯示給其他使用者時，使用哪個使用者的存取權。 如需以其他使用者的存取許可權執行報告的詳細資訊，請參閱文章<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">以其他使用者的存取許可權執行並傳遞報告</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告載入時，顯示</td> 
      <td>選擇報告載入時為所有使用者顯示的預設標籤。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">報告在儀表板上載入時，顯示……專案</td> 
      <td>指定報告在儀表板上載入時，為所有使用者顯示的專案數。 預設值為15個專案，專案數量上限為200個。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在詳細資訊標籤上顯示「資源格線」檢視</td> 
      <td> <p>（僅使用者報表）選取此選項可在報表的「詳細資訊」標籤上顯示「資源格線」。</p> <p>注意：套用「資源格線」檢視至使用者報表時，報表只會顯示處於「目前」狀態的專案。 如果您想檢視處於任何其他狀態的專案，可以使用「全域導覽列」之「人員」區域中的「使用者使用率」標籤，然後套用「資源格線檢視」。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在詳細資訊標籤上顯示特殊檢視</td> 
      <td>（僅限專案報告）指定當使用者在詳細資訊標籤上存取此資訊時，將會看到的檢視型別。 例如，您可以選取「里程碑」或「甘特圖」檢視。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">預設為以甘特圖檢視顯示此報告</td> 
      <td>（僅限專案報表與任務報表）選取此選項，可在使用者檢視此報表中的「詳細資訊」索引標籤時，自動啟用「甘特圖」檢視。<br>如需有關檢視專案報告和任務報告中甘特圖的詳細資訊，請參閱<a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">檢視甘特圖</a>中的文章中的「檢視專案清單甘特圖中的任務資訊」一節。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許在報告中變更檢視</td> 
      <td>選取此選項可允許使用者在執行報告時變更檢視。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許在報告中變更群組</td> 
      <td>選擇此選項可允許使用者在執行報告時變更群組。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許在報告中變更篩選</td> 
      <td>選取此選項可允許使用者在執行報告時變更篩選器。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**報告提示**&#x200B;為報告設定任何提示。\
   如需新增提示至報表的詳細資訊，請參閱文章[新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

1. 按一下&#x200B;**完成，**，然後按一下&#x200B;**儲存+關閉**。

## 其他資訊

另請參閱：

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [開始使用報告](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [使用Adobe Workfront內建報告](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
