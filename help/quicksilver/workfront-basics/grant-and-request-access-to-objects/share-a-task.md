---
title: 共用任務
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: 您的Adobe Workfront管理員可在指派存取層級時，授予您檢視或編輯任務的存取權。 有關授予任務訪問權限的詳細資訊，請參閱授予任務訪問權限。
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 4%

---

# 共用任務

您的Adobe Workfront管理員可在指派存取層級時，授予您檢視或編輯任務的存取權。 有關授予任務訪問權限的詳細資訊，請參閱 [授予任務的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

除了授予用戶的訪問級別之外，您還可以授予他們查看、貢獻或管理您有權訪問共用的特定任務的權限。

權限是Workfront中一個項目專屬的權限，並定義可對該項目採取的動作。

## 共用任務時的考量事項

除了下列考量事項外，另請參閱 [對象共用權限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* 任務的建立者預設具有任務的「管理」權限。
* 您可以個別共用工作，也可以一次大量共用其中幾個工作。\
   共用任務與共用其他對象相同。 如需在Workfront中共用項目的詳細資訊，請參閱 [共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* 您可以授予任務下列權限： 

   * 檢視
   * 管理
   * 參與\
      ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)

* 當您共用任務時，預設情況下，用戶將繼承與任務關聯的所有子對象的相同權限。 例如，它們繼承了與任務相關聯的子任務、問題和文檔的相同權限。\
   如需Workfront中物件階層的詳細資訊，請參閱  [了解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   Workfront管理員可以指定文檔是否應繼承用戶訪問級別較高對象的權限。 有關限制對文檔繼承的權限的詳細資訊，請參見 [建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 您可以從任務中移除繼承的權限。\
   如需從物件移除繼承權限的詳細資訊，請參閱  [從對象中刪除權限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## 共用任務的方式

您可以透過下列方式共用任務：

* 個別或大量手動操作。 手動共用工作類似於在Workfront中共用任何其他物件。

   如需在Workfront中共用物件的詳細資訊，請參閱  [共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* 自動執行下列操作：

   * 指定任何任務父對象的權限：專案、方案或產品組合。 任務將繼承其父對象的權限。 有關查看對象繼承的權限的資訊，請參見 [查看對象的繼承權限](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * 在用於建立任務所在項目的模板上將實體添加到項目共用。 如需從範本共用專案的相關資訊，請參閱 [共用範本](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * 在編輯專案時，指定專案中所有工作的權限。 如需根據使用者對專案的權限管理專案任務存取權限的相關資訊，請參閱 [](../../manage-work/projects/manage-projects/edit-projects.md#access) 文章一節 [編輯專案](../../manage-work/projects/manage-projects/edit-projects.md).
   >[!TIP]
   >
   >如果未指定將用戶分配給項目任務時希望用戶擁有的任務權限，預設情況下，這些用戶將獲得與其在項目上擁有的相同權限。

## 任務權限

下表顯示了在允許用戶查看、貢獻或管理任務時可以授予的權限：

<table border="2" cellspacing="15" cellpadding="1"> 
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
   <td scope="row">添加任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加前置任務</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加問題</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">刪除任務</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>一般任務編輯<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">更改任務狀態</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">編輯任務約束</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">檢視任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">添加文檔</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">複製任務*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">移動任務*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">記錄時數</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">修改計畫日期</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">接受分配</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">進行指派</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">附加自訂表格</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">編輯自訂欄位</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">建立核准流程</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">核准任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">編輯財務*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加/編輯費用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">檢視財務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">更新/注釋</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">共用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">共用系統範圍</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;由專案的存取層級和權限控制。
