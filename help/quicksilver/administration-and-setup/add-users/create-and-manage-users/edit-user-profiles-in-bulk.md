---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 大量編輯使用者設定檔
description: 身為Adobe Workfront管理員，您可以大量編輯使用者帳戶。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# 大量編輯使用者設定檔

>[!IMPORTANT]
>
>本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>如需在Adobe Admin Console中編輯使用者設定檔的指示，請參閱文章中的「編輯使用者詳細資料」一節 [大量上傳使用者](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) 或聯絡您的Adobe Admin Console管理員。
>
>如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

您可以大量編輯使用者帳戶。 批量編輯用戶時，只有您專門選擇的欄位會更新為所有選定用戶的相同資訊。 您未選取的所有其他欄位對每個個別使用者而言都會保持相同，即使每個使用者的欄位不同亦然。

>[!NOTE]
>
>* 您無法大量編輯使用者設定檔的「個人資訊」區段，因為該資訊對於每個使用者都必須是唯一的。
>* 為確保資料的準確性和最佳效能，建議您一次選取不超過2000位使用者，進行大量編輯。
>


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

## 大量編輯使用者帳戶

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).

1. 選取多個使用者，然後按一下「編輯」圖示 ![](assets/edit-icon.png).

1. 在 **編輯用戶** 框中，更改以下任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">喜好設定</td> 
      <td> 
       <ul> 
        <li><b>時區：</b> 使用者的時區。</li> 
        <li><b>地區</b>:用戶首選的區域設定。 這會影響來自Workfront之電子郵件中的數字和日期格式。</li> 
        <li><b>顯示更新狀態完成百分比</b>:如果要在更新任務流內顯示所有用戶的完成百分比欄，請核取此選項。</li> 
        <li><b>將我指派給自己的工作發送到「工作」頁簽</b>:如果希望用戶指派給自己的所有內容都直接顯示在其「正在工作」(Working On)頁簽上，請核取此選項。 預設值是在其「工作請求」索引標籤中列出指派給使用者的所有內容。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">通知</td> 
      <td>選取應為新使用者啟用的電子郵件通知。<p>您可以選取即時通知和每日摘要通知。 所有選取的使用者，在同一時間之後的某個時間，會傳送所有每日摘要通知。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">為系統中的每個人配置事件通知</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">存取</td> 
      <td> 
       <ul> 
        <li><b>活動：</b> 選取此欄位以指出使用者是否使用中。 作用中使用者使用Workfront授權。 取消選取欄位會停用使用者。</li> 
        <li> 
        <p><b>訪問級別：</b> 選擇要分配給這些用戶的訪問級別。 所有選取的使用者都會有相同的存取層級。
        </p> 
        <p>將訪問級別分配給用戶時，可以將一個級別分配給等於或小於您自己的訪問級別。 （例如，如果訪問級別為「計畫員」，則無法分配管理員訪問級別。） </p>
        <p>不過，如果Workfront管理員已對您未自行啟用的存取層級啟用權限，則您無法指派低於您自己的存取層級（透過微調設定），如 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>)。</p> 
        <p>有關訪問級別的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">設定Adobe Workfront的存取權</a>.</p> 
         </li> 
        <li> 
        <p><b>版面範本</b>:為使用者選擇版面範本。 分配給用戶的佈局模板將優先於分配給其「主組」、「主組」或「主作業」角色的任何佈局模板。 有關佈局模板的分配優先順序的詳細資訊，請參見 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立和管理版面範本</a>.</p> 
        <p><b>注意</b>:您在此欄位中可用的版面範本清單取決於您的存取權：
          <ul>
           <li>身為Workfront管理員，您可以查看所有系統層級和群組層級的版面範本。</li>
           <li>身為群組管理員，您可以查看系統層級版面範本，以及與您管理之群組相關聯的範本。</li>
           <li><p>作為具有計畫員許可證和編輯用戶訪問權限的用戶，您只能查看系統級佈局模板。 </p>
           <p>如需群組層級配置範本的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立和管理版面範本</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">組織</td> 
      <td> 
       <ul> 
        <li><b>公司</b>:使用者的公司。 使用者只能與一個公司相關聯。 您必須先建立公司，才能將其與使用者建立關聯。 清單中只會顯示作用中的公司。 有關建立公司的資訊，請參閱了解和管理公司。</li> 
        <li><b>主隊</b>:指定使用者的主團隊。 使用者只能有一個主團隊。 </li> 
        <li><b>其他團隊</b>:使用者可屬於多個團隊。 </li> 
        <li> <p><b>家庭組：</b> 選取適當的群組，將使用者指派為其首頁群組。 這可讓使用者存取與群組共用的物件。</p> <p><b>注意</b>:這是必填欄位。 不能有未與首頁組關聯的用戶。</p> <p>只有在下列情況下，您才可將群組指派給使用者：</p> 
         <ul> 
          <li>您是Workfront管理員。</li> 
          <li>您是該群組的管理員。</li> 
          <li>這個群體是公開的。</li> 
         </ul> </li> 
        <li> <p><b>其他群組</b>:使用者可屬於多個群組。 只有在下列情況下，您才可將群組指派給使用者：</p> 
         <ul> 
          <li>您是Workfront管理員。</li> 
          <li>您是該群組的管理員。</li> 
          <li> <p>這個群體是公開的。 </p> 
          <p>如需公開群組的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">建立群組</a>.</p> 
          <p>如需群組的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群組概觀</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">資源規劃</td> 
      <td> 
       <ul> 
        <li><b>計畫停用</b>:如果您想要排程在一段時間後停用使用者，請核取此方塊。</li> 
        <li><b>計畫的停用日期</b>:使用者停用的日期。 如需排程使用者停用的詳細資訊，請參閱區段 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">排程使用者停用</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>.</li> 
        <li> <p><b>主要角色</b>:這是使用者在Workfront中擁有的主要工作角色。 預設情況下，將用戶分配到的每個任務和問題也分配給此作業角色。 作業角色在資源管理中是必不可少的。 有關作業角色的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a></p> <p>只有在您擁有具有管理用戶訪問權限的計畫許可證，或者您是Workfront管理員時，才能更新此欄位。 有關設定具有管理用戶訪問權限的用戶的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
        <li>（條件性）如果您選取 <b>主要角色</b>, <b>FTE可用性百分比</b> 欄位。 指定分配給此作業角色的用戶調度的時間百分比。 主要角色的FTE可用性百分比的預設值為100%。</li> 
        <li> <p><b>其他角色</b>:使用者在Workfront中可以有多個工作角色。 作業角色在資源管理中是必不可少的。 用戶可履行的職務數沒有限制。 但是，我們建議不要將一個用戶分配給過多的作業角色，因為對這些用戶來說，資源管理可能變得太複雜了。</p> <p>有關作業角色的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a>.</p> <p>只有在您擁有具有管理用戶訪問權限的計畫許可證，或者您是Workfront管理員時，才能更新此欄位。 有關設定具有管理用戶訪問權限的用戶的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
        <li> <p>（條件性）如果您選取一或多個 <b>其他角色</b>, <b>FTE可用性百分比</b> 欄位隨即顯示。 指定分配給每個作業角色的用戶調度的時間百分比。 其他角色的FTE可用性百分比的預設值為0%。</p> <p><b>附註</b>:  
          <ul> 
           <li>如果其他職責的FTE可用性為0%，則它們不會顯示在資源計畫器中，除非將用戶分配給這些職責中的任務。</li> 
           <li> <p>所有角色的FTE可用性的所有百分比之和必須等於100%。 每個FTE可用性百分比計算資源計畫員中每個用戶每個角色的可用小時數。 每個用戶的每個角色的可用小時數取決於用戶的可用時間。</p> <p>用戶的可用時間由Workfront計算，具體取決於Workfront管理員在「資源管理首選項」中選擇的計算FTE的方法。</p> <p>有關計算用戶可用性的詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">在資源計畫員中計算用戶和角色的小時數和FTE的概覽</a>.</p> <p>有關配置資源管理首選項的詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置資源管理首選項</a>.</p> </li> 
          </ul> </p> </li> 
        <li> <p><b>排程</b>:將排程與使用者建立關聯。 用戶的時間表計算分配給用戶的任務的時間表。</p> <p>Workfront管理員或群組管理員必須先建立排程，才能與使用者建立關聯。</p> <p>選擇系統級或組計畫，將其分配給選定用戶。</p> <p>有關係統級和組計畫的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>.</p> <p><b>重要</b>:只有在「使用計算資源可用性」設定設為「使用者的排程」時，Workfront才會使用使用者的排程。 有關「使用計算資源可用性」設定如何影響用於資源管理的計畫的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置資源管理首選項</a>.</p> </li> 
        <li> <p><b>時間表配置檔案</b>:將時間表配置檔案與用戶關聯。 這可確保為用戶自動生成工時單。</p> 
        <p><b>附註</b>:  
          <ul> 
           <li>您在此欄位中可用的時間表配置檔案清單取決於您的訪問權限：
            <ul>
             <li>作為Workfront管理員，您可以查看所有系統級和組級時間表配置檔案。</li>
             <li><p>作為組管理員，您可以查看系統級時間表配置檔案以及與您管理的組關聯的時間表配置檔案。</p></li>
             <li><p>作為具有計畫員許可證和編輯用戶訪問權限的用戶，您只能查看系統級時間表配置檔案。</p></li>
            </ul></li> 
           <li>如果您是群組管理員，您編輯的所有使用者都必須是您所管理之群組的成員。</li> 
          </ul> </p> </li> 
        <li><b>預設小時類型</b>:為用戶選擇預設的小時類型。 這是使用者記錄時間時，預設使用的小時類型。</li> 
        <li> <p><b>可用小時類型</b>:選取使用者應可使用的小時類型。 這些小時類型在Workfront中任何地方都可見，使用者可在其中記錄時間。 使用者只能查看專案層級和使用者層級已啟用的小時類型。</p> 
        <p>如需使用者可使用的小時類型詳細資訊，請參閱 <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">定義工時單的工時類型和可用性</a>.</p> 
        </li> 
        <li> <p><b>FTE</b>:只有當系統級別的「資源管理首選項」設定為 <b>預設排程</b>.</p> 
        <p>例如，如果FTE值為0.5，預設計畫為40小時，則用戶每週可工作20小時。 有關選擇「預設計畫」時計畫異常或超時可能如何影響用戶可用性的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置資源管理首選項</a>. </p> 
        <p>如果系統級別上的「資源管理首選項」設定為 <b>使用者的排程</b>，則會忽略您在此指定的值，且會根據使用者的排程指定內容，將使用者視為可用。 在這種情況下，資源計畫員的用戶FTE按以下公式計算：</p>
        <p><code style="font-style: normal;">User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code> </p> <p>有關計算用戶FTE的詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">在資源計畫員中計算用戶和角色的小時數和FTE的概覽</a>.</p> <p>如需在Workfront中建立排程的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>.</p> <p>有關配置資源管理首選項的詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">配置資源管理首選項</a>.</p> 
        </li> 
        <li> <p><b>資源池</b>:將用戶與資源池關聯。</p> <p><b>注意</b>:此欄位中只會顯示所有所選使用者的共同資源池。 如果所選用戶沒有共用資源池，則此欄位為空。 如果此欄位為空，則在此處指定的資源池將覆蓋其各個資源池。</p> 
        <p>有關資源池的詳細資訊，請參見 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 資源池概述 </a>.</p> </li> 
        <li><b>每小時成本</b>:使用者每小時的成本金額。 </li> 
        <li><b>每小時計費</b>:使用者每小時的計費金額。</li> 
        <li><b>自訂Forms</b>:將現有用戶自定義表單與用戶關聯。 您必須先建立自訂表單，才能將其與使用者建立關聯。 清單中只會顯示使用中的自訂表單。 如需建立自訂表單的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a>.</li> 
        <li><b>註解</b>:在提供的欄位中輸入注釋。 所有選取的使用者都會收到應用程式內通知，以及含有您意見的電子郵件通知。 註解會顯示在使用者設定檔的「更新」標籤中。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）在 **自訂Forms** 區段，選取 **重新計算自定義運算式** 選項，確保附加至所選使用者的自訂表單中所有計算的自訂欄位都是最新的。

1. 按一下 **儲存變更**.
