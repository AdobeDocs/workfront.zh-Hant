---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在畫布控制面板中將報表資料分組
description: 將報告結果組織成群組。 根據報告型別，分組的運作方式不同。
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 375d62fc12af075c2224f979d3ef87cdffdf03ea
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 4%
---
# 在畫布控制面板中將報表資料分組

>[!IMPORTANT]
>
>畫布儀表板功能目前僅適用於參與Beta階段的使用者。 在此階段中，部分功能可能無法完成或如預期般運作。 請依照「畫布控制面板」測試版概觀文章中[提供意見回饋](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)一節的指示，提交有關您體驗的任何意見回饋。<br>
>如果您對可能的錯誤或技術問題有回饋，請向Workfront支援提交票證。 如需詳細資訊，請參閱[聯絡客戶支援](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>請注意，以下雲端服務供應商未提供此測試版：
>
>* 自備Amazon Web Services金鑰
>* Azure
>* Google Cloud Platform

分組會組織您的報表結果，以便相關記錄一起顯示。 分組的運作方式取決於報表型別，因此本文會為各報告型別撰寫個別章節。

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
<p>標準</p> 
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

您必須在控制面板上擁有報表，或正在建立報表，才能將其資料分組。 如需詳細資訊，請參閱[建立畫布控制面板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)。

## 分組表格報表中的列

在表格報表中，群組會組織報表本身的列。

1. 在&#x200B;**設定**&#x200B;對話方塊中，按一下左側面板中的&#x200B;**群組設定**&#x200B;圖示。

1. 按一下&#x200B;**新增群組**，然後選取您要作為群組依據的欄位。 該分組會顯示在右側的預覽中。

1. （選用）重複以上步驟以新增更多群組。

## 在圖表和KPI報告中設定向下鑽研群組

在圖表和KPI報表中，您不會將主要視覺效果分組。 反之，您可以設定當檢視器鑽研至值時，深入分析表格的分組方式。

1. 在&#x200B;**設定**&#x200B;對話方塊中，按一下左側面板中的&#x200B;**向下鑽研群組設定**&#x200B;圖示。

1. 按一下&#x200B;**新增群組**，然後選取您要將深入分析表格群組依據的欄位。

## 在樞紐分析表中設定區段

樞紐分析表報表不使用群組。 相反地，您最多會定義兩個區段，這些區段是樞紐分析表量度分組和加總所依據的類別。

1. 在&#x200B;**設定**&#x200B;對話方塊中，按一下左側面板中的&#x200B;**區段**&#x200B;圖示。

1. 按一下&#x200B;**新增區段**，然後選取您想要的欄位。 區段在預覽中顯示為一欄。

1. （選用）重複以上步驟以新增第二個區段。 您最多可以新增兩個區段。

## 在儀表板上檢視分組的資料

報表檢視器可以展開、摺疊和排序群組資料。 如需詳細資訊，請參閱[使用畫布儀表板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md)中的[檢視包含分組資料的報告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md#view-reports-with-grouped-data)。
