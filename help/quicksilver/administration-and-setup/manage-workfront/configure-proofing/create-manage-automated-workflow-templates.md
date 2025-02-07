---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 建立及管理自動化工作流程範本
description: 作為Adobe Workfront管理員，如果您的組織的內容稽核程式經常重複或內容經常由同一人稽核，您可以建立包含稽核者的自動化工作流程範本，該範本具有您指定的校訂角色和通知設定。 自動化工作流程範本可能很簡單，只需一或兩個稽核者，或複雜且有許多階段和相依性。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '2079'
ht-degree: 0%

---

# 建立及管理自動化工作流程範本

<!-- Audited: 2/2024 -->

作為Adobe Workfront管理員，如果您的組織的內容稽核程式經常重複或內容經常由同一人稽核，您可以建立包含稽核者的自動化工作流程範本，該範本具有您指定的校訂角色和通知設定。 自動化工作流程範本可能很簡單，只需一或兩個稽核者，或複雜且有許多階段和相依性。

自動化工作流程範本可讓您輕鬆建立具有自動化工作流程的校訂。 當使用者建立校訂時，他們只需選擇所需的範本。

您可以隨時輕鬆變更任何「自動化工作流程」範本，新增或移除稽核者和階段。 而使用範本的校訂建立者可以新增或移除校訂的稽核者。

使用自動化工作流程範本時，請考量下列事項：

1. 自動化工作流程範本的設定會決定您可以使用自動化工作流程做哪些事來校訂。 例如，如果範本中停用「新增階段」按鈕，當您使用校訂的「自動化工作流程」設定時，將無法看到該按鈕。
1. 將人員新增至自動化工作流程範本中的階段時，但同時也以稽核者身分出現在校樣中，套用範本會從階段中移除稽核者。 如果您未將其他稽核者新增至階段，則會出現一則訊息，提示您新增稽核者。
1. 您修改自動化工作流程範本的能力取決於Workfront管理員設定的範本設定，如所述。 如果修改範本的功能已停用，則只有範本的擁有者可以修改它。

