---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: 更新 [!DNL Jira] 和 [!DNL Adobe Workfront]之間的連結專案
description: 當您將 [!DNL Jira] 問題連結至 [!DNL Adobe Workfront] 個任務或問題時，您的使用者可以更新一個應用程式中的專案，而該專案的對應專案也會更新第二個應用程式中工作的使用者。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: 064418302767ad20e176080ba9a12db548750f3c
workflow-type: tm+mt
source-wordcount: '1662'
ht-degree: 0%

---

# 更新[!DNL Jira]和[!DNL Adobe Workfront]之間的連結專案

>[!IMPORTANT]
>
>為了提供更穩定且更可擴充的整合，我們改用現代、彈性的整合方法，即使用Workfront自動化與整合(Fusion)。 在此轉換過程中，Jira整合的Workfront在&#x200B;**2026年2月28日**&#x200B;後將無法使用。
>
>根據貴組織與Jira的整合需求，我們建議使用Workfront自動化和整合。
>
>如需Workfront自動化與整合的概觀，請參閱[Adobe Workfront Fusion概觀](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>如需Jira的Workfront自動化與整合模組特定功能的相關資訊，請參閱[Jira軟體模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)。

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

當您將[!DNL Jira]問題連結至[!DNL Adobe Workfront]個任務或問題時，您的使用者可以更新一個應用程式中的專案，而該專案的對應專案也會更新第二個應用程式中工作的使用者。

如需在[!DNL Workfront]和[!DNL Jira]之間連結專案的詳細資訊，請參閱[在Adobe Workfront和Jira之間連結專案](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md)。

當您為[!DNL Workfront]設定[!DNL Jira]時，身為[!DNL Jira]系統管理員，您可以設定一個應用程式中的特定欄位，以便與另一個應用程式中連結專案的欄位同步。

如需有關在連結的[!DNL Jira]和[!DNL Workfront]專案之間同步處理欄位的詳細資訊，請參閱[設定 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td><p>新增：任何</p>
       <p>或</p>
       <p>目前： [!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>新增：[!UICONTROL Standard]</p>
       <p>或</p>
       <p>目前： [!UICONTROL 計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 存取</td> 
   <td> <p>系統管理員存取權</p> <p>重要：建議您在[!DNL Jira]和[!DNL Workfront]中建立個別的系統管理員帳戶以專用於此整合，而不使用可能附加至使用者的現有帳戶。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是[!DNL Workfront]管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先決條件

在[!DNL Workfront]和[!DNL Jira]之間連結專案之前，您必須：

* 安裝[!DNL Workfront for Jira]。

  如需安裝[!DNL Workfront for Jira]的說明，請參閱[安裝 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)。

* 設定[!DNL Workfront for Jira]。

  如需設定[!DNL Workfront for Jira]的說明，請參閱[設定 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

* 連結介於[!DNL Workfront]和[!DNL Jira]之間的專案。

  如需指示，請參閱[介於 [!DNL Adobe Workfront] 和 [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md)之間的連結專案。

## 更新[!DNL Workfront]中的連結專案

如果您主要在[!DNL Workfront]中工作，則可以更新[!DNL Workfront]中的工作專案，而[!DNL Jira]中的對應專案也會更新。 此更新是透過[!DNL Workfront]的[!DNL Jira]整合而進行，不需要您擁有[!DNL Jira]授權。

只要您的[!DNL Workfront]管理員已設定[!DNL Workfront for Jira]同步處理連結專案之間的欄位，您在[!DNL Workfront]中更新的某些欄位也會更新連結的[!DNL Jira]問題。 如需有關更新[!DNL Workfront]中專案的詳細資訊，請參閱[編輯問題](../../manage-work/issues/manage-issues/edit-issues.md)和[編輯任務](../../manage-work/tasks/manage-tasks/edit-tasks.md)。

下列清單顯示哪些[!DNL Workfront]欄位與連結專案上的[!DNL Jira]欄位同步：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>已更新[!DNL Workfront]欄位</strong> </th> 
   <th><strong>已同步的[!DNL Jira]欄位/更新</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 問題或任務名稱]</td> 
   <td> <p>[!UICONTROL 問題名稱]</p> <p>有關名稱變更的註解已新增至<strong>[!DNL Workfront]</strong>問題的[!DNL Jira]索引標籤。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 問題或任務說明]</td> 
   <td> <p> [!UICONTROL 問題說明]</p> <p>有關已更新說明的註解已新增至<strong>[!DNL Workfront]</strong>問題的[!DNL Jira]索引標籤。<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL 已上傳檔案]</p> <p>注意：從外部伺服器連結到[!DNL Workfront]個專案的檔案未傳輸到[!DNL Jira]個問題。 只有直接上傳至[!DNL Workfront]個專案的檔案才會更新為連結的[!DNL Jira]問題。 </p> </td> 
   <td> <p>[!UICONTROL 附件]</p> <p>已上傳附件的相關註解已新增至<strong>[!DNL Workfront]</strong>問題的[!DNL Jira]索引標籤。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 計畫完成日期]</td> 
   <td> <p>[!UICONTROL 到期日期]</p> <p>有關[!UICONTROL 到期日]已變更的註解已新增至[!DNL Workfront]問題的[!DNL Jira]索引標籤。 </p> <p>注意：您必須針對您的<strong>問題啟用</strong>[!UICONTROL 到期日][!DNL Jira]，才能在[!UICONTROL Jira]中看到此欄位已更新。 </p> </td> 
  </tr> 
  <tr> 
   <td>自訂Forms和自訂欄位</td> 
   <td> <p> 顯示在[!DNL Workfront]問題的[!DNL Jira]右側面板中。 <br>面板中只會顯示具有實際值的自訂欄位。<br></p> <p>注意：自訂表單區段會以[!DNL Workfront]管理員的存取層級顯示。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 問題或任務優先順序]</td> 
   <td>顯示在[!DNL Workfront]問題的[!DNL Jira]右側面板中。 <br>它不會更新<strong>中的問題</strong>[!UICONTROL 優先順序][!DNL Jira]欄位。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 記錄時間] </td> 
   <td> <p>有關記錄時間的註解已新增到<strong>[!DNL Workfront]</strong>問題的[!DNL Jira]索引標籤中。 這包括記錄時間的使用者名稱，以及記錄時間的使用者名稱（如果不同）。 <strong>中的</strong>[!UICONTROL 工作記錄檔][!DNL Jira]索引標籤未記錄任何時間。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 註解]</td> 
   <td> <p>註解已新增至<strong>[!DNL Workfront]</strong>問題的[!DNL Jira]索引標籤。 未新增至<strong>問題的</strong>[!UICONTROL 註解][!DNL Jira]索引標籤</p> <p>注意：當您手動連結兩個現有專案時，在連結至[!DNL Workfront]之前新增至[!DNL Jira]專案的評論不會同步至[!DNL Jira]問題。 </p> <p>Jira註解會同步至Workfront。</td> 
  </tr> 
 </tbody> 
