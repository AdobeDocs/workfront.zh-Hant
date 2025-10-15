---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 設定 [!DNL Adobe Workfront for Jira]
description: 您可以使用 [!DNL Adobe Workfront for Jira] 整合 [!DNL Jira] 和 [!DNL Workfront] 系統。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '2454'
ht-degree: 0%

---

# 設定[!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->


>[!IMPORTANT]
>
>為了提供更穩定且更可擴充的整合，我們改用現代、彈性的整合方法，即使用Workfront自動化與整合(Fusion)。 在此轉換過程中，Jira整合的Workfront在&#x200B;**2026年2月28日**&#x200B;後將無法使用。
>
>根據貴組織與Jira的整合需求，我們建議使用Workfront自動化和整合。
>
>如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>如需Jira的Workfront自動化與整合模組特定功能的相關資訊，請參閱[Jira軟體模組](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)。

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

您可以使用[!DNL Adobe Workfront for Jira]來整合您的[!DNL Jira]和[!DNL Workfront]系統。

安裝附加元件後，您可以在建立[!DNL Jira]個工作專案時，定義自動建立[!DNL Workfront]問題的工作流程。 兩個應用程式中的專案會變成連結，而且其部分資訊會在兩個系統中自動更新。

[!DNL Workfront]和[!DNL Jira]中的所有使用者都可以受益於這項整合。 他們只需要最常使用的系統授權，而不需要兩個系統的授權。

此附加元件適用於[!UICONTROL 軟體的]伺服器[!UICONTROL 和]OnDemand[!UICONTROL  （或]雲端[!DNL Jira]）版本。

如需[!DNL Jira]目前支援的[!DNL Workfront for Jira]版本清單，請參閱[[!DNL Workfront for Jira]的](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview)[!DNL Atlassian Marketplace]。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td><p>任何</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準 </p>
       <p>規劃 </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira存取</td> 
   <td> <p>系統管理員存取權</p> <p>重要：建議您在Jira和Workfront中建立個別系統管理員帳戶，以專門用於此整合，而不使用可能附加至使用者的現有帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

設定[!DNL Workfront for Jira]之前，您必須：

* 安裝[!DNL Workfront for Jira]。
如需安裝[!DNL Workfront for Jira]的說明，請參閱[安裝 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)。

## 設定[!DNL Workfront for Jira]

透過設定[!DNL Workfront for Jira]，您可以：

* 定義將在建立[!DNL Jira]個專案時建立[!DNL Workfront]個專案的觸發器。
* 指定在[!DNL Jira]和[!DNL Workfront]之間連結的專案之間應同步處理哪些欄位。

>[!NOTE]
>
>* 在您的[!DNL Workfront for Jira]環境中設定[!DNL Jira]後，所有[!DNL Jira]使用者都會在所有[!DNL Workfront]專案上看到[!DNL Jira]右側面板。 面板包含可能從[!DNL Workfront]連結之專案的相關資訊，或指定沒有[!DNL Workfront]專案連結至[!DNL Jira]專案。
>* 使用[!DNL Jira Server]安裝時，只有與識別為Workfront整合觸發器的專案關聯的問題才會顯示Workfront面板。 如需為[!DNL Workfront to Jira]工作流程設定觸發程式的詳細資訊，請參閱[設定觸發程式，以自動連結 [!DNL Jira] 與 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront)之間的專案。
>

若要設定[!DNL Workfront for Jira]：

1. 以[!DNL Jira]管理員身分登入[!DNL Jira]。
1. 在主&#x200B;**[!UICONTROL 功能表中按一下]**&#x200B;設定[!DNL Jira]。
1. 按一下&#x200B;**[!UICONTROL 附加元件]**，然後按一下&#x200B;**[!UICONTROL 管理附加元件]**。

1. 展開&#x200B;**[!DNL Workfront]**&#x200B;附加元件。
1. 按一下&#x200B;**[!UICONTROL 設定]**。
1. 依照提示登入[!DNL Workfront]。

   >[!NOTE]
   >
   >使用者必須在`apiKey`Workfront[!UICONTROL 中擁有有效的]，才能建立成功的連線。

   您必須以[!DNL Workfront]管理員身分登入[!DNL Workfront]才能繼續設定。

   >[!NOTE]
   >
   >* [!UICONTROL Workfront]使用OAuth 2.0連線至[!DNL Jira]，這是大部分的網頁式整合所使用的標準，用於驗證及授權使用者。
   >* 當系統提示您輸入[!DNL Workfront]帳戶的網域時，請使用此格式輸入它： *yourCompany&#39;sDomain.my.workfront.com*。 您公司的網域通常是您公司的名稱。
   >* 增強式驗證必須由[!DNL Workfront]系統管理員針對這項整合啟用才能使用。

