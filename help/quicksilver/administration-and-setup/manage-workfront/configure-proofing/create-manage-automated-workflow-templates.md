---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 建立和管理自動化工作流模板
description: 身為Adobe Workfront管理員，如果您組織的內容審核程式經常重複，或內容經常由同一人審核，您可以建立「自動化工作流程」範本，其中包含那些具有您所指定校樣角色和通知設定的審核者。 「自動化工作流」模板可以簡單，只需一兩個審核者，或複雜且具有許多階段和依賴項。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2096'
ht-degree: 0%

---

# 建立和管理自動化工作流模板

身為Adobe Workfront管理員，如果您組織的內容審核程式經常重複，或內容經常由同一人審核，您可以建立「自動化工作流程」範本，其中包含那些具有您所指定校樣角色和通知設定的審核者。 「自動化工作流」模板可以簡單，只需一兩個審核者，或複雜且具有許多階段和依賴項。

自動化工作流程範本可讓您使用自動化工作流程輕鬆建立校樣。 當使用者建立校樣時，只需選擇所需的範本。

您可以隨時輕鬆更改任何「自動化工作流」模板，添加或刪除審核者和階段。 使用模板的校樣建立者可以添加或刪除校樣的審閱者。

使用「自動化工作流程」範本時，請考量下列事項：

1. 「自動化工作流程」範本的設定決定了您可以對「自動化工作流程」執行哪些校樣。 例如，如果在範本中停用了「新增階段」按鈕，當您使用校樣的「自動化工作流程」設定時，該按鈕將不會顯示。
1. 將人員添加到「自動化工作流」模板中的某個頁面，但同時已作為校樣的審閱者出現時，應用模板會將審閱者從舞台中刪除。 如果您未將另一個審核者添加到舞台，則會出現一條消息提示您添加一個審核者。
1. 您修改「自動化工作流程」範本的能力取決於Workfront管理員所設定的範本設定，如中所述。 如果禁用了修改模板的功能，則只有模板的所有者才能修改它。

