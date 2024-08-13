---
product-area: projects
navigation-topic: manage-issues
title: 編輯問題
description: 您可以編輯您已建立的問題資訊，或其他使用者已建立的問題（如果他們與您共用問題）的相關資訊。 本文說明如果您有搜尋、尋找和編輯問題的許可權，該如何搜尋、尋找和編輯問題。
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: f3641e2207563f3fc9d9ed059d889ab6c22f05b1
workflow-type: tm+mt
source-wordcount: '2529'
ht-degree: 2%

---

# 編輯問題

您可以編輯您已建立的問題資訊，或其他使用者已建立的問題（如果他們與您共用問題）的相關資訊。

您可以編輯單一問題，也可以編輯清單中的問題。 如需有關編輯清單中問題的資訊，請參閱[編輯清單中的問題](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>要求或更高版本</p> <p>檢閱或更高授權以編輯任務或專案的問題區段中的問題</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯問題的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需存取您存取層級中問題的相關資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授與問題的存取權</a>。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。 </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>Contribute對問題的許可權，以便編輯詳細資訊區域中的以下欄位： </p>
   <ul>
   <li>說明</li>
   <li>狀態</li>
   <li>嚴重程度</li>
   </ul>
   <p>管理問題的許可權，以編輯詳細資訊區域或編輯問題方塊中的所有欄位</p> <p> 如需授與問題許可權的相關資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題</a></p> <p>如需請求其他許可權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 編輯問題時的限制

有些限制可能會阻止您編輯問題。

* 您無法編輯核准流程中的問題。 您只能記錄時間或更新擱置核准中問題的狀態。
* 只有當您的Workfront管理員或群組管理員在專案偏好設定區域中啟用此功能時，您才能編輯檔案並將其新增到專案上狀態為「完成」、「廢棄」或「未決核准」的問題中。 如需有關設定專案偏好設定的資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

## 編輯單一問題

您可以使用編輯問題或問題詳細資訊區域編輯問題。 下列步驟說明如何編輯「編輯問題」方塊中的問題。

1. 移至&#x200B;**主功能表**。
1. 按一下&#x200B;**專案**，然後按一下專案名稱以開啟專案。
1. （選擇性）按一下&#x200B;**工作**，然後按一下工作的名稱以開啟工作。
1. 按一下左側面板中的&#x200B;**問題**。

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. （選擇性）若要編輯問題的有限資訊，請按一下左側面板中的&#x200B;**問題詳細資訊**。

   >[!NOTE]
   >
   >根據您的Workfront管理員或群組管理員如何修改您的版面配置範本，問題詳細資訊區域中的欄位可能會重新排列或不顯示。 如需詳細資訊，請參閱[使用配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

   若要編輯「詳細資訊」段落中的資訊，請執行下列動作：

   1. （選擇性）按一下右上角的&#x200B;**全部收合**&#x200B;圖示以收合所有區域。
   1. （選擇性和條件性）當區域摺疊時，按一下每個區域旁的&#x200B;**向右箭頭** ![](assets/right-pointing-arrow.png)以展開您要編輯的區域。
   1. （選擇性）若要附加自訂表單，請在&#x200B;**新增自訂表單**&#x200B;欄位中開始輸入表單的名稱，然後在清單中顯示時選取它，然後按一下&#x200B;**儲存變更**。
   1. （選擇性）按一下&#x200B;**匯出**&#x200B;圖示![](assets/export.png)，將概述和自訂表單資訊匯出至PDF檔案，然後按一下&#x200B;**匯出**。 從下列選項中選取：

      * 全選（至少附加一個自訂表單時顯示）
      * 概觀
      * 一或多個自訂表單的名稱

      PDF檔案會下載到您的電腦。

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      如需詳細資訊，請參閱[匯出自訂表單和物件詳細資料](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)。

   如需問題詳細資訊區段中可見欄位的相關資訊，請繼續編輯編輯問題方塊中的問題，如下所述。

1. 若要編輯關於問題的所有資訊，請選取清單中的問題，然後按一下清單頂端的&#x200B;**編輯**

   或

   按一下清單中問題的名稱，然後按一下問題名稱旁的&#x200B;**更多**&#x200B;功能表，然後&#x200B;**編輯。**

   **編輯問題**&#x200B;對話方塊隨即顯示。

   >[!IMPORTANT]
   >
   >您必須擁有問題的管理許可權才能檢視編輯連結。

   所有問題欄位都可在「編輯問題」方塊中使用，並按左側面板中列出的區域分組。

1. 請考慮在下列任何一節中指定資訊：

   * [問題名稱](#issue-name)
   * [概觀](#overview)
   * [指派](#assignments)
   * [自訂表單](#Custom%C2%A0F)
   * [設定](#settings)

   >[!NOTE]
   >
   >根據您的Workfront管理員如何設定版面配置範本，您的環境中編輯問題方塊中的欄位可能會不同。 如需詳細資訊，請參閱[使用配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。
   >
   >當您建立問題時，以下區段中列出的大多數欄位也可以從「新增問題」方塊存取。 欄位所在的區段與新問題方塊不符。 如需建立問題的相關資訊，請參閱[建立問題](../../issues/manage-issues/create-issues.md)。

### 問題名稱 {#issue-name}

1. 如上所述開始編輯問題。
1. 按一下&#x200B;**問題名稱**。

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. 更新&#x200B;**問題名稱**&#x200B;欄位。
1. 按一下&#x200B;**儲存**&#x200B;或繼續編輯下列區段。

### 概觀 {#overview}

1. 如上所述開始編輯問題。
1. 按一下&#x200B;**概觀**。

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. 更新或檢閱下表中的任何欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td> <p>新增問題的相關額外資訊。</p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader">基本資訊區段</td> 
     </tr> 
     <tr> 
      <td role="rowheader">狀態</td> 
      <td> <p>選取問題的狀態。 如需問題狀態的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">存取系統問題狀態清單</a>。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">優先等級</td> 
      <td> <p>這是視覺化標幟，可讓您排定問題的優先順序。</p> <p>從下列選項中選取：</p> 
       <ul> 
        <li> <p><strong>無</strong> </p> </li> 
        <li> <p><strong>低</strong> </p> </li> 
        <li> <p><strong>一般</strong> </p> </li> 
        <li> <p><strong>高</strong> </p> </li> 
        <li> <p><strong>緊急</strong> </p> </li> 
       </ul> <p>根據Workfront管理員選取的專案偏好設定，您的優先順序名稱可能會不同。 如需有關編輯優先順序的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">建立及自訂優先順序</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">嚴重程度</td> 
      <td> <p>這是視覺化旗標，可指出問題中所述問題的嚴重程度。 嚴重程度是問題的專屬值。 從下列選項中選取：</p> 
       <ul> 
        <li> <p style="font-weight: bold;">輕微</p> </li> 
        <li> <p style="font-weight: bold;">導致混淆</p> </li> 
        <li> <p style="font-weight: bold;">有因應措施的錯誤</p> </li> 
        <li> <p style="font-weight: bold;">無因應措施的錯誤</p> </li> 
        <li> <p style="font-weight: bold;">致命錯誤</p> </li> 
       </ul> <p>根據您的Workfront管理員所選取的專案偏好設定，嚴重程度的名稱可能會有所不同。 如需有關編輯嚴重程度的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">建立或自訂問題嚴重程度</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>鍵入與問題相關資訊相關的網頁連結。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">類型</td> 
      <td> <p>根據專案經理在專案的佇列詳細資料區域中選取的佇列屬性，您或許可以指定問題的型別。 從<b>型別</b>下拉式功能表中的下列選項中選取： </p> 
       <ul> 
        <li> <p><strong>錯誤報告</strong> </p> </li> 
        <li> <p><strong>變更順序</strong> </p> </li> 
        <li> <p><strong>問題</strong> </p> </li> 
        <li> <p><strong>請求</strong> </p> </li> 
       </ul> <p>根據您的Workfront管理員所選取的專案偏好設定，問題型別的名稱可能有所不同。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">主要連絡人</td> 
      <td>依預設，主要連絡人是問題的建立者。 若要修改此專案，請在Workfront中開始輸入任何作用中使用者的名稱，然後從清單中選取它。 問題只能有一個主要連絡人。<br>如果您變更主要連絡人，原始主要連絡人仍擁有此問題的管理存取權。 在共用問題時，您必須從「問題存取權」方塊手動移除此存取權。

   <b>提示</b>

   <p>新增主要聯絡人使用者時，請注意頭像、使用者的主要角色及其電子郵件地址，以區分具有相同名稱的使用者。 使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。</p>
      <p> 您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">授予使用者存取權</a>。</p>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">認可日期和時間</td> 
      <td> <p>這是問題的受分派者估計問題將完成的日期。 僅受指派人可以編輯此欄位。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計劃開始日期</td> 
      <td>依預設，計劃開始日期是建立問題的日期和時間。 您可以更新問題的<strong>規劃開始日期</strong>。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計畫完成日期和時間</td> 
      <td> 依預設，計畫完成日期是從預設計劃開始日期起的24小時。 依預設，問題的持續時間為1天。 您可以更新問題的<strong>規劃完成日期</strong>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際開始日期和時間</td> 
      <td>當您將問題的狀態變更為<strong>進行中</strong>時，會自動填入實際開始日期。 您可以更新問題的<strong>實際開始日期</strong>。 如有需要，您可以手動更新日期。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際完成日期和時間</td> 
      <td>當您將問題的狀態變更為<strong>已關閉</strong>或<strong>已解決</strong>時，會自動填入實際完成日期。 您可以更新問題的<strong>實際完成日期</strong>。 如有需要，您可以手動更新日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">解決者</td> 
      <td> <p>這會顯示問題是否已由其他物件解決。 您可以從下拉式選單中選取此問題是由任務、專案還是其他問題解決，然後開始輸入將解決此問題的任務、專案或問題的名稱。 當它出現在清單中時選取它。</p>

   <b>附註</b>

   當您選取要解決問題的物件時，問題狀態會連結到解決物件的狀態，並且無法在此問題上變更。 如需解析物件的詳細資訊，請參閱<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析物件概述</a>。

   <b>提示</b>

   當您的系統或群組管理員將「解決者」欄位新增到問題自訂標題時，當存在與問題關聯的解決物件時，該欄位將變更為「解決問題」、「解決任務」或「解決專案」。

   當此欄位顯示在問題標題中時，您無法編輯它。 如需自訂問題標題的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">使用版面配置範本自訂物件標題</a>
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">解決問題、解決任務或解決專案</td> 
      <td>解決問題(Issue)的問題、任務或問題的連結名稱。  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">解決了</td> 
      <td>在您存取的問題獲得解決時完成的問題連結名稱。  </td> 
     </tr>


   </tbody> 
   </table>





1. 按一下&#x200B;**儲存**&#x200B;或繼續編輯下列區段。

#### 指派 {#assignments}

1. 如上所述開始編輯問題。
1. 按一下左側面板中的&#x200B;**工作**。

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. 按一下&#x200B;**搜尋人員、角色和團隊**，然後開始輸入您要指派給工作的使用者、角色或團隊的名稱，然後按一下它，或當它顯示在清單上時按下Enter鍵。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >如果使用者名稱包含特殊字元，您必須在搜尋欄位中包含特殊字元。

   >[!TIP]
   >
   >您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
   >
   >
   >如果使用者、工作角色或團隊在停用之前已被指派，則他們仍被指派給工作專案。 在此情況下，我們建議採取下列步驟：
   >
   >* 將工作專案重新指派給作用中的資源。
   >* 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。

1. （選擇性）藉由將游標移至受指派人名稱上並按一下&#x200B;**設為主要受指派人**，指出受指派人是否為問題的主要受指派人。 團隊不能是問題的主要受指派人。
1. 更新下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">規劃時數</td> 
      <td> <p>這是問題的受指派人完成問題所需的實際時間。 輸入問題的計畫時數數目。<br></p> <p>附註：變更問題的計畫時數不會變更問題的計畫完成日期。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">受指派人角色</td> 
      <td> <p>當您選取某人作為受指派人時，請從<strong>受指派人的角色</strong>下拉式功能表中選取角色。 這是受指派人可以在此問題上履行的角色。 </p> <p><b>秘訣</b>

   下拉式功能表中只會顯示與其設定檔中每個受指派人相關聯的工作角色。</p> </td>
   </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**&#x200B;或繼續編輯下列區段。

### 自訂Forms

1. 如上所述開始編輯問題。
1. 按一下&#x200B;**自訂Forms**。

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. 在&#x200B;**新增自訂表單**&#x200B;欄位中，選取您要與問題相關聯的一或多個自訂表單。 您必須先建置自訂表單，才能在此欄位中選取它們。 清單中只會顯示作用中的自訂表單。 如需建立自訂表單的詳細資訊，請參閱[使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。 您可以新增最多10個自訂表單至問題。

1. （視條件而定）如果您將自訂表單附加到問題，請編輯表單上的任何欄位。 您必須指定所有必填欄位，然後才能儲存問題。

   >[!NOTE]
   >
   >根據您的Workfront管理員如何設定自訂表單中區段的許可權，不是每個人都可以檢視或編輯給定自訂表單上的相同欄位。 編輯自訂表單區段內欄位的許可權取決於您對問題本身的許可權。 如需設定自訂表單區段許可權的相關資訊，請參閱[使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。 如需關於設定問題許可權的資訊，請參閱[共用問題](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)。

1. 按一下&#x200B;**儲存**&#x200B;或繼續編輯下列區段。

### 設定 {#settings}

1. 如上所述開始編輯問題。
1. 按一下&#x200B;**設定**。

   ![](assets/settings-section-edit-issue-box-nwe-350x240.png)

   更新下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">核准流程</td> 
      <td> 
       <div> 
       <p>選取您要與問題關聯的核准流程。 您的Workfront管理員必須定義系統層級的核准流程，您才能將其與問題相關聯。 對核准程式<span>具有管理存取許可權的使用者也可以建立群組特定的核准程式。</span>如需有關建立核准流程的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">建立工作專案的核准流程</a>。 </p> 
       <p>新增核准程式時，請考量下列事項： </p> 
       <ul> 
       <li>清單中只會顯示有效的核准流程。 </li> 
       <li> <p>系統範圍及群組特定的核准程式會顯示在清單中。 與專案群組以外的群組相關聯的核准程式不會顯示在清單中。</p> <p>重要：如果專案的群組變更，群組特定核准流程會變成單一使用核准流程。 如需關於專案群組的變更或核准程式變更如何影響核准設定的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">群組和核准程式變更如何影響指派的核准程式</a>。 </p> </li> 
       <li> <p>您可以定義在建立請求佇列或佇列主題時，自動附加到問題的預設核准流程。 如需有關更新佇列詳細資料的資訊，請參閱<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a>。 如需有關建立佇列主題的資訊，請參閱<a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">建立佇列主題</a>。 </p> </li> 
       <li>大量編輯問題時，會出現以下情況： 
       <ul> 
       <li><p>當您從相同群組選取多個問題時，此欄位中會顯示系統層次和群組特定核准流程。</p></li> 
       <li><p>當您從不同的群組選取多個問題時，此欄位中只會顯示系統層級的核准流程。</p></li> 
       <li><p>當任何問題附加單一使用核准流程時，它會由您選取的系統層級或群組層級核准流程取代。 </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td> <p>選取您要為此問題附加提醒通知的核取方塊。 所有問題提醒通知都會顯示。 您的Workfront管理員必須先設定提醒通知，您才能在問題中選取通知。 如需設定提醒通知的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">設定提醒通知</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存。**

## 編輯問題標題中的問題（受限）

您可以在問題標題中編輯有限數量的資訊。

您的系統或群組管理員可以自訂您在問題標題中看到的欄位。 如需詳細資訊，請參閱[使用配置範本自訂物件標頭](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

![](assets/issue-header-350x19.png)

依預設，問題標題中包含下列欄位：

* 問題名稱
* 完成百分比
* 指派
* 計畫完成日期和時間
* 狀態
* 如果您在目前的核准程式中設為核准者，請進行核准決定