1. 在Jira中，選取&#x200B;**[!UICONTROL 觸發器]**&#x200B;索引標籤，當建立新的[!DNL Jira]專案時，設定自動建立[!DNL Workfront]專案。

   如需設定Workfront至[!DNL Jira]工作流程觸發程式的詳細資訊，請參閱[設定自動連結 [!DNL Jira] 與 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront)之間專案的觸發程式。

1. 選取「**[!UICONTROL 設定]**」標籤，以設定連結[!DNL Jira]與[!DNL Workfront]專案之間的欄位同步化。

   如需設定[!DNL Jira]與[!DNL Workfront]之間欄位同步化的詳細資訊，請參閱[設定 [!DNL Jira] 與 [!DNL Workfront] 專案之間的欄位同步化](#configure-field-synchronization-between-jira-and-workfront-items)。

   >[!NOTE]
   >
   >定義兩個應用程式之間的觸發器和欄位同步之後，任何可以建立任務或問題的[!DNL Workfront]使用者都可能觸發在[!DNL Jira]中建立專案。 如果使用者建立專案的條件符合[!DNL Jira]中的觸發程式，即使使用者沒有[!DNL Jira]授權，使用者也可以建立專案。 此外，任何[!DNL Jira]使用者都可以立即開始處理[!DNL Jira]專案，且可在[!DNL Workfront]中看到其更新，而無需擁有[!DNL Workfront]授權。 [!DNL Workfront]中的任何更新也會顯示在[!DNL Jira]個專案上。

1. （選擇性）選取&#x200B;**[!UICONTROL 活動記錄]**&#x200B;標籤，以檢閱整合期間可能發生的任何錯誤。

   如需[!UICONTROL 活動記錄]的詳細資訊，請參閱[檢視 [!DNL Jira] [!UICONTROL 活動記錄]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md)。

## 設定在[!DNL Jira]和[!DNL Workfront]之間自動連結專案的觸發程式

作為[!DNL Jira]系統管理員，您可以定義在[!DNL Jira]中的專案符合特定條件時，在[!DNL Workfront]中自動建立問題的觸發程式。

>[!NOTE]
>
>整合最多可能需要10分鐘的時間才能在[!DNL Jira]中建立新問題。

當已建立[!DNL Jira]個專案，在設定觸發建立[!DNL Workfront]專案時，請考量下列事項：

* 整合是單向的：您只能觸發您在[!DNL Workfront]中建立的專案，使其自動在[!DNL Jira]中建立。 您無法觸發您在[!DNL Jira]中建立的專案，使其自動在[!DNL Workfront]中建立。
* 您可以使用的觸發器數量沒有限制。
* 如果您在[!DNL Workfront]中建立的專案符合多個觸發程式，則在[!DNL Jira]中只會建立一個專案。 專案是根據第一個觸發程式在[!DNL Jira]中建立（按照它們在[!DNL Jira]中定義的順序）。 忽略所有其他觸發程式。
* 在[!DNL Workfront]中只有一個專案可以連結到Jira中的一個專案。 您永遠無法將一個[!DNL Workfront]專案連結至多個[!DNL Jira]問題，或一個[!DNL Jira]問題連結至多個[!DNL Workfront]專案。

若要設定在[!DNL Jira]中自動建立專案的觸發程式：

1. 以系統管理員身分登入[!DNL Jira]。
1. 在主&#x200B;**[!UICONTROL 功能表中按一下]**&#x200B;設定[!DNL Jira]。
1. 按一下&#x200B;**[!UICONTROL 附加元件]**，然後按一下&#x200B;**[!UICONTROL 管理附加元件]**。
1. 展開&#x200B;**[!DNL Workfront]**&#x200B;附加元件。
1. 按一下&#x200B;**[!UICONTROL 設定]**。
1. 以系統管理員身分登入[!DNL Workfront]。

   Jira預設會選取&#x200B;**[!UICONTROL 觸發器]**&#x200B;標籤。

1. 按一下&#x200B;**[!UICONTROL 新增觸發器]**&#x200B;以新增觸發器。
1. 在&#x200B;**[!UICONTROL Workfront團隊/使用者/角色]**&#x200B;欄位中，指定[!DNL Workfront]團隊、使用者或工作角色的名稱，然後按一下以在清單中顯示時選取它。

   >[!NOTE]
   >
   >同一個團隊、使用者或角色不能有多個觸發程式。

   當有人建立任務或問題並將其指派給其中一個實體時，問題會自動在[！DNL [!DNL Jira]]中建立。

1. 在&#x200B;**[!UICONTROL [!DNL Jira]專案]**&#x200B;欄位中，開始輸入[!DNL Jira]專案的名稱，然後按一下以在清單中顯示時選取它。

   建立[!DNL Jira]問題時，它會放置在您在此處選擇的專案上。

1. 從下拉式功能表中選取&#x200B;**I[!UICONTROL 問題型別]**。

   這表示當符合此觸發器的條件時，根據[!DNL Jira]中該特定專案的設定，在[!DNL Jira]中建立的問題型別。

1. 按一下「**[!UICONTROL 儲存]**」。

   使用此設定，每當[!DNL Workfront]使用者建立符合指定觸發器的專案時，[!DNL Jira]中就會建立新問題。

## 設定[!DNL Jira]和[!DNL Workfront]專案之間的欄位同步處理

作為[!DNL Jira]管理員，您可以定義哪些欄位應該自動同步處理[!DNL Workfront]和Jira之間連結的專案。 某些欄位可以從[!DNL Workfront]同步到[!DNL Jira]專案，而其他欄位則可以從Jira同步到Workfront。

若要定義應在兩個應用程式之間連結的專案上自動同步化的欄位：

1. 以Jira管理員身分登入[!DNL Jira]。
1. 在主&#x200B;**[!UICONTROL 功能表中按一下]**&#x200B;設定[!DNL Jira]。
1. 按一下&#x200B;**[!UICONTROL 附加元件]**，然後按一下&#x200B;**[!UICONTROL 管理附加元件]**。
1. 展開&#x200B;**[!DNL Workfront]**&#x200B;附加元件。
1. 按一下&#x200B;**[!UICONTROL 設定]**。
1. 以Workfront管理員身分登入[!DNL Workfront]。
1. 在Jira中，按一下&#x200B;**[!UICONTROL 設定]**&#x200B;標籤。
1. 在&#x200B;**[!UICONTROL 從Workfront同步到Jira]**&#x200B;區段中，選取在Workfront中更新欄位時，您要在[!DNL Jira]中更新的欄位。

   1. 選取下列任何與欄位同步化的頻率：

      <table style="table-layout:auto">
         <tr>
              <td>[！UICONTROL建立時]</td>
              <td>在Workfront中建立專案時，您指定的欄位會在連結的Workfront和[!DNL Jira]專案之間同步。</td>
          </tr>
          <tr>
              <td>[！UICONTROL Always]</td>
              <td>在Workfront中更新欄位時，您指定的欄位會在連結的Workfront和[!DNL Jira]專案之間同步。 </td>
          </tr>
          <tr>
              <td>[！UICONTROL從不]</td>
              <td>您指定的欄位永遠不會在連結的[!DNL Workfront]和[!DNL Jira]專案之間同步。 [!DNL Jira]中沒有表示欄位已在[!DNL Workfront]中更新。 </td>
          </tr>
      </table>

   1. 選取下列任一項，同步處理從[!DNL Workfront]到[!DNL Jira]的欄位：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL名稱]</td>
         <td><p>[!DNL Workfront]中任務或問題的名稱會變成[!DNL Jira]中連結問題的名稱。</p><p>注意：在[!DNL Jira]中自動建立新專案時，[!DNL Workfront]名稱一律會在[!DNL Jira]專案上更新，無論此處是否啟用此欄位。 當[!DNL Jira]專案手動連結至[!DNL Workfront]專案時，當您選取[!DNL Workfront]一律同步[!DNL Jira]此欄位時，<strong>專案的名稱只會在</strong>中更新。 如需手動或自動連結專案的詳細資訊，請參閱<a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">在[!DNL Adobe Workfront]和[!DNL Jira]</a>之間連結專案。</p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL說明]</td>
         <td>[!DNL Workfront]中任務或問題的描述會變成它在[!DNL Jira]中連結到的問題的描述。</td>
        </tr>
        <tr>
         <td role="rowheader">文件</td>
         <td><p>附加至[!DNL Workfront]中之任務或問題的檔案也會附加至Jira中連結的問題。 來自[!DNL Workfront]的新檔案版本會新增為個別檔案至Jira，並附加<i>_v&lt;version number&gt;</i>以表示Workfront中的編號版本。 </p><p>例如，如果[!DNL Workfront]中檔案的名稱是<strong>Main Ad</strong>，而您在[!DNL Workfront]中新增新版本，則新版本會以名稱為[!DNL Jira]Main Ad_v2<strong>的新檔案形式傳輸至</strong>。</p><p>重要： <p>同步檔案時，請考量下列事項：</p>
           <ul>
            <li><p>大於5MB的檔案不會同步。 如果檔案同步因為檔案太大而失敗，活動記錄中會記錄一個錯誤。 </p><p>如需活動記錄檔的詳細資訊，請參閱<a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">檢視Jira活動記錄檔</a>。</p></li>
            <li><p>連結到外部伺服器之任務和問題的檔案未傳輸到[!DNL Jira]專案。 只有直接在任務上上傳的檔案或[!DNL Workfront]中的問題才會傳輸到[!DNL Jira]中的連結問題。</p></li>
            <li><p>若要從檔案建立校訂，您必須在[!DNL Workfront]中產生校訂。 </p><p>如需有關產生校訂的詳細資訊，請參閱<a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">建立檔案的校訂</a>中的<a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">為現有的檔案</a>建立校訂。<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL計畫完成日期]</td>
         <td><p>[!DNL Workfront]中任務或問題的[！UICONTROL規劃完成日期]成為[!DNL Jira]中連結之問題的[！UICONTROL到期日]。</p><p>注意：請確定您在<strong>個問題上顯示</strong>[！UICONTROL到期日][!DNL Jira]，以便同步處理此值。</p></td>
        </tr>
       </tbody>
      </table>

