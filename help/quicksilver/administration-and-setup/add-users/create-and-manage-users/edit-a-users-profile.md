---
title: 編輯使用者的設定檔
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 身為Adobe Workfront管理員，您可以建立新使用者並管理現有使用者的設定檔。
author: Courtney, Alina
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2557'
ht-degree: 0%

---

# 編輯使用者的設定檔

<!--drafted for Work Time field: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

In the table below, under Resource Planning, add the "Work Time" field and update the "FTE" field:

<b><span class="preview">Work Time</span></b>: <span class="preview">Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.</span> 

<span class="preview">The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work.</span>  

<span class="preview">The system uses this number to calculate the availability of the user for actual, project-related work. </span> 

<span class="preview">For more information about creating schedules in Workfront, see Create a schedule.</span>

<span class="preview">Schedule exceptions and time off might also affect the user capacity. 

Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see Configure Resource Management preferences. (*****INSERT LINK****)

<b>TIP</b>

<span class="preview">Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.</span>


***UPDATED FTE FIELD***

FTE: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. The FTE indicates the amount of time that the user can spend at work. This includes overhead, and  time that is not spent on project work, but on other type of work. For example, time that is spent in meetings, or training is also included in the FTE. 

The FTE must be a decimal number up to 1, and it cannot be 0. 
The field's default is 1.

For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

Schedule exceptions, time off might, <span class="preview">and the value of Work Time</span> may affect the amount of available hours or the FTE. 

Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see Configure Resource Management preferences. (*****INSERT LINK****)

If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

For more information about creating schedules in Workfront, see Create a schedule. (*****INSERT LINK*****)
-->

