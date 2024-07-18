---
title: 編輯使用者設定檔
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 身為Adobe Workfront管理員，您可以建立新使用者並管理現有使用者的設定檔。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: e52881a03f69d7c4d6a62dcdc9c6044f6f5dd016
workflow-type: tm+mt
source-wordcount: '3297'
ht-degree: 0%

---

# 編輯使用者設定檔

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

身為Adobe Workfront管理員，您可以建立使用者並管理現有使用者的設定檔。 如需建立使用者的詳細資訊，請參閱[新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準</p>
   或
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。 </p> </li> 
     <li> <p>您存取層級中的<b>使用者</b>物件設定為<b>編輯</b>存取，具有<b>建立</b>以及在<b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">下啟用的以下兩個<b>使用者管理員</b>選項中的至少一個。 </p> 
     <ul><li> 使用者管理 (所有使用者)</li>
     <li>管理使用者 (所有使用者)</li></ul>
     <p>如果已啟用<b>使用者管理員（群組使用者）</b>，您必須是該使用者所屬群組的群組管理員，才能編輯使用者。</p> 
     <p>如需存取層級中<b>使用者</b>設定的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

+++

## 編輯使用者設定檔

{{step-1-to-users}}

1. 選取使用者，然後按一下&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)。

   編輯使用者方塊隨即顯示。