如需有關自動化工作流程的資訊，請參閱[自動化工作流程概觀](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>新增：任何</p><p>目前：Pro或更高</p><p>舊版：進階版或選取版</p> <p>如需有關不同方案的校訂存取許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準</p><p>目前：工作或計畫</p> <p>舊版：任何（您必須為使用者啟用校樣）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須在校訂許可權設定檔中選取管理員。 </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立自動化工作流程範本

{{step1-to-proofing}}

1. 按一下左側面板中的&#x200B;**工作流程**。
1. 在&#x200B;**工作流程**&#x200B;標籤上，按一下&#x200B;**新增** > **新增範本**。

1. 在&#x200B;**詳細資料**&#x200B;區段中，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">範本名稱</td> 
      <td>（必要）輸入範本的名稱。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">範本所有者</td> 
      <td>您可以選取將管理範本的Workfront管理員或Workfront Proof管理員。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">範本群組</td> 
      <td> <p> 如果您組織的自動化工作流程已組織成群組，您可以選取群組名稱。 如需詳細資訊，請參閱本文稍後的<a href="#create-automated-workflow-template-groups" class="MCXref xref">建立自動化工作流程範本群組</a>。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">範本時區 </td> 
      <td> <p>範本的預設時區是您正在使用的時區。 如果校樣建立者和將使用範本的稽核者的時區不同，您可以在此處變更它，以確保為這些使用者設定正確的時間舞台截止日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許</td> 
      <td> <p>您可以選取您希望人員可以使用範本建立校訂的階段活動。</p> 
      <p><b>警告</b>：如果您未選取「新增階段」和「將人員新增至階段」選項，則範本擁有者或使用此範本之任何校訂的擁有者，都無法新增階段或共用校訂。 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 在&#x200B;**階段**&#x200B;區段中，設定自動化工作流程範本的每個階段。

   您可以新增多個階段，並在它們之間建立。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td> <p>階段名稱會顯示在「工作流程」區段頂端的「自動化工作流程」圖表中、「校訂詳細資訊」頁面上，以及傳送給檢閱者的電子郵件通知中。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">啟用階段</td> 
      <td> <p>指定舞台是自動啟動還是手動啟動。 在第一階段，您可以選取<strong>建立校訂時</strong>、<strong>特定日期和時間</strong>或<strong>手動</strong>。</p> <p>當您新增第二個階段時，其他選項會變成可用，因為它們需要您選取父級階段。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">截止日期計算自</td> 
      <td> <p>指定計算截止日期的方式：</p> 
       <ul> 
        <li> <p><strong>校訂建立</strong>：在<strong>截止日期（+個工作日）</strong>下的下拉式清單中，選取要新增至校訂建立日期的營業日，以在校訂上自動設定截止日期。</p> </li> 
        <li><strong>階段開始時</strong>：在<strong>截止日期（+個工作日）</strong>下的下拉式清單中，選取要新增至階段啟用日期的營業日，以在校訂上自動設定截止日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">鎖定階段</td> 
      <td>指定是否允許將舞台鎖定以供註解。 選項包括手動或自動鎖定階段（在下一個階段開始時，或在父級階段上作出所有決定時）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">主要決策進行者</td> 
      <td> <p>只有您將稽核者新增到舞台後，可用的決策者才會顯示在清單中。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">只需要一個決定</td> 
      <td>當其中一位決策者提交其決定時，此階段的稽核程式即會完成。 如需詳細資訊，請參閱<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront Proof中設定校訂設定</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">私人階段</td> 
      <td>隱藏來自而未新增至階段或不是Workfront管理員的使用者的評論和決定。 如需詳細資訊，請參閱<a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動化工作流程總覽</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不允許刪除此階段</td> 
      <td> <p>將階段設為必要。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 如果使用此範本的校訂一律會傳送給階段中的相同人員，請在此處新增校訂，這樣使用者就不必每次建立校訂時都新增校訂。

   在將會使用此範本的校訂上選擇每個人的&#x200B;**角色**，以及您希望在使用者處理使用此範本的校訂時收到的&#x200B;**電子郵件警示**。

   有關校訂上角色的資訊，請參閱[設定預設校訂角色](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md)。 如需有關校訂電子郵件警示的資訊，請參閱文章[在Workfront Proof中設定電子郵件通知設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)中的[設定使用者的校訂預設值](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur)一節。

   每個使用者只能新增到一個階段。 您可以新增任意數量的使用者至階段。

   >[!TIP]
   >
   >您可以在階段圖表上的階段之間拖放檢閱者名稱。 可用的階段會以藍色反白顯示。

1. 對要新增至範本的任何其他階段重複前兩個步驟。

   在&#x200B;**工作流程**&#x200B;區段的頂端，您可以看到您正在設定的自動化工作流程圖表。 當您繼續新增階段時，它們會出現在圖表上，其中行顯示它們之間的相依性。 您可以按一下圖表中的某個階段，以檢視該階段的設定。

   如果您不需要檢視圖表，可以按一下&#x200B;**隱藏圖表**。

1. 在&#x200B;**與**&#x200B;共用範本區段中，按一下選項（如果範本尚未與整個組織共用）以指定能夠使用範本的人員。

   依預設，新的「自動化工作流程」範本會與您組織中的所有人共用。

1. 按一下「**建立**」。

## 修改自動化工作流程範本

身為Workfront Proof管理員，您可以修改自動工作流程範本。 您的變更會在您進行時自動儲存。

{{step1-to-proofing}}

1. 按一下左側面板中的&#x200B;**工作流程**。
1. 在出現的&#x200B;**工作流程範本**&#x200B;清單中，按一下您要修改的範本。
1. 在&#x200B;**詳細資料**&#x200B;區段中，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">範本名稱</td> 
      <td>（必要）輸入範本的名稱。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">範本所有者</td> 
      <td>您可以選取將管理範本的Workfront管理員或Workfront Proof管理員。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">範本群組</td> 
      <td> <p> 如果您組織的自動化工作流程已組織成群組，您可以選取群組名稱。 如需詳細資訊，請參閱本文稍後的<a href="#create-automated-workflow-template-groups" class="MCXref xref">建立自動化工作流程範本群組</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">範本時區 </td> 
      <td> <p>範本的預設時區是您正在使用的時區。 如果校樣建立者和將使用範本的稽核者的時區不同，您可以在此處變更它，以確保為這些使用者設定正確的時間舞台截止日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許</td> 
      <td> <p>選取您想要讓使用範本建立校訂的人可用的階段活動。 </p> <p><b>警告</b>：如果您未選取「新增階段」和「將人員新增至階段」選項，則範本擁有者或使用此範本之任何校訂的擁有者，都無法新增階段或共用校訂。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在&#x200B;**工作流程**&#x200B;區段中，變更任何階段的名稱並展開其設定![展開按鈕](assets/arrow-button.png)以進行任何必要的變更：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">截止日期計算自</td> 
      <td> <p>指定計算截止日期的方式：</p> 
       <ul> 
        <li> <p><strong>從校訂建立計算出的截止日期</strong>：在<strong>設定階段截止日期</strong>下拉式清單中，選取要新增至校訂建立日期的營業日數，以在校訂上自動設定截止日期。</p> </li> 
        <li><strong>從階段啟用計算出的截止日期</strong>：在<strong>設定階段截止日期</strong>下拉式清單中，選取要新增至階段啟用日期的營業天數，以在校訂上自動設定截止日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">啟用階段</td> 
      <td> <p>指定舞台是自動啟動還是手動啟動。 在第一階段，您可以選取<strong>建立校訂時</strong>、<strong>特定日期和時間</strong>或<strong>手動</strong>。</p> <p>當您新增第二個階段時，其他選項會變成可用，因為它們需要您選取父級階段。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">鎖定階段</td> 
      <td>指定是否允許將舞台鎖定以供註解。 選項包括手動或自動鎖定階段（在下一個階段開始時，或在父級階段上作出所有決定時）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">決策</td> 
      <td>在決策者第一次提交決策時結束階段。 如需詳細資訊，請參閱<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront Proof中設定校訂設定</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隱私權</td> 
      <td>將的評論和決定隱藏給未新增到舞台或帳戶中不是主管或以上人員的人員。 如需詳細資訊，請參閱<a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動化工作流程總覽</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">階段刪除</td> 
      <td>將階段設為必要。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">更多 <img src="assets/more-icon.png"></td> 
      <td>新增檢閱者至舞台或刪除舞台。<p>如果您的每個校樣都傳送給在特定階段的相同人員，您可以在此處指定他們的名稱，這樣您就不必每次建立校樣時都新增他們。 輸入並選取您要新增到階段的使用者名稱，然後在校訂上新增他們的<strong>角色</strong>，以及您想要給使用者的<strong>電子郵件警示</strong>設定。 如需校訂角色的資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">設定預設校訂角色</a>。 如需有關校訂電子郵件警示的資訊，請參閱文章<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">在Workfront Proof中設定電子郵件通知設定</a>中的<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">設定使用者的校訂預設值</a>一節。</p><p>您可以新增任意數量的使用者至階段</p><p>提示：您可以在階段圖表上的階段之間拖放檢閱者名稱。 可用的階段會以藍色反白顯示。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 對要新增至範本的任何其他階段重複此步驟。

   在&#x200B;**工作流程**&#x200B;區段的頂端，您可以看到您正在設定的自動化工作流程圖表。 當您繼續新增階段時，它們會出現在圖表上，其中行顯示它們之間的相依性。 您可以按一下圖表中的某個階段，以檢視該階段的設定。

   如果您不需要檢視圖表，可以按一下&#x200B;**隱藏圖表**。

1. 在&#x200B;**與**&#x200B;共用區段中，如果您想要刪除使用者，請按一下右側的[更多![更多]圖示](assets/more-icon.png)按鈕，然後按一下[移除]。****

## 建立自動化工作流程範本群組 {#create-automated-workflow-template-groups}

作為Workfront管理員，您可以檢視和管理組織帳戶中的所有自動化工作流程範本。 將範本組織到群組中會很有幫助。

若要建立「自動化工作流程」範本群組：

{{step1-to-proofing}}

1. 按一下左側面板中的&#x200B;**工作流程**。
1. 在&#x200B;**工作流程**&#x200B;標籤上，按一下&#x200B;**新增** > **新增範本群組**。
1. 輸入新範本群組的描述性名稱，然後按&#x200B;**Enter**。

您可以拖放方式在群組之間移動範本。

## 管理自動化工作流程範本

{{step1-to-proofing}}

1. 在Workfront Proof的左側面板中，按一下&#x200B;**工作流程**。
1. 在出現的&#x200B;**工作流程**&#x200B;頁面上，執行下列任一項作業：

   * 新增範本
   * 新增範本群組
   * 刪除一或多個範本群組
   * 存取範本的詳細資料
   * 將範本拖曳至其他範本群組
