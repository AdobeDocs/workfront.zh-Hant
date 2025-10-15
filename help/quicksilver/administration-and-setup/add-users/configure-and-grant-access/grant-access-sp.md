---
title: 授予Scenario Planner的存取權
description: 作為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Scenario Planner的存取權。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# 授予Scenario Planner的存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對「情境規劃工具」的存取權，如[存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

除了存取「案例規劃工具」之外，具有非系統管理員存取層次的使用者也必須具有財務資料的存取權，才能檢視計畫中包含的任何財務資訊，例如預算、成本及職務角色費率。 如需詳細資訊，請參閱[授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront套件</p> </td> 
   <td>商務或以上版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>淺色或更高</p>
   <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td> <p>您必須為Adobe Workfront Scenario Planner購買額外的授權。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視「情境規劃工具」的存取權或以上許可權</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>物件許可權</p> </td> 
   <td> <p>檢視計畫的許可權或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用自訂存取層級設定使用者對Scenario Planner的存取權

1. 開始建立或編輯存取層級，如[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 按一下您要用於此存取層級的&#x200B;**情境規劃工具**&#x200B;右邊的選項。

   >[!NOTE]
   >
   >請求或外部授權型別不允許檢視或編輯情景規劃工具。

1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續使用[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中所列的文章之一，例如[授與對工作的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授與對財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成時，按一下&#x200B;**儲存**。

## 依授權型別存取Scenario Planner

如需有關每個存取層級中的使用者可以使用Scenario Planner做什麼，請參閱每個物件型別[可用的](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario)功能文章中的[Scenario Planner區域](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)一節。

## 依存取層級設定的「案例規劃工具」存取權

以下資訊可協助您瞭解如何使用存取層級設定來控制使用者對Workfront Scenario Planner中資訊的存取。

* [無存取權](#no-access)
* [檢視存取權](#view-access)
* [編輯存取權](#edit-access)

### 無存取權 {#no-access}

無權存取「情境規劃工具」的使用者，在新增至其版面配置範本時，無法在主功能表中看到「情境」圖示，也無法檢視與其共用的計畫和方案。 如果計畫的連結共用給無權存取「情境規劃工具」的使用者，則使用者無法檢視或編輯計畫。

### 檢視存取權 {#view-access}

對Scenario Planner具有「檢視」存取權的使用者可以執行以下操作：

* 檢視主功能表![](assets/esp-icon-in-main-menu.png)中的「案例」圖示，不過「計畫」區域是空的，除非使用者按一下其他使用者共用的計畫連結。
* 當其他使用者共用計畫的連結時，檢視計畫。

  這包括計畫中的任何職務角色資訊。

  如果收件者使用者也可存取財務資料，則其中也會包含工作角色費率與計畫的成本資訊。 如需詳細資訊，請參閱[授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

### 編輯存取權 {#edit-access}

具有Scenario Planner編輯存取許可權的使用者可以執行以下操作：

* 檢視主功能表![](assets/esp-icon-in-main-menu.png)中的案例圖示，並使用它來存取計畫資料。
* 建立計畫。
* 檢視、編輯和刪除他們建立的計畫。
* 檢視、編輯和刪除其他使用者使用共用連結存取的計畫。

  這包括計畫中的任何職務角色資訊。

  如果收件者使用者有權存取財務資料，其中也會包含工作角色費率與計畫的成本資訊。 如需詳細資訊，請參閱[授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
