---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 建立新版本的校訂
description: 管理作品多個版本或修訂版本的意見回饋可能是一項巨大的挑戰。 Workfront可讓您建立和比較多個版本的校樣，藉此簡化此程式。
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '1734'
ht-degree: 0%

---

# 建立新版本的校訂

管理作品多個版本或修訂版本的意見回饋可能是一項巨大的挑戰。 Workfront可讓您建立和比較多個版本的校樣，藉此簡化此程式。

建立新版本的校樣時，請考慮下列資訊：

* 您可以授予使用者檢視某個版本的許可權，但不能授予另一個版本的許可權。 反之，如果您與使用者共用較新版本，除非您返回並明確授予使用者存取先前版本的許可權，否則該使用者無法看到較舊版本。
* 若要建立新版本的校訂，您必須擁有該校訂的編輯許可權。

  請參閱[在Workfront Proof中管理校訂角色](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)和[在Workfront Proof中的校訂許可權設定檔](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)，以取得誰擁有校訂編輯許可權的詳細資訊。

  如需共用校訂版本的相關資訊，請參閱  [在Workfront Proof中共用校訂](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)。

>[!IMPORTANT]
>
>如果在Adobe Workfront中建立校訂，則該校訂建立的任何新版本也必須在Workfront中建立。 如果校訂是在Workfront Proof中建立，則無法在Workfront中建立新版本的校訂。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前計畫：Pro或更高版本</p> <p>或</p> <p>舊版計畫：選擇或Premium</p> <p>如需有關不同方案的校訂存取許可權的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前計畫：工作或計畫</p> <p>舊版計畫：任何（您必須為使用者啟用校訂）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣權限設定檔 </td> 
   <td>經理或以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、角色或校訂許可權設定檔，請連絡您的Workfront或Workfront Proof管理員。

+++

## 在Workfront中建立新版本的校訂

有幾種方式可以在Workfront中上傳新的校訂版本。 預設校樣設定可能會或不會延續自上一個版本，端視您選擇的方法而定：

* **上傳檔案時自動產生校訂**：預設校訂設定不會延續。 如果您在使用者設定檔中啟用此設定，當您拖放新版本時，預設校樣設定不會延續。
* **建立校訂>簡單**：預設校訂設定不會延續。 如果您在建立新校訂版本時選擇簡單，預設校訂設定不會延續到先前的版本。
* **新增>版本>校訂**：預設校訂設定延續自上一個版本。
* **建立校訂>進階**：預設校訂設定延續自上一個版本。

  <table>
  <tbody>
  <tr>
  <td>上傳文件時自動產生憑證</td>
  <td>預設校樣設定不會延續。 如果您在使用者設定檔中啟用此設定，當您拖放新版本時，預設校樣設定不會延續。</td>
  </tr>
  <tr>
  <td>建立校訂&gt;簡單</td>
  <td>預設校樣設定不會延續。 如果您在建立新校訂版本時選擇簡單，預設校訂設定不會延續到先前的版本。</td>
  </tr>
  <tr>
  <td>新增&gt;版本&gt;校訂</td>
  <td>預設校訂設定延續自上一個版本。</td>
  </tr>
  <tr>
  <td>建立校訂&gt;進階</td>
  <td>預設校訂設定延續自上一個版本。</td>
  </tr>
  </tbody>
  </table>




若要建立新版本的校訂：

1. 開啟包含校樣的檔案清單。
1. 從電腦的檔案系統中，將新檔案拖放到校樣上。

   或

   選取列出校訂的列，按一下&#x200B;**新增** > **版本**，然後按一下您要用來新增新版本的校訂的選項。

   ![](assets/add-new-version-350x185.png)

## 從校訂檢視器建立新版本的校訂(僅限Workfront Proof)

如果您使用獨立Workfront Proof，您可以建立包含單一檔案或網頁擷取的新版校訂。 

>[!NOTE]
>
>如果您的帳戶採用Enterprise計畫，且您上傳多個檔案或網頁擷取，系統會自動將它們合併為單一新版本。 如需詳細資訊，請參閱[建立多頁校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)。

若要在Workfront Proof中建立新版本的校訂：

1. 開啟校訂。
1. 按一下左上角的&#x200B;**版本**&#x200B;下拉式功能表，然後在出現的方塊中按一下&#x200B;**+新版本**。

   在出現的&#x200B;**新校訂版**&#x200B;頁面上，您可以看到所有舊版的稽核者，包括其角色和電子郵件通知設定。 您可以在此頁面上輕鬆編輯現有稽核者的角色和通知，或從新版本中移除現有稽核者。

1. 在「**新增檔案**」下，從電腦拖放或按一下「**瀏覽**」並選取您想要的檔案，將檔案上傳為新的校訂版本。 您可以為版本輸入&#x200B;**校訂名稱**，或將此方塊留空以使用在結尾處新增版本編號的相同檔案名稱。

   或

   輸入URL以擷取網頁作為新版本的校訂。

   >[!NOTE]
   >
   >拖放功能僅適用於完全支援HTML5的瀏覽器。 這不包括Internet Explorer 7到9和Safari。