如需自動化工作流程的相關資訊，請參閱 [自動化工作流程概觀](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Premium或Select</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須在校樣權限設定檔中選取管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">設定使用者的校對存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立自動化工作流模板

1. 在Workfront中，按一下主功能表 ![](assets/main-menu-icon.png)，然後按一下「校對」 ![](assets/proofing-in-main-menu.png) 存取Workfront校樣。
1. 按一下 **工作流程** 中。
1. 在 **工作流程** 按一下 **新增** > **新範本**.

1. 在 **詳細資料** 區段，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">範本名稱</td> 
      <td>（必要）輸入範本的名稱。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">範本擁有者</td> 
      <td>您可以選取要管理範本的Workfront管理員或Workfront校樣管理員。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">範本群組</td> 
      <td> <p> 如果貴組織的「自動化工作流程」組織成群組，您可以選取群組的名稱。 請參閱 <a href="#create-automated-workflow-template-groups" class="MCXref xref">建立自動化工作流模板組</a> 以取得詳細資訊。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">範本時區 </td> 
      <td> <p>範本的預設時區是您正在使用的時區。 如果將使用模板的校樣建立者和審閱者的時區不同，您可以在此處進行更改，以確保在正確的時間為這些用戶設定階段截止時間。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許</td> 
      <td> <p>您可以選取要讓人員使用範本建立校樣的預備活動。</p> <!--
        <p><b>WARNING</b>: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof. <!--
          <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span>
         --></p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **階段** 一節，配置「自動化工作流」模板的每個階段。

   您可以新增多個階段，並在其之間建立。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名稱</td> 
      <td> <p>階段名稱會顯示在「工作流」區段頂端的「自動化工作流」圖表、「證明詳細資訊」頁面，以及傳送給審核者的電子郵件通知中。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">啟動階段</td> 
      <td> <p>指定是否自動激活舞台或手動激活舞台。 對於第一階段，您可以選取 <strong>論校樣建立</strong>, <strong>在特定日期和時間</strong>，或 <strong>手動</strong>.</p> <p>添加第二個階段時，其他選項可用，因為它們要求您選擇父級階段。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">根據</td> 
      <td> <p>指定您要如何計算截止日期：</p> 
       <ul> 
        <li> <p><strong>校樣建立</strong>:在 <strong>截止日期（+工作天）</strong>，選取您要新增至校樣建立日期的工作天數，以自動設定校樣的截止日期。</p> </li> 
        <li><strong>舞台開始時</strong>:在 <strong>截止日期（+工作天）</strong>，選取您要新增至階段啟動日期的工作天數，以自動設定校樣的截止日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">鎖台</td> 
      <td>指定是否允許鎖定舞台以供評論。 選項是手動或自動鎖定階段，無論是在下一個階段開始時，還是在父級階段上做出所有決策時。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">主要決策進行者</td> 
      <td> <p>只有在將審閱者添加到舞台後，可用的決策者才會顯示在清單中。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">只需要一個決定</td> 
      <td>一旦一名決策者提交其決定，就將完成該階段的審查進程。 如需詳細資訊，請參閱 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront校樣中設定校樣設定</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">私人舞台</td> 
      <td>隱藏未新增至階段或非Workfront管理員的人員的意見和決策&lt;!&gt; — 在FLARE中起草：監事及以上

       -->. 如需詳細資訊，請參閱自&lt;a href=&quot;../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md&quot; class=&quot;MCXref xref&quot;>動化工作流程概&lt;/a>觀。&lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader">不允許刪除此階段</td> 
      <td> <p>讓舞台成為必備的。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 如果將使用此範本的校樣一律傳送給舞台上的相同人員，請在此處新增校樣，讓使用者不必在每次建立校樣時都新增校樣。

   選擇每個人的 **角色** 將使用此範本的校樣，以及 **電子郵件警報** 您希望使用此範本的校樣時使用者收到。

   如需校樣的角色相關資訊，請參閱 [配置預設校對角色](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). 如需校樣電子郵件警報的相關資訊，請參閱 [配置用戶的校樣預設值](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) 在文章中  [在Workfront Proof中設定電子郵件通知設定](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   每個使用者只能新增至一個階段。 您可以新增任意數量的使用者至舞台。

   >[!TIP]
   >
   >可以在階段圖的各階段之間拖放審閱者名稱。 可用階段會以藍色強調顯示。

1. 對要添加到模板的任何其他階段重複上述兩個步驟。

   在 **工作流程** 區段中，您會看到您設定的「自動化工作流程」圖表。 在繼續添加階段時，這些階段會出現在圖表上，其中的線條顯示它們之間的依賴關係。 您可以按一下圖表中的舞台，以檢視該舞台的設定。

   如果您不需要查看圖表，可以按一下 **隱藏圖**.

1. 在 **共用範本，與** 區段中，按一下選項（如果範本尚未與整個組織共用）以指定可以使用該選項的人員。

   依預設，新的自動化工作流程範本會與組織中的每個人共用。

1. 按一下 **建立**。

## 修改自動化工作流程範本

身為Workfront校樣管理員，您可以修改「自動化工作流程」範本。 您的變更會在您進行時自動儲存。

1. 在Workfront中，按一下主功能表 ![](assets/main-menu-icon.png)，然後按一下「校對」 ![](assets/proofing-in-main-menu.png) 存取Workfront校樣。
1. 按一下 **工作流程** 中。
1. 在 **工作流程範本** 列出，按一下要修改的範本。
1. 在 **詳細資料** 區段，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">範本名稱</td> 
      <td>（必要）輸入範本的名稱。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">範本擁有者</td> 
      <td>您可以選取要管理範本的Workfront管理員或Workfront校樣管理員。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">範本群組</td> 
      <td> <p> 如果貴組織的「自動化工作流程」組織成群組，您可以選取群組的名稱。 請參閱 <a href="#create-automated-workflow-template-groups" class="MCXref xref">建立自動化工作流模板組</a> 以取得詳細資訊。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">範本時區 </td> 
      <td> <p>範本的預設時區是您正在使用的時區。 如果將使用模板的校樣建立者和審閱者的時區不同，您可以在此處進行更改，以確保在正確的時間為這些用戶設定階段截止時間。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許</td> 
      <td> <p>選取您要供使用範本建立校樣的使用者使用的預備活動。 </p> <p><b>警告</b>:如果您未選擇「添加階段」和「將人員添加到階段」選項，則模板所有者或使用此模板的任何校樣的所有者都無法添加階段或共用校樣。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **工作流程** 部分，更改任何階段的名稱並展開其設定 ![](assets/arrow-button.png) 進行任何需要的更改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">根據</td> 
      <td> <p>指定您要如何計算截止日期：</p> 
       <ul> 
        <li> <p><strong>從校樣建立計算的截止日期</strong>:在 <strong>設定階段截止日期</strong> 下拉式清單中，選取您要新增至校樣建立日期的工作天數，以自動設定校樣的截止日期。</p> </li> 
        <li><strong>從階段激活計算的截止時間</strong>:在 <strong>設定階段截止日期</strong> 下拉式清單中，選取您要新增至階段啟動日期的工作天數，以自動設定校樣的截止日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">啟動階段</td> 
      <td> <p>指定是否自動激活舞台或手動激活舞台。 對於第一階段，您可以選取 <strong>論校樣建立</strong>, <strong>在特定日期和時間</strong>，或 <strong>手動</strong>.</p> <p>添加第二個階段時，其他選項可用，因為它們要求您選擇父級階段。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">鎖台</td> 
      <td>指定是否允許鎖定舞台以供評論。 選項是手動或自動鎖定階段，無論是在下一個階段開始時，還是在父級階段上做出所有決策時。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">決定</td> 
      <td>第一個決策者提交其決定時，就結束了這一階段。 如需詳細資訊，請參閱 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront校樣中設定校樣設定</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隱私權</td> 
      <td>隱藏未新增至舞台或非帳戶中監控人員及以上人員的留言和決策。 如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自動化工作流程概觀</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">階段刪除</td> 
      <td>讓舞台成為必備的。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">更多 <img src="assets/more-icon.png"></td> 
      <td>將審閱者添加到舞台或刪除舞台。<p>如果您的每個校樣在特定階段傳送給相同的人員，您可以在名稱處指定其名稱，這樣就不必在每次建立校樣時都新增這些校樣。 鍵入並選擇要添加到舞台的用戶的名稱，然後添加其名稱 <strong>角色</strong> 證據和 <strong>電子郵件警報</strong> 所需的設定。 有關校對角色的資訊，請參見 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">配置預設校對角色</a>. 如需校樣電子郵件警報的相關資訊，請參閱 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">配置用戶的校樣預設值</a> 在文章中 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">在Workfront Proof中設定電子郵件通知設定</a>.</p><p>您可以新增想要進入階段的使用者數量</p><p>提示：可以在階段圖的各階段之間拖放審閱者名稱。 可用階段會以藍色強調顯示。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 對要添加到模板的任何其他階段重複此步驟。

   在 **工作流程** 區段中，您會看到您設定的「自動化工作流程」圖表。 在繼續添加階段時，這些階段會出現在圖表上，其中的線條顯示它們之間的依賴關係。 您可以按一下圖表中的舞台，以檢視該舞台的設定。

   如果您不需要查看圖表，可以按一下 **隱藏圖**.

1. 在 **共用給** 區段中，如果您想要刪除使用者，請按一下「更多」 ![](assets/more-icon.png) 按鈕，然後按一下 **移除**.

## 建立自動化工作流模板組 {#create-automated-workflow-template-groups}

身為Workfront管理員，您可以在組織的帳戶中檢視及管理所有「自動化工作流程」範本。 將範本組織成群組會很實用。

要建立「自動化工作流」模板組，請執行以下操作：

1. 在Workfront中，按一下主功能表 ![](assets/main-menu-icon.png)，然後按一下「校對」 ![](assets/proofing-in-main-menu.png) 存取Workfront校樣。
1. 按一下 **工作流程** 中。
1. 在 **工作流程** 按一下 **新增** > **新範本群組**.
1. 為新範本群組輸入描述性名稱，然後按 **輸入**.

您可以拖放，在群組之間移動範本。

## 管理自動化工作流模板

1. 在Workfront中，按一下主功能表 ![](assets/main-menu-icon.png)，然後按一下「校對」 ![](assets/proofing-in-main-menu.png) 存取Workfront校樣。

1. 在Workfront Proof的左側面板中，按一下 **工作流程**.
1. 在 **工作流程** 頁面，執行下列任一操作：

   * 新增範本
   * 新增範本群組
   * 刪除一個或多個模板組
   * 存取範本的詳細資訊
   * 將範本拖曳至不同的範本群組
