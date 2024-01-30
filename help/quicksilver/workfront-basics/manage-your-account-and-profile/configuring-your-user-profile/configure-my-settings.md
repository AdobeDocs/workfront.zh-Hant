---
product-area: user-management;setup
navigation-topic: configure-your-user-profile
title: 設定我的設定
description: 您的 [!DNL Adobe Workfront] 設定檔包含自己的相關資訊（例如，您的姓名、電子郵件地址、地址、電話號碼、職稱等）。 其中也包含您與互動的相關資訊 [!DNL Workfront] 和您公司中的其他使用者。
author: Nolan
feature: Get Started with Workfront
exl-id: 0199bf74-0611-48f0-9c05-da6afac85033
source-git-commit: a750d2707699e1d4783d950807138a74baf78715
workflow-type: tm+mt
source-wordcount: '3311'
ht-degree: 1%

---

# 設定我的設定

<!-- Audited: 01/2024 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Edit the job role FTE percentage allocation blurbs when more functionality is released: now, it says that the % is that of the user's schedule, but it will be either the user's schedule or the system schedule.</p>
-->

您的 [!DNL Adobe Workfront] 設定檔包含自己的相關資訊（例如，您的姓名、電子郵件地址、地址、電話號碼、職稱等）。 其中也包含您與互動的相關資訊 [!DNL Workfront] 和您公司中的其他使用者（例如，您的通知設定，您想要在其中顯示的標籤） [!DNL Workfront]，或您的工作角色、經理和群組及團隊成員資格)。

您的網站已設定此資訊的大部分 [!DNL Workfront] 管理員，當 [!DNL Workfront] 帳戶已建立。

視您在中擁有的存取層級而定 [!DNL Workfront]，您可以設定您的 [!UICONTROL 我的設定] 區域。

## 存取層級如何影響編輯 [!UICONTROL 我的設定] 區域

視您擁有的存取層級而定，您不一定能夠編輯您的區段 [!UICONTROL 我的設定] 區域。

