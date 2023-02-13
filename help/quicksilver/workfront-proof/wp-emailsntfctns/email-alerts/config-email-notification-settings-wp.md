---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: 在中配置電子郵件通知設定 [!DNL Workfront Proof]
description: 電子郵件通知會通知共同作業人員最近關於校樣（例如留言、回覆、決策）的活動。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '1998'
ht-degree: 0%

---

# 在中配置電子郵件通知設定 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

電子郵件通知會通知共同作業人員最近關於校樣（例如留言、回覆、決策）的活動。

可在「新校樣」(New proof)頁面上設定審核者的電子郵件通知， [!UICONTROL 新版本] 頁面，並在中管理 [!UICONTROL 工作流程] 區段 [!UICONTROL 校樣詳細資料] 頁面。 如需詳細資訊，請參閱 [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [在中產生校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [在中管理校樣詳細資料 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

每位使用者也可以設定自己的電子郵件警報設定，當與他們共用校樣時，系統會自動套用這些設定。 如果共同作業人員有其偏好設定，或帳戶管理員有其關於警報頻率的建議。 這可設為使用者詳細資料頁面上的校樣預設值。

>[!NOTE]
>
>當使用者建立校樣並新增這些共同作業人員時，建議使用這些設定。 不過，這些僅是建議，因此在審核過程中可隨時加以調整，變更會套用至變更後進行的所有活動。 校樣預設設定被校樣層級的設定覆蓋。

具有 [!UICONTROL 管理員] 或 [!UICONTROL 帳單管理員] 設定檔也可以從帳戶設定中為帳戶中的其他使用者設定校樣預設值。

如需設定檔的相關資訊，請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [在個人設定中配置校樣預設值([!DNL Workfront Proof] 僅限使用者)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [變更收件者的電子郵件警報](#change-email-alerts-for-a-recipient)
* [配置用戶的校樣預設值](#configure-proof-defaults-for-a-user)

## 在個人設定中配置校樣預設值([!DNL Workfront Proof] 僅限使用者)

您可以為建立的校樣配置校樣設定。

如需校樣設定的相關資訊，請參閱 [!DNL Workfront] 管理員或 [!DNL Workfront Proof] 管理員可進行配置，請參閱。

1. 按一下 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.

1. 按一下 **[!UICONTROL 校對預設值]** 標籤。
1. 按一下 **[!UICONTROL 預設電子郵件通知設定]** 來擴展。
1. 在下列兩個設定右側的下拉式清單中，選取下表中說明的其中一個選項。

   * **[!UICONTROL 預設電子郵件警報]**:會影響與您共用的每個校樣。 可在校樣層級覆寫此設定。
   * **[!UICONTROL 新來賓審核者的預設電子郵件警報]**:影響先前不作為帳戶聯繫人存在的審閱者。

   >[!NOTE]
   >
   >如果您未選擇下列其中一個選項， [!DNL Workfront Proof] 傳送校樣上活動的每日摘要。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL全部活動]</td> 
      <td>每當校樣上有任何活動（例如新留言、回覆或決定）時，[!UICONTROL Workfront]都會傳送電子郵件給審核者。 <p>對於管理校對程式的人員來說，這是絕佳選項，因為這可讓他們查看活動發生的時間。 </p><p>使用者不會收到有關其自身活動的電子郵件警報。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL對我評論的答復]</td> 
      <td>只有當有人明確回覆其留言時，系統才會傳送電子郵件給審閱者（這會排除其對其留言的回覆）。 這表示如果校樣上的某人發表新意見，則不會通知審核者。<p>建議您的用戶端使用此設定，以便他們不會收到關於證明的任何其他意見的通知，而且只會收到對其意見的回覆通知。</p><p>雖然具有此電子郵件警報設定的審核者不會收到其他新留言的通知，但他們仍可在校對檢視器中檢視校樣上的所有留言。</p><p>如需註解的相關資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">檢視並回覆校樣留言</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL決策]</td> 
      <td>[!DNL Workfront] 只有在有人作出決定時，才會傳送電子郵件給審核者。<p>這對於管理審批流程的人員（如項目經理）來說非常有用，他們需要監控校樣的進度，並查看哪些用戶已做出決策。</p><p>除非您在提交決策時選取電子郵件確認選項，否則系統不會通知您自己的決策。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL最終決定]</td> 
      <td>[!DNL Workfront] 當校樣的最後一個核准者做出決定時，會傳送電子郵件。<p>此警報常由設計人員使用，他們通常不需要參與實際的審閱討論。 當做出最終決定時，設計人員會收到通知，然後可以對任何必要的變更採取行動。</p><p>此警報對於只有在審核流程完成時才需要通知的部門主管也很有用。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL每小時摘要]</td> 
      <td>[!DNL Workfront] 每小時傳送電子郵件給審核者，內含該小時內發生的所有留言、回覆和決定的摘要。<p>只有在過去一小時內發生您自己以外的活動時，才會傳送電子郵件。 </p><p>此警報是查看專案概覽的好方法。</p><p>此摘要的範例使用案例是需要專案概覽但不需要立即收到校樣上所有活動的通知的資深審核者。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL每日摘要]</td> 
      <td>[!DNL Workfront] 只會在您自己的活動以外的日子，傳送一封電子郵件，其中列出所有留言、回覆和決策。<p>此警報是您查看專案摘要的好方法，不會在一天中多次更新。</p><p>此摘要的使用案例範例是部門主管，他想要監控專案的整體進度。</p><p>如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校樣意見和決策的通知</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL無電子郵件]</td> 
      <td>[!DNL Workfront] 不會傳送任何電子郵件警報。<br>對於只為了參考而新增至校樣，且不需要收到任何變更通知的人，這個用法很有幫助。<p>系統預設值為[!UICONTROL Daily Summary]（也顯示為[!UICONTROL Not Set]）。 如果您或您的審核者未進行任何其他更改，則所有校樣都具有此設定。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 變更下列任一項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL校樣就緒時的電子郵件確認]</td> 
      <td>指定在建立校樣時，是否要接收[!UICONTROL校樣製作]電子郵件。 如需詳細資訊，請參閱 <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">[!UICONTROL校樣製作]電子郵件</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL發送給我的電子郵件格式]</strong> </td> 
      <td> <p>在HTML樣式的電子郵件和純文字電子郵件之間進行選擇。 </p> <p>注意： 校對預設設定被校樣層級的設定覆蓋。 不過，如果在[!UICONTROL帳戶]設定中針對整個帳戶停用校樣電子郵件通知，即使未在校樣上選取[!UICONTROL已停用電子郵件警報]，也不會將電子郵件警報傳送給共同作業人員。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **[!UICONTROL 訊息設定]**，變更下列任一項：

   | **[!UICONTROL 校樣主題範本]** | 顯示在「新校樣」頁面、「新版本」頁面、「訊息」頁面和「提醒」頁面。 可在傳送前加以編輯。 |
   |---|---|
   | **[!UICONTROL 校樣訊息範本]** | 顯示在「新校樣」頁面、「新版本」頁面、「訊息」頁面和「提醒」頁面。 可在傳送前加以編輯。 |

   {style=&quot;table-layout:auto&quot;}