1. 在&#x200B;**[!UICONTROL 從[!DNL Jira]同步至[!DNL Workfront]]**&#x200B;區段中，選取在[!DNL Workfront]中更新欄位時，您要在[!DNL Jira]中更新的欄位。

   1. 選取下列任何與欄位同步化的頻率：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL Always]</td>
         <td>在[!DNL Workfront]中更新欄位時，您指定的欄位一律會在連結的[!DNL Jira]和[!DNL Jira]專案之間同步。 </td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL從不]</td>
         <td><p>您指定的欄位永遠不會在連結的[!DNL Workfront]和[!DNL Jira]專案之間同步。 [!DNL Workfront]中沒有表示欄位已在[!DNL Jira]中更新。 </p><p>注意：當您選取[永不]時，仍可以從[!DNL Workfront]問題左側[!DNL Jira]面板的[!DNL Workfront]手動更新[!DNL Jira]欄位。 這些更新只會顯示在[!DNL Workfront]和[!DNL Jira]中的[!DNL Workfront]個專案上，不會顯示在[!DNL Jira]個專案上。</p></td>
        </tr>
       </tbody>
      </table>

   1. 選取以同步處理從[!DNL Jira]到[!DNL Workfront]的下列任何欄位：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL狀態]</td>
         <td>[!DNL Jira]中問題的[！UICONTROL狀態]會變成[!DNL Workfront]中連結至的任務或問題的[！UICONTROL狀態]。<br>如需[!DNL Workfront]狀態的詳細資訊，請參閱<a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>。</td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL受託人]</td>
         <td><p>[!DNL Jira]中問題的[！UICONTROL受指派人]會成為[!DNL Workfront]中連結至該問題或任務的[！UICONTROL受指派人]。</p><p>重要：當您將[!DNL Jira]中的專案指派給沒有[!DNL Workfront]帳戶的使用者時，整合僅當[!DNL Workfront]使用者沒有<strong>帳戶[!DNL Workfront]設定為[!DNL Jira][！UICONTROL Always][!DNL Workfront]時，</strong>在<strong>中自動建立使用者時，才會在</strong>中建立新的作用中使用者。 此使用者未佔用[!DNL Workfront]授權。 可將作用中的使用者指派給[!DNL Workfront]中的工作專案，但不能包含在更新中。 </p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL附件]</td>
         <td>[!DNL Jira]中問題的附件也附加至它在[!DNL Workfront]中連結的任務或問題。 </td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL註解]</td>
         <td><p>[!DNL Jira]問題的註解也會張貼在[！UICONTROL更新]區域中連結的[!DNL Workfront]專案上。 相反地，針對[!DNL Workfront]任務或問題在[！UICONTROL更新]區域張貼的註解，會同步至[!DNL Jira]的連結問題原生註解流。 </p><p>預設會設為<strong>[！UICONTROL一直]</strong>。 如果您在這裡選取<strong>[！UICONTROL Never]</strong>，您仍可在[!DNL Workfront]或[!DNL Jira]中手動在連結專案上張貼註解。</p></td>
        </tr>
       </tbody>
      </table>

