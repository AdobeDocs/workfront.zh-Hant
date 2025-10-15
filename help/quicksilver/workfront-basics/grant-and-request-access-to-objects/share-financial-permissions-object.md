---
title: 共用物件的財務許可權
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: 指派存取層級時，您的Adobe Workfront管理員可授予您檢視或編輯財務資料的存取權。 如需詳細資訊，請參閱授予財務資料的存取權。
author: Alina
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# 共用物件的財務許可權

指派存取層級時，您的Adobe Workfront管理員可授予您檢視或編輯財務資料的存取權。 如需詳細資訊，請參閱[授予財務資料的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

除了授予使用者的存取層級之外，您還可以授予他們檢視或管理您有權共用之特定專案、任務或問題的財務的許可權。

如需有關每個存取層級中的使用者可以對財務資料執行哪些操作的資訊，請參閱文章[每個物件型別可用的功能](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia)中的[財務資料](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)小節。

## 存取需求

<!--drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial&nbsp;Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> 
   <p>規劃</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視專案、任務、問題和財務資料的或更高存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案、任務和問題的許可權或以上包括至少檢視財務許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共用物件並授與財務許可權

將財務許可權授與物件時，請考量下列事項：

* 您可以授予專案、任務和問題的財務許可權。
* 許可權可繼承：如果您擁有專案的檢視財務許可權，您則會自動繼承專案上任務和問題的檢視財務許可權。

若要授與物件的財務許可權：

1. 前往您要與他人共用的任務、專案或問題。
1. 在物件名稱附近，按一下[更多]功能表![](assets/more-icon.png)，然後按一下[共用]****。

1. 在&#x200B;**將`<Object name>`存取權授予**&#x200B;欄位中，開始輸入您要共用物件的使用者、團隊、角色、群組或公司的名稱。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用物件。

1. 如果您選取的名稱右側出現下拉式功能表，請按一下下列其中一個可用選項：

   * **檢視它**
   * **協助撰寫**
   * **管理它**

1. 在同一個下拉式功能表中，按一下&#x200B;**進階設定**，然後執行下列其中一項作業：

   * 如果您在上一個步驟中選取了三個選項之一，請確定已選取&#x200B;**檢視財務**。
   * 如果您在上一個步驟中選取&#x200B;**管理財務**，請確定已選取&#x200B;**管理財務**。

1. 按一下「**儲存**」。

## 所有共用層級的財務許可權

下表顯示當您將物件的「檢視」、「貢獻」或「管理」許可權授與使用者時，他們可獲得的財務許可權： 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>動作</strong> </th> 
   <th><strong>管理</strong> </th> 
   <th><strong>貢獻</strong> </th> 
   <th><strong>檢視</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>管理付費記錄</td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>管理/檢視角色帳單與成本費率</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>管理/檢視使用者帳單與成本費率</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>檢視財務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td>在資源計畫工具中依成本檢視資訊</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>資源規劃工具中的預算資源*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>在「資源規劃」工具中檢視資源*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;需要額外的資源管理存取權。

如需有關資源管理存取許可權的資訊，請參閱[授予資源管理的存取許可權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)。
