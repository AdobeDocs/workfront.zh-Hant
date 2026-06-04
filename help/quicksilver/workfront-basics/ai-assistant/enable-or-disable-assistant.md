---
title: 啟用或停用AI助理
content-type: reference
description: 您可以控制組織中哪些存取層級有權存取AI助理。
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/h1895B7LDBKIhpJPrMROBoi-85LqrBUS1Rmw-m2n2Bo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 289
ht-degree: 7%

---

# 啟用或停用AI助理

身為Workfront管理員，您可以控制組織中哪些使用者已啟用AI助理。 這項作業可透過存取層級來管理。

您必須先為組織啟用AI助理，才能為存取層級啟用。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 為您的組織啟用或停用AI助理

若要為貴組織啟用AI助理：

{{step-1-to-setup}}

1. 在左側導覽中選取&#x200B;**系統**，然後選取&#x200B;**偏好設定**。
1. 向下捲動至&#x200B;**AI偏好設定**&#x200B;區段。
1. 開啟&#x200B;**啟用AI**&#x200B;切換開關。

>[!IMPORTANT]
>
>在使用AI Assistant之前，您必須與Adobe就檔案問題簽署了Gen AI合約。
>如需Gen AI合約的詳細資訊，請參閱Workfront的AI助理一文中的[簽署Adobe Gen AI合約](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。

## 啟用或停用存取層級的AI助理

若要為指定的存取層級啟用AI助理：

{{step-1-to-setup}}

1. 在左側導覽中選取&#x200B;**存取層級**。
1. 選取所需的存取層級，然後按一下清單上方的&#x200B;**編輯** ![編輯圖示](assets/edit-icon.png)圖示。
1. 在&#x200B;**編輯存取層級**&#x200B;方塊的&#x200B;**設定其他限制……**&#x200B;區域中，取消勾選&#x200B;**停用Workfront AI小幫手**&#x200B;核取方塊。
1. 按一下「**儲存**」。
1. 針對您想要為其啟用AI助理的每個存取層級，重複步驟3至5。



>[!NOTE]
>
>* 預設情況下，非管理員會停用AI助理。
>* 如果非管理員與Workfront中的AI助理圖示互動，則AI助理協定會出現，要求非管理員接受條款與條件。 如果他們接受協定，則可以使用AI Assistant，即使在其版面配置範本中停用它亦然。

