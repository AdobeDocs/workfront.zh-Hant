---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: 設定專案的時間軸重新計算
description: 重新計算時間表使管理員能夠查看項目外部的力量如何影響項目的時間表。 項目時間表是指項目的計畫日期和預計日期。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 設定專案的時間軸重新計算

重新計算時間表使管理員能夠查看項目外部的力量如何影響項目的時間表。 項目時間表是指項目的計畫日期和預計日期。

作為 [!DNL Adobe Workfront] 管理員，您可以手動重新計算系統中所有項目的時間表。 項目所有者也可以手動重新計算各個項目的時間表。 如需詳細資訊，請參閱 [重新計算項目時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

本文說明您如何 [!DNL Workfront] 管理員可決定 [!DNL Workfront] 通過在中配置項目首選項自動計算項目時間軸 [!UICONTROL 設定] 的上界。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>系統管理員訪問級別</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置自動重新計算

作為 [!DNL Adobe Workfront] 管理員，您可以設定 [!DNL Workfront] 自動重新計算項目時間表。 [!DNL Workfront] 可以每晚或項目範圍更改時重新計算項目時間表，或者同時重新計算兩者。

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 專案偏好設定]** > **[!UICONTROL 專案].**

1. 在 **[!UICONTROL 時間軸]** 部分，啟用或禁用以下一項或兩項設定。 預設會啟用這兩項設定。

   * **每晚：** [!DNL Workfront&#x200B;&#x200B;&#x200B;] 僅對狀態為 [!UICONTROL 目前] 和在過去三個月中更新。

      在這種情況下， [!DNL Workfront] 會重新計算所有具有 [!UICONTROL 更新類型] of [!UICONTROL 自動] 或 [!UICONTROL 自動和更改].

   * **項目範圍更改時**:有關構成項目範圍更改的資訊，請參見 [重新計算項目時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

      在這種情況下， [!DNL Workfront] 會重新計算「更新類型」為的所有項目的時間表 [!UICONTROL 自動和更改] 或 [!UICONTROL 僅更改].
如需專案更新類型的相關資訊，請參閱 [專案更新類型概觀](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   系統中所有項目的時間表根據每個項目的更新類型自動重新計算。

## 重新計算整個時間表 [!DNL Workfront] 執行個體

您可以執行 [!UICONTROL 重新計算時間表] 手動重新計算中所有時間表的診斷 [!DNL Workfront] 系統。 這可讓所有項目經理立即查看外部更改對計畫日期和預計日期的影響。 如需詳細資訊，請參閱 [使用診斷程式觸發自動化流程](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