視存取層級中可能設定或未設定的其他設定而定，無法編輯可編輯區段中包含的某些欄位。 如需有關編輯某些您在中找到的欄位所需的額外存取權的詳細資訊 [!UICONTROL 我的設定]，請參閱以下小節： [設定 [!UICONTROL 我的設定] 區域](#configuring-the-my-settings-area).

若要瞭解您具備的存取層級，請連絡您的 [!DNL Workfront] 管理員。

下列方格顯示 [!UICONTROL 我的設定] 區域是否可見或可編輯取決於您的存取層級：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[！UICONTROL我的設定]區域</strong> </th> 
   <th><strong>可見或可編輯</strong> </th> 
   <th><strong>[！UICONTROL系統管理員]</strong> </th> 
   <th><strong>[！UICONTROL Standard]或[！UICONTROL Planner]</strong> </th> 
   <th><strong>[！UICONTROL Worker]</strong> </th> 
   <th><strong>[！UICONTROL Light]或[！UICONTROL Reviewer]</strong> </th> 
   <th><strong>[！UICONTROL Contributor]或[！UICONTROL Requestor]</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2">[！UICONTROL個人資訊]</td> 
   <td> <p>可見</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td> <p>可編輯</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[！UICONTROL喜好設定]</td> 
   <td> <p>可見</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>可編輯</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[！UICONTROL通知]</td> 
   <td> <p>可見</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>可編輯</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td rowspan="2">[！UICONTROL存取]</td> 
   <td>可見</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>可編輯</td> 
   <td> ✔</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[！UICONTROL組織]</td> 
   <td>可見</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>可編輯</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[！UICONTROL資源規劃]</td> 
   <td>可見</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>可編輯</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[！UICONTROL自訂Forms]</td> 
   <td>可見</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>可編輯</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[！UICONTROL註解]</td> 
   <td>可見</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>可編輯</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
 </tbody> 
</table>

## 設定 [!UICONTROL 我的設定] 區域

{{step1-click-profile-pic}}

1. 按一下 **[!UICONTROL 更多]** 名稱旁的功能表 ![更多選單](assets/more-icon.png)，然後按一下 **[!UICONTROL 編輯]**.

1. 根據您的存取層級，您可以更新下列區段：

   * [個人資訊](#personal-info)
   * [偏好設定](#preferences)
   * [通知](#notifications)
   * [存取](#access)
   * [組織](#organization)
   * [資源規劃](#resource-planning)
   * [自訂表單](#custom-form)
   * [評論](#comment)

1. 按一下「**[!UICONTROL 儲存]**」。

### [!UICONTROL 個人資訊]

本節包含下列子章節：

* [基本資訊](#basic-info)
* [工作資訊](#job-info)
* [連絡資訊](#contact-info)

#### [!UICONTROL 基本資訊]

您的應已設定此資訊 [!DNL Workfront] 管理員。 此子區段中的所有欄位都是必填欄位。

您可以在此子區段中變更下列任一專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL名字]</strong></td> 
   <td>更新您的名字。 這是必填欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL姓氏]</strong></td> 
   <td>更新您的姓氏。 這是必填欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL電子郵件地址]</strong></td> 
   <td> 更新您的電子郵件地址。 這是必填欄位。 請記住，您的電子郵件地址也是您的使用者名稱 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL重設密碼]</strong></td> 
   <td>在此區段中重設您的密碼。 如需重設密碼的詳細資訊，請參閱 <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">重設密碼</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（視條件而定） &lt;sso configuration=""&gt; [！UICONTROL使用者名稱]</strong></td> 
   <td> 若您的 [!DNL Workfront] 管理員已啟用SSO整合，與 [!DNL Workfront]，您的SSO使用者名稱會顯示在此欄位中。 已為您的啟用的SSO組態型別 [!DNL Workfront] 執行個體會顯示在此欄位中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（條件式） [！UICONTROL僅允許 &lt;sso configuration=""&gt; 驗證]</strong></td> 
   <td> <p> 若您的 [!DNL Workfront] 管理員已啟用SSO整合，與 [!DNL Workfront] 且已更新SSO的使用者，此欄位預設為選取。 已為您的啟用的SSO組態型別 [!DNL Workfront] 執行個體會顯示在此欄位中。</p> <p>選取此欄位時，您必須登入 [!DNL Workfront] 使用您的SSO憑證。 取消核取它將允許您登入 [!DNL Workfront] 與您的 [!DNL Workfront] 認證。</p> <p>如需關於設定的詳細資訊 [!DNL Workfront] 若使用SSO解決方案，請參閱 <a href="../../../administration-and-setup/add-users/single-sign-on/single-sign-on.md" class="MCXref xref">單一登入 [!DNL Adobe Workfront]</a>. 如需更新SSO使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">更新單一登入的使用者</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 工作資訊]

您可以在此子區段中變更下列任一專案：

<table style="table-layout:auto">
    <tr>
        <td><strong>[！UICONTROL標題]</strong></td>
        <td>指定您的標題。 這與您的工作角色不同。 您的職稱不是資源排程的一部分，而您的工作角色是。 您的標題會顯示在 [!DNL Workfront] 介面可隨時隨地顯示您的姓名和頭像。 所有有權存取您使用者設定檔的人皆可檢視此設定檔。</td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL與我談關於]</strong></td>
        <td>在此欄位中指定您的專業興趣。</td>
    </tr>
</table>

#### [!UICONTROL 連絡資訊]

您可以在此子區段中變更下列任一專案：

<table style="table-layout:auto">
    <tr>
        <td><strong>[！UICONTROL電話號碼]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL副檔名]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL手機號碼]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL位址]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL City]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL狀態]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL郵遞區號]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL Country]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[！UICONTROL個人資料圖片]</strong></td>
        <td>您的個人資料圖片會變成您的虛擬人偶，並會在整個過程中顯示 [!DNL Workfront] 系統，無論您的名稱在何處顯示。</td>
    </tr>
</table>

### [!UICONTROL 偏好設定]

指定您要在 [!DNL Workfront] 介面。

>[!NOTE]
>
>使用者具有 [!UICONTROL 投稿人] 或 [!UICONTROL 請求者] 授權沒有其他左側面板專案可新增至其 [!UICONTROL 主要功能表]，在之外 [!UICONTROL 請求] 區域。 A [!DNL Workfront] 管理員可以將使用者指派給 [!UICONTROL 投稿人] 或 [!UICONTROL 請求者] 版面配置範本的授權，該範本包含 [!UICONTROL 主要功能表]. 之後，他們可以選取要顯示在其中的區域 [!UICONTROL 主要功能表] 藉由編輯其使用者設定檔。

