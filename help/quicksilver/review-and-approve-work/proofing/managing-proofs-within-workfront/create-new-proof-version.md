---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 建立校樣的新版本
description: 管理作品的多個版本或修訂版本之間的意見反應可能是一項巨大的挑戰。 Workfront可讓您建立和比較多個版本的校樣，以簡化此程式。
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1721'
ht-degree: 0%

---

# 建立校樣的新版本

管理作品的多個版本或修訂版本之間的意見反應可能是一項巨大的挑戰。 Workfront可讓您建立和比較多個版本的校樣，以簡化此程式。

建立新版校樣時，請考量下列資訊：

* 您可以授予使用者權限，讓使用者可以查看某個版本，但不能查看其他版本。 反之，如果您與使用者共用較新版本，該使用者將看不到較舊版本，除非您返回並明確授予該使用者對這些舊版本的存取權。
* 若要建立校樣的新版本，您必須對校樣具有編輯權限。

   請參閱 [在Workfront校樣中管理校樣角色](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) 和 [Workfront Proof中的校樣權限設定檔](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 以取得關於誰對校樣具有編輯權限的詳細資訊。

   如需共用校樣版本的相關資訊，請參閱  [在Workfront校樣中共用校樣](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>如果在Adobe Workfront中建立校樣，則必須為該校樣建立的任何新版本也必須在Workfront中建立。 如果校樣是在Workfront內建立，則無法在Workfront內建立新版校樣。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Select或Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>管理員或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 在Workfront中建立校樣的新版本

在Workfront中上傳新校樣版本有數種方式。 預設校樣設定可能延續至舊版，也可能不延續至舊版，端視您選擇的方法而定：

* **上傳檔案時自動產生校樣**:預設校樣設定不會繼續。 如果您在使用者設定檔中啟用了此設定，當您拖放新版本時，預設校樣設定不會持續存在。
* **建立校樣>簡單**:預設校樣設定不會繼續。 如果您在建立新校樣版本時選擇「簡單」，則預設校樣設定不會延續於舊版。
* **新增>版本>校樣**:預設校樣設定會延續至舊版。
* **建立校樣>進階**:預設校樣設定會延續至舊版。

   <table>
  <tbody>
  <tr>
  <td>上傳文件時自動產生憑證</td>
  <td>預設校樣設定不會繼續。 如果您在使用者設定檔中啟用了此設定，當您拖放新版本時，預設校樣設定不會持續存在。</td>
  </tr>
  <tr>
  <td>建立校樣&gt;簡單</td>
  <td>預設校樣設定不會繼續。 如果您在建立新校樣版本時選擇「簡單」，則預設校樣設定不會延續於舊版。</td>
  </tr>
  <tr>
  <td>新增&gt;版本&gt;校樣</td>
  <td>預設校樣設定會延續至舊版。</td>
  </tr>
  <tr>
  <td>建立校樣&gt;進階</td>
  <td>預設校樣設定會延續至舊版。</td>
  </tr>
  </tbody>
  </table>




要建立校樣的新版本：

1. 開啟包含校樣的文檔清單。
1. 從電腦的檔案系統中，將新檔案拖放到校樣上。

   或

   選取校樣列出的列，按一下 **新增** > **版本**，然後按一下您要用來新增校樣新版本的選項。

   ![](assets/add-new-version-350x185.png)

## 從校對檢視器建立校樣的新版本(僅限Workfront Proof)

如果您使用獨立Workfront校樣，則可建立包含單一檔案或Web擷取的校樣的新版本。 

>[!NOTE]
>
>如果您的帳戶位於企業計畫中，而您上傳了多個檔案或網路擷取，則這些檔案會自動合併為單一新版本。 請參閱 [建立多頁校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) 以取得更多資訊。

若要在Workfront校樣中建立新版校樣：

1. 開啟校樣。
1. 按一下 **版本** 左上角的下拉式功能表，然後按一下 **+新版本** 框中。

   在 **新的校樣版本** 顯示的頁面中，您可以查看上一版本的所有審閱者，包括其角色和電子郵件通知設定。 您可以輕鬆編輯現有審閱者的角色和通知，或從此頁的新版本中刪除現有審閱者。

1. 在 **新增檔案**，從電腦拖放或按一下，即可上傳檔案作為新版校樣 **瀏覽** 並選取您想要的檔案。 您可以輸入 **校樣名稱** 對於版本，或將此框留空，以使用與結尾添加的版本號相同的檔案名。

   或

   輸入URL，將網頁擷取為新版校樣。

   >[!NOTE]
   >
   >拖放功能僅適用於完全支援HTML5的瀏覽器。 這不包括Internet Explorer 7至9和Safari。

1. 在 **工作流程**，請進行下列任一變更，以指定此版本校樣的審核者。

   以前版本的審閱者將被添加的審閱者替換。

   * 變更 **擁有者** 版本傳送給帳戶中的其他使用者。\
      有關所有者權限的資訊，請參閱 [Workfront Proof中的校樣權限設定檔](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * 使用 **鍵入聯繫人姓名或電子郵件地址以添加收件人框**，將審核者新增至版本。 您可以指定 **證明角色** 和 **電子郵件警報** 為每個收件者輸入。

      如需將群組新增至校樣的資訊，請參閱  [新增群組至校樣](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md). 如需角色的相關資訊，請參閱 [在Workfront校樣中管理校樣角色](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      >[!NOTE]
      >
      >如果校樣的建立者或擁有者 [校樣製作的電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) 預設為停用（在其個人設定中），即使「新校樣」頁面上已勾選「透過電子郵件通知人員」方塊，他們也不會收到任何製作的校樣或新校樣電子郵件。 如需電子郵件通知的詳細資訊，請參閱 [在Workfront Proof中設定電子郵件通知設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md). 另請參閱 [校樣製作的電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) 和 [新校樣電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * 設定版本的校樣截止日期。
   * 將滑鼠指標暫留在審核者的名稱上，即可查看他/她對舊版所做的任何決定。

1. 在 **電子郵件通知**，執行下列任一操作：

   * 指定是否要通知審閱者新版本。\
      您的選取項目將記錄在校樣詳細資料頁面的「活動」區段中。 如需詳細資訊，請參閱 [在Workfront校樣中管理校樣詳細資料](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * 新增自訂主旨和訊息。

1. 在 **組織** ，請執行下列任一操作： 

   * 套用一或多個標籤至校樣。 如需詳細資訊，請參閱 [在Workfront校樣中建立和管理標籤](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md).\
      請注意，標籤也繼承自舊版校樣。 如果您將新標籤新增至新版本，舊版也會加上標籤。

   * 將版本新增至資料夾。 請參閱 [在Workfront校樣中管理資料夾](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) 以取得更多資訊。 資料夾將從舊版校樣複製。 如果您選取不同的資料夾，則會移動整個校樣（所有版本）。

   * 帳單管理員和管理員可在「設定」標籤的整個帳戶中，將資料夾欄位設為必填欄位。 如需詳細資訊，請參閱。

1. 在「校樣」設定下，進行下列任何變更：

   * 需要登錄校樣
   * 校樣上需要電子簽名（僅限企業計畫）
   * 做出所有決定時鎖定證明
   * 允許或阻止下載原始檔案
   * 公開分享校樣，包括公開分享設定
   * 訂閱校樣\
      在此區段中所做的選取將顯示在「校樣詳細資訊」頁面中（可在其中編輯某些欄位）。 如需詳細資訊，請參閱 [在Workfront校樣中管理校樣詳細資料](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create a new version of a proof from the proofing viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new version from the proofing viewer</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof.</li>
<li value="2"> <p>Click the <strong>Version</strong> drop-down menu in the upper-left corner, then click <strong>+ New version</strong> in the box that appears.</p> <p>On the <strong>New proof version of</strong> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li>
<li value="3"> <p>Under <strong>Add files</strong>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <strong>browse</strong> and selecting the file you want. You can type a&nbsp;<strong>Proof name</strong>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
<br>
</note> </li>
<li value="4"> <p>Under <strong>Workflow</strong>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p>
<ul>
<li>Change the <strong>Owner</strong> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li>
<li> <p>Using the <strong>Type contact name or email address to add a recipient box</strong>, add reviewers to the version. You can specify a <strong>Proof role</strong> and an <strong>Email alerts</strong> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
If the creator or owner of&nbsp;&nbsp;the proof has
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see
<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
<br>
</note> </li>
<li>Set a proof deadline for the version.</li>
<li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li>
</ul> </li>
<li value="5">Under <strong>Email notification</strong>, do any of the following:
<ul>
<li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Proof activity section on the Proof details page.</li>
<li>Add a custom subject and message.</li>
</ul></li>
<li value="6">Under Proof settings, make any of the changes below:
<ul>
<li>Require login on the proof</li>
<li>Require electronic signatures on the proof (Enterprise plan only)</li>
<li>Lock the proof when all decisions are made</li>
<li>Allow or block download of original file</li>
<li>Public sharing of the proof,&nbsp;including public sharing settings</li>
<li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page.</li>
</ul></li>
</ol>
-->

## 關於新版本訊息

如果舊版校樣中包含自訂主旨/訊息，則預設會顯示在新版本頁面上。 您可以：

* 編輯主旨和訊息。
* 取消選取「以電子郵件通知人員」方塊，表示不會傳送任何電子郵件給審核者，通知他們有要審核的新版本。

   >[!NOTE]
    這不受您個人設定中儲存的任何預設自訂主旨/訊息影響。

如果您的個人設定中有儲存的預設主旨和訊息，這會影響「新版本」頁面上預設顯示的訊息：

* 如果您選擇使用標準電子郵件（例如，無自訂主旨/訊息），透過電子郵件通知審核者上一版校樣（例如，無自訂主旨/訊息），您的預設自訂主旨/訊息（您的個人設定）會顯示在「新版」頁面上。 然後，您可以編輯自訂主旨和訊息，或取消選取「透過電子郵件通知人員」方塊（這表示不會傳送任何電子郵件給審核者，通知他們有要審核的新版本）。
* 如果您選擇不以電子郵件通知審核者校樣的舊版（例如，沒有標準或自訂電子郵件），則新版本頁面預設不會包含任何訊息。 若要通知審核者新版本，請按一下「傳送訊息」連結，該連結會顯示您的預設自訂主旨/訊息（根據您的個人設定）。 接著，您就可以視需要編輯自訂主旨和訊息。

如果您的個人設定中未儲存預設主旨和訊息，則下列項目會顯示在「新版本」頁面上：

* 如果您選擇使用標準電子郵件（例如，無自訂主旨/訊息），透過電子郵件通知審核者上一版校樣，則「新版本」頁面會預設選取「透過電子郵件通知人員」選項。 若要新增自訂訊息，請按一下連結。
* 如果您選擇不以電子郵件通知審核者校樣的舊版（例如，沒有標準或自訂電子郵件），則新版本頁面預設不會包含任何訊息。 若要通知審核者新版本，請按一下「傳送訊息」連結。 然後，您可以按一下「新增自訂訊息」連結，以新增自訂主旨和訊息。
