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
source-git-commit: de7432c66d9d71a4c1b0b4b6c43b306d0fae9fef
workflow-type: tm+mt
source-wordcount: '3425'
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

如需使用者更新自己設定檔的詳細資訊，請參閱[設定我的設定](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td><p>新增：標準</p><p>或</p><p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 </li> 
     <li> <p>您的存取層級中的<b>使用者</b>設定已設定為<b>編輯</b>存取權，其中<b>建立</b>以及在<b>微調您的設定</b> <b>下啟用的兩個</b>使用者管理員<img src="assets/gear-icon-in-access-levels.png">選項中的至少一個。 </p> <p>在這兩個選項中，如果已啟用<b>使用者管理員（群組使用者）</b>，您必須是使用者所屬群組的群組管理員。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 編輯使用者設定檔

{{step-1-to-users}}

1. 選取使用者，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

   編輯使用者方塊隨即顯示。

1. 在&#x200B;**編輯使用者**&#x200B;方塊中，變更任何區段中的資訊，然後隨時按一下&#x200B;**儲存**。

### 個人資訊

* **名字**
* **姓氏**

  >[!NOTE]
  >
  >在Workfront中編輯使用者名稱不會在Adobe Admin Console中編輯使用者名稱。

* **電子郵件地址**：使用者的電子郵件地址也是他們在Workfront的使用者名稱。 此欄位區分大小寫，且必須是唯一的。 如果有任何使用者嘗試在10分鐘視窗內新增非唯一電子郵件地址3次，就會出現reCAPTCHA回應。

  選取&#x200B;**我不是自動機制**&#x200B;設定，然後才能繼續。

  如果您使用電子郵件允許清單並輸入不在清單中的電子郵件網域，使用者將不會收到電子郵件通知。 如需允許清單的詳細資訊，請參閱[設定您的電子郵件允許清單](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)。

  如果您的組織已移轉至Adobe Admin Console，您便無法在Workfront中編輯使用者的電子郵件地址。 使用者的電子郵件地址是在Adobe Admin Console中設定。

* **變更密碼**：按一下此按鈕，重設使用者的密碼。 您必須先輸入自己的密碼，才能重設其他使用者的密碼。

  若要重設其他使用者的密碼，您必須是Workfront管理員或群組管理員。

  如果您是群組管理員，則只能為您指定為管理員的群組中的使用者重設密碼。 此外，您必須在存取層級中啟用「使用者管理員（群組使用者）」許可權：

  ![使用者管理員存取層級設定](assets/group-admin-user.png)

  此設定預設為停用。 如需詳細資訊，請參閱[建立或修改自訂存取層級](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

  您無法重設Workfront管理員的密碼。

* **&lt;SSO設定>使用者名稱**：如果您的Workfront管理員已啟用Workfront的SSO整合，則SSO使用者名稱會顯示在此欄位中。 此欄位會顯示為您的Workfront執行個體啟用的SSO設定型別。
* **OnlyAllow &lt;SSO Configuration>驗證**：如果您的Workfront管理員已啟用Workfront的SSO整合，並已更新所有SSO使用者，則預設會選取此欄位。 此欄位會顯示為您的Workfront執行個體啟用的SSO設定型別。

  選取此欄位時，使用者必須使用其SSO憑證登入Workfront。 取消核取此專案將允許他們使用其Workfront憑證登入Workfront。

  如需使用SSO解決方案設定Workfront的詳細資訊，請參閱[Adobe Workfront單一登入概觀](/help/quicksilver/administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)。

  如需更新SSO使用者的詳細資訊，請參閱[更新單一登入的使用者](/help/quicksilver/administration-and-setup/add-users/single-sign-on/update-users-sso.md)。

  >[!NOTE]
  >
  >如果您是群組管理員，則只能為您指定為此類群組的使用者編輯&lt;SSO組態>欄位。 此外，您必須在存取層級中啟用「使用者管理員（群組使用者）」許可權。
  >
  >如果您是群組管理員，且您的存取層級中已啟用「使用者管理員（所有使用者）」許可權，您可以編輯所有使用者的&lt;SSO設定>欄位。

* **設定檔像片**：按一下&#x200B;**上傳新像片**&#x200B;以載入使用者的設定檔像片。 您可以上傳JPG、GIF或PNG檔案。 檔案大小限製為4 MB。

  個人資料圖片會成為使用者的頭像，且無論使用者名稱在何處顯示，都可在整個Workfront系統中看到。

* **工作資訊**：工作的相關資訊，例如工作職稱（在&#x200B;**職稱**&#x200B;欄位中），以及使用者所負責的專業領域（在&#x200B;**與我談關於**&#x200B;欄位中）。
* **連絡資訊**：使用者的電話號碼(**電話號碼**，**分機。**&#x200B;和&#x200B;**手機號碼**&#x200B;欄位)和地址（在&#x200B;**地址**、**城市**、**州**、**郵遞區號**&#x200B;和&#x200B;**國家**&#x200B;欄位中）。

  如果使用者已啟用統一使用者管理(UUM)或Adobe Identity Management系統(IMS)，則連絡人資訊區段中的&#x200B;**國家/地區**&#x200B;欄位僅接受國家/地區代碼值（例如，US、GB、IN）。

### 偏好設定

* **時區**：使用者的時區。

  如需有關協助使用者在Workfront中跨時區共同作業的資訊，請參閱[跨時區工作](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)。

* **電子郵件地區設定**：使用者偏好的電子郵件地區設定。 這會影響從Workfront傳送給此使用者的電子郵件中的數字和日期格式。

  >[!NOTE]
  >
  >當您的組織使用Adobe統一體驗時，使用者的語言偏好設定會儲存在其Adobe設定檔中，而不使用電子郵件地區設定。 如需有關存取這些偏好設定的資訊，請參閱[Workfront的Adobe Unified Experience ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

* **接收來自此測試環境的電子郵件**：如果您要接收來自目前登入之環境的電子郵件通知，請核取此選項。

  >[!NOTE]
  >
  >此選項僅在預覽和沙箱環境中可用。 生產環境中預設會啟用電子郵件通知。

<!--* **Automatically set the task status to In Progress when tasks are self-assigned**: When this option is selected, work that the user self-assigns is automatically set to In Progress status instead of New.-->

* **將我指派給自己的工作傳送到[正在處理]索引標籤**：選取此選項時，使用者自行指派的工作會自動設定為[進行中]狀態，而非[新增]。<!--This setting refers to a deprecated feature that has been removed from Workfront.-->

* **上傳檔案時自動產生校訂**：如果您希望使用者上傳的檔案立即產生校訂，請勾選此選項。

### 通知

選取應該為新使用者啟用的電子郵件通知。

您可以選取即時和每日摘要通知。

如需詳細資訊，請參閱[設定系統中每個人的事件通知](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

### 存取

* **使用者處於作用中狀態**：啟用此選項以表示使用者處於作用中狀態。 作用中使用者使用Workfront授權。 停用欄位會停用使用者並防止他們登入Workfront。

* **存取層級**：選取要指派給此使用者的存取層級。

  將存取層級指派給使用者時，可以指派等於或低於您自己的存取層級的層級。 （例如，如果您的存取層級為「標準」，則無法指派「管理員」存取層級。）

  但是，如果Workfront管理員在存取層級上啟用非預設許可權，而您自己的存取層級中未啟用該許可權，則您不能指派預設低於您自己的存取層級的存取層級。

  例如，如果您擁有無權刪除任務的Standard授權，則無法將有權刪除任務的Light授權指派給某人，儘管Light授權低於Standard授權。 如需詳細資訊，請參閱[建立或修改自訂存取層級](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

  如需存取層級的詳細資訊，請參閱[設定Adobe Workfront的存取權](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md)。

  >[!NOTE]
  >
  >如果您的組織使用新的存取模式（標準/輕度/貢獻者），如果標準或輕度使用者已達到其當月的決策限制，則無法將該使用者重新指派給貢獻者存取層級。
  >
  >如需新存取模式的詳細資訊，請參閱[新存取層級概觀](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)。
  >
  >如需決定限制的資訊，請參閱[非付費使用者的有限檔案與校訂決定概覽](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)。

* **配置範本**：選擇使用者的配置範本。 此配置範本優先於任何指派給使用者主群組、主團隊或主要角色的配置範本。 如需配置範本的指派優先順序的詳細資訊，請參閱[建立和管理配置範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

  下列清單說明您在此欄位中可用的範本清單如何取決於您的存取權：

   * 身為Workfront管理員，您可以檢視所有系統層級和群組層級的版面配置範本。
   * 身為群組管理員，您可以檢視系統層級配置範本，以及與您管理的群組相關聯的配置範本。
   * 作為具有Standard或Plan授權並擁有編輯使用者存取權的使用者，您只能看到系統層級的版面配置範本。

     如需群組層級配置範本的詳細資訊，請參閱[建立和修改群組的配置範本](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

### 組織

* **公司**：使用者的公司。 使用者只能與一個公司相關聯。 您必須先建立公司，然後才能與使用者建立關聯。 清單中只會顯示作用中的公司。 如需有關建立公司的資訊，請參閱[建立和編輯公司](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。
* **報告給**：如果您為使用者指定了公司，也可以在此欄位中指定使用者的直接經理。 使用者只能有一個管理員。 如果使用者沒有先與公司建立關聯，則不會顯示此欄位。
* **直接下屬**：如果您為使用者指定公司，也可以指定使用者的直接下屬。 一個使用者可以有多個直接下屬。 如果使用者沒有先與公司建立關聯，則不會顯示此欄位。
* **主團隊**：指定使用者的主團隊。 使用者只能有一個主團隊。 在指派版面配置範本，或為指派給使用者的任務和問題定義「處理它」按鈕時，主團隊很重要。
* **其他團隊**：使用者可以屬於多個團隊。 使用者可以在他們的首頁區域檢視指派給他們的任何團隊的工作專案。
* **目前主群組**：選取適當的群組以指派使用者。 這可讓使用者存取與群組共用的物件。 您也可以和使用者的主群組共用版面範本。

  這是必填欄位。 每個使用者都必須與主群組相關聯。 如果您未選取主群組，則會將您的主群組指派為新使用者的主群組。

  只有符合下列其中一項，您才能將群組指派給使用者：

   * 您是Workfront管理員
   * 您是群組的管理員
   * 群組是公開的

* **其他群組**：使用者可以屬於多個群組。 只有當您是Workfront管理員、您是群組管理員或群組為公用時，才能將群組指派給使用者。

  >[!IMPORTANT]
  >
  >新增使用者至超過100個群組可能會在載入群組清單的Workfront任何區域造成效能問題。

  如需公用群組的詳細資訊，請參閱[建立群組](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)。

  如需群組的詳細資訊，請參閱[群組概述](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md)。

### 資源規劃

* **工作時間**：代表使用者可用於實際工作的全職相當時間(FTE)百分比，不包括額外負荷。 「工作時間」必須為最多1的小數，且不可以是0。 例如，實際工作的20%可用性為0.2。

  該欄位的預設值為1，這表示使用者將其整個FTE用於實際的、專案相關的工作。

  系統會使用此數字來計算使用者進行實際專案相關工作的可用性。

  如需有關在Workfront中建立排程的詳細資訊，請參閱[建立排程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

  排程例外狀況與休假也可能會影響使用者的容量。

  Workfront會根據您設定區域中的Resource Management偏好設定來計算使用者的可用性。 如需詳細資訊，請參閱[設定資源管理喜好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

  >[!TIP]
  >
  >將「工作時間」值設為1，表示使用者可用於專案相關工作的整個全職同等工作。

* **設定停用日期**：如果您要排程此使用者在特定日期與特定時間停用，請按一下此按鈕。
* **停用日期**：停用使用者的日期和時間。 如需排程使用者停用的相關資訊，請參閱[停用或重新啟用使用者](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation)中的[排程使用者停用](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。
* **主要角色**：這是使用者可以在Workfront中完成的主要工作角色。 指派給使用者的每個任務和問題也會指派給此工作角色。 職務角色在資源管理中至關重要。 只有在您擁有具有管理使用者存取許可權的「標準」或「計畫」授權，或者您是Workfront管理員時，才能更新此欄位。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱[授予使用者存取許可權](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

  清單中只會顯示作用中的職位角色。

* （視條件而定）如果您選取&#x200B;**主要角色**，則會顯示&#x200B;**FTE可用性百分比**&#x200B;欄位。 指定將使用者排程的時間百分比分配給此工作角色。 主要角色的FTE可用性百分比預設值為100%。
* **其他角色**：使用者可以在Workfront中擁有多個工作角色。 職務角色在資源管理中至關重要。 使用者可以完成的工作角色數量沒有限制。 但是，我們建議不要將一位使用者指派給太多工作角色，因為這些使用者可能很難管理資源。

  清單中只會顯示作用中的職位角色。 如需有關工作角色的詳細資訊，請參閱[建立和管理工作角色](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

  只有在您擁有具有管理使用者存取許可權的「標準」或「計畫」授權，或者您是Workfront管理員時，才能更新此欄位。

  如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱[授予使用者存取許可權](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

* （視條件而定）如果您選取一或多個&#x200B;**其他角色**，則會針對每個角色顯示&#x200B;**FTE可用性百分比**&#x200B;欄位。 指定將使用者排程的時間百分比分配給每個工作角色。 其他角色的FTE可用性百分比預設值為0%。

  如果「其他角色」具有0%的FTE可用性，除非將使用者指派給這些角色中的任務，否則它們不會顯示在「資源規劃工具」中。

  ![使用者角色和FTE](assets/user-roles-fte-2025.png)

  所有角色的所有&#x200B;**FTE可用性**&#x200B;百分比的總和必須等於100%。 每個FTE可用性的百分比會計算「資源規劃工具」中每個使用者的「可用時數」。 每個使用者每個角色的可用時數取決於使用者的可用時數。

  使用者的可用時間由Workfront根據Workfront管理員在資源管理偏好設定中計算約當全職人數時所選取的方法計算。

  如需有關計算使用者可用性的資訊，請參閱[計算資源規劃工具中使用者和角色的時數和FTE的概觀](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)。

  如需有關設定資源管理偏好設定的資訊，請參閱[設定資源管理偏好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

  <span class="preview"> （選擇性）如果使用者在專案期間的工作角色變更，則財務計算中會使用生效日期的工作角色指派。</span>

  <span class="preview">按一下&#x200B;**依日期定義角色**，選取&#x200B;**主要角色**&#x200B;和&#x200B;**其他角色**，然後輸入每個角色的配置百分比。 這些角色可能與現有角色（使用不同的百分比）或新角色相同。 選取這些角色生效時的「開始」日期。 這可以是未來的日期。 當最新的角色作用中時，您可以按一下[顯示先前的角色]&#x200B;**&#x200B;**，檢視先前的非作用中角色。</span>

* **排程**：將排程與使用者建立關聯。 使用者的排程會計算指派給使用者的任務的時間表。

  您必須先建立排程，然後才能與使用者建立關聯。 如需建立排程的詳細資訊，請參閱[建立排程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

  >[!NOTE]
  >
  >我們建議您與使用者建立關聯的排程符合使用者的時區。

  >[!IMPORTANT]
  >
  >只有在&#x200B;**使用來計算資源可用性**&#x200B;設定設為&#x200B;**使用者的排程**&#x200B;時，Workfront才會使用使用者的排程。 如需此設定如何影響用於資源管理的排程的詳細資訊，請參閱[設定資源管理喜好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

* **時程表設定檔**：將時程表設定檔與使用者建立關聯，以確保自動為該使用者產生時程表。

  您在此欄位中可用的設定檔清單取決於您的存取權：

   * 身為Workfront管理員，您可以檢視所有系統層級和所有群組層級的時程表設定檔。
   * 作為群組管理員，您可以檢視系統層級的時程表設定檔，以及與您管理的群組相關聯的時程表設定檔。
   * 作為具有標準或計畫授權並存取許可權以編輯使用者的使用者，您只能看到系統層級的時程表設定檔。 如需群組層級週期性時程表的詳細資訊，請參閱[建立、編輯和指派週期性時程表](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

* **預設時數型別**：為使用者選取預設時數型別。 這是使用者記錄時間時，預設使用的小時型別。
* **可用時數型別**：選取使用者應該可用的時數型別。 這些小時型別在Workfront中任何使用者可記錄時間的位置都可見。 使用者只能看到在專案層級和使用者層級啟用的小時型別。 如需使用者可以使用哪些時數型別的詳細資訊，請參閱[定義時數型別和可用性](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)。
* **在**&#x200B;中記錄時間：選取使用者應該以小時或天為單位在工作專案上記錄時間。 如需詳細資訊，請參閱[設定以小時或天記錄時間](/help/quicksilver/timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)。
* **FTE**：此為使用者的Full Time同等專案。 只有當系統層級的「資源管理偏好設定」設定為「預設排程」時，Workfront才會根據預設排程使用此數字來計算使用者的可用性。

  FTE代表使用者可在工作上花費的時間量。 這包括管理費用，以及在專案工作上所花費的時間。 例如，在會議或培訓中花費的時間也會納入FTE。

  FTE必須是最高為1的小數位數，而且不能為0。 例如，如果FTE值為0.5，而Workfront中的預設排程為40小時，則使用者每週可使用20小時。

  欄位的預設值為1。

  排程例外、休假及「工作時間」的值可能會影響使用者的可用性。

  Workfront會根據您設定區域中的Resource Management偏好設定來計算使用者的可用性。

  如果系統層級的「資源管理偏好設定」設定為「使用者排程」，則您在此處指定的值會被忽略，而且會根據排程中指定的內容，將使用者視為可用。

  如需詳細資訊，請參閱[設定資源管理喜好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

  如需有關在Workfront中建立排程的詳細資訊，請參閱[建立排程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

* **資源集區**：將使用者與資源集區建立關聯。 如需詳細資訊，請參閱[將資源集區與使用者關聯](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md)。
* **成本費率**：使用者每小時的成本金額。

  若要取得日期有效成本費率，請按一下[新增費率]。**&#x200B;** 輸入時間期間的成本費率值，並視需要指定「開始日期」與「結束日期」。 成本費率1不會有開始日期，而最後的成本費率不會有結束日期。

  部分日期會自動新增。 例如，如果「成本費率1」沒有結束日期，而您新增了開始日期為2023年5月1日的「成本費率2」，則會將結束日期為2023年4月30日的成本費率新增至「成本費率1」，因此不會出現間隙。

* **收費率**：使用者每小時的收費金額。

  若要取得日期有效收費率，請按一下[新增費率]。**&#x200B;** 輸入時間期間的帳單費率值，並視需要指定「開始日期」與「結束日期」。 帳單費率1不會有開始日期，而最後的帳單費率不會有結束日期。

  部分日期會自動新增。 例如，如果「收費率1」沒有結束日期，而您新增了開始日期為2023年5月1日的第二個日期，則結束日期為2023年4月30日的日期會新增至「收費率1」，因此不存在間隔。

  ![使用者成本和收費率](assets/user-cost-billing-rates-2025.png)

### 自訂表單

將現有的使用者自訂表單與此使用者建立關聯。 您必須先建立自訂表單，然後才能將其與使用者建立關聯。 清單中只會顯示作用中的自訂表單。 您無權編輯的欄位不會顯示在個別自訂表單中。

>[!NOTE]
>
>進階自訂表單功能(例如外部查詢欄位和Workfront原生欄位)只有在您於詳細資訊頁面上開啟使用者記錄時才可用，無法在「編輯使用者」對話方塊中開啟。 （從使用者清單中，按一下使用者名稱以開啟詳細資訊。）

如需建立自訂表單的相關資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

### 評論

輸入您要傳送給使用者的註解，以及使用者設定檔的更新區域。

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Personal Info </td> 
      <td> 
       <ul> 
        <li><p><b>First Name</b></p></li>
        <li><p><b>Last Name</b></p><p><b>NOTE:</b></p><p>Editing a user's name in Workfront does not edit the user's name in the Adobe Admin Console.</p></li> 
        <li> <p><b>Email Address:</b> The email address for a user is also their username in Workfront. This field is case-sensitive and must be unique. If any user attempts to add a non-unique email address 3 times within a 10-minute window, a reCAPTCHA response appears.</p> <p> Select the <b>I am not a robot</b> setting before you can proceed.</p><p>If you use the email allowlist and enter an email domain not on the list, the user will not receive email notifications. For more information about the allowlist, see <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configure your email allowlist</a>.</p><p>If your organization has been migrated to the Adobe Admin Console, you cannot edit a user's email address in Workfront. The user's email address is set in the Adobe Admin Console. </li> 
        <li> <p><b>Reset Password</b>: Click this link to reset the user's password. You must enter your own password before you can reset another user's password.</p> <p>To reset another user's password, you must be a Workfront administrator, or a group administrator.</p> <p><b>NOTE</b>:  
          <ul> 
           <li> <p>If you are a group administrator, you can reset passwords only for users in the groups where you are designated as an administrator. Also, the User Admin (Group Users) permission must be enabled in your access level:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>This setting is disabled by default. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
           <li> <p>You cannot reset the password of a Workfront administrator.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;SSO Configuration&gt; Username</b>: If your Workfront administrator enabled an SSO integration with Workfront, the SSO Username displays in this field. The type of SSO configuration enabled for your Workfront instance is visible in this field. </li> 
        <li> <p><b>OnlyAllow &lt;SSO Configuration&gt; Authentication</b>: If your Workfront administrator enabled an SSO integration with Workfront and has updated all users for SSO, this field is selected by default. The type of SSO configuration enabled for your Workfront instance is visible in this field.</p> <p>When this field is selected, the user is required to log into Workfront with their SSO credentials. Unchecking it will allow them to log in to Workfront with their Workfront credentials.</p> <p>For more information about configuring Workfront with an SSO solution, see <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Overview of single sign-on in Adobe Workfront</a></p> <p>For more information about updating users for SSO, see <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Update users for single sign-on</a>.</p> 
        <p><b>NOTE</b>:</p> 
        <p> If you are a group administrator, you can edit the &lt;SSO Configuration&gt; fields only for users in the groups where you are designated as such. Also, the User Admin (Group Users) permission must be enabled in your access level.
        <p>If you are a group administrator and you have the User Admin (All Users) permission enabled in your access level, you can edit the &lt;SSO Configuration&gt; fields for all users.</p> </li> 
        <li><b>Job Info:</b> Information about the job, like the job title (in the <b>Title</b> field), and what area of expertise the user is responsible for (in the <b>Talk to Me About</b> field).</li> 
        <li><p><b>Contact Info</b>: The user's phone number (in the <b>Phone number, Ext.</b>, and <b>Mobile number</b> fields) and address (in the <b>Address, City, State, Postal Code, Country</b> fields ).</p>
        <p>If the user is enabled for Unified User Management (UUM) or Adobe Identity Management System (IMS), the <b>Country</b> field in the Contact Info section only accepts country code values (for example, US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferences </td> 
      <td> 
       <ul> 
      <li> <p><b>Time Zone:</b> The user's time zone.</p> <p>For information about helping users collaborate in Workfront across time zones, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Working across time zones</a>.</p> </li>

      <li><p><b>Email Locale</b>: The user's preferred email locale. This affects the format of numbers and dates in the emails that come from Workfront to this user.</p>
      <p><b>NOTE:</b> When your organization is on the Adobe Unified Experience, the user's language preferences are stored in their Adobe profile and the email locale is not used. For information about accessing these preferences, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></li> 
      
      <li><b>Receive emails from this test environment</b>: Check this option if you want to receive email notifications from the environment that you are currently logged in.
      <p><b>NOTE</b></p>
      <p>This option is available only in the Preview and Sandbox environments. Email notifications are enabled in the Production environment by default. </p>
      </li> 
      
      </li> 
       <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       <li><b>Automatically generate proofs when uploading documents</b>: Check this option if you want the documents that the user uploads to immediately generate a proof. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td> <p>Select the email notifications which should be enabled for the new user.</p> <p>You can select instant as well as daily digest notifications.</p> <p>For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
      <li><b>Is Active:</b> Select this box to indicate that the user is active. Active users use a Workfront license. Clearing the box deactivates the user and prevents them from logging in to Workfront.</li> 
       <li> <p><b>Access Level:</b> Select the access level to assign to this user.</p> 
       <p>When you assign an access level to a user, you can assign a level equal to or lower than your own access level.</p>
       <p>For example, if your access level is Plan, you cannot assign the Administrator access level. However, you cannot assign an access level that by default is lower than your own access level if the Workfront administrator has enabled non-default permissions on the access level that are not also enabled in your own access level. </p>
       <p>For example, if you have a Plan license with no access to delete tasks, you cannot assign someone a Work license with access to delete tasks, although the Work license is lower than the Plan license. For more information, see  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> 
       <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p>
       <p> <b>NOTE:</b></p> 
       <p> If your organization uses the new access model (Standard/Light/Contributor), you cannot reassign a Standard or Light user to a Contributor access level if that user has already reached their decision limit for the month. </p><p>For more information on the new access model, see <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">New access levels overview</a>. </p><p>For information on decision limits, see <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Limited document and proof decision for non-paid users overview</a>.</p></li> 
       <li> <p><b>Layout Template</b>: Choose a Layout Template for the user. This Layout Template takes precedence over any Layout Template assigned to the user's Home Group, Home Team or Primary Role. For more information about the assignment priority of Layout Templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> <p><b>NOTE</b>:  <p>The following list describes how the list of templates you have available in this field depends on your access:</p> 
       <ul> 
       <li>As a Workfront administrator, you can see all system-level and group-level Layout Templates.</li> 
       <li>As a group administrator, you can see system-level layout template, as well as those associated with the groups that you manage.</li> 
       <li>As a user with a Plan license and access to edit users, you can see only system-level Layout Templates.</li> 
       </ul> <p>For more information about group-level Layout Templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization </td> 
      <td> 
       <ul> 
      <li><b>Company</b>: The company of the user. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Create and edit companies</a>.</li> 
      <li><b>Reports to:</b> If you specified a company for the user, you can also specify the direct manager of the user in this field. A user can have only one manager. This field does not display if the user is not associated with a company first. </li> 
      <li><b>Direct Reports:</b> If you specified a company for the user, you can also specify the direct reports of the user. A user can have multiple direct reports. This field does not display if the user is not associated with a company first.</li> 
      <li><b>Home Team</b>: Specify the home team for the user. Users can only have one home team. The Home Team is important when assigning a layout template or when defining the Work On It button for the tasks and issues assigned to the user. </li> 
      <li><b>Other Teams</b>: Users can belong to multiple teams. A user can view work items assigned to any of their teams in their Home area. </li> 
      <li> <p><b>Home Group:</b> Select an appropriate group to assign the user. This gives the user the ability to access objects that are shared with the group. You can also share layout templates with the user's Home Group.</p> <p>This is a required field. Every user must be associated with a home group. If you don't select one, your Home Group is assigned as the new user's Home Group.</p> <p><b>NOTE</b>:</p> 
      <p> You can assign a group to a user only if one of the following is true:</p>
      <ul><li>you are a Workfront administrator</li>
      <li>you are the administrator of the group</li>
      <li>the group is public.</li></ul> 
      <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only if you are a Workfront administrator, you are the administrator of the group, or the group is public.</p> <p><b>IMPORTANT</b>:</p> 
      <p>Adding a user to more than 100 groups may cause performance issues in any area of Workfront that loads the list of groups.</p> <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning </td> 
      <td> 
       <ul>
       <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.  

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user's capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to 1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 
      <li> <b>Schedule Deactivation</b>: Check this box if you want to schedule this user to be deactivated on a certain date and at a certain time. </li> 
       <li><b>Scheduled Deactivation Date</b>: The date and time on which the user becomes deactivated. For information about scheduling users for deactivation, see the <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that the user can fulfill in Workfront. Every task and issue that the user is assigned to is also assigned to this job role. Job roles are essential in resource management. You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> <p>Only active job roles display in the list. </p> </li> 
       <li>If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the user's schedule is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%. </li> 
       <li> <p><b>Other Roles</b>: A user can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.<p>Only active job roles display in the list. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. <br>For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the user's schedule is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTE</b>: <p>The sum of all <b>Percentages of FTE Availability</b> for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </p>
       <span class="preview"><p>(Optional) Date effective job role assignments are used in financial calculations if the user's job role changes during a project.</p><p>Click <b>Define roles by date</b>, select the <b>Primary Role</b> and <b>Other Roles</b>, and enter the allocation percentage for each role. The roles could be the same as the existing roles (using different percentages), or new roles. Select the <b>Start date</b> when these roles become active. This can be a future date. When the newest roles become active, you can click <b>Show previous roles</b> to see the previous, inactive roles.</p> </li></span>
       <li> <p><b>Schedule</b>: Associate a schedule with the user. The schedule of the user calculates the timeline of the tasks the user is assigned to.</p> <p>You must create a schedule before you can associate it with a user. For more information about creating schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>NOTE</b>: We recommend that the schedule you associate with the user matches the user's Time Zone.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the user to ensure that timesheets generate automatically for the user.</p> <p><b>NOTE</b>:  The list of profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and all group-level Timesheet Profiles.</li>
       <li>As a group administrator, you can see system-level Timesheet Profiles, as well as those associated with the groups that you manage.</li>
       <li>As a user with a Plan license and access to edit users, you can see only system-level Timesheet Profiles. For more information about group-level Timesheet Profiles, see <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Create, edit, and assign timesheet profiles</a>.</li>
      </ul></p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the user. This is the hour type that is used by default when the user logs time.</li> 
       <li><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the user can log time. A user can only see the hour types that are enabled at the project level as well as the user level. For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</li> 
       <li><b>Log Time in:</b> Select whether the user should log time on work items in hours or days. For more information, see <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configure whether time is logged in hours or days</a>.</li>
       
      <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
      
      <li><b>Resource Pools</b>: Associate the user with Resource Pools. For more information, see <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associate resource pools with users </a>.</li> 
      
      <li><b>Cost Rate</b>: The amount of cost per hour for the user.
      <p>For date effective cost rates, click <strong>Add Rate</strong>. Enter the value of the cost rate for the time period, and assign a Start Date and End Date as needed. Cost Rate 1 will not have a start date and the last cost rate will not have an end date.</p><p>Some dates are added automatically. For example, if Cost Rate 1 does not have an end date, and you add Cost Rate 2 with a start date of May 1, 2023, an end date of April 30, 2023 is added to Cost Rate 1 so that no gaps exist.</p></li> 
      
      <li><b>Billing Rate</b>: The amount of billing per hour for the user.
      <p>For date effective billing rates, click <strong>Add Rate</strong>. Enter the value of the billing rate for the time period, and assign a Start Date and End Date as needed. Billing Rate 1 will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if Billing Rate 1 does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to Billing Rate 1 so that no gaps exist.</p><p> <img alt="User cost and billing rates" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

      </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custom Forms</td> 
      <td><p>Associate an existing user custom form with this user. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. Fields you do not have access to edit are not displayed in an individual custom form.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the user record on the details page, not on the Edit User dialog. (From the list of users, click the user name to open the details.)</p> <p>For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref">Create a custom form</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comment</td> 
      <td>Type the comment you want to send to the users and to the Updates area of their user profiles.</td> 
     </tr> 
    </tbody> 
   </table>
-->
