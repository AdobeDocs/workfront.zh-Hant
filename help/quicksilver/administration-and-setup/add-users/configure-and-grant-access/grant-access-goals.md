---
title: 授予Adobe Workfront目標的存取權
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: 作為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront目標的存取權。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8639da14-d545-4f9a-894b-12c29699b0db
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YY7P4MbYrAENaxVmfdZ8LOeF-CSNTstq-k-0Hx0jPME
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 6%

---

# 授予Adobe Workfront目標的存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Adobe Workfront目標的存取權，如[存取層級總覽](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)所述。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

您必須具備下列專案才能授與使用者存取Workfront目標的許可權：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront套件</td> 
   <td> <p>Workfront Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須擁有系統管理員存取層級。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Workfront Goals <p>Contact your Workfront account manager to learn about a Workfront Goals license. </p> <p>Workfront Goals is available only in the new Adobe Workfront experience.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration*</td> 
   <td> <p>You must have the System Administrator access level.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## 使用自訂存取層級授與使用者對Workfront目標的存取權

1. 開始建立或編輯存取層級，如[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 按一下您要用於此存取層級的&#x200B;**目標**&#x200B;右邊的選項。


   >[!NOTE]
   >
   >外部授權型別不允許檢視或編輯對Workfront目標的存取權。

1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續使用[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中所列的文章之一，例如[授與對工作的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授與對財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成時，按一下&#x200B;**儲存**。

## 依授權型別存取Workfront目標

Workfront管理員可使用存取層級，將對Workfront目標的存取權授與具有下列授權的使用者：

* 標準、輕度、投稿人
* 計畫、工作、請求或稽核授權。

如需存取Workfront目標的詳細資訊，請參閱[使用Workfront目標的需求](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md)。