## 變更收件者的電子郵件警報

您可以在批次動作中變更特定收件者的電子郵件警報。

1. 按一下 **[!UICONTROL 聯繫人]** ，即可取得Advertising Cloud的說明。
1. 按一下 **[!UICONTROL 更多]** （三個點）功能表，然後按一下 **[!UICONTROL 查看成員詳細資訊]** 中。

1. 開啟 **[!UICONTROL 共用項目]** 區段。
1. 選取您要變更電子郵件警報之項目左側的核取方塊。
1. 按一下 **[!UICONTROL 更多]** 在共用項目清單上方，然後按一下 **[!UICONTROL 變更電子郵件警報]** 中。

1. 變更電子郵件警報，然後按一下 **[!UICONTROL 提交]**.

## 配置用戶的校樣預設值

如果您是 [!DNL Workfront Proof] 管理員，您可以為帳戶中的使用者設定校樣預設值。

1. 按一下 **[!UICONTROL 設定]** > **[!UICONTROL 帳戶設定]**.

1. 開啟 **[!UICONTROL 使用者]** 標籤。
1. 開啟 **[!UICONTROL 更多]** 功能表。 ![More_button_small.png](assets/more-button-small.png)

1. 按一下 **[!UICONTROL 查看用戶詳細資訊]** 中。
1. 在 **[!UICONTROL 設定]**，按一下 **[!UICONTROL 預設電子郵件警報設定]** 來擴展。

