---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 設定使用者更新的偏好設定
description: 當使用者在物件的[!UICONTROL 更新]區域新增註解時，您可以設定存取特定功能的偏好設定。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 設定使用者更新的偏好設定

<!--Audited: 08/2025-->

當使用者在物件的[!UICONTROL 更新]區域新增註解時，您可以設定讓使用者存取特定功能的偏好設定。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>[！UICONTROL標準]</p>
   <p>[！UICONTROL計畫]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td><p>系統管理員，在系統層級執行這些步驟。 </p>
   <p>供需規劃員，除了擔任群組的經理外，還可為群組執行這些步驟。</p></td>
  </tr> 
 </tbody> 
</table>

*如需此表格中資訊的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>To perform these steps at the system level, you need the [!UICONTROL System Administrator] access level.</p><p>To perform them for a group, you must be a manager of that group.</p></td>
  </tr> 
 </tbody> 
</table>-->

## 允許使用者在更新中新增影像

依預設，使用者無法在更新中新增影像。 當您啟用此偏好設定時，使用者將可以在更新中附加影像。 偏好設定適用於您[!DNL Workfront]執行個體所有區域中的所有更新。

>[!NOTE]
>
>* 更新中儲存的影像會計入檔案儲存限制。 如需詳細資訊，請參閱[檢查檔案儲存限制](../../../documents/managing-documents/check-document-storage.md)。
>* 影像可透過物件上的[!UICONTROL 更新]標籤存取，也可在[!UICONTROL 主要功能表]下的[!UICONTROL 檔案]區域取得。
>

1. 按一下&#x200B;**[!UICONTROL 右上角的]**&#x200B;主功能表![圖示](assets/main-menu-icon.png)主功能表圖示[!DNL Adobe Workfront]，然後按一下&#x200B;**[!UICONTROL 設定]** ![齒輪設定圖示](assets/gear-icon-settings.png)。
1. 在左側面板中，選取&#x200B;**[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**。
1. 選取&#x200B;**[!UICONTROL 偏好設定]**&#x200B;標籤。

   ![更新摘要的使用者偏好設定](assets/updatefeeds-preferences-350x137.png)

1. 選取&#x200B;**[!UICONTROL 允許使用者在更新中新增影像]**&#x200B;核取方塊。
1. 選取&#x200B;**[!UICONTROL 「儲存」]**。

   啟用此偏好設定後，您可以隨時將其停用。 任何已在更新中張貼的影像將保留在物件的[!UICONTROL 更新]區域中。
