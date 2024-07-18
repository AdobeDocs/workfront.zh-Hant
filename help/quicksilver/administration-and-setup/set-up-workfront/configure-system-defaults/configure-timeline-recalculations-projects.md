---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: 設定專案的時間表重新計算
description: 重新計算時間表可讓管理員檢視專案外的力量如何影響專案的時間表。 專案的時間表是指專案的計畫和預計日期。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 4705c3fc76c1544f8c71e70a773432f164282abb
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# 設定專案的時間表重新計算

重新計算時間表可讓管理員檢視專案外的力量如何影響專案的時間表。 專案的時間表是指專案的計畫和預計日期。

作為[!DNL Adobe Workfront]管理員，您可以手動重新計算系統中所有專案的時間表。 專案所有者也可以手動重新計算個別專案的時間表。 如需詳細資訊，請參閱[重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

本文說明您身為[!DNL Workfront]管理員，如何在[!UICONTROL 設定]區域中設定專案偏好設定，以決定[!DNL Workfront]自動計算專案時間表的方式和時間。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>系統管理員存取層級</p> <p><b>注意</b>：如果您仍然沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 設定自動重新計算

作為[!DNL Adobe Workfront]管理員，您可以設定[!DNL Workfront]何時自動重新計算專案時間表。 [!DNL Workfront]可以每晚或專案範圍變更時重新計算專案時間表，或兩者皆重新計算。

1. 按一下右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，或[!DNL Workfront]左上角的&#x200B;[!UICONTROL **主功能表**]&#x200B;圖示![](assets/lines-main-menu.png) （如果可用），然後按一下&#x200B;**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**[!UICONTROL 專案偏好設定]** > **[!UICONTROL 專案]。**

1. 在&#x200B;**[!UICONTROL 時間表]**&#x200B;區段中，啟用或停用以下一項或兩項設定。 預設會啟用這兩個設定。

   * **每晚：** [!DNL Workfront&#x200B;&#x200B;&#x200B;]只針對狀態為[!UICONTROL 目前]且過去三個月已更新的專案，每24小時、每晚重新計算一次時間表。 根據系統負載和其他因素，重新計算時間可能會延遲超過24小時。

     在此情況下，[!DNL Workfront]會重新計算所有專案的時間表，這些專案的[!UICONTROL 更新型別]為[!UICONTROL Automatic]或[!UICONTROL Automatic and On Change]。

   * **專案範圍變更時**：如需有關構成專案範圍變更的資訊，請參閱[重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

     在此情況下，[!DNL Workfront]會重新計算所有更新型別為[!UICONTROL 自動且僅於變更時]或[!UICONTROL 僅於變更時]的專案的時間表。
如需有關專案更新型別的資訊，請參閱[專案更新型別總覽](../../../manage-work/projects/planning-a-project/project-update-type-overview.md)。

1. 按一下「**[!UICONTROL 儲存]**」。

   系統會根據每個專案的更新型別，自動重新計算系統中所有專案的時間表。

## 重新計算整個[!DNL Workfront]執行個體的時間表

您可以執行[!UICONTROL 重新計算時間表]診斷，以手動重新計算[!DNL Workfront]系統中的所有時間表。 這可讓所有專案經理立即檢視外部變更對計畫和預計日期的影響。 如需詳細資訊，請參閱[使用診斷來觸發自動化程式](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md)。
