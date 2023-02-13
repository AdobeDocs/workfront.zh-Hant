---
product-area: projects
navigation-topic: manage-tasks
title: 將里程碑與任務關聯
description: 您可以將里程碑與任務關聯，以指出您何時到達專案期限內的重要步驟。
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 將里程碑與任務關聯

您可以將里程碑與任務關聯，以指出您何時到達專案期限內的重要步驟。

## 存取需求

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
  <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理任務的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

在將里程碑與任務關聯之前，必須存在以下內容：

* Workfront管理員必須建立里程碑路徑，如 [建立里程碑路徑](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* 要將里程碑路徑與項目關聯，項目必須處於「計畫」或「當前」狀態。

>[!TIP]
>
>若要使用「里程碑」檢視取得專案里里程碑進度的最佳概覽，您應建立父任務，並將它們與專案的每個主要階段建立關聯。 然後，將這些父任務與里程碑路徑的每個里程碑相關聯。

## 將里程碑與任務關聯

1. 前往專案，然後按一下 **更多** 圖示 ![](assets/more-icon.png)，然後 **編輯**.
1. 使用 **設定** 節，設定要在項目上使用的里程碑路徑。
1. 按一下&#x200B;**儲存**。

   將里程碑路徑與項目關聯後，可以為任務分配里程碑。

1. 前往任務，然後按一下 **更多** 圖示 ![](assets/more-icon.png)，然後 **編輯**.

   任務和里程碑之間有1:1關係。 不能將相同的里程碑附加到多個任務。 每個任務可以連結到單個里程碑，或者每個里程碑可以映射到一個任務。

1. 按一下 **設定**，然後選取 **里程碑** 欄位。
1. 按一下 **儲存**.
1. （選用）在任務清單中，新增 **狀態表徵圖** 欄，以識別哪些工作具有里程碑。

   ![](assets/amwt3.png)

1. （選用）在專案清單中，選取 **里程碑** 查看以識別里程碑任務的進度。

   ![Screen_Shot_2018-06-13_at_3.57.56_PM.png](assets/screen-shot-2018-06-13-at-3.57.56-pm-350x57.png)