1. 在&#x200B;**[!UICONTROL OTHER]**&#x200B;區段中，選取連結專案之間應更新的其他欄位。

   1. 選取選項，以決定您指定的欄位在修改時，是在&#x200B;**[!UICONTROL 或]**&#x200B;中的&#x200B;**[!UICONTROL 一律]**&#x200B;或[!DNL Jira]永不[!DNL Workfront]更新。

   1. 從下列欄位和更新中選取：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL複製[!DNL Workfront]中右側面板中的[!DNL Jira]自訂資料</td>
         <td><p>顯示[!DNL Workfront]右側面板中專案的[!DNL Workfront]自訂資料。</p><p>注意：自訂表單區段會顯示在具有[!DNL Workfront]系統管理員存取層級的[!DNL Workfront]右側面板中。</p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL複製[!DNL Workfront]中右側面板的[!DNL Jira]優先順序</td>
         <td>顯示[!DNL Workfront]右側面板中專案的[!DNL Workfront]優先順序。</td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL在「[!DNL Workfront] Updates」索引標籤中新增有關「[!DNL Jira]」中到期日變更的更新</td>
         <td>當連結的[!DNL Workfront]專案中的[！UICONTROL到期日]變更時，在[!DNL Jira]專案的[！UICONTROL Update]索引標籤中新增註解。</td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL如果[!DNL Workfront]使用者沒有[!DNL Jira]帳戶，則在[!DNL Workfront]中自動建立使用者]</td>
         <td><p>存在下列情況：</p>
          <ul>
           <li>當您選取<strong>[！UICONTROL Always]</strong>時，您啟用整合，以便在每次沒有[!DNL Jira]帳戶的[!DNL Workfront]使用者對連結的[!DNL Jira]問題執行下列動作時，建立新的Workfront使用者：
            <ul>
             <li>已指派給[!DNL Jira]問題</li>
             <li><p>將時間記錄到[!DNL Jira]問題</p><p>此新使用者未佔用[!DNL Workfront]授權。 預設設定為「一律」。 在[!DNL Workfront]中以此方式建立的使用者已將「[！UICONTROL Jira]」新增至其名稱。</p></li>
            </ul></li>
           <li>當您選取<strong>[！UICONTROL Never]</strong>時，會發生下列情況：
            <ul>
             <li>您無法在[!DNL Jira]個專案上看到任何[!DNL Workfront]指派。 在此情況下，只有在[!DNL Workfront]中完成的指派會顯示在[!DNL Workfront]個專案上。</li>
             <li>沒有[!DNL Jira]帳戶的使用者登入已連結[!DNL Workfront]問題的時間不會自動傳輸至已連結的[!DNL Workfront]專案。 您仍然可以在[!DNL Workfront]問題的右側面板中的[!DNL Jira]專案上記錄時間。</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. 按一下「**[!UICONTROL 儲存]**」。

   現在，每當使用者更新此設定中在[!DNL Jira]或[!DNL Workfront]中專案上指定的任何欄位時，其他應用程式中的連結專案也會更新。

