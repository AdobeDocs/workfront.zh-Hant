---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 設定使用者更新的偏好設定
description: 您可以設定當使用者在物件的 [!UICONTROL 更新] 區域。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: fd876089c964d57224452023b4656cd6df40b5a3
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# 設定使用者更新的偏好設定

您可以設定偏好設定，讓使用者在物件的中新增註釋時，能夠存取特定功能 [!UICONTROL 更新] 區域。

## 存取需求

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
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>若要在系統層級執行這些步驟，您需要[！UICONTROL系統管理員]存取層級。</p><p>若要為群組執行這些動作，您必須是該群組的管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 允許使用者在更新中新增影像

依預設，使用者無法在更新中新增影像。 當您啟用此偏好設定時，使用者將可以在更新中附加影像。 偏好設定會套用至您所有區域的所有更新 [!DNL Workfront] 執行個體。

>[!NOTE]
>
>* 更新中儲存的影像會計入檔案儲存限制。 如需詳細資訊，請參閱 [檢查檔案儲存限制](../../../documents/managing-documents/check-document-storage.md).
>* 影像可透過 [!UICONTROL 更新] 標籤內的標籤，也可在以下位置使用： [!UICONTROL 檔案] 下的區域 [!UICONTROL 主要功能表].
>

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 在左側面板中，選取 **[!UICONTROL 介面]** > **[!UICONTROL 更新摘要]**.
1. 選取 **[!UICONTROL 偏好設定]** 標籤。

   ![更新摘要的使用者偏好設定](assets/updatefeeds-preferences-350x137.png)

1. 選取 **[!UICONTROL 允許使用者在更新中新增影像]** 核取方塊。
1. 選取 **[!UICONTROL 儲存]**.

   啟用此偏好設定後，您可以隨時將其停用。 更新中張貼的任何影像將保留在 [!UICONTROL 更新] 物件上的區域。
