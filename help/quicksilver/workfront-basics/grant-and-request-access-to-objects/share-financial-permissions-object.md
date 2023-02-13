---
title: 共用物件的財務權限
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: 您的Adobe Workfront管理員可在指派存取層級時，授予您檢視或編輯財務資料的存取權。 如需詳細資訊，請參閱授予金融資料的存取權。
author: Alina
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 3%

---

# 共用物件的財務權限

您的Adobe Workfront管理員可在指派存取層級時，授予您檢視或編輯財務資料的存取權。 如需詳細資訊，請參閱 [授予金融資料的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

除了授予用戶的訪問級別之外，您還可以授予他們查看或管理您有權共用的特定項目、任務或問題的財務的權限。

如需每個存取層級的使用者可以對財務資料執行哪些動作的相關資訊，請參閱區段 [財務資料](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) 在文章中 [每種物件類型皆可使用的功能](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

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
必須具備以下條件才能共用有關對象的財務資料資訊：

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
   <td> <p>查看或更高程度地訪問項目、任務、問題和財務資料</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看項目、任務和問題的權限或更高權限（至少包括查看財務權限）</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 共用物件並授予財務權限

為對象授予財務權限時，請考慮以下事項：

* 您可以將財務權限授予專案、任務和問題。
* 可繼承權限：如果您具有項目的查看財務權限，則會自動繼承項目任務和問題的查看財務權限。

要向對象授予財務權限：

1. 轉到要與他人共用的任務、項目或問題。
1. 在對象名稱附近，按一下「更多」菜單 ![](assets/more-icon.png)，然後按一下 **共用**.

1. 在 **提供 `<Object name>` 存取** 欄位開始鍵入要與其共用對象的用戶、團隊、角色、組或公司的名稱。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用物件。

1. 如果下拉式功能表出現在您選取的名稱右側，請按一下下列可用選項之一：

   * **檢視它**
   * **分配給它**
   * **管理它**

      ![](assets/12.png)      ![](assets/13.png) ![](assets/14.png)

1. 在相同的下拉式功能表中，按一下 **進階設定**，然後執行下列其中一項操作：

   * 如果您在上一步中選取了三個選項之一，請確定 **查看財務** 中所有規則的URL。
   * 如果您選取 **管理財務** 在上一步中，請確定 **管理財務** 中所有規則的URL。

1. 按一下&#x200B;**儲存**。

## 所有共用級別的財務權限

下表顯示了當您授予對象的「查看」、「貢獻」或「管理」權限時，用戶獲得的財務權限： 

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
   <td>管理計費記錄</td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>管理/查看職責開單和成本費率</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>管理/查看用戶開單和成本費率</td> 
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
   <td>在資源計畫工具中按成本查看資訊</td> 
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
   <td>在資源規劃工具中查看資源*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;需要其他資源管理訪問。

有關資源管理訪問的資訊，請參見 [授予資源管理的訪問權限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
