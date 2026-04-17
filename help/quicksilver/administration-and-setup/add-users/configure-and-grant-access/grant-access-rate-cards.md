---
title: 授予費率卡的存取權
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: 身為Adobe Workfront管理員，您可以透過使用者存取層級，定義使用者對Workfront中財務資料的存取權。
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
exl-id: b21e65d3-3c9f-4f3d-95d3-de4c09199622
source-git-commit: 85399542ce8e92de6da5a1de0960194e72958987
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 5%

---

# 授與費率卡的存取權

身為Adobe Workfront管理員，您可以透過使用者的存取層級定義使用者對評等卡的存取權，如[存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

如需費率卡的資訊，請參閱[管理費率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>標準</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 授予評等卡存取權的考量事項

在Workfront中授與費率卡的存取權時，請考量下列事項：

* 使用者必須擁有對評等卡、專案及財務資料的編輯存取權，才能將評等卡附加至專案。
* 無權存取費率卡和編輯財務資料的使用者無法將費率卡附加到專案，但他們可以編輯專案上來自其他來源的其他計費費率。

## 使用自訂存取層級設定使用者存取權以評等卡片

1. 開始建立或編輯存取層級，如[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 按一下費率卡右側![](assets/gear-icon-settings.png)檢視&#x200B;**或**&#x200B;編輯&#x200B;**按鈕上的齒輪圖示**，然後在&#x200B;**微調您的設定**&#x200B;下選取您要授與的功能。

   ![微調速率卡存取權](assets/rate-card-access-fine-tune.png)

1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，例如[授予工作存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)。
1. 完成時，按一下&#x200B;**儲存**。

   建立存取層級後，您可以將其指派給使用者。 如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 存取共用的費率卡

您可以授予其他使用者許可權來共用費率卡，如[共用費率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md)中所述。

當您與另一個使用者共用任何物件時，收件者對該物件的權利取決於兩個專案的組合：

* 您授予收件者的物件許可權
* 收件者物件型別的存取層級設定
