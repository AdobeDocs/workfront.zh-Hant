---
title: 共用檔案
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: 當使用者指派存取層級時，您的Adobe Workfront管理員會授予他們檢視或編輯檔案的存取權，如授予檔案存取權中所述。
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: fcf6165c9c641316c701d92af2e39294a9fe0123
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 1%

---

# 共用檔案

當使用者指派存取層級時，您的Adobe Workfront管理員會授與使用者檢視或編輯檔案的存取權，如[授與檔案的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)中所述。

Workfront管理員授予使用者的存取層級可讓他們檢視或編輯檔案。 除此之外，其他使用者還可以授予其他人許可權，讓他們檢視或管理自己上傳或有權共用的特定檔案。

許可權專屬於Workfront中的一個專案，可定義使用者可對該專案執行的動作。 如需物件許可權的相關資訊，請參閱[物件許可權共用簡介](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

依預設，將檔案上傳至Workfront的使用者擁有檔案管理許可權。

如需共用整個檔案資料夾的資訊，請參閱[共用檔案資料夾](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能共用物件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準</p> 
   或
   <p>目前：工作或以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視您要共用之物件的存取許可權或以上許可權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視您要共用之物件的許可權或更高的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

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

## 共用檔案

{{step1-to-documents}}

1. 在&#x200B;**檔案**&#x200B;頁面上，暫留在您要共用的檔案上，然後按一下出現的&#x200B;**檔案詳細資料**&#x200B;連結。 **檔案詳細資料**&#x200B;頁面隨即開啟。

   ![檔案詳細資料連結](assets/document-details-link.png)

1. 按一下檔名稱右側的&#x200B;**更多**&#x200B;圖示![更多圖示](assets/more-icon.png)，然後按一下&#x200B;**共用**。 **共用[檔名稱]**&#x200B;對話方塊開啟。

   ![共用檔案](assets/share-a-document-350x160.png)

1. 在&#x200B;**授與檔案存取權**&#x200B;欄位中，開始輸入您要共用檔案的使用者、團隊、角色、群組或公司的名稱，然後當名稱出現在下拉式清單中時按一下該名稱。

   >[!TIP]
   >
   >您只能與作用中使用者、團隊、角色或公司共用檔案。


1. （選擇性）選取&#x200B;**誰有存取權**&#x200B;下拉式清單，並選取檔案的存取層級：

   * **只有受邀者才能存取：**&#x200B;只有受邀加入檔案的使用者才能存取（預設）。
   * **系統中的每個人都可以檢視**：系統中的所有使用者都可以在沒有邀請的情況下檢視檔案。

1. （選擇性）若要公開檔案，請按一下齒輪圖示![選取齒輪圖示](assets/gear-icon.png)，然後按一下與&#x200B;**內嵌的方塊**。 **複製公開連結**&#x200B;按鈕會出現在對話方塊底部。

1. 按一下使用者名稱右側的下拉式清單，並選取他們對於此檔案的許可權層級：

   * **檢視**：使用者可以檢閱和共用檔案。
   * **管理**：使用者擁有此程式的完整存取權，但沒有管理許可權，這些許可權是在存取層級授與的（也包含所有檢視許可權）。

1. （可選）按一下您已授與的許可權層級旁的進階選項圖示，以設定程式的特定許可權。

   ![已設定的進階許可權選項](assets/advanced-options-icon.png)

1. （選擇性）若要關閉檔案子物件的繼承許可權，請按一下&#x200B;**關閉**&#x200B;與&#x200B;**繼承許可權**&#x200B;連結。

1. （視條件而定）若要複製可讓您與外部使用者共用檔案的公用連結，請按一下&#x200B;**複製公用連結**。

   >[!CAUTION]
   >
   >建議您將包含機密資訊的檔案與外部使用者共用時務必謹慎。 這可讓他們檢視資訊，而不需要身為Workfront使用者或屬於您的組織。

1. 按一下「**儲存**」。


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
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">編輯檔案詳細資訊</td> 
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
   <td scope="row">簽出</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">新增核准者</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">核准檔案</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">附加自訂表單</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">編輯自訂欄位</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移動至（物件）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">傳送至（整合）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">更新/評論</td> 
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
   <td scope="row">檢視檔案</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">預覽</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">證明**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">產生校訂**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移除校訂**</td> 
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
   <td scope="row">公開共用檔案*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">與外部電子郵件地址共用</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">新增/移除</td> 
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
   <td scope="row">取消連結（與整合）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;動作由檔案和檔案資料夾共用。

&#42;&#42;您必須擁有與您的Workfront帳戶相關聯的個別校訂授權，才能校訂檔案。 請聯絡您的客戶經理，瞭解如何取得校訂授權。 如需Workfront中校訂的詳細資訊，請參閱[校訂](../../review-and-approve-work/proofing/proofing.md)。
