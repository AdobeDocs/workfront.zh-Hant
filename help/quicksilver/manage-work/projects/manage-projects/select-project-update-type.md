---
product-area: projects
navigation-topic: manage-projects
title: 選擇項目更新類型
description: 通過為項目選擇「更新類型」(Update Type)，您可以控制在父任務或項目上保存對項目時間軸所做的更改的頻率。
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# 選擇項目更新類型

通過為項目選擇「更新類型」(Update Type)，您可以控制在父任務或項目上保存對項目時間軸所做的更改的頻率。

更新項目時間軸時，將根據對項目、其任務所做的更改或對時間軸所依賴的其他項目所做的更改重新計算項目時間軸。

例如，對項目上的任務所做的以下更改將觸發對項目時間軸的更新：

* 更新任務日期
* 更改任務的前置關係
* 更改父子關係、添加或刪除分配以及更改任務約束或持續時間類型。

## 存取需求

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 更新項目的更新類型

當任務更新時，其父對象（父任務或項目）會在更新類型指示的時間更新。  要指定項目的更新類型，請執行以下操作：

1. 轉到要指定其更新類型的項目。
1. 按一下「更多」功能表 ![](assets/more-icon.png) 在專案名稱旁，按一下 **編輯** .

1. 按一下  **專案** **設定**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. 在 **更新類型** 欄位中，選擇是否要讓Workfront每天自動計算項目時間軸、是否要項目經理手動計算項目時間軸。

   從下方清單的選項中選取。 

   >[!IMPORTANT]
   >
   >如果專案的時間軸超過15年，Workfront不會自動或在變更時計算時間軸。 超過15年的專案更新類型一律為手動。

   * **自動和更改：** 這是預設設定。 每次在項目中或時間軸所依賴的其他項目中發生更改時，都會更新項目時間軸。 每晚也會更新專案時間軸。 \
      這是建議的設定，因為它可確保項目時間軸始終保持最新。

      更新任務或項目並觸發時間軸重新計算時，將立即顯示所有可用日期，允許您繼續工作。 若專案的工作超過100個，需要較長計算時間的日期則會變灰。

      ![](assets/dates-dimmed-when-insline-editing-350x146.png)

      這表示重新計算尚未完成，日期可能會有所變更。

   * **僅更改：** 每次在項目中或時間軸所依賴的其他項目中發生更改時，都會更新項目時間軸；未進行排程更新。\
      如果您擔心繫統效能，而且如果項目或時間軸所依賴的其他項目中很少發生更改，則可能需要選擇此選項。

   * **僅自動：** 每晚更新項目時間表；進行變更後不會立即更新。\
      如果您擔心繫統效能，以及是否每天在項目中或時間軸所依賴的其他項目中發生許多更改，則可能需要選擇此選項。

      >[!NOTE]
      >
      >如果項目處於「計畫」狀態，則不會每晚自動重新計算該項目。 它只會在變更時重新計算。

   * **僅手動：** 只有在您選取要 **重新計算時間表**，如文章的「手動重新計算」一節所述 [重新計算項目時間表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
      如果您同時對專案進行許多變更，且希望時間軸重新計算在所有變更完成之後（而非每次個別變更後），您可以選取此選項。

1. 按一下&#x200B;**儲存**。