>[!IMPORTANT]
>
>本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>如需在Adobe Admin Console中編輯使用者設定檔的指示，請參閱文章中的「編輯使用者詳細資料」一節 [個別管理使用者](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 或聯絡您的Adobe Admin Console管理員。
>
>如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

身為Adobe Workfront管理員，您可以建立新使用者並管理現有使用者的設定檔。 如需建立使用者的相關資訊，請參閱 [新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

擁有計畫許可證的用戶也可以建立和管理用戶。 如需編輯使用者所需存取權的相關資訊，請參閱 [授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員訪問級別。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>. </p> </li> 
     <li> <p><b>使用者</b> 在您的存取層級中設定 <b>編輯</b> 存取，使用 <b>建立</b> 和兩者中的至少一個 <b>使用者管理</b> 選項 <b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>在這兩個選項中，如果用戶 <b>管理員（群組使用者）</b> 啟用時，您必須是使用者所屬群組的群組管理員。</p> <p>如需 <b>使用者</b> 在存取層級中設定，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 編輯使用者設定檔

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).
1. 選取使用者，然後按一下「編輯」圖示 ![](assets/edit-icon.png).

1. 在 **編輯用戶** 框中，更改以下任何資訊，然後按一下 **儲存變更**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">個人資訊 </td> 
      <td> 
       <ul> 
        <li><b>名字</b>, <b>姓氏</b></li> 
        <li> <p><b>電子郵件地址：</b> 使用者的電子郵件地址也是其在Workfront中的使用者名稱。 此欄位區分大小寫，且必須是唯一的。 如果任何使用者在10分鐘內嘗試新增非唯一電子郵件地址3次，則會顯示reCAPTCHA回應。</p> <p>如果您使用電子郵件允許清單，並輸入未在清單上的電子郵件網域，則使用者不會收到電子郵件通知。 如需允許清單的詳細資訊，請參閱 <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">設定您的電子郵件允許清單</a>.</p> </li> 
        <li> <p><b>重設密碼</b>:按一下此連結以重設使用者的密碼。 系統會要求您輸入自己的密碼，之後才能重設使用者的密碼。</p> <p>若要重設其他使用者的密碼，您必須是Workfront管理員或群組管理員。</p> <p><b>附註</b>:  
          <ul> 
           <li> <p>如果您是組管理員，則只能為指定為的組中的用戶重置密碼。 此外，您必須在存取層級中啟用使用者管理員（群組使用者）權限：</p> <p> <img src="assets/group-admin-user.png" > </p> <p>預設會停用此設定。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </li> 
           <li> <p>您無法重設Workfront管理員的密碼。</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; 使用者名稱</b>:如果您的Workfront管理員啟用了與Workfront的SSO整合，則此欄位中會顯示SSO使用者名稱。 此欄位會顯示為Workfront執行個體啟用的SSO設定類型。 </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; 驗證</b>:如果您的Workfront管理員已啟用與Workfront的SSO整合，且已更新所有SSO使用者，則此欄位預設為選取。 此欄位會顯示為Workfront執行個體啟用的SSO設定類型。</p> <p>選取此欄位時，使用者必須使用其SSO憑證登入Workfront。 取消勾選後，使用者就能使用其Workfront憑證登入Workfront。</p> <p>如需使用SSO解決方案設定Workfront的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Adobe Workfront中的單一登入概觀</a></p> <p>如需更新SSO使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">更新單一登入的使用者</a>.</p> <p><b>注意</b>:如果您是群組管理員，可以編輯 &lt;sso configuration=""&gt; 欄位僅適用於指定您的群組中的使用者。 此外，您必須在存取層級啟用使用者管理員（群組使用者）權限。
        <p>如果您是群組管理員，且在存取層級中啟用了「使用者管理員」（所有使用者）權限，您可以編輯 &lt;sso configuration=""&gt; 欄位。</p> </li> 
        <li><b>作業資訊：</b> 有關工作的資訊，如職稱，以及用戶負責的專業領域。</li> 
        <li><p><b>聯繫資訊</b>:使用者的電話號碼和地址。</p>
        <p>如果使用者已啟用統一使用者管理(UUM)或AdobeIdentity Management系統(IMS)，則 <b>國家/地區</b> 「連絡資訊」區段中的欄位僅接受國家/地區代碼值（例如US、GB、IN）。</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">喜好設定 </td> 
      <td> 
       <ul> 
        <li> <p><b>時區：</b> 使用者的時區。</p> <p>如需協助使用者在Workfront中跨時區進行協作的詳細資訊，請參閱 <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">跨時區工作</a>.</p> </li> 
        <li><b>電子郵件地區</b>:使用者偏好的電子郵件地區設定。 這會影響來自Workfront之電子郵件中的數字和日期格式。</li> 
        <li><b>顯示更新狀態完成百分比</b>:如果要在此用戶任務的「更新」區域內顯示完成百分比欄，請核取此選項。</li> 
        <li><b>將我指派給自己的工作發送到「工作」頁簽</b>:如果希望用戶指派給自己的所有內容都直接顯示在「正在工作」(Working On)頁簽上，請核取此選項。 預設值是在其「工作請求」索引標籤中列出指派給使用者的所有內容。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通知</td> 
      <td> <p>選取應為新使用者啟用的電子郵件通知。</p> <p>您可以選取即時通知和每日摘要通知。</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">為系統中的每個人配置事件通知</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">存取</td> 
      <td> 
       <ul> 
        <li><b>活動：</b> 選取此方塊以指出使用者處於作用中狀態。 作用中使用者使用Workfront授權。 清除該框會停用使用者。</li> 
        <li> <p><b>訪問級別：</b> 選擇要分配給此用戶的訪問級別。</p> 
        <p>將訪問級別分配給用戶時，可以將級別分配給等於或小於您自己的訪問級別。 （例如，如果訪問級別為「計畫員」，則無法分配管理員訪問級別。） 但是，如果Workfront管理員已對未在您自己的訪問級別中啟用的訪問級別啟用非預設權限（通過微調設定），則不能指定預設小於您自己的訪問級別的訪問級別，如 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>)。 </p> 
        <p>有關訪問級別的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">設定Adobe Workfront的存取權</a>.</p> </li> 
        <li> <p><b>版面範本</b>:為用戶選擇「佈局模板」。 此「配置模板」優先於分配給用戶的「主組」、「主組」或「主作業」角色的任何「配置模板」。 有關佈局模板的分配優先順序的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立和管理版面範本</a>.</p> <p><b>附註</b>:  <p>您在此欄位中可用的範本清單取決於您的存取權：</p> 
          <ul> 
           <li>身為Workfront管理員，您可以查看所有系統層級和群組層級的版面範本。</li> 
           <li>身為群組管理員，您可以查看系統層級配置範本，以及與您管理之群組相關聯的配置範本。</li> 
           <li>作為擁有計畫許可證和編輯用戶訪問權限的用戶，您只能看到系統級佈局模板。</li> 
          </ul> <p>如需群組層級「版面範本」的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立和管理版面範本</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">組織 </td> 
      <td> 
       <ul> 
      <li><b>公司</b>:使用者的公司。 使用者只能與一個公司相關聯。 您必須先建立公司，才能將其與使用者建立關聯。 清單中只會顯示作用中的公司。 如需建立公司的相關資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">建立和編輯公司</a>.</li> 
      <li><b>報表：</b> 如果您為使用者指定了公司，您也可以在此欄位中指定使用者的直接經理。 使用者只能有一個管理員。</li> 
      <li><b>直接報表：</b> 如果您為使用者指定了公司，您也可以指定使用者的直接報表。 使用者可以有多個直接報表。</li> 
      <li><b>主隊</b>:指定使用者的主團隊。 使用者只能有一個主團隊。</li> 
      <li><b>其他團隊</b>:使用者可屬於多個團隊。</li> 
      <li> <p><b>家庭組：</b> 選取要指派使用者的適當群組。 這可讓使用者存取與群組共用的物件。</p> <p>這是必填欄位. 每個用戶都必須與一個主組相關聯。 如果您未選取群組，則會將您的群組指派為新使用者的首頁群組。</p> <p><b>注意</b>:只有在您是Workfront管理員、您是群組管理員或群組為公用時，才可將群組指派給使用者。</p> </li> 
      <li> <p><b>其他群組</b>:使用者可屬於多個群組。 只有在您是Workfront管理員、您是群組管理員或群組為公用時，才可將群組指派給使用者。</p> <p><b>重要</b>:將使用者新增至超過100個群組，可能會在載入群組清單的Workfront的任何區域中造成效能問題。</p> <p>如需公開群組的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">建立群組</a>.</p> <p>如需群組的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群組概觀</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">資源規劃 </td> 
      <td> 
       <ul>
       <li><b>計畫停用</b>:如果要將此使用者排程在一段時間後停用，請核取此方塊。 </li> 
       <li><b>計畫的停用日期</b>:使用者停用的日期。 如需排程使用者停用的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">排程使用者停用</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>.</li> 
       <li> <p><b>主要角色</b>:這是使用者可在Workfront中履行的主要工作角色。 將用戶分配給的每個任務和問題也分配給此作業角色。 作業角色在資源管理中是必不可少的。 只有在您擁有具有管理用戶訪問權限的計畫許可證，或者您是Workfront管理員時，才能更新此欄位。 有關設定具有管理用戶訪問權限的用戶的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> <p>清單中只顯示活動作業角色。 </p> </li> 
       <li>如果您選取 <b>主要角色</b>, <b>FTE可用性百分比</b> 欄位。 指定將用戶調度的時間百分比分配給此作業角色。 主要角色的FTE可用性百分比的預設值為100%。 </li> 
       <li> <p><b>其他角色</b>:使用者在Workfront中可以有多個工作角色。 作業角色在資源管理中是必不可少的。 用戶可履行的職務數沒有限制。 但是，我們建議不要將一個用戶分配給過多的作業角色，因為對這些用戶來說，資源管理可能變得太複雜了。<p>清單中只顯示活動作業角色。 有關作業角色的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a>.</p> <p>只有在您擁有具有管理用戶訪問權限的計畫許可證，或者您是Workfront管理員時，才能更新此欄位。 <br>有關設定具有管理用戶訪問權限的用戶的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
       <li> <p>（條件性）如果您選取一或多個 <b>其他角色</b>, <b>FTE可用性百分比</b> 欄位隨即顯示。 指定將用戶調度的時間百分比分配給每個作業角色。 其他角色的FTE可用性百分比的預設值為0%。</p> <p><b>注意</b>:如果其他職責的FTE可用性為0%，則它們不會顯示在資源計畫器中，除非將用戶分配給這些職責中的任務。</p> <p> <img alt="user_settings_roles_and_dte_boxes_rp_story_png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>附註</b>: <p>總和 <b>FTE可用性百分比</b> 對於所有角色，必須等於100%。 每個FTE可用性百分比計算資源計畫員中每個用戶每個角色的可用小時數。 每個用戶的每個角色的可用小時數取決於用戶的可用時間。</p> <p>用戶的可用時間由Workfront計算，具體取決於Workfront管理員在「資源管理首選項」中選擇的計算FTE的方法。</p> <p>有關計算用戶可用性的資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">在資源計畫員中計算用戶和角色的小時數和FTE的概覽</a>.</p> <p>有關配置資源管理首選項的資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置資源管理首選項</a>.</p> </p> </li> 
       <li> <p><b>排程</b>:將排程與使用者關聯。 用戶的計畫計算分配給用戶的任務的時間表。</p> <p>您必須先建立排程，才能將其與使用者建立關聯。 如需建立排程的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>.</p> <p><b>注意</b>:建議您將您與使用者相關聯的排程與使用者的時區相符。</p> </li> 
       <li> <p><b>時間表配置檔案</b>:將時間表配置檔案與用戶關聯，以確保為用戶自動生成時間表。</p> <p><b>注意</b>:您在此欄位中可用的設定檔清單取決於您的存取權：
       <ul>
       <li>作為Workfront管理員，您可以查看所有系統級別和所有組級別的時間表配置檔案。</li>
       <li>作為組管理員，您可以查看系統級時間表配置檔案以及與您管理的組關聯的時間表配置檔案。</li>
       <li>作為具有計畫許可證和編輯用戶訪問權限的用戶，您只能看到系統級時間表配置檔案。 有關組級時間表配置檔案的詳細資訊，請參閱 <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">建立、編輯和分配工時單配置檔案</a>.</li>
      </ul></p> </li> 
       <li><b>預設小時類型</b>:為用戶選擇預設小時類型。 這是使用者記錄時間時，預設使用的小時類型。</li> 
       <li><b>可用小時類型</b>:選取使用者應可使用的小時類型。 這些小時類型在Workfront中任何地方都可見，使用者可在其中記錄時間。 使用者只能查看專案層級和使用者層級已啟用的小時類型。 如需使用者可使用的小時類型詳細資訊，請參閱 <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">定義工時單的工時類型和可用性</a>.</li> 
       <li><b>登入時間：</b> 選擇用戶是否應以小時或天登錄工作項。 如需詳細資訊，請參閱 <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">配置時間是以小時還是天記錄</a>.</li> 
       <li> <p><b>FTE</b>:只有當系統級別的「資源管理首選項」設定為 <b>預設排程</b>. 值必須是 <i>0</i> 或介於 <i>.1</i> 和 <i>1</i>.</p> <p>例如，如果FTE值為0.5，預設計畫為40小時，則用戶每週可工作20小時。</p> <p>如果系統級別上的「資源管理首選項」設定為 <b>使用者的排程</b>，則會忽略您在此指定的值，且會根據使用者的排程指定內容，將使用者視為可用。 在這種情況下，資源計畫員的用戶FTE按以下公式計算：</p> <p ><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><em><br></em> </p> <p>有關計算用戶FTE的詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">在資源計畫員中計算用戶和角色的小時數和FTE的概覽</a>.<br>如需在Workfront中建立排程的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>.</p> <p>計畫例外和休假時間可能會影響計畫小時數或FTE的數量。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置資源管理首選項</a>. </p> </li> 
        <li><b>資源池</b>:將用戶與資源池關聯。 如需詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">將資源池與用戶關聯 </a>.</li> 
        <li><b>每小時成本</b>:使用者每小時的成本金額。 </li> 
        <li><b>每小時計費</b>:使用者每小時的計費金額。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂表單</td> 
      <td>將現有用戶自定義表單與此用戶關聯。 您必須先建立自訂表單，才能將其與使用者建立關聯。 清單中只會顯示使用中的自訂表單。 如需建立自訂表單的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">評論</td> 
      <td> <p>輸入要傳送給使用者的註解，並輸入其使用者設定檔的「更新」區域。</p> </td> 
     </tr> 
    </tbody> 
   </table>
