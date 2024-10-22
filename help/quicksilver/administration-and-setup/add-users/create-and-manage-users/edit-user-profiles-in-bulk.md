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
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 0%

---

# 大量編輯使用者設定檔

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
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
   <td><p>新增：標準</p><p>或</p><p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 </li> 
     <li> <p>您的存取層級中的<b>使用者</b>設定已設定為<b>編輯</b>存取權，其中<b>建立</b>以及在<b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">下啟用的兩個<b>使用者管理員</b>選項中的至少一個。 </p> <p>在這兩個選項中，如果已啟用<b>使用者管理員（群組使用者）</b>，您必須是使用者所屬群組的群組管理員。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 大量編輯使用者帳戶

{{step-1-to-users}}

1. 選取多個使用者，然後按一下「編輯」圖示![](assets/edit-icon.png)。

1. 在出現的&#x200B;**編輯使用者**&#x200B;方塊中，變更下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">偏好設定</td> 
      <td> 
       <ul> 
        <li><b>時區：</b>使用者的時區。</li> 
        <li><b>地區</b>：使用者偏好的地區。 這會影響來自Workfront之電子郵件中的數字和日期格式。</li> 
        <li><b>將我指派給自己的工作傳送至我的「正在處理」標籤</b>：此設定參考已從Workfront移除的已棄用功能。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通知</td> 
      <td>選取應為新使用者啟用的電子郵件通知。<p>您可以選取即時和每日摘要通知。 所有選定使用者的所有每日摘要通知會在同一時間傳送。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">設定系統中每個人的事件通知</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">存取</td> 
      <td> 
       <ul> 
        <li><b>作用中：</b>選取此欄位以指出使用者是否作用中。 作用中使用者使用Workfront授權。 取消選取欄位會停用使用者。</li> 
        <li> 
        <p><b>存取層級：</b>選取要指派給這些使用者的存取層級。 所有選取的使用者將具有相同的存取層級。
        </p> 
        <p>將存取層級指派給使用者時，可以指派等於或小於您自己的存取層級的層級。 （例如，如果您的存取層級是「供需規劃員」，則您無法指派「管理員」存取層級。） </p>
        <p>但是，如果Workfront管理員已啟用存取層級的許可權，但您自己未啟用，則您無法指派低於您自己的存取層級（透過「微調」設定，如<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>中所述）。</p> 
        <p>如需存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">設定Adobe Workfront的存取權</a>。</p> 
         </li> 
        <li> 
        <p><b>配置範本</b>：選擇使用者的配置範本。 指派給使用者的版面配置範本優先於指派給其「主群組」、「主團隊」或「主要工作角色」的任何版面配置範本。 如需配置範本的指派優先順序的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立和管理配置範本</a>。</p> 
        <p><b>注意</b>：您在此欄位中可用的版面配置範本清單取決於您的存取權：
          <ul>
           <li>身為Workfront管理員，您可以檢視所有系統層級和群組層級的版面配置範本。</li>
           <li>身為群組管理員，您可以檢視系統層級版面配置範本，以及與您管理之群組相關聯的範本。</li>
           <li><p>作為具有Planner授權和編輯使用者存取權的使用者，您只能看到系統層級的版面配置範本。 </p>
           <p>如需群組層級配置範本的相關資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立和管理配置範本</a>。</p>
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
        <li><b>其他團隊</b>：使用者可以屬於多個團隊。 </li> 
        <li> <p><b>主群組：</b>選取適當的群組，將使用者指派為其主群組。 這可讓使用者存取與群組共用的物件。</p> <p><b>注意</b>：這是必要欄位。 您無法讓使用者與主群組沒有關聯。</p> <p>您只能在下列情況下將群組指派給使用者：</p> 
         <ul> 
          <li>您是Workfront管理員。</li> 
          <li>您是該群組的管理員。</li> 
          <li>群組是公開的。</li> 
         </ul> </li> 
        <li> <p><b>其他群組</b>：使用者可以屬於多個群組。 您只能在下列情況下將群組指派給使用者：</p> 
         <ul> 
          <li>您是Workfront管理員。</li> 
          <li>您是該群組的管理員。</li> 
          <li> <p>群組是公開的。 </p> 
          <p>如需公用群組的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">建立群組</a>。</p> 
          <p>如需群組的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群組概述</a>。</p> 
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
       <b>工作時間</b>：代表使用者可用於實際工作的全職相當時間(FTE)百分比，不包括額外負荷。 「工作時間」必須為最多1的小數，且不可以是0。 例如，實際工作的20%可用性為0.2。

   該欄位的預設值為1，這表示使用者將其整個FTE用於實際的、專案相關的工作。

   系統會使用此數字來計算使用者進行實際專案相關工作的可用性。

   如需有關在Workfront中建立排程的詳細資訊，請參閱<a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">建立排程</a>。

   排程例外和休假也可能會影響使用者容量。

   Workfront會根據您設定區域中的Resource Management偏好設定來計算使用者的可用性。 如需詳細資訊，請參閱<a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">設定資源管理喜好設定</a>。

   <b>提示</b>

   將「工作時間」值設為1，表示使用者可用於專案相關工作的整個全職同等工作。
   </li>

   <li><b>排程停用</b>：如果您要排程使用者在一段時間後停用，請勾選此方塊。</li> 
       <li><b>已排程的停用日期</b>：停用使用者的日期。 如需排程使用者停用的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>中的<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">排程使用者停用</a>一節。</li> 
       <li> <p><b>主要角色</b>：這是使用者在Workfront中的主要工作角色。 根據預設，指派給使用者的每個任務和問題也會指派給此工作角色。 職務角色在資源管理中至關重要。 如需有關工作角色的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理工作角色</a></p> <p>只有當您擁有具有管理使用者存取權的計畫授權，或您是Workfront管理員時，才能更新此欄位。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>。</p> </li> 
       <li>（視條件而定）如果您選取<b>主要角色</b>，則會顯示<b>FTE可用性百分比</b>欄位。 指定將使用者排程的時間百分比分配給此工作角色。 主要角色的FTE可用性百分比預設值為100%。</li> 
       <li> <p><b>其他角色</b>：使用者可以在Workfront中擁有多個工作角色。 職務角色在資源管理中至關重要。 使用者可以完成的工作角色數量沒有限制。 但是，我們建議不要將一位使用者指派給太多工作角色，因為這些使用者可能很難管理資源。</p> <p>如需有關工作角色的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理工作角色</a>。</p> <p>只有當您擁有具有管理使用者存取權的計畫授權，或您是Workfront管理員時，才能更新此欄位。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>。</p> </li> 
       <li> <p>（視條件而定）如果您選取一或多個<b>其他角色</b>，則會針對每個角色顯示<b>FTE可用性百分比</b>欄位。 指定將使用者排程的時間百分比分配給每個工作角色。 其他角色的FTE可用性百分比預設值為0%。</p> <p><b>附註</b>：  
       <ul> 
       <li>如果「其他角色」具有0%的FTE可用性，除非將使用者指派給這些角色中的任務，否則它們不會顯示在「資源規劃工具」中。</li> 
       <li> <p>所有角色的所有FTE可用性百分比總和必須等於100%。 每個FTE可用性的百分比會計算「資源規劃工具」中每個使用者的「可用時數」。 每個使用者每個角色的可用時數取決於使用者的可用時數。</p> <p>使用者的可用時間由Workfront根據Workfront管理員在資源管理偏好設定中計算約當全職人數時所選取的方法計算。</p> <p>如需有關計算使用者可用性的詳細資訊，請參閱<a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">計算資源規劃工具中使用者和角色的時數和FTE的概觀</a>。</p> <p>如需有關設定資源管理偏好設定的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">設定資源管理偏好設定</a>。</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>排程</b>：將排程與使用者建立關聯。 使用者的排程會計算指派給使用者的任務的時間表。</p> <p>Workfront管理員或群組管理員必須先建立排程，才能與使用者建立關聯。</p> <p>選取系統層級或群組排程，將其指派給選取的使用者。</p> <p>如需有關系統層級和群組排程的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>。</p> <p><b>重要</b>： Workfront僅在「計算資源使用狀態」設定設為「使用者的排程」時，才會使用使用者的排程。 如需有關使用計算資源可用性設定如何影響用於資源管理的排程的資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">設定資源管理喜好設定</a>。</p> </li> 
       <li> <p><b>時程表設定檔</b>：將時程表設定檔與使用者建立關聯。 這可確保自動為使用者產生時間表。</p> 
       <p><b>附註</b>：  
       <ul> 
       <li>您在此欄位中可用的週期性時程表清單取決於您的存取權：
       <ul>
       <li>身為Workfront管理員，您可以檢視所有系統層級和群組層級的時程表設定檔。</li>
       <li><p>作為群組管理員，您可以檢視系統層級的時程表設定檔，以及與您管理的群組相關聯的時程表設定檔。</p></li>
       <li><p>作為具有規劃工具授權和編輯使用者存取權的使用者，您只能看到系統層級的時程表設定檔。</p></li>
       </ul></li> 
       <li>如果您是群組管理員，您編輯的所有使用者都必須是您管理之群組的成員。</li> 
       </ul> </p> </li> 
       <li><b>預設小時型別</b>：為使用者選取預設小時型別。 這是使用者記錄時間時，預設使用的小時型別。</li> 
       <li> <p><b>可用時數型別</b>：選取使用者應該可用的時數型別。 這些小時型別在Workfront中任何使用者可記錄時間的位置都可見。 使用者只能看到在專案層級和使用者層級啟用的小時型別。</p> 
       <p>如需使用者可以使用哪些時數型別的詳細資訊，請參閱<a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">定義時數型別和可用性</a>。</p> 
       </li> 
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
       <li> <p><b>資源集區</b>：將使用者與資源集區建立關聯。</p> <p><b>注意</b>：此欄位只會顯示所有選取使用者共用的資源集區。 如果選取的使用者沒有共用資源集區，則此欄位為空白。 如果此欄位空白，您在此指定的資源集區將會覆寫其個別資源集區。</p> 
       <p>如需資源集區的詳細資訊，請參閱<a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">資源集區概述</a>。</p> </li> 
       <li><b>每小時成本</b>：使用者每小時的成本金額。 </li> 
       <li><b>每小時計費</b>：使用者每小時的計費金額。</li> 
       <li><b>自訂Forms</b>：將現有的使用者自訂表單與使用者建立關聯。 您必須先建立自訂表單，然後才能將其與使用者建立關聯。 清單中只會顯示作用中的自訂表單。 如需建立自訂表單的相關資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">使用表單設計工具設計表單</a>。</li> 
       <li><b>註解</b>：在提供的欄位中輸入註解。 所有選取的使用者都會收到應用程式內通知以及包含您評論的電子郵件通知。 註解會顯示在使用者設定檔的更新索引標籤中。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）在&#x200B;**自訂Forms**&#x200B;區段中，選取&#x200B;**重新計算自訂運算式**&#x200B;選項，以確保附加到所選使用者的自訂表單中的所有計算自訂欄位都是最新狀態。

1. 按一下「**儲存變更**」。
