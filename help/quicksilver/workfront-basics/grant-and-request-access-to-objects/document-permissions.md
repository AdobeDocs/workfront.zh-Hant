---
title: 共用檔案
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: 您的Adobe Workfront管理員授予使用者在指派存取層級時（如授與檔案存取權一文所述）的檢視或編輯檔案存取權。
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 4%

---

# 共用檔案

您的Adobe Workfront管理員在使用者指派存取層級時，授予其檢視或編輯檔案的存取權，如 [授予對文檔的訪問權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Workfront管理員授予使用者的存取層級可讓使用者檢視或編輯檔案。 除此之外，其他用戶還可以授予其他用戶查看或管理他們上傳或有權共用的特定文檔的權限。

權限是Workfront中一個項目專屬的權限，並定義可對該項目採取的動作。 如需物件權限的相關資訊，請參閱 [對象共用權限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

依預設，將檔案上傳至Workfront的使用者擁有該檔案的「管理」權限。

有關共用整個文檔資料夾的資訊，請參見 [共用文檔資料夾](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## 共用檔案的考量事項

除了下列考量事項外，另請參閱 [對象共用權限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Workfront管理員可以為所有使用者新增或移除系統中任何項目的權限，而不是這些項目的擁有者。

* 共用檔案類似於在Workfront中共用任何其他物件。 如需如何在Workfront中共用檔案的相關資訊，請參閱 [共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* 您可以授予檔案下列權限：

   * 檢視
   * 管理

* 您也可以公開或在全系統共用檔案。

   >[!CAUTION]
   >
   >建議您在與外部使用者共用包含機密資訊的物件時，務必小心。 這可讓使用者檢視資訊，而不需要是Workfront使用者或您組織的一員。

* 您可以在「授予檔案存取權」欄位中新增其電子郵件地址，與沒有Workfront帳戶的人共用檔案。
* 當您共用文檔時，用戶對所有文檔版本和所有文檔校樣具有相同的訪問權限。\
   如需有關在Workfront中進行校對的詳細資訊，請參閱 [校對](../../review-and-approve-work/proofing/proofing.md) 區段。

* 您可以從文檔關聯的對象繼承文檔的權限。 您的Workfront管理員可以限制存取層級中檔案的權限繼承。

   有關限制對文檔繼承的權限的詳細資訊，請參見 [建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

   您可以手動移除檔案的繼承權限。 如需詳細資訊，請參閱 [從對象中刪除權限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* 附加的文檔僅繼承附加的對象的權限。 如果在對象上建立資料夾並將文檔移動到資料夾中，它會繼承資料夾的權限。 但是，如果在父或祖父對象上建立資料夾，並將文檔移入該資料夾，則不會繼承該資料夾的權限。

## 檔案權限

下表顯示了允許用戶查看或管理文檔時可以授予哪些權限：

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>動作</strong> </p> </th> 
   <th> <p><strong>管理</strong> </p> </th> 
   <th> <p><strong>檢視</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">建立</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">編輯文檔詳細資訊</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">刪除*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">下載</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">結帳</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加批准者</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">批准文檔</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">附加自訂表格</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">編輯自訂欄位</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移至（物件）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">傳送至（整合）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">更新/注釋</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">上傳新版本</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">刪除版本</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">查看文檔</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">預覽</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">校訂**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">產生證據**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移除校稿**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">共用*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">共用系統範圍*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">共用公開文件*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">與外部電子郵件地址共用</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">添加/刪除</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">重新命名</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">連結（與整合）</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">取消連結（整合）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 操作由「文檔」和「文檔資料夾」共用。

&#42;&#42; 您必須有與Workfront帳戶相關聯的獨立校對授權，才能校對檔案。 請連絡您的帳戶管理員，以取得校對授權。 如需有關在Workfront中進行校對的詳細資訊，請參閱 [校對](../../review-and-approve-work/proofing/proofing.md).
