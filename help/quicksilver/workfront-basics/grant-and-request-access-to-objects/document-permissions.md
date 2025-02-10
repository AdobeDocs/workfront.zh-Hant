---
title: 共用檔案
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: 當使用者指派存取層級時，您的Adobe Workfront管理員會授予他們檢視或編輯檔案的存取權，如授予檔案存取權中所述。
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: 3bd377ba2dec29bb956632cf3e9e3e33afe4305d
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---

# 共用檔案

當使用者指派存取層級時，您的Adobe Workfront管理員會授與使用者檢視或編輯檔案的存取權，如[授與檔案的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)中所述。

Workfront管理員授予使用者的存取層級可讓他們檢視或編輯檔案。 除此之外，其他使用者還可以授予其他人許可權，讓他們檢視或管理自己上傳或有權共用的特定檔案。

許可權專屬於Workfront中的一個專案，可定義使用者可對該專案執行的動作。 如需物件許可權的相關資訊，請參閱[物件許可權共用簡介](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

依預設，將檔案上傳至Workfront的使用者擁有檔案管理許可權。

如需共用整個檔案資料夾的資訊，請參閱[共用檔案資料夾](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)。

## 關於共用檔案的考量事項

除了下列考量事項外，另請參閱[物件共用許可權概觀](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

>[!NOTE]
>
>Workfront管理員可以新增或移除系統中所有使用者的任何專案許可權，而無需擁有這些專案。

* 共用檔案類似於在Workfront中共用任何其他物件。 如需有關如何在Workfront中共用檔案的資訊，請參閱[共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。
* 您可以將下列許可權授與檔案：

   * 檢視
   * 管理

* 您也可以公開或全系統共用檔案。

  >[!CAUTION]
  >
  >建議您將包含機密資訊的物件與外部使用者共用時務必謹慎。 這可讓他們檢視資訊，而不需要身為Workfront使用者或屬於您的組織。

* 如果某人沒有Workfront帳戶，您可以在「將檔案存取權授予」欄位中新增其電子郵件地址，以與他共用檔案。
* 當您共用檔案時，使用者對所有檔案版本和所有檔案校訂都擁有相同的存取權。\
  如需Workfront中校訂的詳細資訊，請參閱[校訂](../../review-and-approve-work/proofing/proofing.md)區段。

* 您可以從檔案相關聯的物件繼承檔案的許可權。 您的Workfront管理員可以限制存取層級中檔案的許可權繼承。

  如需有關限制檔案繼承許可權的詳細資訊，請參閱[建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

  您可以手動移除檔案的繼承許可權。 如需詳細資訊，請參閱[從物件移除許可權](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* 附加的檔案只會從附加它的物件繼承許可權。 如果您在物件上建立資料夾並將檔案移至資料夾，則會繼承資料夾的許可權。 但是，如果您在父項或祖項物件上建立資料夾，並將檔案移至該資料夾，則不會繼承該資料夾的許可權。

## 檔案許可權

下表顯示當允許使用者檢視或管理檔案時，您可以授予他們哪些許可權：

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
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">編輯檔案詳細資訊</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">刪除*</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">下載</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td scope="row">簽出</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">新增核准者</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">核准檔案</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td scope="row">附加自訂表單</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">編輯自訂欄位</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移動至（物件）</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">傳送至（整合）</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">更新/評論</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td scope="row">上傳新版本</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">刪除版本</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">檢視檔案</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td scope="row">預覽</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td scope="row">證明**</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td scope="row">產生校訂**</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移除校訂**</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">共用*</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td scope="row">共用系統範圍*</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">公開共用檔案*</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">與外部電子郵件地址共用</td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td scope="row">新增/移除</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td scope="row">重新命名</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">連結（與整合）</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td scope="row">取消連結（與整合）</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;動作由檔案和檔案資料夾共用。

&#42;&#42;您必須擁有與您的Workfront帳戶相關聯的個別校訂授權，才能校訂檔案。 請聯絡您的客戶經理，瞭解如何取得校訂授權。 如需Workfront中校訂的詳細資訊，請參閱[校訂](../../review-and-approve-work/proofing/proofing.md)。
