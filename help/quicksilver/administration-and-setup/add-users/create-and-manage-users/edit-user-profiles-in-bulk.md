---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 大量編輯使用者設定檔
description: 身為Adobe Workfront管理員，您可以大量編輯使用者帳戶。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: c7b91828e5a4f961fc48e857eb63756b9b38f664
workflow-type: tm+mt
source-wordcount: '2625'
ht-degree: 0%

---

# 大量編輯使用者設定檔

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/tw/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

您可以大量編輯使用者帳戶。 當大量編輯使用者時，只有您特別選取的欄位會更新為所選的所有使用者提供相同的資訊。 您未選取的所有其他欄位，每位使用者都將維持不變，即使每位使用者各有不同。

>[!NOTE]
>
>* 您無法大量編輯使用者設定檔的個人資訊區段，因為此資訊對於每個使用者都必須是唯一的。
>* 為確保資料的準確性和最佳效能，建議您一次選取不超過2000名使用者進行大量編輯。
>

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

## 大量編輯使用者帳戶

{{step-1-to-users}}

1. 選取多個使用者，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

1. 在&#x200B;**編輯使用者**&#x200B;方塊中，變更任何區段中的資訊，然後隨時按一下&#x200B;**儲存變更** <span class="preview">或&#x200B;**儲存**</span>。

### 偏好設定

* **時區**：使用者的時區。

  如需有關協助使用者在Workfront中跨時區共同作業的資訊，請參閱[跨時區工作](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)。

