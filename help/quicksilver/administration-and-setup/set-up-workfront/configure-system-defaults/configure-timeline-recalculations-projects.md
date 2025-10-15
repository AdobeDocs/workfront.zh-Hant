---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: 設定專案的時間表重新計算
description: 重新計算時間表可讓管理員檢視專案外的力量如何影響專案的時間表。 專案的時間表是指專案的計畫和預計日期。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# 設定專案的時間表重新計算

重新計算時間表可讓管理員檢視專案外的力量如何影響專案的時間表。 專案的時間表是指專案的計畫和預計日期。

作為[!DNL Adobe Workfront]管理員，您可以手動重新計算系統中所有專案的時間表。 專案所有者也可以手動重新計算個別專案的時間表。 如需詳細資訊，請參閱[重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

本文說明您身為[!DNL Workfront]管理員，如何在[!DNL Workfront]設定[!UICONTROL 區域中設定專案偏好設定，以決定]自動計算專案時間表的方式和時間。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[!UICONTROL 標準]</p>
       <p>[!UICONTROL 計畫]</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定自動重新計算

作為[!DNL Adobe Workfront]管理員，您可以設定[!DNL Workfront]何時自動重新計算專案時間表。 [!DNL Workfront]可以每晚或專案範圍變更時重新計算專案時間表，或兩者皆重新計算。

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 專案偏好設定]** > **[!UICONTROL 專案]。**

1. 在&#x200B;**[!UICONTROL 時間表]**&#x200B;區段中，啟用或停用以下一項或兩項設定。 預設會啟用這兩個設定。

   * **每晚：** [!DNL Workfront&#x200B;&#x200B;&#x200B;]只針對狀態為[!UICONTROL 目前]且過去三個月已更新的專案，每24小時、每晚重新計算一次時間表。 根據系統負載和其他因素，重新計算時間可能會延遲超過24小時。

     在此情況下，[!DNL Workfront]會重新計算所有專案的時間表，這些專案的[!UICONTROL 更新型別]為[!UICONTROL Automatic]或[!UICONTROL Automatic and On Change]。

   * **專案範圍變更時**：如需有關構成專案範圍變更的資訊，請參閱[重新計算專案時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

     在此情況下，[!DNL Workfront]會重新計算所有更新型別為[!UICONTROL 自動且僅於變更時]或[!UICONTROL 僅於變更時]的專案的時間表。
如需有關專案更新型別的資訊，請參閱[專案更新型別總覽](../../../manage-work/projects/planning-a-project/project-update-type-overview.md)。

1. 按一下「**[!UICONTROL 儲存]**」。

   系統會根據每個專案的更新型別，自動重新計算系統中所有專案的時間表。

>[!IMPORTANT]
>
>針對「預覽」和「自訂重新整理沙箱」環境，會停用每晚重新計算，且不會自動重新計算專案時間表。 您必須手動重新計算預覽和自訂重新整理沙箱環境的專案時間表。 如需詳細資訊，請參閱[重新計算專案時間表](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md)。


## 重新計算整個[!DNL Workfront]執行個體的時間表

您可以執行[!UICONTROL 重新計算時間表]診斷，以手動重新計算[!DNL Workfront]系統中的所有時間表。 這可讓所有專案經理立即檢視外部變更對計畫和預計日期的影響。 如需詳細資訊，請參閱[使用診斷來觸發自動化程式](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md)。