## 疑難排解

### 無法在[!DNL Jira]中建立專案，因為找不到標示為&quot;&quot;的觸發欄位

#### 問題

當[!DNL Workfront for Jira]應用程式發生錯誤時，[!DNL Workfront]會停用觸發程式以避免進一步的複雜性。 當這些觸發程式停用時，會顯示為&quot;[!UICONTROL 找不到]&quot;。

#### 解決方案

找出停用觸發程式的錯誤。 您可以在[!DNL Workfront for Jira] [!UICONTROL 活動記錄]中找到錯誤。

發生此行為的最常見原因是錯誤&#39;&#39;[!UICONTROL 無法設定&#39;duedate&#39;欄位。 不在適當的熒幕上，或未知。]」

此錯誤表示您正嘗試將&quot;[!UICONTROL 規劃完成日期]&quot;從[!DNL Workfront]同步至[!DNL Jira]。 若要這麼做，您必須確定您的[!DNL Jira]物件有一個名為&quot;[!UICONTROL 到期日]&quot;的欄位。 如果他們沒有此欄位，[!DNL Workfront]將無法從[!DNL Workfront]同步計畫完成日期，並停用您的觸發器。

若要解決此錯誤，請嘗試下列方法之一：

* 請要求您的[!DNL Jira]管理員更新受影響的[!DNL Jira]物件，以確保它們有到期日欄位。
* 在Workfront [!DNL Workfront]安裝程式[!UICONTROL 頁面中停用]計畫完成日期的同步處理。
