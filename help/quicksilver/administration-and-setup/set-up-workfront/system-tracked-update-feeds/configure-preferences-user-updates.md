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
source-git-commit: 594f224e11b0e7708ed555410b7c331741113791
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 1%

---

# 設定使用者更新的偏好設定

<!--Audited: 06/2025-->

當使用者在物件的[!UICONTROL 更新]區域新增註解時，您可以設定讓使用者存取特定功能的偏好設定。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td><p>新增：[！UICONTROL Standard]</p>
   或
   <p>目前： [！UICONTROL計畫]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td><p>若要在系統層級執行這些步驟，您需要[！UICONTROL系統管理員]存取層級。</p><p>若要為群組執行這些動作，您必須是該群組的管理員。</p></td>
  </tr> 
 </tbody> 
</table>

*如需此表格中資訊的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 允許使用者在更新中新增影像

依預設，使用者無法在更新中新增影像。 當您啟用此偏好設定時，使用者將可以在更新中附加影像。 偏好設定適用於您[!DNL Workfront]執行個體所有區域中的所有更新。

>[!NOTE]
>
>* 更新中儲存的影像會計入檔案儲存限制。 如需詳細資訊，請參閱[檢查檔案儲存限制](../../../documents/managing-documents/check-document-storage.md)。
>* 影像可透過物件上的[!UICONTROL 更新]標籤存取，也可在[!UICONTROL 主要功能表]下的[!UICONTROL 檔案]區域取得。
>

1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![齒輪設定圖示](assets/gear-icon-settings.png)。
1. 在左側面板中，選取&#x200B;**[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**。
1. 選取&#x200B;**[!UICONTROL 偏好設定]**&#x200B;標籤。

   ![更新摘要的使用者偏好設定](assets/updatefeeds-preferences-350x137.png)

1. 選取&#x200B;**[!UICONTROL 允許使用者在更新中新增影像]**&#x200B;核取方塊。
1. 選取&#x200B;**[!UICONTROL 「儲存」]**。

   啟用此偏好設定後，您可以隨時將其停用。 任何已在更新中張貼的影像將保留在物件的[!UICONTROL 更新]區域中。
