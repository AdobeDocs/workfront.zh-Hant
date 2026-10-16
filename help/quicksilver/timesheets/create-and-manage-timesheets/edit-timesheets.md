---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 編輯時程表資訊
description: 作為具有時程表管理存取許可權的使用者，您可以在Adobe Workfront中編輯現有時程表的資訊。 例如，您可以編輯時程表的「擁有者」、「核准者」或時間範圍。
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
TQID: https://experienceleague.adobe.com/--QshuygnTfcEJtt6-Tx-2QtNT-5p9TrTWaQTMBZNAg
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
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a3c1ab8fc8012199d9863fc978cca7418fa0a2f5
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 5%
---
# 編輯時程表資訊

作為具有時程表管理存取許可權的使用者，您可以在Adobe Workfront中編輯現有時程表的資訊。 例如，您可以編輯時程表的「擁有者」、「核准者」或時間範圍。

您可以編輯單一時程表上的資訊，也可以大量編輯多個時程表。

>[!IMPORTANT]
>
>如果使用者與週期性時程表相關聯，且時程表會自動產生，則您對現有時程表進行的變更不會反映在為未來日期產生的時程表中。 所有自動產生的時程表都會在時程表設定檔中建立設定。 如需詳細資訊，請參閱[建立週期性時程表](../create-and-manage-timesheets/create-timesheet-profiles.md)

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td><p>對時程表的管理存取權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 編輯時間表

{{step1-to-timesheets}}

預設會顯示您有權檢視的所有時間表。

![時程表清單](assets/list-of-all-timesheets.png)

1. （選擇性）按一下&#x200B;**搜尋**&#x200B;圖示![搜尋圖示](assets/search-icon.png)並輸入關鍵字以搜尋特定時程表。 例如，您可以搜尋時程表的時間範圍或擁有者名稱。

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

1. 選取一或多個時間表，然後按一下時間表清單頂端的&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。
1. 檢視或輸入下列資訊：

   | 欄位名稱 | 說明 |
   | --------- | ---------- |
   | 所有者 | <p>這是為其建立時程表的使用者名稱。 您無法編輯此欄位。</p><p>當您選取多個時程表時，此欄位未顯示。</p> |
   | 開始日期 | 這是時程表的開始日期。 |
   | 結束日期 | 這是時程表的結束日期。 |
   | 狀態 | <p>這是時程表的狀態。 以下為可能的時程表狀態選項：</p><ul><li>**開啟**：時程表已開啟，可以編輯小時專案。</li><li>**已提交**：已提交時程表以供指定核准者核准。</li><li>**已拒絕**：核准者未核準時程表，現在使用者可再次編輯時間專案。</li><li>**已關閉**：時程表已由使用者關閉或由核准者核准，因此現在已關閉。 您無法將時間新增至已關閉的時程表。</li></ul> |
   | 核准者 | <p>核准者指核准與時程表相關聯之使用者之時程表的使用者。 只有具有時程表管理許可權的使用者才能設定為核准者。 如需時程表管理許可權的詳細資訊，請參閱[授予使用者對特定區域的管理存取權](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。</p> <p>開始輸入時程表核准者的名稱，並在他們出現在清單中時選取他們。</p> <p>您可以在時程表上擁有多個核准者。 在這種情況下，在核准者核準時程表後，該時程表會被標籤為&#x200B;**已關閉**，並且會從所有剩餘核准者的時程表核准清單中消失。</p> |
   | 可編輯時間 | <p>如果您希望允許核准者編輯時程表上的小時，請選取此選項。</p><p>當您選取多個時程表時，此選項不可用。</p> |
   | 加班 | <p>您可以選擇隱藏時程表上的「加班」方塊。</p><p>此選項預設為停用。</p> |

1. 按一下「**儲存**」。
