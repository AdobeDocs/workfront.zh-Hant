---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 匯出時程表清單
description: 身為人員管理員或時程表核准者，您可能需要下載時程表清單以快速檢視您負責之人員的時程表相關資訊。 您可以匯出時程表清單來執行此操作。
author: Alina
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 2%

---

# 匯出時程表清單

身為人員管理員或時程表核准者，您可能需要下載時程表清單以快速檢視您負責之人員的時程表相關資訊。 您可以匯出時程表清單來執行此操作。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視任務或問題的存取權或以上許可權</p> <p>如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視或更高的時程表許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫或授權型別，請連絡您的Workfront管理員。

## 匯出時程表清單

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**時程表**。 依預設會選取&#x200B;**全部**&#x200B;篩選器。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （選擇性）按一下&#x200B;**搜尋**&#x200B;圖示![](assets/search-icon.png)並輸入關鍵字及搜尋特定時間表。 例如，您可以搜尋時間設定時間範圍或擁有者名稱。

1. （選用）執行下列任一項作業，更新時程表清單中的篩選器：

   * 選取頁面右上角的&#x200B;**我的時程表核准**，僅檢視您核准的時程表

     或

     選取&#x200B;**我的時程表**&#x200B;以僅檢視您的時程表。

     這會套用我的時程表核准或我的時程表篩選器到時程表清單。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * 按一下「篩選」圖示![](assets/filter-nwepng.png)以套用不同的篩選，或建立新的篩選。 如需建立或更新篩選的資訊，請參閱[在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)。

   >[!NOTE]
   >
   >如果您的Workfront管理員或群組管理員從「設定」區域的「清單控制項」或您的「版面配置範本」中移除了「我的時程表核准」和「我的時程表」，則「我的時程表核准」和「我的時程表」選項不會顯示在時程表清單頂端或篩選器清單中。 如需詳細資訊，請參閱下列文章：
   >
   >   
   >   
   >   * [使用配置範本自訂篩選器、檢視和群組](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （選擇性）按一下&#x200B;**檢視** ![](assets/view-icon.png)或&#x200B;**群組** ![](assets/grouping.png)圖示以套用不同的檢視或群組或建立新的檢視或群組。

   如需有關建立篩選器、檢視或群組的資訊，請參閱下列文章：

   * [在Adobe Workfront中建立或編輯篩選器](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [在Adobe Workfront中建立或編輯檢視](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [在Adobe Workfront中建立群組](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 選取您要匯出的時程表，然後按一下&#x200B;**匯出** ![](assets/export-38x15.png)圖示。

   ![](assets/all-timesheets-list-with-export-button-nwe-350x262.png)

1. 從下列選項中選取您要匯出時程表清單的檔案型別：

   * PDF領地
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
