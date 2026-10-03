---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在畫布儀表板中複製和移動報告
description: 您可以在畫布控制面板之間複製或移動報表。
author: Courtney
feature: Reports and Dashboards
exl-id: e0f9d091-bb89-4c5b-a18d-b1e339084e67
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/5ioNl-M-KgnYE0huAbxMmLlE-qIrnwwKp-eeTRRiYLo'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 45491118778279522358f87c1c4185c4cf824829
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 4%
---
# 在畫布儀表板中複製和移動報告

{{highlighted-preview}}

>[!IMPORTANT]
>
>畫布儀表板功能目前僅適用於參與Beta階段的使用者。 在此階段中，部分功能可能無法完成或如預期般運作。 請依照「畫布控制面板」測試版概觀文章中[提供意見回饋](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)一節的指示，提交有關您體驗的任何意見回饋。<br>
>如果您對可能的錯誤或技術問題有回饋，請向Workfront支援提交票證。 如需詳細資訊，請參閱[聯絡客戶支援](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>請注意，以下雲端服務供應商未提供此測試版：
>
>* 自備Amazon Web Services金鑰
>* Azure
>* Google Cloud Platform

KPI、表格或圖表報表建立後，您可以在畫布控制面板中複製該報表。 複製後，您可在儲存前視需要編輯報表。


## 存取需求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<p>任何 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td> 
<p>標準 </p> 
<p>規劃</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td><p>編輯報告、儀表板和行事曆的存取權</p>
  </td> 
  </tr>  
      <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td><p>管理儀表板的許可權</p>
  </td> 
  </tr>
</tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先決條件

您必須先將報表新增到控制面板，然後才能複製。

如需詳細資訊，請參閱[建立畫布儀表板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)。

## 在生產環境中複製報告

{{step1-to-dashboards}}

1. 在左側面板中，按一下&#x200B;**畫布控制面板**。
1. 在&#x200B;**畫布控制面板**&#x200B;頁面上，按一下您要複製之報告右上角的&#x200B;**更多** ![更多](assets/more-icon.png)按鈕，然後選取&#x200B;**複製**。

   ![重複按鈕](assets/duplicate-button.png)

1. （選擇性）在出現的&#x200B;**設定**&#x200B;方塊中，在&#x200B;**詳細資料**&#x200B;索引標籤中輸入新報告&#x200B;**名稱**。

1. （選用）使用左側的標籤，對設定進行任何需要的調整。

   >[!NOTE]
   >
   >這些標籤會因您複製的KPI、表格或圖表報告而異。  如需詳細資訊，請參閱[在畫布儀表板中建置KPI報告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md)、[在畫布儀表板中建置圖表報告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md)以及[在畫布儀表板中建置表格報告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md)。

1. 按一下「**儲存**」。 重複的報告會出現在控制面板上。

<div class="preview">

## 在預覽中複製或移動報告

您可以將報告複製到目前的儀表板、複製到另一個儀表板，或將其移動到另一個儀表板。 複製會在目的地建立重複的報表；移動會將報表從目前的儀表板重新定位。

>[!IMPORTANT]
>
>* 若要複製報表，您需要目的地控制面板的管理許可權。
>* 若要移動報表，您必須同時具備來源和目的地控制面板的「管理」存取權。
>* 如果報告已設定「以使用者身分執行」設定，而您不是系統管理員或「以使用者身分執行」，您仍可複製或移動報告，但「以使用者身分執行」會從產生的報告中移除。


若要複製或移動報表：

{{step1-to-dashboards}}

1. 在左側面板中，按一下&#x200B;**畫布控制面板**。
1. 開啟包含報表的控制面板。
1. 按一下報告右上角的&#x200B;**更多** ![更多按鈕](assets/more-icon.png)圖示，然後選取&#x200B;**複製報告**。

   ![複製報告選項](assets/copy-report-button.png)

1. 在&#x200B;**複製報告**&#x200B;對話方塊中，選擇下列其中一個選項：

   <table>
   <tr>
   <td><strong>複製</strong></td>
   <td>按一下畫面底部的<strong>[複製</strong>]以複製報告。 依預設，會選取目前的儀表板。 您需要「管理」控制面板的存取權才能複製報告。</td>
   </tr>
   <tr>
   <td><strong>複製並移動</strong></td>
   <td>選取不同的目標控制面板以複製報表，並將其移至新控制面板。 原始報告會保留在目前的儀表板上。您需要「管理」目的地控制面板的存取權，才能複製和移動報表。 </td>
   </tr>
   <tr>
   <td><strong>移動</strong></td>
   <td>選取要移動報表的其他目標控制面板。 這會將報表重新定位到目標控制面板，並將其從目前控制面板移除。 您需要「管理」來源和目的地控制面板的存取權才能移動報表。</td>
   </tr>
   </table>

   >[!NOTE]
   >
   >如果報告已設定「以使用者身分執行」，而您不是系統管理員或設定為「以使用者身分執行」的使用者，您仍可複製或移動報告。 「以使用者身分執行」會從產生的報表中移除。

1. 按一下「**儲存**」。

   ![複製並移動](assets/copy-and-move.png)

</div>
