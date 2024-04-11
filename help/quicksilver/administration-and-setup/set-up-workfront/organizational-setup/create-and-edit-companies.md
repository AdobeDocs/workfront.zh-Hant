---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 建立和編輯公司
description: 您可以將公司新增至 [!DNL Adobe Workfront] 並將它們用於財務規劃、報表、定義物件相關許可權以及保密資訊。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 0%

---

# 建立和編輯公司

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

公司是中的組織單位 [!DNL Adobe Workfront] 可以代表您的組織、組織內的部門或您合作的客戶。 您可以將公司新增至 [!DNL Workfront] 並將它們用於財務規劃、報表、定義物件相關許可權以及保密資訊。

## 存取需求

若要管理中的公司，您必須具備下列條件 [!DNL Workfront]：

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] 計劃</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 授權*</p> </td> 
   <td><p>目前： [！UICONTROL計畫]</p>
   或
   <p>新增：[！UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>下列其中一項：</p> 
    <ul> 
     <li> <p>[！UICONTROL系統管理員]存取層級，可讓您編輯系統中的任何公司。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md">授予使用者完整管理存取權</a>. </p> </li> 
     <li> <p>管理公司的管理存取權，可讓您編輯系統中的任何公司。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md">授予使用者管理特定區域的存取權</a>.</p> </li> 
    </ul> <p><b>注意</b>：  
     <ul> 
      <li> <p>您也可以管理與您被指派為群組管理員的任何群組相關聯的公司。</p> </li> 
      <li> <p>若要新增和移除使用者，請 [!DNL Workfront] 系統，您必須具備下列其中一項：</p> 
       <ul> 
        <li> <p>[！UICONTROL系統管理員]存取層級。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>. </p> </li> 
        <li> <p>在您的存取層級中，必須為[！UICONTROL使用者]設定選取[！UICONTROL編輯] 。 此外，針對[！UICONTROL使用者]設定，請在[！UICONTROL下微調您的設定] <img src="assets/gear-icon-in-access-levels.png">，則必須啟用[！UICONTROL Create]選項以及兩個[！UICONTROL User Admin]選項中的至少一個。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>如果您使用[！UICONTROL使用者管理員（群組使用者）]選項，您必須是使用者所屬群組的群組管理員。</p> </li> 
       </ul> <p>如需存取層級中「使用者」設定的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取層級設定，請聯絡您的 [!DNL Workfront] 管理員。 如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 將使用者新增至公司的好處 {#benefits-of-adding-users-to-a-company}

* 您可以將使用者與直接下屬建立關聯，藉此建立公司的組織圖。 只有來自同一公司的使用者才能新增為該公司其他使用者的直接下屬。
* 身為專案經理，您可以識別同一公司內的可用資源。
* 您可以選擇下列一或所有設定，讓公司之間的資訊保持私密：

   * 來自同一公司的使用者可以看到彼此的請求。

     如需關於如何 [!DNL Workfront] 管理員可以根據使用者的公司授予請求類似的存取權，請參閱區段 [設定每個人的任務和問題偏好設定 [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) 在文章中 [設定系統範圍的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

     如需群組管理員如何根據使用者的公司授予請求類似存取權的詳細資訊，請參閱 [設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   * 使用者只能看到與其公司相關聯的請求佇列。 如需限制要求佇列可見性的詳細資訊，請參閱 [提供請求佇列的存取權](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md).
   * 您可以限制使用者只能看見其公司中的使用者，或其公司和主要公司的使用者。 如需有關使用者隱私權的主要公司功能資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   * 使用者可以限制只讓公司使用者看到他們對專案進行的更新。 如需有關將更新設為公司私人的詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## 在中建立或編輯公司 [!DNL Workfront] {#create-or-edit-a-company-in-workfront}

可新增的公司數目沒有限制。 但是，由於物件許可權可能發生問題，我們建議您限制您使用的公司數目 — 太多的片段可能會干擾使用者對工作專案的可見度。

根據預設，與您執行個體相關聯的公司 [!DNL Workfront] 已在您的中建立 [!DNL Workfront] 系統，是您組織的主要公司。 其名稱與您的客戶名稱相同。 如需有關您客戶資訊的詳細資訊，請參閱 [!DNL Workfront]，請參閱 [設定系統的基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

若要新增或編輯公司：

{#step-1-to-setup}

1. 按一下 **[!UICONTROL 公司]**.

   公司清單隨即顯示。
1. 如果您要新增公司，請按一下 **[!UICONTROL 建立公司]**.

   或

   如果您正在編輯現有的公司，請選取公司，然後按一下 **[!UICONTROL 編輯]** 位於公司清單頂端。

1. 更新下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL基本資訊]區段</td> 
      <td> 
       <ul> 
        <li> <p><b>[！UICONTROL公司名稱]</b>：輸入公司的名稱。</p> </li> 
        <li> <p><b>[！UICONTROL作用中]</b>：啟用此選項後，使用者可以找到公司並將其附加至建立和編輯的專案。 非作用中的公司無法附加到專案。 此選項預設為啟用。</p> </li> 
        <li> <p><b>[！UICONTROL這是主要公司]</b>：將公司指派為您組織的主要公司。 主要公司通常代表您的 [!DNL Workfront] 大部分使用者工作的帳戶。</p> <p>您可以將一家公司或沒有公司指定為主要公司，但不得將多家公司指定為主要公司。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> <p><b>注意</b>：透過修改其存取層級，您可以限制使用者只能看見其他使用者：僅限在其主要公司中，或在其關聯的公司和主要公司中。 如需主要公司如何處理使用者存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </li> 
        <li> <p><b>[！UICONTROL群組]</b>：如果存在與公司進行業務的群組，您可以在此處新增群組名稱。 這對於需要報告和管理其群組業務所在的所有公司的群組管理員非常有用。</p> <p><b>重要</b>：如果您未關聯將與此公司合作的群組，則群組的管理員無法存取公司，除非他們擁有存取層級中公司的管理存取權。 如需如何授與此存取權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者管理特定區域的存取權</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">開始輸入群組名稱，然後按 <strong>[！UICONTROL Enter]</strong> 當它出現時。</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">將群組指派給公司時，該群組的群組管理員會獲得[！UICONTROL管理]公司存取權。 如需詳細資訊，請參閱 <a href="#group-administrators-and-companies" class="MCXref xref">群組管理員和公司</a> 本文章內容。</p> </li> 
        <li> <p><b>[！UICONTROL公司成員]</b>：將現有使用者新增至公司。 透過這樣做，您可將這些使用者與此公司建立關聯。</p> <p>您與一個公司建立關聯的使用者數量沒有限制，但一個使用者不能與多個公司建立關聯。</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[！UICONTROL自訂Forms]區段</td> 
      <td> <p>如果存在您想要新增至公司的欄位，但該欄位在中無法使用 [!DNL Workfront]，您可以建立自訂表單，並將其與您的公司建立關聯。 </p> <p>您可以從下拉式選單中選取此表單，以將其附加至您的公司。 只有作用中的自訂表單會列在功能表中。</p> <p><strong>注意：</strong> 進階自訂表單功能(例如，外部查詢欄位和Workfront原生欄位)只有在您於詳細資訊頁面開啟公司記錄時，才可使用，不能在編輯公司對話方塊中開啟。 （從公司清單中，按一下公司名稱以開啟詳細資訊。）</p> <p> 如需建立自訂表單的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>

1. （視條件而定）如果您正在建立公司，請按一下 **[!UICONTROL 建立公司]**.

   或

   如果您正在編輯現有公司，請按一下 **[!UICONTROL 儲存變更]**.

## 管理公司成員資格

如需有關管理現有公司成員資格的資訊，請參閱 [管理公司成員資格](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## 管理收費率

如需有關在公司層級覆寫收費率的資訊，請參閱 [覆寫公司層級的工作角色收費率](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

## 與公司共用物件的概觀

與公司相關聯的使用者可使用某些許可權，如區段中所述 [將使用者新增至公司的好處](#benefits-of-adding-users-to-a-company). 除了這些許可權之外，您還可以允許使用者在中檢視、貢獻或編輯物件的許可權 [!DNL Workfront] 透過與他們的公司共用物件。

與其一次與一個個別使用者共用物件，您可以與其整個公司共用該物件。 公司中的每個使用者對該物件具有相同的許可權。

如需共用物件的詳細資訊，請參閱 [物件許可權共用概觀](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## 群組管理員和公司 {#group-administrators-and-companies}

當 [!DNL Workfront] 管理員將群組指派給公司，群組管理員可取得群組收益 [!UICONTROL 管理] 存取中的公司 [!UICONTROL 設定]. 這包含對的存取 [!UICONTROL 公司] 頁面位置 [!UICONTROL 設定]，可讓他們檢視及管理與其群組相關聯的公司。

透過此許可權可存取 [!UICONTROL 公司] 頁面上，群組管理員可以將群組指派給公司，但是它必須是群組管理員建立的公司。 如果群組管理員的存取層級未設定為對公司的管理存取權， [!UICONTROL 群組] 當群組管理員建立公司時，需要欄位，其粗體標題指示如下：

![編輯公司](assets/group-admin-add-company.png)

如需有關使用者如何在其存取層級中取得公司的管理存取權的資訊，請參閱 [授予使用者管理特定區域的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

有關管理中公司的資訊 [!UICONTROL 設定] 區域，請參閱 [在中建立或編輯公司 [!DNL Workfront]](#create-or-edit-a-company-in-workfront) 本文章內容。