您可以在此子區段中變更下列任一專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL時區]</strong> </td> 
   <td><p>指定您的時區。 這會控制您外寄電子郵件訊息中所顯示的時間。</p>
       <p>時區也會影響PTO行事曆報表中所顯示的內容。</p></td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL電子郵件地區設定]</strong> </td> 
   <td>在這裡指定您偏好的語言。 這會控制外寄電子郵件中所使用的語言、日期和數字格式。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL在更新狀態上顯示完成百分比]</strong> </td> 
   <td>如果您想在使用舊版註解體驗時，在任務的更新區域內顯示完成百分比列，請選取此選項。 如需詳細資訊，請參閱 <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">新的評論體驗</a>.

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL將指派給我自己的工作傳送至我的「正在處理」索引標籤]</strong> </td> 
   <td>選取此欄位會顯示您直接在[！UICONTROL Working On]索引標籤上指派給自己的工作，而非[！UICONTROL Work Requests]索引標籤。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（視條件而定）上傳檔案時自動產生校樣</strong></td> 
   <td>選取此欄位可在檔案載入到之後立即開始產生校訂 [!DNL Workfront]. 此欄位預設為停用，僅可由Workfront管理員更新。<br>此欄位僅在貴公司已購買Workfront的Workfront Proof元件，且您已啟用為校訂使用者身分時可用。 如需Workfront Proof的詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md" class="MCXref xref">在Adobe Workfront中管理校樣</a>.
   <p><b>注意：</b> 上傳到請求的檔案不會自動產生校訂。 </p></td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 通知]

指定您希望從哪些通知接收 [!DNL Workfront]. 如需有關設定通知的詳細資訊，請參閱 [修改您自己的電子郵件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### [!UICONTROL 存取]

您的存取權及與其關聯的其他元件是由您的 [!DNL Workfront] 管理員（設定您的帳戶時）。

僅a [!DNL Workfront] 管理員可以檢視和編輯此部分中的所有欄位。

您可以在此子區段中變更下列任一專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL作用中]</strong> </td> 
   <td>只有身為「 」的使用者才能看見此欄位 [!DNL Workfront] 管理員，預設應該勾選。 這表示使用者處於作用中狀態並可以登入 [!DNL Workfront]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL存取層級]</strong> </td> 
   <td>此欄位對具有[！UICONTROL Standard]、[！UICONTROL Plan]或[！UICONTROL Workfront administrator]存取層級的使用者可見，並且僅對以下使用者可編輯 [!DNL Workfront] 管理員。 如果您是 [!DNL Workfront] 管理員，在修改此欄位時請注意不要將您的存取層級變更為較低的存取層級。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL配置範本]</strong> </td> 
   <td>擁有[！UICONTROL Standard]、[！UICONTROL Plan]或[！UICONTROL Plan]的使用者可看見此欄位 [!DNL Workfront] administrator]存取層級，而且只能為[！UICONTROL編輯 [!DNL Workfront] 擁有[！UICONTROL Standard]或[！UICONTROL Plan]授權且擁有管理使用者存取權的管理員]或使用者。 在此處選取版面範本，以更新Workfront介面的外觀和欄位。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">設定使用者的存取權，以使用自訂存取層級編輯使用者</a> 在 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.<br>有關版面範本及其如何影響介面的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立及管理版面範本</a></td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><strong>Log in as</strong> </td> 
    <td> <p><strong>Add access</strong> for a Workfront administrator or group administrator (associated with a group you are in) to log in as you. Select an <strong>Access expiration date</strong> for the login. </p> <p>You can repeat this to grant login access to multiple administrators.</p> <p>The settings you choose in this section are visible only to you.
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <span class="PinkDraftNote">Add a note about this being only for the Enterprise package if they decide to do it that way. Functionality that may come in a later sprint: If you want to be notified when the administrator logs in as you, select Receive an email when this user logs in.</span> 
       </MadCap:conditionalText>
      </p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader"><strong>（視條件而定） [！UICONTROL使用者可以產生校訂（剩下……個校訂授權中的……）]</strong></td> 
   <td>此欄位僅在貴公司使用舊版時可用 [!DNL Workfront] 計畫且已購買 [!DNL Workfront Proof] 元件。 選取後，您即成為校訂使用者。 它也會顯示系統中使用的校訂授權數量在購買的總校訂授權數量中。 此欄位只有同時具有下列身分的使用者才能看見及編輯： [!DNL Workfront] 管理員。 有關校訂計畫選項的詳細資訊，請參閱 [!DNL Workfront]，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md">存取中的校訂功能 [!DNL Workfront]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（視條件而定） [！UICONTROL許可權設定檔]</strong></td> 
   <td> <p>此欄位會顯示您在中擁有的存取層級 [!DNL Workfront Proof]. 它僅在以下情況下才可用：</p> 
    <ul> 
     <li>貴公司使用舊版 [!DNL Workfront] 計畫且已購買 [!DNL Workfront Proof] 元件或您擁有更新版本的[！UICONTROL Standard]、[！UICONTROL Work]或[！UICONTROL Plan]授權 [!DNL Workfront] 計畫。</li> 
     <li>您已啟用為校訂使用者。</li> 
    </ul> <p>[!DNL Workfront] 管理員可以編輯除了他們自己以外的所有使用者的欄位，因此所有使用者在自己的設定檔上都會將該欄位視為僅限檢視。 如需許可權設定檔的詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/proofing-overview/permission-profiles.md" class="MCXref xref">校訂許可權設定檔概述</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 組織]

