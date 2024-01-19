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
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '2387'
ht-degree: 0%

---

# 大量編輯使用者設定檔

>[!IMPORTANT]
>
>此頁面中說明的程式僅適用於尚未加入Admin Console的組織。 如果您的組織已加入Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>如需在Adobe Admin Console中編輯使用者設定檔的說明，請參閱文章中的「編輯使用者詳細資訊」一節 [大量上傳使用者](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) 或聯絡Adobe Admin Console管理員。
>
>如需根據貴組織是否已加入Adobe Admin Console而有所差異的程式清單，請參閱 [平台型管理差異(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

您可以大量編輯使用者帳戶。 當大量編輯使用者時，只有您特別選取的欄位會更新為所選的所有使用者提供相同的資訊。 您未選取的所有其他欄位，每位使用者都將維持不變，即使每位使用者各有不同。

>[!NOTE]
>
>* 您無法大量編輯使用者設定檔的個人資訊區段，因為此資訊對於每個使用者都必須是唯一的。
>* 為確保資料的準確性和最佳效能，建議您一次選取不超過2000名使用者進行大量編輯。
>

## 存取需求

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>. </p> </li> 
     <li> <p><b>使用者</b> 將存取層級中的設定設為 <b>編輯</b> 存取，使用 <b>建立</b> 以及兩者中的至少一個 <b>使用者管理員</b> 選項已啟用於 <b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>這兩個選項中，如果使用者 <b>管理員（群組使用者）</b> 已啟用，您必須是使用者所屬群組的群組管理員。</p> <p>如需關於的詳細資訊 <b>使用者</b> 在存取層級中設定，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 大量編輯使用者帳戶

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).

1. 選取多個使用者，然後按一下「編輯」圖示 ![](assets/edit-icon.png).

1. 在 **編輯使用者** 方塊中，變更下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">偏好設定</td> 
      <td> 
       <ul> 
        <li><b>時區：</b> 使用者的時區。</li> 
        <li><b>地區設定</b>：使用者偏好的地區設定。 這會影響來自Workfront之電子郵件中的數字和日期格式。</li> 
        <li><b>顯示更新狀態的完成百分比</b>：如果您想在使用舊版評論體驗時，在所有使用者工作的「更新」區域內顯示完成百分比列，請核取此選項。 如需詳細資訊，請參閱 <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">新的評論體驗</a>.</li> 
        <li><b>將我指派給我自己的工作傳送至我的「正在處理」標籤</b>：如果您希望使用者指派給自己的所有內容直接顯示在其工作索引標籤上，請核取此選項。 預設為在使用者的「工作請求」標籤上列出指派給使用者的所有內容。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通知</td> 
      <td>選取應為新使用者啟用的電子郵件通知。<p>您可以選取即時和每日摘要通知。 所有選定使用者的所有每日摘要通知會在同一時間傳送。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">為系統中的每個人設定事件通知</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">存取</td> 
      <td> 
       <ul> 
        <li><b>作用中：</b> 選取此欄位以指出使用者是否為使用中。 作用中使用者使用Workfront授權。 取消選取欄位會停用使用者。</li> 
        <li> 
        <p><b>存取層級：</b> 選取要指派給這些使用者的存取層級。 所有選取的使用者將具有相同的存取層級。
        </p> 
        <p>將存取層級指派給使用者時，可以指派等於或小於您自己的存取層級的層級。 （例如，如果您的存取層級是「供需規劃員」，則您無法指派「管理員」存取層級。） </p>
        <p>但是，如果Workfront管理員在存取層級上啟用了您自己未啟用的許可權（透過「微調」設定），則您無法指派低於您自己的存取層級，如所述 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>)。</p> 
        <p>如需存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">設定Adobe Workfront的存取權</a>.</p> 
         </li> 
        <li> 
        <p><b>版面配置範本</b>：選擇使用者的版面配置範本。 指派給使用者的版面配置範本優先於指派給其「主群組」、「主團隊」或「主要工作角色」的任何版面配置範本。 如需有關配置範本的指派優先順序的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立及管理版面範本</a>.</p> 
        <p><b>注意</b>：您可以在此欄位中使用的版面配置範本清單取決於您的存取權：
          <ul>
           <li>身為Workfront管理員，您可以檢視所有系統層級和群組層級的版面配置範本。</li>
           <li>身為群組管理員，您可以檢視系統層級版面配置範本，以及與您管理之群組相關聯的範本。</li>
           <li><p>作為具有Planner授權和編輯使用者存取權的使用者，您只能看到系統層級的版面配置範本。 </p>
           <p>如需群組層級配置範本的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立及管理版面範本</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">組織</td> 
      <td> 
       <ul> 
        <li><b>公司</b>：使用者的公司。 使用者只能與一個公司相關聯。 您必須先建立公司，然後才能與使用者建立關聯。 清單中只會顯示作用中的公司。 如需有關建立公司的資訊，請參閱瞭解和管理公司。</li> 
        <li><b>主團隊</b>：指定使用者的主團隊。 使用者只能有一個主團隊。 </li> 
        <li><b>其他團隊</b>：使用者可隸屬於多個團隊。 </li> 
        <li> <p><b>主群組：</b> 選取適當的群組以將使用者指派為其主群組。 這可讓使用者存取與群組共用的物件。</p> <p><b>注意</b>：此為必填欄位。 您無法讓使用者與主群組沒有關聯。</p> <p>您只能在下列情況下將群組指派給使用者：</p> 
         <ul> 
          <li>您是Workfront管理員。</li> 
          <li>您是該群組的管理員。</li> 
          <li>群組是公開的。</li> 
         </ul> </li> 
        <li> <p><b>其他群組</b>：使用者可屬於多個群組。 您只能在下列情況下將群組指派給使用者：</p> 
         <ul> 
          <li>您是Workfront管理員。</li> 
          <li>您是該群組的管理員。</li> 
          <li> <p>群組是公開的。 </p> 
          <p>如需公用群組的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">建立群組</a>.</p> 
          <p>如需群組的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群組概述</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">資源規劃</td> 
      <td> 
       <ul>

   <li>
       <b>工作時間</b>：代表使用者可用於實際工作（不包括額外負荷）的相當全職(FTE)時間百分比。 「工作時間」必須為最多1的小數，且不可以是0。 例如，實際工作的20%可用性為0.2。

   該欄位的預設值為1，這表示使用者將其整個FTE用於實際的、專案相關的工作。

   系統會使用此數字來計算使用者進行實際專案相關工作的可用性。

   如需有關在Workfront中建立排程的詳細資訊，請參閱 <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">建立排程</a>.

   排程例外和休假也可能會影響使用者容量。

   Workfront會根據您設定區域中的Resource Management偏好設定來計算使用者的可用性。 如需詳細資訊，請參閱 <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">設定資源管理喜好設定</a>.

   <b>秘訣</b>

   將「工作時間」值設為1，表示使用者可用於專案相關工作的整個全職同等工作。
   </li>

   <li><b>排程停用</b>：如果您想要排程在一段時間後停用使用者，請核取此方塊。</li> 
       <li><b>排程的停用日期</b>：停用使用者的截止日期。 如需排程使用者停用的詳細資訊，請參閱區段 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">排程使用者停用</a> 在 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>.</li> 
       <li> <p><b>主要角色</b>：這是使用者在Workfront中的主要職務角色。 根據預設，指派給使用者的每個任務和問題也會指派給此工作角色。 職務角色在資源管理中至關重要。 如需有關工作角色的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理職位角色</a></p> <p>只有當您擁有具有管理使用者存取權的計畫授權，或您是Workfront管理員時，才能更新此欄位。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.</p> </li> 
       <li>（視條件而定）如果您已選取 <b>主要角色</b>，則 <b>FTE可用性百分比</b> 欄位隨即顯示。 指定將使用者排程的時間百分比分配給此工作角色。 主要角色的FTE可用性百分比預設值為100%。</li> 
       <li> <p><b>其他角色</b>：使用者在Workfront中可以有多個職位角色。 職務角色在資源管理中至關重要。 使用者可以完成的工作角色數量沒有限制。 但是，我們建議不要將一位使用者指派給太多工作角色，因為這些使用者可能很難管理資源。</p> <p>如需有關工作角色的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理職位角色</a>.</p> <p>只有當您擁有具有管理使用者存取權的計畫授權，或您是Workfront管理員時，才能更新此欄位。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.</p> </li> 
       <li> <p>（視條件而定）如果您選取一或多個 <b>其他角色</b>，則 <b>FTE可用性百分比</b> 每個角色都會顯示欄位。 指定將使用者排程的時間百分比分配給每個工作角色。 其他角色的FTE可用性百分比預設值為0%。</p> <p><b>注意</b>：  
       <ul> 
       <li>如果「其他角色」具有0%的FTE可用性，除非將使用者指派給這些角色中的任務，否則它們不會顯示在「資源規劃工具」中。</li> 
       <li> <p>所有角色的所有FTE可用性百分比總和必須等於100%。 每個FTE可用性的百分比會計算「資源規劃工具」中每個使用者的「可用時數」。 每個使用者每個角色的可用時數取決於使用者的可用時數。</p> <p>使用者的可用時間由Workfront根據Workfront管理員在資源管理偏好設定中計算約當全職人數時所選取的方法計算。</p> <p>如需有關計算使用者可用性的詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">計算資源規劃工具中使用者和角色的時數和FTE的概觀</a>.</p> <p>如需有關設定資源管理偏好設定的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">設定資源管理喜好設定</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>排程</b>：將排程與使用者建立關聯。 使用者的排程會計算指派給使用者的任務的時間表。</p> <p>Workfront管理員或群組管理員必須先建立排程，才能與使用者建立關聯。</p> <p>選取系統層級或群組排程，將其指派給選取的使用者。</p> <p>如需有關系統層級和群組排程的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>.</p> <p><b>重要</b>：只有在「使用計算資源可用性」設定設為使用者的排程時，Workfront才會使用使用者的排程。 如需有關「使用計算資源可用性」設定如何影響用於「資源管理」之排程的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">設定資源管理喜好設定</a>.</p> </li> 
       <li> <p><b>週期性時程表</b>：建立週期性時程表與使用者的關聯。 這可確保自動為使用者產生時間表。</p> 
       <p><b>注意</b>：  
       <ul> 
       <li>您在此欄位中可用的週期性時程表清單取決於您的存取權：
       <ul>
       <li>身為Workfront管理員，您可以檢視所有系統層級和群組層級的時程表設定檔。</li>
       <li><p>作為群組管理員，您可以檢視系統層級的時程表設定檔，以及與您管理的群組相關聯的時程表設定檔。</p></li>
       <li><p>作為具有規劃工具授權和編輯使用者存取權的使用者，您只能看到系統層級的時程表設定檔。</p></li>
       </ul></li> 
       <li>如果您是群組管理員，您編輯的所有使用者都必須是您管理之群組的成員。</li> 
       </ul> </p> </li> 
       <li><b>預設時數型別</b>：為使用者選取預設時數型別。 這是使用者記錄時間時，預設使用的小時型別。</li> 
       <li> <p><b>可用小時型別</b>：選取使用者應能使用的小時型別。 這些小時型別在Workfront中任何使用者可記錄時間的位置都可見。 使用者只能看到在專案層級和使用者層級啟用的小時型別。</p> 
       <p>如需有關使用者可用的時數型別的詳細資訊，請參閱 <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">定義時程表的小時型別和可用性</a>.</p> 
       </li> 
       <li> <b>FTE</b>：這是使用者的全職同等功能。 只有當系統層級的「資源管理偏好設定」設定為「預設排程」時，Workfront才會根據預設排程使用此數字來計算使用者的可用性。

   <p>FTE代表使用者可在工作上花費的時間量。 這包括管理費用，以及在專案工作上所花費的時間。 例如，在會議或培訓中花費的時間也會納入FTE。</p>

   FTE必須是最高為1的小數位數，而且不能為0。 例如，如果FTE值為0.5，而Workfront中的預設排程為40小時，則使用者每週可使用20小時。

   欄位的預設值為1。

   排程例外、休假可能以及「工作時間」的值可能會影響使用者的可用性。

   Workfront會根據您設定區域中的Resource Management偏好設定來計算使用者的可用性。

   如果系統層級的「資源管理偏好設定」設定為「使用者排程」，則您在此處指定的值會被忽略，而且會根據排程中指定的內容，將使用者視為可用。

   如需詳細資訊，請參閱 <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">設定資源管理喜好設定</a>.

   如需有關在Workfront中建立排程的詳細資訊，請參閱 <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">建立排程</a>.
   </li> 
       <li> <p><b>資源集區</b>：將使用者與資源集區建立關聯。</p> <p><b>注意</b>：此欄位只會顯示所有選定使用者共用的資源集區。 如果選取的使用者沒有共用資源集區，則此欄位為空白。 如果此欄位空白，您在此指定的資源集區將會覆寫其個別資源集區。</p> 
       <p>如需有關資源集區的詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 資源集區概觀 </a>.</p> </li> 
       <li><b>成本/小時</b>：使用者每小時的成本金額。 </li> 
       <li><b>記帳/小時</b>：使用者每小時的計費金額。</li> 
       <li><b>自訂Forms</b>：將現有的使用者自訂表單與使用者建立關聯。 您必須先建立自訂表單，然後才能將其與使用者建立關聯。 清單中只會顯示作用中的自訂表單。 如需建立自訂表單的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a>.</li> 
       <li><b>註解</b>：在提供的欄位中輸入註解。 所有選取的使用者都會收到應用程式內通知以及包含您評論的電子郵件通知。 註解會顯示在使用者設定檔的更新索引標籤中。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）在 **自訂Forms** 區段，選取 **重新計算自訂運算式** 選項，確保附加到所選使用者的自訂表單中的所有計算自訂欄位都是最新狀態。

1. 按一下「**儲存變更**」。
