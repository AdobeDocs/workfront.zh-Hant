---
title: 授予品牌許可權的存取權
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: 作為Adobe Workfront管理員，您可以透過在Admin Console中建立使用者群組並指派GenStudio系統管理員產品設定檔來設定品牌許可權。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 727efbd6-79b4-42c5-bfa2-e5350f30ff23
source-git-commit: 3e76f4a798a55a674a5ada2661c4b6bbb55195f2
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 4%

---

# 授予品牌許可權的存取權

使用者新增至使用者群組時，會獲得Adobe GenStudio系統管理員的品牌建立、編輯和發佈許可權。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console許可權</td> 
   <td> <p>您必須是Adobe Admin Console的系統管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 需求

* 您的Workfront執行個體必須已啟用統一核准。

* 您的組織必須有GenStudio Foundation。
   * Workfront中的內容檢閱者提供GenStudio Foundation中可用的功能，以進行資產檢閱和核准工作流程。 您不需要直接存取GenStudio Foundation即可完成工作。 您透過「內容檢閱者」存取GenStudio Foundation功能時，需遵守Workfront合約的條款。
* Adobe必須有已簽署的Adobe Gen AI合約檔案。
如需簽署合約的詳細資訊，請參閱[簽署Adobe Gen AI合約](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。

## 1.在Admin Console中設定品牌許可權

### 步驟1：建立使用者群組

在Admin Console中建立新的使用者群組，以管理品牌建立和編輯的許可權。

### 步驟2：將產品設定檔指派給使用者群組

與指派的設定檔相關聯的軟體權利檔案會提供此群組中的所有使用者「GenStudio品牌」許可權（建立、更新和刪除品牌）。

若要指派設定檔：

1. 導覽至新建立的使用者群組。
1. 按一下&#x200B;**指派的產品設定檔**&#x200B;索引標籤。
1. 按一下&#x200B;**指派設定檔**。
1. 在快顯視窗中，從產品清單中選取&#x200B;**Adobe GenStudio**，然後按一下&#x200B;**套用**。
1. 選取&#x200B;**Adobe GenStudio Foundation編輯器**&#x200B;設定檔。
1. 按一下「**套用**」。
1. 按一下「**儲存**」。

### 步驟3：將使用者新增至使用者群組

若要指派建立、編輯和發佈品牌的使用者許可權，請將他們新增至使用者群組。

>[!NOTE]
>
>在將群組新增到專案之前，您必須至少新增一個使用者，如步驟4所述。

若要新增使用者：

1. 移至&#x200B;**Admin Console** > **使用者** > **使用者群組**。
1. 選取您的使用者群組。
1. 依使用者名稱或電子郵件地址新增使用者。
1. 從現有使用者的建議相符項中選取。

### 步驟4：建立品牌專案

專案為使用者提供可儲存品牌資產的儲存位置。

若要建立專案：

1. 導覽至Admin Console中的&#x200B;**儲存體**&#x200B;索引標籤。
1. 按一下&#x200B;**專案**。
1. 按一下&#x200B;**建立專案**。
1. 在快顯視窗中輸入專案名稱： **Adobe GenStudio品牌**。

   >[!IMPORTANT]
   >
   >如圖所示輸入專案名稱。 請勿新增額外空格或變更大小寫。

1. 按一下「**建立**」。

### 步驟5：邀請使用者群組加入專案

將使用者群組新增至Brands專案，讓使用者能夠存取和管理資產。

1. 在&#x200B;**邀請加入專案**&#x200B;快顯視窗中，新增您建立的使用者群組。
1. 選取&#x200B;**可以編輯**&#x200B;許可權。
1. 按一下&#x200B;**邀請**。

### 結果

群組使用者現在擁有在Workfront中建立、編輯和發佈品牌資產的許可權。

## 2.在Workfront存取層級中授予品牌存取權

您必須先完成上一節中的所有步驟，才能在Workfront存取層級中授與個別使用者對Brands的存取權。

>[!IMPORTANT]
>
>* 只有在Admin Console中具有GenStudio系統管理員產品設定檔指派給使用者群組的使用者，才能在Workfront中建立、編輯和發佈品牌，即使其他使用者有權存取其存取層級設定中啟用的品牌。
>* 在Admin Console中將「品牌」存取權啟用但未新增至使用者群組的情況下，已新增至存取層級的使用者只能檢視品牌。


若要授與Workfront存取層級中品牌的存取權：

{{step-1-to-setup}}

1. 按一下左側面板中的&#x200B;**存取層級**。
1. 找到您要編輯的存取層級，然後按一下編輯圖示![編輯圖示](assets/edit-icon.png)進行編輯。

   或

   按一下&#x200B;**新增存取層級**&#x200B;以建立新的存取層級。 如需有關建立存取層級的詳細資訊，請參閱[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。
1. 向下捲動至&#x200B;**設定其他限制**，然後選取&#x200B;**允許使用者存取品牌**。
   ![允許存取品牌設定](assets/access-for-brands.png)
1. 按一下「**儲存**」。

設定「品牌」後，您可以建立「內容檢閱者」，在檢閱和核准工作流程中根據品牌指引檢閱資產。 如需詳細資訊，請參閱[設定AI共同作業人員](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)。
