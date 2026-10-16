---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 匯出時程表清單
description: 身為人員管理員或時程表核准者，您可能需要下載時程表清單以快速檢視您負責之人員的時程表相關資訊。 您可以匯出時程表清單來執行此操作。
author: Lisa
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-bihpKoVoPCwTpAj-SK-RPPFpaCubsyLAfnfSmpTnyI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 64bb9e6dba8976ba413ec9b58e926da931bba1c5
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 6%
---
# 匯出時程表清單

<!--Audited: 8/2024-->

身為人員管理員或時程表核准者，您可能需要下載時程表清單以快速檢視您負責之人員的時程表相關資訊。 您可以匯出時程表清單來執行此操作。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td> <p>淺色或更高 </p>
   <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>檢視或更高的任務與問題存取權</p> </td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td> <p>檢視或更高的任務和問題許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 匯出時程表清單

{{step1-to-timesheets}}

預設會顯示您有權檢視的所有時間表。

![時程表清單](assets/list-of-all-timesheets.png)

1. （選用）執行下列任一項作業，更新時程表清單中的篩選器：

   * 選取頁面右上角的&#x200B;**我的時程表核准**，僅檢視您核准的時程表，

     或

     選取&#x200B;**我的時程表**&#x200B;以僅檢視您的時程表。

     這會將&#x200B;**我的時程表核准**&#x200B;或&#x200B;**我的時程表**&#x200B;篩選器套用至時程表清單。

   * 按一下&#x200B;**篩選器**&#x200B;圖示![篩選器圖示](assets/filter-nwepng.png)以套用篩選器或建立新篩選器。 如需建立或更新篩選的資訊，請參閱[在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。

   >[!NOTE]
   >
   >如果您的Workfront管理員或群組管理員從「設定」區域的「清單控制項」或您的「版面配置範本」中移除了這些篩選器，「我的時程表核准」和「我的時程表」選項不會顯示在時程表清單頂端或篩選器清單中。 如需詳細資訊，請參閱[使用配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)。

1. （選擇性）按一下&#x200B;**檢視** ![檢檢視示](assets/view-icon.png)或&#x200B;**群組** ![群組圖示](assets/grouping.png)圖示，以套用檢視或群組或建立新檢視或群組。

   如需有關建立篩選器、檢視或群組的資訊，請參閱下列文章：

   * [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中建立或編輯檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中建立群組](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 選取您要匯出的時程表，然後按一下&#x200B;**匯出** ![匯出圖示](assets/export-38x15.png)圖示。

   ![按一下「匯出」圖示](assets/export-timesheets.png)

1. 從下列選項中選取您要匯出時程表清單的檔案型別：

   * PDF Ladscape
   * PDF縱向
   * PDF其他大小
   * Excel
   * Excel (xlsx)
   * 頁籤分隔檔

   時程表清單會以選取的格式下載到您的電腦，並包含下列時程表資訊：

   * 日期範圍
   * 所有者名稱
   * 總時數
   * 加班金額
   * 核准者名稱
   * 狀態
