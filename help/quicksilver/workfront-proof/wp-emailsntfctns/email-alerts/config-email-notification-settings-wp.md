---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: 在中設定電子郵件通知設定 [!DNL Workfront Proof]
description: 從Workfront校訂產生的電子郵件通知會通知共同作業人員有關校訂的最近活動，例如評論、回覆或決定。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: e80a3ede9ccf6ccf9ea7777aab35cc859f13a6ac
workflow-type: tm+mt
source-wordcount: '2058'
ht-degree: 0%

---

# 在中設定電子郵件通知設定 [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>本文提及獨立版產品中的功能 [!DNL Workfront Proof]. 有關內部校訂的資訊 [!DNL Adobe Workfront]，請參閱 [校訂](../../../review-and-approve-work/proofing/proofing.md).

電子郵件通知會通知共同作業人員有關校訂的最近活動，例如評論、回覆或決定。

您可以在下列區域為檢閱者設定電子郵件通知：

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
<tr> 
   <td role="rowheader">產品</td> 
   <td>Workfront Proof Standalone</td> 
  </tr> 
</table>

可在新校訂頁面上設定檢閱者的電子郵件通知， [!UICONTROL 新版本] 頁面，並在中管理 [!UICONTROL 工作流程] 的區段 [!UICONTROL 校訂詳細資訊] 頁面。 如需詳細資訊，請參閱 [產生校訂於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* 新校訂頁面
* 此 [!UICONTROL 新版本] 頁面
* 此 [!UICONTROL 工作流程] 的區段 [!UICONTROL 校訂詳細資訊] 頁面。

如需詳細資訊，請參閱 [產生校訂於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)


* [產生校訂於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [產生校訂於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [在中管理校訂詳細資訊 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).


如果共同作業人員有自己的偏好設定或帳戶管理員對警報頻率有他們的建議，則每位使用者都可以設定自己的電子郵件警報設定，在與他們共用校訂時自動套用這些設定。 這可在使用者詳細資訊頁面上設定為校訂預設值。

每個使用者也可以設定自己的電子郵件警報設定，這些設定將在與他們共用校訂時自動套用。 <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>使用者建立校樣並新增這些共同作業人員時，建議使用這些設定。 不過，這些只是建議，因此在稽核流程中可隨時調整，而變更會套用至變更後進行的所有活動。 校樣層級的設定會覆寫校樣預設設定。

使用者 [!UICONTROL 管理員] 或 [!UICONTROL 帳單管理員] 設定檔也可在「帳戶」設定中，為其帳戶中的其他使用者設定校訂預設值。

如需設定檔的相關資訊，請參閱 [中的校訂許可權設定檔 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [在個人設定中設定校訂預設值([!DNL Workfront Proof] 僅限使用者)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [變更收件者的電子郵件警示](#change-email-alerts-for-a-recipient)
* [設定使用者的校訂預設值](#configure-proof-defaults-for-a-user)

## 在個人設定中設定校訂預設值([!DNL Workfront Proof] 僅限使用者)

您可以為您建立的校樣設定校樣設定。

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. 按一下 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.

1. 按一下 **[!UICONTROL 校訂預設值]** 標籤。
1. 按一下 **[!UICONTROL 預設電子郵件通知設定]** 以展開它。
1. 在下列兩個設定右側的下拉式清單中，選取下表說明的其中一個選項。

   * **[!UICONTROL 預設電子郵件警報]**：會影響與您共用的每個校訂。 此設定可在校訂層級覆寫。
   * **[!UICONTROL 新訪客稽核者的預設電子郵件警報]**：影響您帳戶中先前未作為聯絡人存在的檢閱者。

   >[!NOTE]
   >
   >如果您不選擇下列其中一個選項， [!DNL Workfront Proof] 會傳送校樣上有關活動的每日摘要給您。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL所有活動]</td> 
      <td>每次校訂上有任何活動（例如新評論、回覆或決定）時，[！UICONTROL Workfront]都會傳送電子郵件給檢閱者。 <p>這是管理校訂流程之人員的絕佳選項，因為可讓他們檢視活動發生的情形。 </p><p>使用者不會收到有關其活動的電子郵件警報。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL回覆我的意見]</td> 
      <td>只有當某人明確回覆其評論時（這不包括他們自己的評論），才會傳送電子郵件給稽核者。 這表示如果校訂上的某人發表新評論，則不會通知檢閱者。<p>建議將此設定提供給校訂上的客戶，這樣他們就不會收到校訂上任何其他評論的通知，而只會在回覆他們自己的評論時收到通知。</p><p>雖然具有此電子郵件警報設定的檢閱者不會收到其他新評論的通知，但他們仍可在校訂檢視器中檢視校訂上的所有評論。</p><p>如需有關註解的資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">檢視並回覆校訂評論</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL決策]</td> 
      <td>[!DNL Workfront] 只有在有人做出決定時，才會傳送電子郵件給稽核者。<p>這對於管理核准流程的人員（例如專案經理）非常有用，他們需要監視校訂的進度並檢視哪些使用者已做出決定。</p><p>除非您在提交決定時選取電子郵件確認選項，否則不會通知您自己的決定。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL最終決定]</td> 
      <td>[!DNL Workfront] 當校訂的最後一位核准者做出決定時傳送電子郵件。<p>設計人員經常會使用此警示，他們通常不需要參與實際的稽核討論。 做出最終決定時，設計人員會收到通知，然後可以對任何必要的變更採取行動。</p><p>此警示對於必須在複查程式完成後才收到通知的部門主管來說也很有用。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL每小時摘要]</td> 
      <td>[!DNL Workfront] 每小時會傳送電子郵件給稽核者，其中包含該小時發生的所有評論、回覆和決定的摘要。<p>只有當您以外的活動發生在過去一小時內，才會傳送電子郵件。 </p><p>此警報是檢視專案概觀的好地方。</p><p>此摘要的範例使用案例是資深檢閱者，他需要專案的概觀，但不需要立即收到校訂上所有活動的通知。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL每日摘要]</td> 
      <td>[!DNL Workfront] 只會在您擁有的活動以外的日期傳送一封電子郵件，其中包含列出的所有評論、回覆和決定。<p>此警報是檢視專案摘要的好方法，而不會在一天中忙於多次更新。</p><p>此摘要的範例使用案例是部門負責人，他想要監控專案的整體進度。</p><p>如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校訂評論和決定的通知</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[！UICONTROL無電子郵件]</td> 
      <td>[!DNL Workfront] 不會傳送任何電子郵件警示。<br>這對於僅供參考而新增到校樣而無需通知任何變更的人非常有用。<p>系統預設為[！UICONTROL Daily summary] （亦稱為[！UICONTROL未設定]）。 如果您或您的稽核者未進行任何其他變更，則您的所有校樣都會具有此設定。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 變更下列任一專案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL校訂就緒時透過電子郵件確認]</td> 
      <td>指定您是否要在建立校訂時接收[！UICONTROL Proof maked]電子郵件。 如需詳細資訊，請參閱 <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">[！UICONTROL Proof Maked]電子郵件</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL傳送給我的電子郵件格式] </td> 
      <td> <p>在HTML樣式電子郵件和純文字電子郵件之間選擇。 </p> <p><b>附註</b></p>
      <p>校訂層級的設定會覆寫校訂預設設定。 不過，如果在[！UICONTROL帳戶]設定中針對整個帳戶停用校訂電子郵件通知，即使未在校訂上選取[！UICONTROL停用的電子郵件通知]，也不會傳送任何電子郵件通知給共同作業人員。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **[!UICONTROL 訊息設定]**，變更下列任一專案：

   | 校訂範本 | 說明 |
   |---|---|
   | **[!UICONTROL 校訂主旨範本]** | 顯示於新校訂頁面、新版本頁面、訊息頁面和提醒頁面。 可以在傳送前進行編輯。 |
   | **[!UICONTROL 校樣訊息範本]** | 顯示於新校訂頁面、新版本頁面、訊息頁面和提醒頁面。 可以在傳送前進行編輯。 |

## 變更收件者的電子郵件警示

您可以在批次動作中變更特定收件者的電子郵件警示。

1. 按一下 **[!UICONTROL 連絡人]** ，位於左側導覽面板中。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![](assets/more-button-small.png) 收件者的，然後按一下 **[!UICONTROL 檢視成員詳細資料]** 在下拉式功能表中。

1. 開啟 **[!UICONTROL 共用專案]** 區段。
1. 選取您要變更電子郵件警示之每個專案左側的核取方塊。
1. 按一下 **[!UICONTROL 更多]** 在共用專案清單上方，然後按一下 **[!UICONTROL 變更電子郵件警示]** 在下拉式功能表中。

1. 變更電子郵件警示，然後按一下 **[!UICONTROL 提交]**.

## 設定使用者的校訂預設值

如果您是 [!DNL Workfront Proof] 管理員，您可以為您的帳戶中的使用者設定校訂預設值。

1. 按一下 **[!UICONTROL 設定]** > **[!UICONTROL 帳戶設定]**.

1. 開啟 **[!UICONTROL 使用者]** 標籤。
1. 開啟 **[!UICONTROL 更多]** 功能表 ![More_button_small.png](assets/more-button-small.png) 位於使用者名稱右側。

1. 按一下 **[!UICONTROL 檢視使用者詳細資訊]** 在下拉式功能表中。
1. 在 **[!UICONTROL 設定]**，按一下 **[!UICONTROL 預設電子郵件警報設定]** 以展開它。

1. 在下列兩個設定右側的下拉式清單中，選取下表說明的其中一個選項：

   * **[!UICONTROL 預設電子郵件警報]**：會影響與您共用的每個校訂。 此設定可在校訂層級覆寫。
   * **[!UICONTROL 新訪客稽核者的預設電子郵件警報]**：影響您帳戶中先前未作為聯絡人存在的檢閱者。

   >[!NOTE]
   >
   >如果您沒有為使用者選擇下列其中一個選項， [!DNL Workfront Proof] 會傳送使用者有關其校樣活動的每日摘要。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[！UICONTROL所有活動]</td>
      <td>[!DNL Workfront] 每次在校訂上發生任何活動（例如新評論、回覆或決定）時，都會傳送電子郵件給檢閱者。 <p>這是管理校訂流程之人員的絕佳選項，因為可讓他們檢視活動發生的情形。 </p><p>使用者不會收到有關其活動的電子郵件警報。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[！UICONTROL回覆我的意見]</td>
      <td>只有當某人明確回覆其評論時（這不包括他們自己的評論），才會傳送電子郵件給稽核者。 這表示如果校訂上的某人發表新評論，則不會通知檢閱者。<p>建議將此設定提供給校訂上的客戶，這樣他們就不會收到校訂上任何其他評論的通知，而只會在回覆他們自己的評論時收到通知。</p><p>雖然具有此電子郵件警報設定的檢閱者不會收到其他新評論的通知，但他們仍可在校訂檢視器中檢視校訂上的所有評論。</p><p>如需有關註解的資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">檢視並回覆校訂評論</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[！UICONTROL決策]</td>
      <td>[!DNL Workfront] 只有在有人做出決定時，才會傳送電子郵件給稽核者。<p>這對於管理核准流程的人員（例如專案經理）非常有用，他們需要監視校訂的進度並檢視哪些使用者已做出決定。</p><p>除非您在提交決定時選取電子郵件確認選項，否則不會通知您自己的決定。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[！UICONTROL最終決定]</td>
      <td>[!DNL Workfront] 當校訂的最後一位核准者做出決定時傳送電子郵件。<p>設計人員經常會使用此警示，他們通常不需要參與實際的稽核討論。 做出最終決定時，設計人員會收到通知，然後可以對任何必要的變更採取行動。</p><p>此警示對於必須在複查程式完成後才收到通知的部門主管來說也很有用。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[！UICONTROL每小時摘要]</td>
      <td>[!DNL Workfront] 每小時會傳送電子郵件給稽核者，其中包含該小時發生的所有評論、回覆和決定的摘要。<p>只有當您以外的活動發生在過去一小時內，才會傳送電子郵件。 </p><p>此警報是檢視專案概觀的好地方。</p><p>此摘要的範例使用案例是資深檢閱者，他需要專案的概觀，但不需要立即收到校訂上所有活動的通知。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[！UICONTROL每日摘要]</td>
      <td>[!DNL Workfront] 只會在您擁有的活動以外的日期傳送一封電子郵件，其中包含列出的所有評論、回覆和決定。<p>此警報是檢視專案摘要的好方法，而不會在一天中忙於多次更新。</p><p>此摘要的範例使用案例是部門負責人，他想要監控專案的整體進度。</p><p>如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校訂評論和決定的通知</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[！UICONTROL無電子郵件]</td>
      <td>[!DNL Workfront] 不會傳送任何電子郵件警示。<br>這對於僅供參考而新增到校樣而無需通知任何變更的人非常有用。<p>系統預設為[！UICONTROL Daily summary] （亦稱為[！UICONTROL未設定]）。 如果您或您的稽核者未進行任何其他變更，則您的所有校樣都會具有此設定。</p></td>
     </tr>
    </tbody>
   </table>

1. 剩餘 **[!UICONTROL 預設電子郵件警報設定]**，變更下列任一專案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL校訂就緒時透過電子郵件確認]</td> 
      <td>指定您是否要在建立校訂時接收[！UICONTROL Proof maked]電子郵件。 如需詳細資訊，請參閱 <a href="https://support.workfront.com/hc/en-us/article">[！UICONTROL Proof Maked]電子郵件。</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL傳送給我的電子郵件格式] </td> 
      <td> <p>在HTML樣式電子郵件和純文字電子郵件之間選擇。 </p> <p><b>附註</b></p> <p>校訂層級的設定會覆寫校訂預設設定。 不過，如果在[！UICONTROL帳戶]設定中針對整個帳戶停用校訂電子郵件通知，即使未在校訂上選取[！UICONTROL停用的電子郵件通知]，也不會傳送任何電子郵件通知給共同作業人員。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