1. 在&#x200B;**編輯使用者**&#x200B;方塊中，變更下列任何資訊，然後隨時按一下&#x200B;**儲存變更**：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">個人資訊 </td> 
      <td> 
       <ul> 
        <li><p><b>名字</b></p></li>
        <li><p><b>姓氏</b></p></li> 
        <li> <p><b>電子郵件地址：</b>使用者的電子郵件地址也是他們在Workfront的使用者名稱。 此欄位區分大小寫，且必須是唯一的。 如果有任何使用者嘗試在10分鐘視窗內新增非唯一電子郵件地址3次，就會出現reCAPTCHA回應。</p> <p> 選取<b>我不是自動機制</b>設定，然後才能繼續。</p><p>如果您使用電子郵件允許清單並輸入不在清單中的電子郵件網域，使用者將不會收到電子郵件通知。 如需允許清單的詳細資訊，請參閱<a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">設定您的電子郵件允許清單</a>。</p> </li> 
        <li> <p><b>重設密碼</b>：按一下此連結可重設使用者的密碼。 您必須先輸入自己的密碼，才能重設其他使用者的密碼。</p> <p>若要重設其他使用者的密碼，您必須是Workfront管理員或群組管理員。</p> <p><b>附註</b>：  
          <ul> 
           <li> <p>如果您是群組管理員，則只能為您指定為管理員的群組中的使用者重設密碼。 此外，您必須在存取層級中啟用「使用者管理員（群組使用者）」許可權：</p> <p> <img src="assets/group-admin-user.png" > </p> <p>此設定預設為停用。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </li> 
           <li> <p>您無法重設Workfront管理員的密碼。</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;SSO設定&gt;使用者名稱</b>：如果您的Workfront管理員已啟用Workfront的SSO整合，則SSO使用者名稱會顯示在此欄位中。 此欄位會顯示為您的Workfront執行個體啟用的SSO設定型別。 </li> 
        <li> <p><b>OnlyAllow &lt;SSO Configuration&gt;驗證</b>：如果您的Workfront管理員已啟用Workfront的SSO整合，並已更新所有SSO使用者，則預設會選取此欄位。 此欄位會顯示為您的Workfront執行個體啟用的SSO設定型別。</p> <p>選取此欄位時，使用者必須使用其SSO憑證登入Workfront。 取消核取此專案將允許他們使用其Workfront憑證登入Workfront。</p> <p>如需使用SSO解決方案設定Workfront的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Adobe Workfront單一登入概觀</a></p> <p>如需更新SSO使用者的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">更新單一登入的使用者</a>。</p> 
        <p><b>附註</b>：</p> 
        <p> 如果您是群組管理員，則只能為您指定為此類群組的使用者編輯&lt;SSO組態&gt;欄位。 此外，您必須在存取層級中啟用「使用者管理員（群組使用者）」許可權。
        <p>如果您是群組管理員，且您的存取層級中已啟用「使用者管理員（所有使用者）」許可權，您可以編輯所有使用者的&lt;SSO設定&gt;欄位。</p> </li> 
        <li><b>工作資訊：</b>工作的相關資訊，例如工作職稱（在<b>職稱</b>欄位中），以及使用者所負責的專業領域（在<b>與我談關於</b>欄位中）。</li> 
        <li><p><b>連絡資訊</b>：使用者的電話號碼(<b>電話號碼，分機。</b>和<b>手機號碼</b>欄位)和地址（在<b>地址、城市、州/省、郵遞區號、國家/地區</b>欄位中）。</p>
        <p>如果使用者已啟用統一使用者管理(UUM)或AdobeIdentity Management系統(IMS)，則連絡人資訊區段中的<b>國家/地區</b>欄位僅接受國家/地區代碼值（例如，US、GB、IN）。</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">偏好設定 </td> 
      <td> 
       <ul> 
      <li> <p><b>時區：</b>使用者的時區。</p> <p>如需有關協助使用者在Workfront中跨時區共同作業的資訊，請參閱<a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">跨時區工作</a>。</p> </li> 
       <li><b>電子郵件地區設定</b>：使用者偏好的電子郵件地區設定。 這會影響從Workfront傳送給此使用者的電子郵件中的數字和日期格式。</li>

   <li><b>接收來自此測試環境的電子郵件</b>：如果您要接收來自目前登入之環境的電子郵件通知，請核取此選項。
      <p><b>附註</b></p>
      <p>此選項僅在預覽和沙箱環境中可用。 生產環境中預設會啟用電子郵件通知。 </p>
      </li>

   </li> 
       <li><b>將我指派給自己的工作傳送給我的工作標籤</b>：如果您希望使用者指派給自己的所有內容都直接顯示在[首頁]區域的[工作]清單中，請核取此選項。 預設是在首頁區域的「準備開始」或「未就緒」清單中，列出指派給使用者的所有內容。</li> 
       <li><b>上傳檔案時自動產生校訂</b>：如果您希望使用者上傳的檔案立即產生校訂，請勾選此選項。 </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通知</td> 
      <td> <p>選取應為新使用者啟用的電子郵件通知。</p> <p>您可以選取即時和每日摘要通知。</p> <p>如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">設定系統中每個人的事件通知</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">存取</td> 
      <td> 
       <ul> 
      <li><b>作用中：</b>選取此方塊表示使用者作用中。 作用中使用者使用Workfront授權。 清除此方塊會停用使用者並防止他們登入Workfront。</li> 
       <li> <p><b>存取層級：</b>選取要指派給此使用者的存取層級。</p> 
       <p>將存取層級指派給使用者時，可以指派等於或低於您自己的存取層級的層級。</p>
       <p>例如，如果您的存取層級是「計畫」，則您無法指派「管理員」存取層級。 但是，如果Workfront管理員在存取層級上啟用非預設許可權，而您自己的存取層級中未啟用該許可權，則您不能指派預設低於您自己的存取層級的存取層級。 </p>
       <p>例如，如果您擁有無權刪除任務的「計畫」授權，儘管該「工作」授權低於「計畫」授權，但您無法指派有權刪除任務的「工作」授權給某人。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。 </p> 
       <p>如需存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">設定Adobe Workfront的存取權</a>。</p>
       <p> <b>附註：</b></p> 
       <p> 如果您的組織使用新的存取模式（標準/輕度/貢獻者），如果標準或輕度使用者已達到其當月的決策限制，則無法將該使用者重新指派給貢獻者存取層級。 </p><p>如需新存取模式的詳細資訊，請參閱<a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">新存取層級概觀</a>。 </p><p>如需決定限制的資訊，請參閱<a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">非付費使用者的有限檔案與校訂決定概覽</a>。</p></li> 
       <li> <p><b>配置範本</b>：選擇使用者的配置範本。 此配置範本優先於任何指派給使用者主群組、主團隊或主要角色的配置範本。 如需有關配置範本指派優先順序的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立和管理配置範本</a>。</p> <p><b>附註</b>：  <p>下列清單說明您在此欄位中可用的範本清單如何取決於您的存取權：</p> 
       <ul> 
       <li>身為Workfront管理員，您可以檢視所有系統層級和群組層級的版面配置範本。</li> 
       <li>身為群組管理員，您可以檢視系統層級配置範本，以及與您管理的群組相關聯的配置範本。</li> 
       <li>身為擁有計畫授權和編輯使用者存取權的使用者，您只能看到系統層級的版面配置範本。</li> 
       </ul> <p>如需群組層級配置範本的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立和管理配置範本</a>。</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">組織 </td> 
      <td> 
       <ul> 
      <li><b>公司</b>：使用者的公司。 使用者只能與一個公司相關聯。 您必須先建立公司，然後才能與使用者建立關聯。 清單中只會顯示作用中的公司。 如需有關建立公司的資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">建立和編輯公司</a>。</li> 
      <li><b>報告對象：</b>如果您為使用者指定公司，也可以在此欄位中指定使用者的直接經理。 使用者只能有一個管理員。 如果使用者沒有先與公司建立關聯，則不會顯示此欄位。 </li> 
      <li><b>直接下屬：</b>如果您為使用者指定公司，也可以指定使用者的直接下屬。 一個使用者可以有多個直接下屬。 如果使用者沒有先與公司建立關聯，則不會顯示此欄位。</li> 
      <li><b>主團隊</b>：指定使用者的主團隊。 使用者只能有一個主團隊。 在指派版面配置範本，或為指派給使用者的任務和問題定義「處理它」按鈕時，主團隊很重要。 </li> 
      <li><b>其他團隊</b>：使用者可以屬於多個團隊。 使用者可以在他們的首頁區域檢視指派給他們的任何團隊的工作專案。 </li> 
      <li> <p><b>主群組：</b>請選取適當的群組以指派使用者。 這可讓使用者存取與群組共用的物件。 您也可以和使用者的主群組共用版面範本。</p> <p>這是必填欄位。 每個使用者都必須與主群組相關聯。 如果您未選取主群組，則會將您的群組指派為新使用者的主群組。</p> <p><b>附註</b>：</p> 
      <p> 只有符合下列其中一項，您才能將群組指派給使用者：</p>
      <ul><li>您是Workfront管理員</li>
      <li>您是群組的管理員</li>
      <li>群組是公開的。</li></ul> 
      <li> <p><b>其他群組</b>：使用者可以屬於多個群組。 只有當您是Workfront管理員、您是群組管理員或群組為公用時，才能將群組指派給使用者。</p> <p><b>重要</b>：</p> 
      <p>新增使用者至超過100個群組可能會在載入群組清單的Workfront任何區域造成效能問題。</p> <p>如需公用群組的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">建立群組</a>。</p> <p>如需群組的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群組概述</a>。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">資源規劃 </td> 
      <td> 
       <ul>
       <li>
       <b>工作時間</b>：代表使用者可用於實際工作的全職相當時間(FTE)百分比，不包括額外負荷。 「工作時間」必須為最多1的小數，且不可以是0。 例如，實際工作的20%可用性為0.2。

   該欄位的預設值為1，這表示使用者將其整個FTE用於實際的、專案相關的工作。

   系統會使用此數字來計算使用者進行實際專案相關工作的可用性。

   如需有關在Workfront中建立排程的詳細資訊，請參閱<a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">建立排程</a>。

   排程例外狀況與休假也可能會影響使用者的容量。

   Workfront會根據您設定區域中的Resource Management偏好設定來計算使用者的可用性。 如需詳細資訊，請參閱<a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">設定資源管理喜好設定</a>。

   <b>提示</b>

   將「工作時間」值設為1，表示使用者可用於專案相關工作的整個全職同等工作。
   </li> 
      <li> <b>排程停用</b>：如果您要排程此使用者在特定日期和特定時間停用，請勾選此方塊。 </li> 
       <li><b>已排程的停用日期</b>：停用使用者的日期和時間。 如需排程使用者停用的相關資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>中的<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">排程使用者停用</a>。</li> 
       <li> <p><b>主要角色</b>：這是使用者可以在Workfront中完成的主要工作角色。 指派給使用者的每個任務和問題也會指派給此工作角色。 職務角色在資源管理中至關重要。 只有當您擁有具有管理使用者存取權的計畫授權，或您是Workfront管理員時，才能更新此欄位。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>。</p> <p>清單中只會顯示作用中的職位角色。 </p> </li> 
       <li>如果您選取<b>主要角色</b>，則會顯示<b>FTE可用性百分比</b>欄位。 指定將使用者排程的時間百分比分配給此工作角色。 主要角色的FTE可用性百分比預設值為100%。 </li> 
       <li> <p><b>其他角色</b>：使用者可以在Workfront中擁有多個工作角色。 職務角色在資源管理中至關重要。 使用者可以完成的工作角色數量沒有限制。 但是，我們建議不要將一位使用者指派給太多工作角色，因為這些使用者可能很難管理資源。<p>清單中只會顯示作用中的職位角色。 如需有關工作角色的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理工作角色</a>。</p> <p>只有當您擁有具有管理使用者存取權的計畫授權，或您是Workfront管理員時，才能更新此欄位。 <br>如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>。</p> </li> 
       <li> <p>（視條件而定）如果您選取一或多個<b>其他角色</b>，則會針對每個角色顯示<b>FTE可用性百分比</b>欄位。 指定將使用者排程的時間百分比分配給每個工作角色。 其他角色的FTE可用性百分比預設值為0%。</p> <p><b>注意</b>：如果其他角色具有0%的FTE可用性，除非將使用者指派給這些角色中的任務，否則它們不會顯示在「資源規劃工具」中。</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>附註</b>： <p>所有角色的所有<b>FTE可用性</b>百分比的總和必須等於100%。 每個FTE可用性的百分比會計算「資源規劃工具」中每個使用者的「可用時數」。 每個使用者每個角色的可用時數取決於使用者的可用時數。</p> <p>使用者的可用時間由Workfront根據Workfront管理員在資源管理偏好設定中計算約當全職人數時所選取的方法計算。</p> <p>如需有關計算使用者可用性的資訊，請參閱<a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">計算資源規劃工具中使用者和角色的時數和FTE的概觀</a>。</p> <p>如需有關設定資源管理偏好設定的資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">設定資源管理偏好設定</a>。</p> </p>
       <span class="preview"><p>（選擇性）如果使用者在專案期間的工作角色變更，則財務計算中會使用有效日期的工作角色指派。</p><p>按一下<b>依日期定義角色</b>，選取<b>主要角色</b>和<b>其他角色</b>，然後輸入每個角色的配置百分比。 這些角色可能與現有角色（使用不同的百分比）或新角色相同。 選取這些角色生效時的<b>開始日期</b>。 這可以是未來的日期。 當最新的角色作用中時，您可以按一下[顯示先前的角色] <b> </b>，檢視先前的非作用中角色。</p> </li></span>
       <li> <p><b>排程</b>：將排程與使用者建立關聯。 使用者的排程會計算指派給使用者的任務的時間表。</p> <p>您必須先建立排程，然後才能與使用者建立關聯。 如需建立排程的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>。</p> <p><b>注意</b>：建議您與使用者建立關聯的排程符合使用者的時區。</p> </li> 
       <li> <p><b>時程表設定檔</b>：將時程表設定檔與使用者建立關聯，以確保自動為該使用者產生時程表。</p> <p><b>注意</b>：您在此欄位中可用的設定檔清單取決於您的存取權：
       <ul>
       <li>身為Workfront管理員，您可以檢視所有系統層級和所有群組層級的時程表設定檔。</li>
       <li>作為群組管理員，您可以檢視系統層級的時程表設定檔，以及與您管理的群組相關聯的時程表設定檔。</li>
       <li>作為具有計畫授權和編輯使用者存取權的使用者，您只能看到系統層級的時程表設定檔。 如需群組層級週期性時程表的詳細資訊，請參閱<a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">建立、編輯和指派週期性時程表</a>。</li>
      </ul></p> </li> 
       <li><b>預設時數型別</b>：為使用者選取預設時數型別。 這是使用者記錄時間時，預設使用的小時型別。</li> 
       <li><b>可用時數型別</b>：選取使用者應該可用的時數型別。 這些小時型別在Workfront中任何使用者可記錄時間的位置都可見。 使用者只能看到在專案層級和使用者層級啟用的小時型別。 如需使用者可以使用哪些時數型別的詳細資訊，請參閱<a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">定義時數型別和可用性</a>。</li> 
       <li><b>登入時間：</b>選取使用者應以小時或天為單位登入工作專案。 如需詳細資訊，請參閱<a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">設定以小時或天記錄時間</a>。</li>

   <li> <b>FTE</b>：此為使用者的Full Time同等專案。 只有當系統層級的「資源管理偏好設定」設定為「預設排程」時，Workfront才會根據預設排程使用此數字來計算使用者的可用性。

   <p>FTE代表使用者可在工作上花費的時間量。 這包括管理費用，以及在專案工作上所花費的時間。 例如，在會議或培訓中花費的時間也會納入FTE。</p>

   FTE必須是最高為1的小數位數，而且不能為0。 例如，如果FTE值為0.5，而Workfront中的預設排程為40小時，則使用者每週可使用20小時。

   欄位的預設值為1。

   排程例外、休假可能以及「工作時間」的值可能會影響使用者的可用性。

   Workfront會根據您設定區域中的Resource Management偏好設定來計算使用者的可用性。

   如果系統層級的「資源管理偏好設定」設定為「使用者排程」，則您在此處指定的值會被忽略，而且會根據排程中指定的內容，將使用者視為可用。

   如需詳細資訊，請參閱<a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">設定資源管理喜好設定</a>。

   如需有關在Workfront中建立排程的詳細資訊，請參閱<a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">建立排程</a>。
   </li>

   <li><b>資源集區</b>：將使用者與資源集區建立關聯。 如需詳細資訊，請參閱<a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">將資源集區與使用者</a>關聯。</li>

   <li><b>成本費率</b>：使用者每小時的成本金額。
      <p>若要取得日期有效成本費率，請按一下[新增費率]。<strong></strong> 輸入時間期間的成本費率值，並視需要指定「開始日期」與「結束日期」。 成本費率1不會有開始日期，而最後的成本費率不會有結束日期。</p><p>部分日期會自動新增。 例如，如果「成本費率1」沒有結束日期，而您新增了開始日期為2023年5月1日的「成本費率2」，則會將結束日期為2023年4月30日的成本費率新增至「成本費率1」，因此不會出現間隙。</p></li>

   <li><b>收費率</b>：使用者每小時的收費金額。
      <p>若要取得日期有效收費率，請按一下[新增費率]。<strong></strong> 輸入時間期間的帳單費率值，並視需要指定「開始日期」與「結束日期」。 帳單費率1不會有開始日期，而最後的帳單費率不會有結束日期。</p> <p>部分日期會自動新增。 例如，如果「收費率1」沒有結束日期，而您新增了開始日期為2023年5月1日的第二個日期，則結束日期為2023年4月30日的日期會新增至「收費率1」，因此不存在間隔。</p><p> <img alt="使用者成本和收費率" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂表單</td> 
      <td><p>將現有的使用者自訂表單與此使用者建立關聯。 您必須先建立自訂表單，然後才能將其與使用者建立關聯。 清單中只會顯示作用中的自訂表單。 您無權編輯的欄位不會顯示在個別自訂表單中。</p> <p><strong>注意：</strong>進階自訂表單功能，例如外部查詢欄位和Workfront原生欄位，只有在您開啟詳細資訊頁面上的使用者記錄時，才可使用，而不是在[編輯使用者]對話方塊上。 （從使用者清單中，按一下使用者名稱以開啟詳細資訊。）</p> <p>如需建立自訂表單的相關資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref">使用表單設計工具設計表單</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">評論</td> 
      <td>輸入您要傳送給使用者的註解，以及使用者設定檔的更新區域。</td> 
     </tr> 
    </tbody> 
   </table>
