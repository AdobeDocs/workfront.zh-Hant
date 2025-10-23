---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 建立和編輯公司
description: 您可以將公司新增至 [!DNL Adobe Workfront] ，並將它們用於財務規劃、報告、定義物件相關許可權以及保密資訊。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 5e81e18ef667af3e4d08f4fc8987f7a3b6617971
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# 建立和編輯公司

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽沙箱」環境中使用，並且正在分階段推出到生產環境。</span>

公司是[!DNL Adobe Workfront]中的組織單位，可以代表您的組織、組織內的部門或您工作的客戶。 您可以將公司新增至[!DNL Workfront]，並將它們用於財務規劃、報告、定義物件相關許可權以及保密資訊。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] 封裝</p> </td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權</p> </td> 
   <td><p>[！UICONTROL計畫]</p>
   <p>[！UICONTROL標準]</p>
   </td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>[！UICONTROL系統管理員]存取層級，可讓您編輯系統中的任何公司。</p> </li> 
     <li> <p>管理公司的管理存取權，可讓您編輯系統中的任何公司。</p> </li> 
    </ul> <p><b>附註</b>：  
     <ul> 
      <li> <p>您也可以管理與您被指派為群組管理員的任何群組相關聯的公司。</p> </li> 
      <li> <p>若要從[!DNL Workfront]系統中新增和移除使用者，您必須具備下列其中一項：</p> 
       <ul> 
        <li> <p>[！UICONTROL系統管理員]存取層級。 </p> </li> 
        <li> <p>您的存取層級中的<b>[！UICONTROL Users]</b>設定已設定為<b>[！UICONTROL Edit]</b>存取，且<b>[！UICONTROL Create]</b>以及在<b>[！UICONTROL Fine-tune your settings]</b> <b>下啟用的兩個</b>[！UICONTROL User Admin]<img src="assets/gear-icon-in-access-levels.png">選項中的至少一個選項。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>在這兩個選項中，如果已啟用<b>[！UICONTROL User Admin (Group Users)]</b>，您必須是使用者所屬群組的群組管理員。</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將使用者新增至公司的好處 {#benefits-of-adding-users-to-a-company}

* 您可以將使用者與直接下屬建立關聯，藉此建立公司的組織圖。 只有來自同一公司的使用者才能新增為該公司其他使用者的直接下屬。
* 身為專案經理，您可以識別同一公司內的可用資源。
* 您可以選擇下列一或所有設定，讓公司之間的資訊保持私密：

   * 來自同一公司的使用者可以看到彼此的請求。

     如需有關[!DNL Workfront]管理員如何根據使用者的公司授予類似請求存取權的詳細資訊，請參閱[設定全系統的任務和問題偏好設定 [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences)一節中的[設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)中每個人的任務和問題偏好設定。

     如需有關群組管理員如何根據使用者的公司授予類似請求存取權的詳細資訊，請參閱[設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

   * 使用者只能看到與其公司相關聯的請求佇列。 如需限制要求佇列可見性的詳細資訊，請參閱[提供要求佇列的存取權](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md)。
   * 您可以限制使用者只能看見其公司中的使用者，或其公司和主要公司的使用者。 如需有關使用者隱私權的主要公司功能資訊，請參閱[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。
   * 使用者可以限制只讓公司使用者看到他們對專案進行的更新。 如需將更新設為公司私用的詳細資訊，請參閱[更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 在[!DNL Workfront]中建立或編輯公司 {#create-or-edit-a-company-in-workfront}

可新增的公司數目沒有限制。 但是，由於物件許可權可能發生問題，我們建議您限制您使用的公司數目 — 太多的片段可能會干擾使用者對工作專案的可見度。

根據預設，與您[!DNL Workfront]的執行個體相關聯的公司已在您的[!DNL Workfront]系統中建立，並且是您組織的主要公司。 其名稱與您的客戶名稱相同。 如需[!DNL Workfront]中客戶資訊的詳細資訊，請參閱[設定系統的基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

若要新增或編輯公司：

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 公司]**。

   公司清單隨即顯示。

1. 如果您正在新增公司，請按一下[新增公司]。****

   或

   如果您正在編輯現有的公司，請選取公司，然後按一下公司清單頂端的&#x200B;**[!UICONTROL 編輯]**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

1. 更新&#x200B;**基本資訊**&#x200B;區段中的下列資訊：

   * **公司名稱** <span class="preview">或&#x200B;**名稱**</span>：輸入公司的名稱。
   * **為使用中**：啟用此選項後，使用者可以找到公司並將其附加至他們建立和編輯的專案。 非作用中的公司無法附加到專案。 此選項預設為啟用。
   * **這是主要公司** <span class="preview">或&#x200B;**是主要公司**</span>：將公司指派為您組織的主要公司。 主要公司通常代表您大部分使用者工作所在的Workfront帳戶。

     您可以將一家公司或沒有公司指定為主要公司，但不得將多家公司指定為主要公司。 如需詳細資訊，請參閱[建立和修改自訂存取層級](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

     >[!NOTE]
     >
     >透過修改其存取層級，您可以限制使用者檢視其他使用者：僅在其主要公司中，或在其關聯的公司和主要公司中。 如需主要公司如何處理使用者存取層級的資訊，請參閱[建立和修改自訂存取層級](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

   * **群組**：如果某個群組與公司有業務往來，您可以在此新增該群組的名稱。 這對於需要報告和管理其群組業務所在的所有公司的群組管理員非常有用。

     如果您未關聯將與此公司合作的群組，則群組的管理員無法存取公司，除非他們擁有其存取層級中公司的管理存取權。 如需如何授與此存取權的資訊，請參閱[授與使用者對特定區域的管理存取權](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

     開始輸入群組的名稱，然後在其出現時選取它。

     將群組指派給公司時，該群組的群組管理員將取得公司的「管理」存取權。 如需詳細資訊，請參閱本文中的[群組管理員和公司](#group-administrators-and-companies)。

   * **公司成員**：新增現有的使用者到公司。 透過這樣做，您可將這些使用者與此公司建立關聯。

     開始輸入使用者的名稱，然後在其出現時選取它。

     您與一個公司建立關聯的使用者數量沒有限制，但一個使用者不能與多個公司建立關聯。

1. 在&#x200B;**自訂Forms**&#x200B;區段中新增或更新自訂表單。

   如果有任何您想要新增至公司的欄位無法在Workfront中使用，您可以建置自訂表單並將其與公司建立關聯。

   您可以從下拉式選單中選取此表單，以將其附加至您的公司。 只有作用中的自訂表單會列在功能表中。

   >[!NOTE]
   >
   >進階自訂表單功能(例如，外部查詢欄位和Workfront原生欄位)只有在您於詳細資訊頁面開啟公司記錄時，才可使用，不能在編輯公司對話方塊中開啟。 （從公司清單中，按一下公司名稱以開啟詳細資訊。）

   如需建立自訂表單的相關資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. （視條件而定）如果您正在建立公司，請按一下&#x200B;**[!UICONTROL 建立公司]**<span class="preview">或**&#x200B;儲存&#x200B;**。</span>

   或

   如果您正在編輯現有的公司，請按一下&#x200B;**[!UICONTROL 儲存變更]**<span class="preview">或**&#x200B;儲存&#x200B;**。</span>

## 管理公司成員資格

如需有關管理現有公司成員資格的資訊，請參閱[管理公司成員資格](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md)。

## 管理收費率

如需有關在公司層級覆寫收費率的資訊，請參閱[在公司層級](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)覆寫工作角色收費率。

## 與公司共用物件的概觀

與公司相關聯的使用者可以使用某些許可權，如[將使用者新增至公司的好處](#benefits-of-adding-users-to-a-company)一節中所述。 除了這些許可權之外，您還可以允許使用者透過與其公司共用物件來檢視、貢獻或編輯[!DNL Workfront]中的物件。

與其一次與一個個別使用者共用物件，您可以與其整個公司共用該物件。 公司中的每個使用者對該物件具有相同的許可權。

如需共用物件的詳細資訊，請參閱[共用物件許可權的總覽](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

## 群組管理員和公司 {#group-administrators-and-companies}

當[!DNL Workfront]管理員將群組指派給公司時，該群組的群組管理員會在[!UICONTROL 設定]中取得公司的[!UICONTROL 管理]存取權。 這包括存取[!UICONTROL 設定]中的[!UICONTROL 公司]頁面，他們可以在此頁面檢視和管理與其群組關聯的公司。

有了此[!UICONTROL 公司]頁面的存取權，群組管理員可以將群組指派給公司，但是它必須是群組管理員建立的公司。 如果群組管理員的存取層級未設定公司的管理存取權，則當群組管理員建立公司時，需要[!UICONTROL 群組]欄位，其粗體標題指示如下：

![編輯公司](assets/group-admin-add-company.png)

若要瞭解使用者如何取得其存取層級中公司的管理存取權，請參閱[授與使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

如需在[!UICONTROL 設定]區域管理公司的相關資訊，請參閱本文中的[在 [!DNL Workfront]](#create-or-edit-a-company-in-workfront)中建立或編輯公司。

<!-- OLD HTML TABLE
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] section</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Type a name for the company.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: When this option is enabled, users can find the company and attach it to projects that they create and edit. An inactive company cannot be attached to projects. This option is enabled by default.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Assigns the company as your organization's primary company. The primary company typically represents your [!DNL Workfront] account where most of your users work.</p> <p>You can have one company or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p><b>NOTE</b>: By modifying their access levels, you can restrict users to see other users: only in their primary company, or in their associated company and the primary company. For information about how the primary company works with users' access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: If there is a group that conducts business with the company, you can add the name of the group here. This is useful for group administrators who need to report on and manage all the companies that their groups do business with.</p> <p><b>IMPORTANT</b>: If you don't associate the group that will be working with this company, administrators for the group can't access the company unless they have administrative access to companies in their access level. For information about how this access is granted, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Start typing the name of the group, then press <strong>[!UICONTROL Enter]</strong> when it appears.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">When you assign a group to a company, the group administrators for the group gain [!UICONTROL Manage] access to the company. For more information, see <a href="#group-administrators-and-companies" class="MCXref xref">Group administrators and companies</a> in this article.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] section</td> 
      <td> <p>If there are fields that you want to add to your company that are not available in [!DNL Workfront], you can build a custom form and associate it with your company. </p> <p>You can attach this form to your company by selecting it from the drop-down menu. Only active custom forms are listed in the menu.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the company record on the details page, not on the Edit Company dialog. (From the list of companies, click the company name to open the details.)</p> <p> For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>
   -->