</table>

## 更新[!DNL Jira]中的連結專案

如果您主要在[!DNL Jira]中工作，則可以更新[!DNL Jira]中的工作專案，而[!DNL Workfront]中的對應專案也會更新。 連結至您[!DNL Workfront]問題的[!DNL Workfront]專案不一定要有[!DNL Jira]授權才能接收您在[!DNL Jira]中進行的更新。

在您的[!DNL Workfront]管理員已為[!DNL Workfront]設定[!DNL Jira]同步處理連結專案之間的欄位的情況下，您在[!DNL Jira]中更新的某些欄位也會更新連結的[!DNL Workfront]專案。

下列清單顯示哪些[!DNL Jira]欄位與連結專案上的[!DNL Workfront]欄位同步：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>已更新[!DNL Jira]欄位</strong> </th> 
   <th><strong>已同步的[!DNL Workfront]欄位/更新</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 問題狀態]</td> 
   <td> <p> [!UICONTROL 問題或任務狀態]</p> <p>在Workfront中，[!DNL Jira]中的問題狀態會與以下狀態同步，或是與以下狀態相等的狀態：</p> 
    <ul> 
     <li> <p>[!UICONTROL NEW] ([!UICONTROL NEW])</p> </li> 
     <li> <p>[!UICONTROL 進行中] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL 已關閉]/[!UICONTROL 完成] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>注意： [!DNL Jira]狀態會與相等於適當狀態的前[!DNL Workfront]個狀態同步。</p> <p>如需[!DNL Workfront]中專案狀態的詳細資訊，請參閱<a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>。</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL 問題附件]</td> 
   <td> [!UICONTROL 問題或任務檔案]<br>有關在[!DNL Jira]中上傳新檔案的註解已新增至[!DNL Workfront]問題或任務的[!UICONTROL 更新]索引標籤。  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 到期日期]</td> 
   <td> <p> 有關[!DNL Jira]中[!UICONTROL 到期日]變更的註解已新增至[!DNL Workfront]問題或任務的[!UICONTROL 更新]索引標籤。 </p> <p>注意： [!DNL Workfront]問題或任務上未變更日期。 </p> </td> 
  </tr> 
  <tr> 
   <td> 在[!DNL Workfront]右側面板中或從[!DNL Jira]問題上的[!UICONTROL 更多]功能表記錄時間<br></td> 
   <td> <p>時數<br>除了將登入Jira的時數新增至連結的[!DNL Workfront]專案外，有關登入時間的註解也會新增至[!DNL Workfront]專案的[!UICONTROL 更新]索引標籤。</p> <p>如需有關連結[!DNL Jira]問題的記錄時間的詳細資訊，包括更新在[!DNL Jira]中記錄時間的[!DNL Workfront]使用者，請參閱連結<a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">和[!DNL Jira]專案的[!DNL Workfront]記錄時間</a>。</p> </td> 
  </tr> 
  <tr> 
   <td> 註解 <br><br></td> 
   <td> <p>如果在[!UICONTROL Setup]索引標籤的[!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT]區段中的[!DNL Workfront][!UICONTROL Comments]<strong>設定為</strong>[!UICONTROL Always]<strong>，則會將評論新增至</strong>問題或任務的[!UICONTROL Updates]索引標籤。</p> <p>如需有關在[!DNL Jira]中設定Workfront設定的資訊，請參閱<a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">設定[!DNL Workfront for Jira]</a>。</p> <p>如需有關對連結[!DNL Jira]問題的專案發表意見的資訊，請參閱連結<a href="#comment-from-a-linked-jira-issue" class="MCXref xref">問題[!DNL Jira]的</a>發表意見。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 記錄已連結[!DNL Jira]個問題的時間