此資訊通常由您的 [!DNL Workfront] 管理員，當他們建立 [!DNL Workfront] 帳戶。 您也可以在此區段中更新組織或組織結構的相關資訊。 僅限具有下列專案的使用者： [!UICONTROL 標準]， [!UICONTROL 計畫]，或 [!UICONTROL 系統管理員] 存取層級可編輯此區段。

您可以在此子區段中變更下列任一專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL公司]</strong></td> 
   <td>從下拉式清單中選取您所屬的公司名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（視條件而定） [！UICONTROL報表給]</strong></td> 
   <td>在您選取 <strong>[！UICONTROL公司]</strong> 對於您的設定檔，您也可以在此欄位中指定經理的名稱。 您只能在此指定一個名稱，建議您指定直屬經理的名稱。 開始輸入其名稱，然後按一下以在清單中顯示時將其選取。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（視條件而定） [！UICONTROL直接下屬]</strong></td> 
   <td>在您選取 <strong>[！UICONTROL公司]</strong> 對於您的設定檔，您也可以在此欄位中指定直接下屬的名稱。 您可以視需要在此指定任意數量的直接下屬。 開始輸入其名稱，然後按一下以在清單中出現時選取它們。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL主團隊]</strong> </td> 
   <td> <p>選取 <strong>[！UICONTROL主團隊]</strong> （從下拉式功能表）。 具有[！UICONTROL Standard]、[！UICONTROL Plan]或[！UICONTROL系統管理員]存取層級的使用者可看見此欄位，而且它僅可編輯 [!DNL Workfront] 擁有[！UICONTROL Standard]或[！UICONTROL Plan]授權且擁有管理使用者存取權的管理員或使用者。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">設定使用者的存取權，以使用自訂存取層級編輯使用者</a> 在 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.<br></p> <p>您的 <strong>主團隊</strong> 可能會影響您的外觀 [!DNL Workfront] 介面（如果配置範本與專案團隊相關聯）。 </p> <p>如需有關團隊的詳細資訊，請參閱 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">團隊概觀</a>.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL其他團隊]</strong> </td> 
   <td> <p>您可以隸屬於多個團隊。 開始輸入團隊名稱，然後按一下以在清單中顯示時選取您屬於此欄位的其他團隊。 屬於太多團隊可能會造成指派給團隊的工作混淆。 如需有關團隊的詳細資訊，請參閱 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">團隊概觀</a>.</p> <p>此欄位對擁有[！UICONTROL Standard]、[！UICONTROL Plan]或[！UICONTROL System Administrator]授權的使用者可見，並且僅可編輯 [!DNL Workfront] 擁有[！UICONTROL Standard]或[！UICONTROL Plan]授權且擁有管理使用者存取權的管理員或使用者。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">設定使用者的存取權，以使用自訂存取層級編輯使用者</a> 在 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL主群組]</strong> </td> 
   <td> <p>選取 <strong>[！UICONTROL主群組]</strong> （從下拉式功能表）。</p> <p>備註：此為必填欄位。 您不能有未與群組相關聯的使用者。<br></p> <p>具有[！UICONTROL Standard]、[！UICONTROL Plan]或[！UICONTROL系統管理員]層級的使用者可看見此欄位。 如需誰可以編輯的詳細資訊， <strong>[！UICONTROL主群組]</strong> 欄位，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"class="MCXref xref">編輯使用者設定檔</a>. 您的 <strong>[！UICONTROL主群組]</strong> 是所有專案的預設群組，也是預設群組 <strong>[！UICONTROL主群組]</strong> 您建立的所有新使用者。 您建立的任何自訂表單都會與您共用 <strong>[！UICONTROL主群組]</strong> 依預設。</p> <p>如需群組的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群組概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL其他群組]</strong> </td> 
   <td> <p>您可以屬於多個群組。 開始輸入群組的名稱，即可在此欄位中指定您所屬的其他群組。 按一下以在清單中顯示時選取它。 具有[！UICONTROL Standard]、[！UICONTROL Plan]或[！UICONTROL系統管理員]存取層級的使用者可看見此欄位。 如需誰可以編輯的詳細資訊， <strong>[！UICONTROL其他群組]</strong> 欄位，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"class="MCXref xref">編輯使用者設定檔</a>.</p> <p>如需群組的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群組概述</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 資源規劃]

