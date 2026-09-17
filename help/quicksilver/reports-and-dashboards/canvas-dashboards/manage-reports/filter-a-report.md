---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在畫布控制面板中篩選報表
description: 在報表上新增或編輯篩選器，以控制哪些資料顯示在畫布控制面板中。
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
source-git-commit: dc9caae8cc85543986eaefb1d3debdebfdf6ce96
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 5%
---
# 在畫布控制面板中篩選報表

>[!IMPORTANT]
>
>畫布儀表板功能目前僅適用於參與Beta階段的使用者。 在此階段中，部分功能可能無法完成或如預期般運作。 請依照「畫布控制面板」測試版概觀文章中[提供意見回饋](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)一節的指示，提交有關您體驗的任何意見回饋。<br>
>如果您對可能的錯誤或技術問題有回饋，請向Workfront支援提交票證。 如需詳細資訊，請參閱[聯絡客戶支援](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>請注意，以下雲端服務供應商未提供此測試版：
>
>* 自備Amazon Web Services金鑰
>* Azure
>* Google Cloud Platform

您可以在建置報表時及之後隨時篩選報表，以控制要顯示哪些資料。 在任何一種情況下，篩選選項和行為都相同。

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

您必須在控制面板上擁有報表，或正在建立報表，才能加以篩選。 如需詳細資訊，請參閱[建立畫布控制面板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)。

## 新增或編輯報告篩選器

若要在報表上新增或編輯篩選器：

1. 開啟報表的篩選面板：

   * 如果您正在建置報表，請按一下&#x200B;**設定**&#x200B;對話方塊左側面板中的&#x200B;**篩選器**&#x200B;圖示。
   * 如果您正在編輯現有報表，請按一下右上角的&#x200B;**更多**&#x200B;圖示，選取&#x200B;**編輯**，然後按一下&#x200B;**設定**&#x200B;對話方塊中的&#x200B;**篩選器**&#x200B;面板。

1. 按一下&#x200B;**編輯篩選器**。

1. 按一下&#x200B;**新增條件**，然後定義條件：

   * 按一下「**挑選欄位**」，然後選取要作為篩選依據的欄位。
   * 選取定義欄位必須符合何種條件的修飾詞。
   * 如果修正因子需要值，請鍵入或選取要評估的值。

   ![新增條件](assets/add-condition.png)

1. （選用）重複上一步驟以新增更多條件。

1. （選擇性）按一下&#x200B;**新增篩選器群組**&#x200B;以新增另一組篩選准則。 集合之間的預設運運算元為AND。 按一下運運算元以將其變更為OR。

>[!NOTE]
>
>如需欄位、運運算元、萬用字元和特殊篩選規則的完整清單，請參閱[畫布控制面板的報告篩選器參考](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md)。

1. 按一下「**儲存**」。
