---
product-area: requests
navigation-topic: create-requests
title: 建立及提交Adobe Workfront請求
description: 在Adobe Workfront，計畫的工作由項目和任務代表。 不過，您可能會在計畫外工作（以隨機請求的形式）隨時可能進入的環境中工作。 Workfront提供工作流程，透過使用「請求佇列」來容納此類環境。
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: b40ade1f1d7a9b81c654a274c5e8c872bf74b180
workflow-type: tm+mt
source-wordcount: '2337'
ht-degree: 2%

---

# 建立及提交Adobe Workfront請求

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE:&nbsp;If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

在Adobe Workfront，計畫的工作由項目和任務代表。 不過，您可能會在計畫外工作（以隨機請求的形式）隨時可能進入的環境中工作。 Workfront提供工作流程，透過使用「請求佇列」來容納此類環境。 

在「請求佇列」中建立請求後，您可以將請求指派給要完成的請求，或將其轉換為任務或專案。\
如需將問題轉換為任務或專案的詳細資訊，請參閱文章 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

您可以透過下列方式建立請求：

* 從頭開始，如本文所述。
* 從草稿。 如需詳細資訊，請參閱 [從草稿建立請求](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* 從現有請求複製並提交副本。 如需詳細資訊，請參閱 [複製和提交請求](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## 存取需求

<!--drafted for P&P - replace table: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯問題的存取權</p> <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 使用請求隊列的先決條件

身為Workfront管理員，您必須建立「請求佇列」，讓使用者可以使用這些功能。 具有計畫員許可證且對特定項目具有「編輯」訪問權限和「管理」權限的用戶也可以建立「請求隊列」。 

有關如何建立請求隊列的資訊，請參閱文章 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

您必須建立請求佇列的下列元件：

* 處於「目前」狀態的專案，會發佈為「說明請求佇列」。
* 佇列主題.\
   如需詳細資訊，請參閱文章 [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* 路由規則.\
   如需詳細資訊，請參閱文章 [建立路由規則](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* （選用）主題群組。\
   如需詳細資訊，請參閱文章 [建立主題群組](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* （選用）要求自訂表單。\
   如需詳細資訊，請參閱文章 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* （可選）請求審批流程。\
   如需詳細資訊，請參閱文章 [建立工作項的審批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 在Workfront網頁應用程式中建立請求並產生草稿

當您在Workfront網頁應用程式中建立請求時，Workfront會在您提交請求前，將請求儲存為草稿。 Workfront會在您選取請求佇列並開始輸入資訊時立即建立草稿。

您可以繼續提交請求，或者您可以填寫盡可能多的資訊，然後從請求處導航到以後完成。 Workfront會儲存您在「草稿」資料夾中啟動的草稿請求。

>[!IMPORTANT]
>
>使用草稿時，請考量下列事項：
>
>* 從協力廠商應用程式提交草稿請求時，Workfront不會建立這些請求，例如將它們以電子郵件傳送至Workfront，或使用任何其他應用程式建立草稿請求。 當您從Workfront Web應用程式外部提交請求時，請求會儲存在已提交區段。
>* 如果請求佇列的結構變更，您將無法再存取現有草稿。 例如，如果移除佇列主題或新增主題群組，則無法再存取儲存的草稿。
>


如需從現有草稿建立請求的相關資訊，請參閱 [從草稿建立請求](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). 如需刪除請求草稿的相關資訊，另請參閱 [刪除請求草稿](../../../manage-work/requests/create-requests/delete-request-draft.md).

若要在Workfront網頁應用程式中建立請求： 

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   </MadCap:conditionalText>
   -->

1. 按一下  **請求**，然後按一下 **新請求** 在頁面的右上角。

   >[!TIP]
   >
   >* 您可以從「請求」區域的任何區段存取「新增請求」選項。
   >* 當您沒有建立問題的存取權時，「新增請求」選項會呈現暗灰色。


1. （條件性）按一下 **請求類型** 欄位，並執行下列其中一項操作：

   * 從 **最近路徑** 區段，選取您最近用來開啟請求佇列的路徑。 路徑包括您最近提交的請求佇列、主題群組和佇列主題。 最後三個路徑依預設會顯示。

      >[!NOTE]
      >
      >Workfront只會在您實際提交請求時儲存路徑。 它不會為草稿請求建立路徑。

      ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * 從 **請求佇列** 區段，選擇請求佇列。
   * 輸入屬於先前存取之路徑的關鍵字，以搜尋請求佇列。

      例如，如果您有一個名為「幫助台」的請求隊列，其主題組名為「位置」，隊列主題名為「遠程」，則可以鍵入「remote」，並在其路徑的任何元素中顯示包含「remote」的所有請求隊列。

      >[!TIP]
      >
      >當您鍵入包含特殊字元的名稱時，即使您未鍵入該字元，請求隊列、隊列主題或主題組也會顯示。

      ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

      可用請求佇列和最近路徑的清單會動態更新，僅包含結果中醒目顯示之關鍵字的路徑。

      搜尋結果會顯示在下列區域下：

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">請求佇列</td> 
        <td>名稱中包含關鍵字的請求佇列</td> 
       </tr> 
       <tr> 
        <td role="rowheader">請求路徑</td> 
        <td> <p>包含關鍵字的路徑（包括請求佇列、主題群組、佇列主題），位於其元素的任何名稱中</p> </td> 
       </tr> 
      </tbody> 
     </table>
   >[!TIP]
   >
   >* 依預設，前200個請求佇列會以字母順序顯示。
   >* 請求佇列的名稱是已發佈為「說明請求佇列」的專案名稱。
   >* 將項目配置為選定請求隊列的說明顯示在請求隊列名稱的右側。

   >   
   >如需如何將專案以說明請求佇列發佈的詳細資訊，請參閱文章 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 在 **新請求** 表單中，執行以下操作之一：

   * （條件性）從「請求類型」欄位下顯示的通知訊息中選取可用的草稿。

      只有在您未提交草稿之前已儲存草稿時，才會顯示此區域。

      預設會顯示來自三個不同佇列主題的三個最近草稿。

      ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * 開始在選取的佇列中輸入新請求。

      當您開始輸入新請求的資訊，並在「主旨」欄位中為請求命名後，新草稿會自動儲存在「草稿」區段。

1. （選用）如果您的請求佇列包含主題群組，請在第一個下拉式欄位中選取主題群組的名稱。 否則，請選擇隊列主題。

   >[!TIP]
   將游標暫留在「主題群組」或「佇列主題」上時，「說明」欄位會顯示在右側。 這包含有關主題組或隊列主題的其他資訊。
   ![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >

   您的「請求佇列」最多可內建10層主題群組。\
   如需如何建立主題群組的詳細資訊，請參閱文章 [建立主題群組](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). 如需建立佇列主題的詳細資訊，請參閱文章 [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   如果您選取草稿或先前的路徑，則已選取主題群組和佇列主題。 您可以視需要選取不同的選項。

1. 視Workfront管理員在 **新問題欄位** 區段 **隊列詳細資訊** 在專案的子標籤上，提交新請求時，您可能會找到下列任何欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>主旨</strong> </td> 
      <td>指定請求的名稱。 這是必填欄位。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>說明</strong> </td> 
      <td>指定請求的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>指定可能與您的請求相關的URL。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先順序</strong> </td> 
      <td> <p>指定請求的優先順序。 優先順序應定義您認為此請求應解決的速度。 預設選項為： </p> 
       <ul> 
        <li>無</li> 
        <li>低 </li> 
        <li>標準</li> 
        <li>高</li> 
        <li>緊急</li> 
       </ul> <p>系統管理員可以修改優先順序的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>嚴重程度</strong> </td> 
      <td> <p>指定請求的嚴重性。 嚴重性應定義此請求對您的工作所產生的影響，以防其及時解決。 預設選項為：</p> 
       <ul> 
        <li>輕微</li> 
        <li>導致混淆</li> 
        <li>有因應措施的錯誤</li> 
        <li>無因應措施的錯誤</li> 
        <li>致命錯誤</li> 
       </ul> <p>系統管理員可以修改嚴重性的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>主要連絡人</strong> </td> 
      <td>請求的主要聯繫人預設為您，因為您是處理與請求相關的任何問題的要員。 不過，您可以將此變更為任何其他Workfront使用者。</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>指派</strong> </td> 
      <td> <p><span>指定應將請求分配給的活動用戶、作業角色或團隊的名稱。</span> </p> <p>您只能指定一個團隊。</p>

   <p> 根據請求佇列的設定方式，您可能只能指派一或兩種類型的資源給請求，而不是全部三種（例如，您可能只能指派請求給使用者）。</p>

   <p>如果路由規則也與請求隊列關聯，並且它自動將請求路由到不同類型的資源（例如，團隊），則您的請求將分配給在提交請求時手動指定的實體（用戶）和路由規則中指定的資源（團隊）。 </p>

   <p> 如需詳細資訊，請參閱下列文章：</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">建立路由規則</a> <br> </p> </li> 
      </ul> </p>

   <p><span>我們建議使用「請求隊列」的「路由規則」，以便自動將它們路由到相應的資源。</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>計畫小時</strong> </td> 
      <td> <p>預估完成此要求所需的時間。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計畫開始日期</strong> </td> 
      <td> <p>指定處理此請求的開始日期。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計畫完成日期</strong> </td> 
      <td>指定您要解析此請求的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>狀態</strong> </td> 
      <td>新請求的預設狀態為「新」。 您的系統管理員可能已更改此狀態的名稱。 您也可以從此下拉式功能表，將狀態變更為其他項目。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文件</strong> </td> 
      <td> <p>將檔案新增至您的請求。 </p> <p> 視請求佇列的設定方式而定， 「檔案」區段可能會在自訂欄位之前或之後顯示。 </p> <p>您上傳至Workfront的檔案會以草擬請求儲存24小時。 之後，您必須在返回編輯並提交草稿時重新附加這些草稿。 從其他驅動器連結的文檔將永久保存在草稿上。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）如果您的Workfront管理員將自訂表單與「請求佇列」或「佇列主題」建立關聯，請指定自訂表單內的欄位。\
   每個Workfront例項的自訂表單都不同。 
1. （選用和條件式）在輸入請求期間的任何時間點，按一下 [!UICONTROL **放棄草稿**] 如果要刪除自動建立的拔模。 這會刪除無法復原的草稿。 系統會顯示確認您正在刪除草稿的確認訊息。

1. （選用）按一下 [!UICONTROL **還原**] 確認訊息上，以回復動作並保留草稿。

1. 執行下列任一項作業：

   * 按一下 **提交** 如果您已準備好提交請求。 請求會儲存在「已提交」區段。 根據「請求隊列」的「路由規則」，此請求可能會路由到與指定為「請求隊列」的項目不同的項目。 有關路由規則的資訊，請參閱 [建立路由規則](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

      或

      按一下 **關閉** 如果您尚未準備好提交，您稍後可能會回來完成。 您的請求會儲存在「草稿」區段，下次您提交此請求佇列的請求時，即可使用。

      ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)
   當您提交請求時，草稿會自動刪除且無法還原。

   有關處理傳入請求的資訊，請參閱文章 [管理工作和團隊請求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   有關查找已提交或已起草請求的資訊，另請參閱 [找出提交的請求](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## 從Workfront外部建立請求

提交新請求並將其嵌入其他應用程式時，您可以共用請求佇列的直接連結。 從網路或其他應用程式存取此連結的使用者，也必須以有效的Workfront帳戶登入，才能存取此佇列並提交請求。 如需詳細資訊，請參閱 [共用請求佇列的連結](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## 以電子郵件傳送至Workfront以建立請求

如果您的「請求佇列」已啟用以透過電子郵件接收請求，您可以將請求直接透過電子郵件傳送至與「請求佇列」相關聯的電子郵件。

電子郵件的內文會新增為請求說明。

>[!NOTE]
當請求進入Workfront時，HTML格式會遭到移除，但簽名和現有的回覆執行緒內容不會遭到移除，並會顯示在請求說明中。

如需如何啟用「請求佇列」以透過電子郵件接收請求的詳細資訊，請參閱 [讓使用者將問題透過電子郵件傳送至「請求佇列」專案](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## 使用Outlook客戶端建立請求

您可以使用Outlook客戶端提交請求。 您可以建立新請求，也可以將電子郵件轉換為請求。 

有關使用Outlook客戶端提交請求的資訊，請參閱文章 [從Outlook電子郵件建立Adobe Workfront請求](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).

## 使用Workfront行動應用程式建立請求

您可以在智慧手機上使用行動應用程式提交請求。 您可以建立新請求，並將其提交到您有權在Web應用程式中查看的請求隊列。 

如需透過行動應用程式提交請求的相關資訊，請參閱 [請求](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests) 一節：

* [Adobe Workfront for Android](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md)
* [Adobe Workfront for iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md)

## 從其他應用程式建立請求

您可以使用已與Workfront整合的任何應用程式來提交請求： 

* 您可以在Workfront與其他應用程式之間建立自訂整合，讓您從其他應用程式將請求提交至Workfront。\
   如需自訂Workfront整合的詳細資訊，請參閱文章 [Adobe Workfront整合](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

* 如果您已安裝適用於Salesforce的Workfront應用程式，則可以提交Salesforce的請求。\
   如需使用適用於Salesforce的Workfront應用程式提交Salesforce請求的相關資訊，請參閱文章 [從Salesforce物件提交Adobe Workfront請求](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

## 找出提交的請求

有關查找已提交或已起草請求的資訊，請參見 [找出提交的請求](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