1. 在&#x200B;**工作流程**&#x200B;底下，進行下列任何變更以指定此版本校訂的稽核者。

   先前版本的稽核者會由您新增的稽核者取代。

   * 將版本的&#x200B;**所有者**&#x200B;變更為您帳戶中的其他使用者。\
     如需關於擁有者許可權的資訊，請參閱[Workfront Proof中的校訂許可權設定檔](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)。

   * 使用&#x200B;**輸入連絡人名稱或電子郵件地址來新增收件者方塊**，將稽核者新增至版本。 您可以為每個收件者指定&#x200B;**校訂角色**&#x200B;和&#x200B;**電子郵件警示**&#x200B;型別。

     如需有關將群組新增到校訂的資訊，請參閱  [將群組新增到校訂](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md)。 如需角色的相關資訊，請參閱[在Workfront Proof中管理校訂角色](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)。

     >[!NOTE]
     >
     >若的建立者或擁有者  校訂已[根據預設，校訂製作的電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)已停用（在他們的個人設定中），即使在[新校訂]頁面上勾選[透過電子郵件通知人員]方塊，他們也不會收到任何校訂或新校訂電子郵件。 如需電子郵件通知的相關資訊，請參閱[在Workfront Proof中設定電子郵件通知設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)。 另請參閱[校訂製作電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md)和[新校訂電子郵件](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md)。

   * 設定版本的校訂期限。
   * 將滑鼠停留在檢閱者的名稱上，即可檢視其在先前版本上所做的任何決定。

1. 在&#x200B;**電子郵件通知**&#x200B;底下，執行下列任一項作業：

   * 指定您是否要將新版本通知稽核者。\
     您的選擇將記錄在Proof詳細資訊頁面的活動區段。 如需詳細資訊，請參閱[在Workfront Proof中管理校訂詳細資訊](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)。

   * 新增自訂主旨和訊息。

1. 在&#x200B;**組織**&#x200B;區段中，執行下列任一項作業： 

   * 將一個或多個標籤套用到校樣。 如需詳細資訊，請參閱[在Workfront Proof中建立及管理標籤](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md)。\
     請注意，標籤也繼承自校訂的先前版本。 如果您將新標籤新增至新版本，先前的版本也會加上標籤。

   * 將版本新增至資料夾。 如需詳細資訊，請參閱[在Workfront Proof中管理資料夾](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)。 資料夾將會從舊版的校樣中複製。 如果您選取不同的資料夾，則會移動整個校訂（所有版本）。

   * 帳單管理員和管理員可在「設定」標籤上將資料夾欄位設為整個帳戶的必填欄位。 如需詳細資訊，請參閱。

1. 在「校訂設定」底下，進行以下任何變更：

   * 需要登入校訂
   * 需要在證明上以電子方式簽章（僅限企業方案）
   * 完成所有決定時鎖定校訂
   * 允許或封鎖原始檔案的下載
   * 公開共用校樣，包括公開共用設定
   * 訂閱證明\
     在此區段中進行的選取將顯示在校訂詳細資訊頁面（可以編輯某些欄位）中。 如需詳細資訊，請參閱[在Workfront Proof中管理校訂詳細資訊](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)。

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
* 取消選取「透過電子郵件通知人員」方塊，表示不會傳送任何電子郵件給稽核者，通知他們他們有要稽核的新版本。

  >[!NOTE]
  >
  >這不會受到您個人設定中儲存的任何預設自訂主旨/訊息的影響。

如果您在個人設定中儲存了預設主旨和訊息，這會影響「新版本」頁面上預設顯示的訊息：

* 如果您選擇使用標準電子郵件（例如無自訂主旨/訊息），以電子郵件方式通知檢閱者先前的校訂版本，則您的預設自訂主旨/訊息（您的個人設定）將顯示在新版本頁面上。 然後，您可以編輯自訂主旨和訊息，或取消選取「透過電子郵件通知人員」方塊（這表示不會向您的稽核者傳送電子郵件，通知他們他們有要稽核的新版本）。
* 如果您選擇不透過電子郵件通知檢閱者先前的校訂版本（例如，沒有標準或自訂電子郵件），則新版本頁面預設不會包含任何訊息。 若要將新版本通知給檢閱者，請按一下「傳送訊息」連結，此連結將顯示您的預設自訂主旨/訊息（根據您的個人設定）。 之後，您可以視需要編輯自訂主旨和訊息。

如果您未在個人設定中儲存預設主旨和訊息，下列內容將會顯示在「新版本」頁面上：

* 如果您選擇使用標準電子郵件（例如無自訂主旨/訊息），以電子郵件通知您上一個校訂版本的檢閱者，依預設將會在「新版本」頁面上選取「以電子郵件通知人員」選項。 若要新增自訂訊息，請按一下連結。
* 如果您選擇不透過電子郵件通知檢閱者先前的校訂版本（例如，沒有標準或自訂電子郵件），則新版本頁面預設不會包含任何訊息。 若要通知檢閱者新版本，請按一下「傳送訊息」連結。 然後，您可以按一下「新增自訂訊息」連結，以新增自訂主旨和訊息。