您在[!DNL Jira]中為[!DNL Jira]專案記錄的時間也會傳輸到連結的[!DNL Workfront]專案，無論您在[!DNL Jira]中記錄時間的位置為何。\
當您在[!DNL Workfront]面板中以Jira記錄時間時，時間僅記錄在[!DNL Workfront]中。\
您在[!DNL Workfront]中記錄的時間不會影響[!DNL Jira]中連結問題的時間。

>[!NOTE]
>
>如果將時間新增至連結至[!DNL Jira]任務的[!DNL Workfront]專案，則[!UICONTROL 中時間的]小時型別[!DNL Workfront]為[!UICONTROL 任務時間]。 如果將時間新增至連結至[!DNL Jira]問題的[!DNL Workfront]專案，則[!UICONTROL 中該時間的]小時型別[!DNL Workfront]為[!UICONTROL 問題時間]。

註解已新增至&#x200B;**[!DNL Workfront]**&#x200B;中的[!DNL Jira]標籤以及&#x200B;**[!UICONTROL 中專案的]**&#x200B;更新[!DNL Workfront]標籤，以記錄記錄記錄時間。\
時間也會顯示在&#x200B;**[!UICONTROL 專案的]**&#x200B;小時[!DNL Workfront]索引標籤中。

* 已連結[和 [!DNL Jira] 專案的 [!DNL Workfront] 記錄時間](#log-time-for-linked-jira-and-workfront-items)
* [將時間從 [!DNL Jira] 記錄到 [!DNL Workfront] 專案](#log-time-from-jira-to-a-workfront-item)

### 連結的[!DNL Jira]和[!DNL Workfront]專案的記錄時間

您可以從連結至[!DNL Jira]專案的[!DNL Workfront]問題記錄時間，該時間會記錄在[!DNL Jira]問題及[!DNL Workfront]專案上。

>[!IMPORTANT]
>
>如果在[!DNL Jira]中記錄時間的使用者不存在於[!DNL Workfront]中，則整合會在Workfront中建立新的作用中使用者(如果&#x200B;**[!UICONTROL 在[!DNL Workfront]中自動建立使用者(&#x200B;如果[!DNL Jira]使用者沒有&#x200B;*[!DNL Workfront]帳&#x200B;戶]**)，設定為&#x200B;**[!UICONTROL &#x200B;一律&#x200B;]**。 此使用者未佔用[!DNL Workfront]授權。 您可以將作用中的使用者指派給[!DNL Workfront]中的工作專案，但您不能將其包含在更新中。 如需有關從[!DNL Workfront]設定[!DNL Jira]使用者自動建立的資訊，請參閱[設定 [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

若要為[!DNL Jira]中的專案記錄時間，並將它同時記錄在[!DNL Jira]和[!DNL Workfront]中：

1. 登入[!DNL Jira]。
1. 移至連結至[!DNL Jira]專案的[!DNL Workfront]問題。
1. 展開&#x200B;**[!UICONTROL 更多]**&#x200B;功能表並按一下&#x200B;**[!UICONTROL 記錄工作]**。

1. 在&#x200B;**[!UICONTROL 逗留時間]**&#x200B;欄位中，指定處理此問題的逗留時間。 您必須使用下列期間來指定時間：

   * [!UICONTROL 周] （寬）
   * [!UICONTROL 天] (d)
   * [!UICONTROL 小時] （小時）

1. 繼續新增資訊至您的時間專案，包括&#x200B;**[!UICONTROL 工作描述]**，然後按一下&#x200B;**[!UICONTROL 記錄]**。\
   時間已新增至&#x200B;**[!UICONTROL 專案的]**&#x200B;工作記錄[!DNL Jira]索引標籤，以及連結至它的[!DNL Workfront]專案。\
   時間專案的工作說明會在[!DNL Workfront]中記錄為時數專案的備註。

### 將時間從[!DNL Jira]記錄到[!DNL Workfront]專案

您可以僅將時間記錄到從[!DNL Workfront]問題連結的[!DNL Jira]專案，而無需將時間記錄到[!DNL Jira]問題。

1. 登入[!DNL Jira]。
1. 導覽至連結至[!DNL Jira]專案的[!DNL Workfront]問題。

   [!DNL Workfront]專案的詳細資訊應顯示在問題的[!DNL Workfront]右側面板中。

1. 按一下&#x200B;**[!UICONTROL 記錄時間]**&#x200B;圖示。

1. 指定您想要針對此問題記錄的&#x200B;**[!UICONTROL 小時]**&#x200B;和&#x200B;**[!UICONTROL 分鐘]**&#x200B;的量。

1. 按一下&#x200B;**[!UICONTROL 記錄時間]**。

   時間已新增至[!DNL Workfront]專案。

   此時間未新增至[!UICONTROL 問題的]工作記錄[!DNL Jira]索引標籤。

## 來自已連結[!DNL Jira]問題的註解 {#comment-from-a-linked-jira-issue}

當您在[!DNL Jira]中從[!DNL Workfront]右側面板註解[!DNL Jira]專案時，註解也會新增到Workfront中連結專案的[!UICONTROL 更新]索引標籤中。

若要從[!DNL Jira]註解[!DNL Workfront]專案：

1. 登入[!DNL Jira]。
1. 導覽至連結至[!DNL Jira]專案的[!DNL Workfront]問題。

   [!DNL Workfront]專案的詳細資訊應顯示在問題的[!DNL Workfront]右側面板中。

1. 按一下「**[!UICONTROL 」面板或「]**&#x200B;註解[!DNL Workfront]」標籤中的「**[!UICONTROL 註解]**」圖示。

1. 開始輸入註解，然後按一下&#x200B;**[!UICONTROL 傳送]**。

   註解會新增至下列專案：

   * **[!DNL Workfront]**&#x200B;問題的[!DNL Jira]標籤。
   * **[!UICONTROL 問題的]**&#x200B;註解[!DNL Jira]標籤。
   * Workfront中連結專案的&#x200B;**[!UICONTROL 更新]**&#x200B;索引標籤。