* **電子郵件地區設定**：使用者偏好的電子郵件地區設定。 這會影響從Workfront傳送給此使用者的電子郵件中的數字和日期格式。

  >[!NOTE]
  >
  >當您的組織使用Adobe統一體驗時，使用者的語言偏好設定會儲存在其Adobe設定檔中，而不使用電子郵件地區設定。 如需有關存取這些偏好設定的資訊，請參閱[Workfront的Adobe Unified Experience ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

### 通知

選取應為使用者啟用的電子郵件通知。

您可以選取即時和每日摘要通知。 對於您選取的所有使用者，所有每日摘要通知會在同一時間傳送。

如需詳細資訊，請參閱[設定系統中每個人的事件通知](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

### 存取

* **為作用中** / <span class="preview">**使用者為作用中**</span>：啟用此選項以指出使用者為作用中。 作用中使用者使用Workfront授權。 停用欄位會停用使用者，並防止他們登入Workfront。

* **存取層級**：選取要指派給這些使用者的存取層級。 您選取的所有使用者都將擁有相同的存取層級。

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

* **配置範本**：選擇使用者的配置範本。 此配置範本優先於任何指派給其「主群組」、「主團隊」或「主要角色」的配置範本。 如需配置範本的指派優先順序的詳細資訊，請參閱[建立和管理配置範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

  下列清單說明您在此欄位中可用的範本清單如何取決於您的存取權：

   * 身為Workfront管理員，您可以檢視所有系統層級和群組層級的版面配置範本。
   * 身為群組管理員，您可以檢視系統層級配置範本，以及與您管理的群組相關聯的配置範本。
   * 作為具有Standard或Plan授權並擁有編輯使用者存取權的使用者，您只能看到系統層級的版面配置範本。

     如需群組層級配置範本的詳細資訊，請參閱[建立和修改群組的配置範本](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

### 組織

* **公司**：使用者的公司。 使用者只能與一個公司相關聯。 您必須先建立公司，然後才能與使用者建立關聯。 清單中只會顯示作用中的公司。 如需有關建立公司的資訊，請參閱[建立和編輯公司](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。
* **主團隊**：指定使用者的主團隊。 使用者只能有一個主團隊。
* **其他團隊**：使用者可以屬於多個團隊。
* **主群組** / <span class="preview">**目前主群組**</span>：選取適當的群組以指派使用者。 這可讓使用者存取與群組共用的物件。 您也可以與主群組共用版面配置範本。

  這是必填欄位。 每個使用者都必須與主群組相關聯。 如果您未選取主群組，則會將您的主群組指派為主群組。

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

* **工作時間**：代表使用者實際工作可用的全職相當時間(FTE)百分比，不包括額外負荷。 「工作時間」必須為最多1的小數，且不可以是0。 例如，實際工作的20%可用性為0.2。

  該欄位的預設值為1，這表示使用者將其整個FTE用於實際的、專案相關的工作。

  系統會使用此數字來計算使用者進行實際專案相關工作的可用性。

  如需有關在Workfront中建立排程的詳細資訊，請參閱[建立排程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

  排程例外狀況與休假也可能會影響使用者的容量。

  Workfront會根據您設定區域中的Resource Management偏好設定來計算使用者的可用性。 如需詳細資訊，請參閱[設定資源管理喜好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

  >[!TIP]
  >
  >將「工作時間」值設為1，表示使用者可用於專案相關工作的整個全職同等工作。

* **排程停用** / <span class="preview">**設定停用日期**</span>：核取此方塊/ <span class="preview">如果您要排程這些使用者在特定日期及特定時間停用，請按一下此按鈕</span>。
* **已排程的停用日期** / <span class="preview">**停用日期**</span>：停用使用者的日期和時間。 如需排程使用者停用的相關資訊，請參閱[停用或重新啟用使用者](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation)中的[排程使用者停用](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。
* **主要角色**：這是使用者可以在Workfront中完成的主要工作角色。 指派給使用者的每個任務和問題也會指派給此工作角色。 職務角色在資源管理中至關重要。 只有在您擁有具有管理使用者存取許可權的「標準」或「計畫」授權，或者您是Workfront管理員時，才能更新此欄位。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱[授予使用者存取許可權](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

  清單中只會顯示作用中的職位角色。

* （視條件而定）如果您選取&#x200B;**主要角色**，則會顯示&#x200B;**FTE可用性百分比**&#x200B;欄位。 指定將使用者排程的時間百分比分配給此工作角色。 主要角色的FTE可用性百分比預設值為100%。
* **其他角色**：使用者可以在Workfront中擁有多個工作角色。 職務角色在資源管理中至關重要。 使用者可以完成的工作角色數量沒有限制。 但是，我們建議不要將一位使用者指派給太多工作角色，因為這些使用者可能很難管理資源。

  清單中只會顯示作用中的職位角色。 如需有關工作角色的詳細資訊，請參閱[建立和管理工作角色](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

  只有在您擁有具有管理使用者存取許可權的「標準」或「計畫」授權，或者您是Workfront管理員時，才能更新此欄位。

  如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱[授予使用者存取許可權](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

* （視條件而定）如果您選取一或多個&#x200B;**其他角色**，則會針對每個角色顯示&#x200B;**FTE可用性百分比**&#x200B;欄位。 指定將使用者排程的時間百分比分配給每個工作角色。 其他角色的FTE可用性百分比預設值為0%。

  如果「其他角色」具有0%的FTE可用性，除非將使用者指派給這些角色中的任務，否則它們不會顯示在「資源規劃工具」中。

  所有角色的所有&#x200B;**FTE可用性**&#x200B;百分比的總和必須等於100%。 每個FTE可用性的百分比會計算「資源規劃工具」中每個使用者的「可用時數」。 每個使用者每個角色的可用時數取決於使用者的可用時數。

  使用者的可用時間由Workfront根據Workfront管理員在資源管理偏好設定中計算約當全職人數時所選取的方法計算。

  如需有關計算使用者可用性的資訊，請參閱[計算資源規劃工具中使用者和角色的時數和FTE的概觀](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)。

  如需有關設定資源管理偏好設定的資訊，請參閱[設定資源管理偏好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

* **排程**：將排程與使用者建立關聯。 使用者的排程會計算指派給使用者的任務的時間表。

  您必須先建立排程，然後才能與使用者建立關聯。 如需建立排程的詳細資訊，請參閱[建立排程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

  >[!IMPORTANT]
  >
  >只有在&#x200B;**使用來計算資源可用性**&#x200B;設定設為&#x200B;**使用者的排程**&#x200B;時，Workfront才會使用使用者的排程。 如需此設定如何影響用於資源管理的排程的詳細資訊，請參閱[設定資源管理喜好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

* **時程表設定檔**：將時程表設定檔與使用者建立關聯，以確保時程表會自動產生。

  您在此欄位中可用的設定檔清單取決於您的存取權：

   * 身為Workfront管理員，您可以檢視所有系統層級和所有群組層級的時程表設定檔。
   * 作為群組管理員，您可以檢視系統層級的時程表設定檔，以及與您管理的群組相關聯的時程表設定檔。
   * 作為具有標準或計畫授權並存取許可權以編輯使用者的使用者，您只能看到系統層級的時程表設定檔。 如需群組層級週期性時程表的詳細資訊，請參閱[建立、編輯和指派週期性時程表](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

* **預設小時型別**：為使用者選取預設小時型別。 這是使用者記錄時間時，預設使用的小時型別。
* **可用時數型別**：選取使用者應該可用的時數型別。 這些小時型別在Workfront中任何使用者可記錄時間的位置都可見。 使用者只能看到在專案層級和使用者層級啟用的小時型別。 如需使用者可以使用哪些時數型別的詳細資訊，請參閱[定義時數型別和可用性](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)。
* **FTE**：這是使用者的全職同等專案。 只有在系統層級的「資源管理偏好設定」設定為「預設排程」時，Workfront才會使用此數字，根據「預設排程」來計算使用者的可用性。

  FTE代表使用者可在工作上花費的時間量。 這包括管理費用，以及在專案工作上所花費的時間。 例如，在會議或培訓中花費的時間也會納入FTE。

  FTE必須是最高為1的小數位數，而且不能為0。 例如，如果FTE值為0.5，而Workfront中的預設排程為40小時，則使用者每週可使用20小時。

  欄位的預設值為1。

  排程例外、休假及「工作時間」的值可能會影響使用者的可用性。

  Workfront會根據您設定區域中的Resource Management偏好設定來計算使用者的可用性。

  如果系統層級的「資源管理偏好設定」設定為「使用者排程」，則您在此處指定的值會被忽略，而且會根據排程中指定的內容，將使用者視為可用。

  如需詳細資訊，請參閱[設定資源管理喜好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

  如需有關在Workfront中建立排程的詳細資訊，請參閱[建立排程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

* **資源集區**：將使用者與資源集區建立關聯。

  >[!NOTE]
  >
  >此欄位中只會顯示所有選取使用者共用的資源集區。 如果您選取的使用者沒有共用資源集區，則此欄位為空白。 如果此欄位空白，您在此指定的資源集區將會覆寫其個別資源集區。

  如需資源集區的詳細資訊，請參閱[將資源集區與使用者關聯](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md)。

* **成本費率**：使用者每小時的成本金額。

  若要取得日期有效成本費率，請按一下[新增費率]。**&#x200B;** 輸入時間期間的成本費率值，並視需要指定「開始日期」與「結束日期」。 成本費率1不會有開始日期，而最後的成本費率不會有結束日期。

  部分日期會自動新增。 例如，如果「成本費率1」沒有結束日期，而您新增了開始日期為2023年5月1日的「成本費率2」，則會將結束日期為2023年4月30日的成本費率新增至「成本費率1」，因此不會出現間隙。

* **收費率**：使用者每小時的收費金額。

  若要取得日期有效收費率，請按一下[新增費率]。**&#x200B;** 輸入時間期間的帳單費率值，並視需要指定「開始日期」與「結束日期」。 帳單費率1不會有開始日期，而最後的帳單費率不會有結束日期。

  部分日期會自動新增。 例如，如果「收費率1」沒有結束日期，而您新增了開始日期為2023年5月1日的第二個日期，則結束日期為2023年4月30日的日期會新增至「收費率1」，因此不存在間隔。

### 自訂表單

將現有的使用者自訂表單與使用者建立關聯。 您必須先建立自訂表單，然後才能將其與使用者建立關聯。 清單中只會顯示作用中的自訂表單。 您無權編輯的欄位不會顯示在個別自訂表單中。

>[!NOTE]
>
>進階自訂表單功能(例如外部查詢欄位和Workfront原生欄位)只有在您於詳細資訊頁面上開啟使用者記錄時才可用，無法在「編輯使用者」對話方塊中開啟。 （從使用者清單中，按一下使用者名稱以開啟詳細資訊。）

您可以選擇選取&#x200B;**重新計算自訂運算式**&#x200B;選項，以確保附加到所選使用者的自訂表單中的所有計算自訂欄位都是最新的。

如需建立自訂表單的相關資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

### 評論

輸入您要傳送給使用者的註解，以及使用者設定檔的更新區域。

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
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
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->