1. 在下列兩個設定右側的下拉式清單中，選取下表中說明的其中一個選項：

   * **[!UICONTROL 預設電子郵件警報]**:會影響與您共用的每個校樣。 可在校樣層級覆寫此設定。
   * **[!UICONTROL 新來賓審核者的預設電子郵件警報]**:影響先前不作為帳戶聯繫人存在的審閱者。

   >[!NOTE]
   >
   >如果您未為使用者選擇下列其中一個選項， [!DNL Workfront Proof] 傳送使用者校樣上活動的每日摘要。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL全部活動]</td>
      <td>[!DNL Workfront] 每次校樣上有任何活動（例如新留言、回覆或決定）時，都會傳送電子郵件給審核者。 <p>對於管理校對程式的人員來說，這是絕佳選項，因為這可讓他們查看活動發生的時間。 </p><p>使用者不會收到有關其自身活動的電子郵件警報。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL對我評論的答復]</td>
      <td>只有當有人明確回覆其留言時，系統才會傳送電子郵件給審閱者（這會排除其對其留言的回覆）。 這表示如果校樣上的某人發表新意見，則不會通知審核者。<p>建議您的用戶端使用此設定，以便他們不會收到關於證明的任何其他意見的通知，而且只會收到對其意見的回覆通知。</p><p>雖然具有此電子郵件警報設定的審核者不會收到其他新留言的通知，但他們仍可在校對檢視器中檢視校樣上的所有留言。</p><p>如需註解的相關資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">檢視並回覆校樣留言</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL決策]</td>
      <td>[!DNL Workfront] 只有在有人作出決定時，才會傳送電子郵件給審核者。<p>這對於管理審批流程的人員（如項目經理）來說非常有用，他們需要監控校樣的進度，並查看哪些用戶已做出決策。</p><p>除非您在提交決策時選取電子郵件確認選項，否則系統不會通知您自己的決策。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL最終決定]</td>
      <td>[!DNL Workfront] 當校樣的最後一個核准者做出決定時，會傳送電子郵件。<p>此警報常由設計人員使用，他們通常不需要參與實際的審閱討論。 當做出最終決定時，設計人員會收到通知，然後可以對任何必要的變更採取行動。</p><p>此警報對於只有在審核流程完成時才需要通知的部門主管也很有用。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL每小時摘要]</td>
      <td>[!DNL Workfront] 每小時傳送電子郵件給審核者，內含該小時內發生的所有留言、回覆和決定的摘要。<p>只有在過去一小時內發生您自己以外的活動時，才會傳送電子郵件。 </p><p>此警報是查看專案概覽的好方法。</p><p>此摘要的範例使用案例是需要專案概覽但不需要立即收到校樣上所有活動的通知的資深審核者。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL每日摘要]</td>
      <td>[!DNL Workfront] 只會在您自己的活動以外的日子，傳送一封電子郵件，其中列出所有留言、回覆和決策。<p>此警報是您查看專案摘要的好方法，不會在一天中多次更新。</p><p>此摘要的使用案例範例是部門主管，他想要監控專案的整體進度。</p><p>如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校樣意見和決策的通知</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL無電子郵件]</td>
      <td>[!DNL Workfront] 不會傳送任何電子郵件警報。<br>對於只為了參考而新增至校樣，且不需要收到任何變更通知的人，這個用法很有幫助。<p>系統預設值為[!UICONTROL Daily Summary]（也顯示為[!UICONTROL Not Set]）。 如果您或您的審核者未進行任何其他更改，則所有校樣都具有此設定。</p></td>
     </tr>
    </tbody>
   </table>

1. 在 **[!UICONTROL 預設電子郵件警報設定]**，變更下列任一項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL校樣就緒時的電子郵件確認]</td> 
      <td>指定在建立校樣時，是否要接收[!UICONTROL校樣製作]電子郵件。 如需詳細資訊，請參閱 <a href="https://support.workfront.com/hc/en-us/article">[!UICONTROL校樣]電子郵件。</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL發送給我的電子郵件格式]</strong> </td> 
      <td> <p>在HTML樣式的電子郵件和純文字電子郵件之間進行選擇。 </p> <p>注意： 校對預設設定被校樣層級的設定覆蓋。 不過，如果在[!UICONTROL帳戶]設定中針對整個帳戶停用校樣電子郵件通知，即使未在校樣上選取[!UICONTROL已停用電子郵件警報]，也不會將電子郵件警報傳送給共同作業人員。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
