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
source-wordcount: '454'
ht-degree: 0%

---

# 設定專案的時間表重新計算

重新計算時間表可讓管理員檢視專案外的力量如何影響專案的時間表。 專案的時間表是指專案的計畫和預計日期。

作為 [!DNL Adobe Workfront] 管理員，您可以手動重新計算系統中所有專案的時間表。 專案所有者也可以手動重新計算個別專案的時間表。 如需詳細資訊，請參閱 [重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

本文說明您如何作為 [!DNL Workfront] 管理員，可以判斷如何以及何時進行 [!DNL Workfront] 透過設定專案偏好設定，自動計算專案時間表 [!UICONTROL 設定] 區域。

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
   <td> <p>系統管理員存取層級</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 設定自動重新計算

作為 [!DNL Adobe Workfront] 管理員，您可以設定 [!DNL Workfront] 自動重新計算專案時間表。 [!DNL Workfront] 可以每晚或專案範圍變更時，或兩者同時進行，重新計算專案時間表。

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於右上角，或 [!UICONTROL **主要功能表**] 圖示 ![](assets/lines-main-menu.png) 位於的左上角 [!DNL Workfront]，如果有，則按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 專案偏好設定]** > **[!UICONTROL 專案].**

1. 在 **[!UICONTROL 時間表]** 區段，啟用或停用以下一項或兩項設定。 預設會啟用這兩個設定。

   * **每天晚上：** [!DNL Workfront&#x200B;&#x200B;&#x200B;] 每隔24小時，在夜間重新計算一次時間表，僅適用於具有狀態的專案 [!UICONTROL 目前] 以及過去三個月更新的專案。 根據系統負載和其他因素，重新計算時間可能會延遲超過24小時。

     在這種情況下， [!DNL Workfront] 重新計算所有具有下列專案的專案時間表： [!UICONTROL 更新型別] 之 [!UICONTROL 自動] 或 [!UICONTROL 自動與變更時].

   * **專案範圍變更時**：如需關於構成專案範圍變更之內容的資訊，請參閱 [重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     在這種情況下， [!DNL Workfront] 重新計算所有更新型別為的專案的時間表 [!UICONTROL 自動與變更時] 或 [!UICONTROL 僅限變更時].
如需有關專案更新型別的資訊，請參閱 [專案更新型別總覽](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   系統會根據每個專案的更新型別，自動重新計算系統中所有專案的時間表。

## 重新計算整個的時間表 [!DNL Workfront] 例項

您可以執行 [!UICONTROL 重新計算時間表] 診斷以手動重新計算 [!DNL Workfront] 系統。 這可讓所有專案經理立即檢視外部變更對計畫和預計日期的影響。 如需詳細資訊，請參閱 [使用診斷來觸發自動化流程](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