您的資源計畫資訊會影響工作指定的時間表、您登入的時間、成本以及您所在專案的收入。 通常，此區域會由 [!DNL Workfront] 管理員、專案或資源管理員，或由您的直屬經理管理。

請在此章節中使用下列任一專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL排程停用]</strong></td> 
   <td>如果您想要排程在一段時間後停用您的帳戶，請勾選此方塊。 在 <p><strong>[！UICONTROL排程停用日期]</strong> 之後，請指定帳戶停用的日期。 如需停用使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation" class="MCXref xref">排程使用者停用</a> 在 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>. </p><p>如果您有[！UICONTROL Standard]或[！UICONTROL Plan]授權，或您是 [!DNL Workfront] 管理員。 </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL主要角色]</strong></td> 
   <td> <p>這是您可以在Workfront中履行的主要職務角色。 依預設，您指派到的每個任務和問題也會指派給此工作角色。 職務角色在資源管理中至關重要。 如需有關工作角色的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理職位角色</a>.</p> <p>只有當您擁有具有管理使用者存取權的[！UICONTROL Standard]或[！UICONTROL Plan]授權，或您是 [!DNL Workfront] 管理員。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">設定使用者的存取權，以使用自訂存取層級編輯使用者</a> 在 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（視條件而定）如果您選取[！UICONTROL主要角色]，則會顯示[！UICONTROL FTE可用性百分比]欄位。</strong></td> 
   <td>指定您的排程時間中分配給此工作角色的百分比。 主要角色的[！UICONTROL FTE可用性百分比]預設值為100%。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL其他角色]</strong> </td> 
   <td> <p>您可以在中擁有多個職務角色 [!DNL Workfront]. 職務角色在資源管理中至關重要。 如需有關工作角色的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理職位角色</a>.</p> <p>只有當您擁有具有管理使用者存取權的[！UICONTROL Standard]或[！UICONTROL Plan]授權，或您是 [!DNL Workfront] 管理員。 如需有關設定具有管理使用者存取許可權的使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">設定使用者的存取權，以使用自訂存取層級編輯使用者</a> 在 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>（視條件而定）如果您選取一或多個其他角色，則會針對每個角色顯示[！UICONTROL FTE可用性百分比]欄位。</strong></td> 
   <td> <p>指定將排程時間的百分比分配給每個工作角色。 [！UICONTROL其他角色]的[！UICONTROL FTE可用性百分比]預設值為0%。</p> <p> <img src="assets/user-settings-roles-and-dte-boxes-rp-story--1--350x224.png" alt="user_settings_roles_and_dte_boxes_rp_story__1_.png" style="width: 350;height: 224;"> </p> <p>注意：  
     <ul> 
      <li>如果[！UICONTROL其他角色]具有0% FTE可用性，除非將使用者指派給這些角色中的任務，否則它們不會顯示在[！UICONTROL資源規劃工具]中。</li> 
      <li> <p>全部的總和 <strong>[！UICONTROL FTE可用性百分比]</strong> 所有角色的必須等於100%。 每個[！UICONTROL FTE可用性百分比]會計算[！UICONTROL資源規劃工具]中每個使用者每個角色的[！UICONTROL可用時數]。 </p> <p>每位使用者各角色的[！UICONTROL可用時數]取決於使用者的可用時間。 使用者的可用時間計算方式： [!DNL Workfront] 視您選取的方法而定 [!DNL Workfront] 管理員可在[！UICONTROL資源管理偏好設定]中計算FTE。 如需有關計算使用者可用性的詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">計算資源規劃工具中使用者和角色的時數和FTE的概觀</a>. 如需有關設定資源管理偏好設定的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">設定資源管理喜好設定</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>排程</strong></td> 
   <td> <p>僅限 [!DNL Workfront] 管理員或擁有[！UICONTROL Standard]或[！UICONTROL Plan]授權且對時程表和時數具有管理存取權的使用者可以更新此欄位。 如需時程表和時數的管理存取許可權詳細資訊，請參閱以下的「時程表和時數」一節： <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者管理特定區域的存取權</a>.</p> <p>從下拉式選單中選取適合您的正確時程表。 這可確保根據您設定的規格自動產生您的時間表 [!DNL Workfront] 管理員。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL預設時數型別]</strong> </td> 
   <td>選取您的預設時數型別。 這是您登入Workfront時系統預設使用的小時型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL可用小時型別]</strong> </td> 
   <td>選擇記錄時間時，您應該可以選擇的時數型別。 此下拉式選單中的小時型別可由您的 [!DNL Workfront] 管理員。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL資源集區]</strong> </td> 
   <td>選取您所屬的資源集區。 此欄位僅供報表和參考之用。 這不會影響資源排程或計畫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL FTE]</strong> </td> 
   <td> <p>只有在系統層級的[！UICONTROL資源管理偏好設定]設定為時，才會考量您在此處指定的數字，以根據預設排程計算可用性 <strong>[！UICONTROL預設排程]</strong>.</p> <p>例如，如果FTE值為0.5，而[！UICONTROL預設排程]為40小時，則您每週可工作20小時。</p> <p>如果系統層級的[！UICONTROL資源管理喜好設定]設定為 <strong>[！UICONTROL使用者的排程]</strong>，您在此指定的值會遭忽略，您可以根據排程中指定的內容來工作。 在此情況下，您的[！UICONTROL資源規劃工具]FTE計算公式如下： </p> <p><code style="font-style: normal;">[!UICONTROL User Available FTE] = [!UICONTROL Hours from the Schedule of the User/ Default Schedule Hours]</code> </p> <p>如需有關計算使用者FTE的詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">計算資源規劃工具中使用者和角色的時數和FTE的概觀</a>.</p> <p>有關在中建立排程的詳細資訊 [!DNL Workfront]，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>.</p> <p>如需有關設定資源管理偏好設定的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">設定資源管理喜好設定</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL每小時成本]</strong> </td> 
   <td>指定使用者的每小時成本金額。 如需有關在中追蹤成本的詳細資訊 [!DNL Workfront]，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>. 除非您有權從存取層級存取財務資料，或您是 [!DNL Workfront] 管理員。 如需財務存取許可權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予財務資料的存取權</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[！UICONTROL每小時帳單]</strong> </td> 
   <td>指定使用者的每小時帳單金額。 如需有關追蹤帳單和收入的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單與收入概要</a>. 除非您有權從存取層級存取財務資料，或您是 [!DNL Workfront] 管理員。 如需財務存取許可權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予財務資料的存取權</a>.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 自訂表單]

您可以將自訂表單與使用者設定檔建立關聯。 這可讓您為使用者儲存其他資訊，這些資訊原本無法儲存在 [!DNL Workfront] 上述原生欄位。

您必須具備下列存取權或許可權之一，才能將自訂表單附加至您的使用者設定檔：

* 您是 [!DNL Workfront] 管理員。
* 您是 [!UICONTROL 標準] 或 [!UICONTROL 計畫] 授權使用者和使用者自訂表單會與您的其中一個群組共用。

所有使用者都可以檢視與其設定檔相關聯的自訂表單。

您的 [!DNL Workfront] 管理員必須為使用者物件設定自訂表單，以便您將自訂表單附加到使用者設定檔中。 如需建立自訂表單的詳細資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### [!UICONTROL 註解]

您可以在使用者設定檔上記錄註解，該註解會儲存在設定檔的 [!UICONTROL 更新] 標籤。

您可以按一下 [!UICONTROL 人物] 圖示將其他專案包含在更新中。

您可以按一下 [!UICONTROL 鎖定] 圖示將此更新設為您所在公司之使用者的私用。
