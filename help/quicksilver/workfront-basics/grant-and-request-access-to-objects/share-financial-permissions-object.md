---
title: 共用物件的財務許可權
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: 指派存取層級時，您的Adobe Workfront管理員可授予您檢視或編輯財務資料的存取權。 如需詳細資訊，請參閱授予財務資料的存取權。
author: Alina
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 3%

---

# 共用物件的財務許可權

{{highlighted-preview}}

指派存取層級時，您的Adobe Workfront管理員可授予您檢視或編輯財務資料的存取權。 如需詳細資訊，請參閱 [授予財務資料的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

除了授予使用者的存取層級之外，您還可以授予他們檢視或管理您有權共用之特定專案、任務或問題的財務的許可權。

如需各個存取層級的使用者可處理財務資料的相關資訊，請參閱區段 [財務資料](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) 在文章中 [適用於每種物件型別的功能](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

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
您必須具備下列專案才能共用物件的財務資料資訊：

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視專案、任務、問題和財務資料的存取權或更高的存取權</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視至少包含檢視財務許可權的專案、任務和問題的許可權或更高</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 共用物件並授予財務許可權

授與物件的財務許可權時，請考量下列事項：

* 您可以授予專案、任務、問題等財務許可權， <span class="preview">和費率卡</span>.
* 許可權可以繼承：如果您擁有專案的檢視財務許可權，您會自動繼承專案上任務和問題的檢視財務許可權。

若要授與物件的財務許可權：

1. 前往您要與他人共用的任務、專案或問題。
1. 在物件名稱附近，按一下「更多」選單 ![](assets/more-icon.png)，然後按一下 **共用**.

1. 在 **授予 `<Object name>` 存取** 欄位開始輸入您要共用物件的使用者、團隊、角色、群組或公司的名稱。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用物件。

1. 如果您選取的名稱右側出現下拉式功能表，請按一下下列其中一個可用選項：

   * **檢視它**
   * **分配給它**
   * **管理它**

     ![](assets/12.png)      ![](assets/13.png) ![](assets/14.png)

1. 在同一下拉式功能表中，按一下 **進階設定**，然後執行下列任一項作業：

   * 如果您在上一個步驟中選取了三個選項之一，請確定 **檢視財務** 「 」已選取。
   * 如果您已選取 **管理財務** 在上一步中，確認 **管理財務** 「 」已選取。

1. 按一下&#x200B;**儲存**。

## 所有共用層級的財務許可權

下表顯示當您將物件的「檢視」、「貢獻」或「管理」許可權授與使用者時，他們獲得的財務許可權： 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>動作</strong> </th> 
   <th><strong>管理</strong> </th> 
   <th><strong>參與</strong> </th> 
   <th><strong>檢視</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>管理付費記錄</td> 
   <td>✓ (N)</td> 
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
   <td><span class="preview">管理費率卡</span></td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span class="preview">檢視費率卡</span></td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr>
  <tr> 
   <td>在「資源計畫」工具中依「成本」檢視資訊</td> 
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
   <td>檢視資源計畫工具中的資源*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;需要其他資源管理存取權。

如需有關「資源管理」存取許可權的資訊，請參閱 [授予對資源管理的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
