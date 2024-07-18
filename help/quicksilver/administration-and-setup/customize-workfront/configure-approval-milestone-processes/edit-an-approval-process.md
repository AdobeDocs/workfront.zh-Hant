---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: 編輯核准流程
description: 如果您是Adobe Workfront管理員，或擁有核准流程的管理存取權，則可檢視及編輯系統中的所有核准流程。
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1954'
ht-degree: 1%

---

# 編輯核准流程

如果您是Adobe Workfront管理員，或擁有核准流程的管理存取權，則可檢視及編輯系統中的所有核准流程。

如果您是群組管理員，則可檢視及編輯與您管理的一或多個群組相關聯的核准流程。

如需有關建立核准流程的資訊，請參閱[建立工作專案的核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

>[!NOTE]
>
>* 當您編輯已使用的全域核准流程時，您的變更會影響整個系統中已與其相關聯的所有物件。
>* 如果您將新核准者新增至物件上已啟動的核准程式上的目前階段，則該物件的程式會重設，且核准者必須重新開始。
>
>  不過，如果您在物件上已啟動的核准程式中執行下列變更，該程式會繼續執行，而不會中斷：
>
>* 新增目前階段以外的階段
>* 在目前階段之前新增其他核准者

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>如果您不是系統管理員，可以管理核准程式的存取權</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 編輯現有的核准流程

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。
1. （視條件而定）如果您正在編輯系統層級的核准程式，請按一下左側面板中的&#x200B;**程式** > **核准**。

   或

   如果您正在編輯群組層級的核准流程，請執行下列動作：

   1. 在左側面板中，按一下&#x200B;**群組** ![](assets/groups-icon.png)。
   1. 按一下您要列出或管理群組核准流程的群組名稱。
   1. 在左側面板中，按一下&#x200B;**核准**。 您可能需要先按一下&#x200B;**顯示更多**。

1. 根據您要編輯的核准程式型別，按一下&#x200B;**專案核准**、**任務核准**&#x200B;或&#x200B;**問題核准**&#x200B;標籤。

1. 選取您要編輯的核准程式，然後按一下清單頂端的&#x200B;**編輯**。 編輯核准流程方塊隨即顯示。

   ![](assets/edit-approval-process-global-area-new.png)

1. 在顯示的方塊中指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">核准流程名稱</td> 
      <td>輸入核准流程的描述性名稱。 將核准程式套用至物件時，使用者可以看到此名稱，如<a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">將新的或現有的核准程式與工作建立關聯</a>中所述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>輸入核准流程的說明。 這會顯示在核准程式名稱旁的<b>設定</b>區域中的<b>核准</b>區段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">為作用中</td> 
      <td> <p>如果您希望其他使用者能夠將核准流程附加到他們建立的專案、任務和問題，請將此選項保持啟用。 </p> <p>此選項預設為啟用。</p> <p>提示：當您的組織不再需要使用核准流程，但您想要保留其使用的相關歷史資訊時，將核准流程標籤為非使用中會很有用。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">此核准流程能由以下人員使用 </td> 
      <td> <p>如果您希望專案、任務、問題和範本的核准流程只屬於特定群組，請開始輸入群組的名稱，然後在其出現時選取名稱：</p> 
       <ul> 
        <li>如果您是系統管理員或您擁有核准流程的管理存取權，則當您鍵入群組名稱時，可以在系統中看到任何群組。 <b>預設會選取所有群組</b>。 </li> 
        <li>如果您是群組管理員，沒有核准程式的管理許可權，則可以在輸入核准程式名稱時，將核准程式指定給您管理的任何群組。 <b>所有群組</b>選項無法使用。</li> 
       </ul> <p>此選項不適用於單次使用的核准流程。</p> <p><b>警告</b>：當您變更群組特定核准程式時，已經與工作專案關聯的現有核准程式可能會變更。 如需這些變更的相關資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">群組和核准流程變更如何影響指派的核准流程</a>。</p> <p>如需從群組頁面列出和管理群組核准流程的資訊，請參閱<a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">群組層級核准流程</a>。 </p> <p>如需有關核准程式之管理存取許可權的資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者對特定區域的管理存取許可權</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 使用下列選項設定核准流程的路徑。

   您可在路徑中指定核准流程中需要執行的動作。 您可在路徑中建立階段，以指出誰需要執行核准工作以及依何種順序。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">開始核准流程 - 當狀態設定為</p> </td> 
      <td> <p>選取將觸發工作專案核准流程的狀態。 當有人將工作專案更新為此狀態時，其核准流程就會開始。 </p> <p>無法為多個核准流程路徑選擇相同狀態。</p> <p>可用的狀態是根據選項<b>下選取的內容而定。此核准可由</b>使用（上表說明）：</p> 
      <ul> 
      <li> 如果選取<b>所有群組</b>，則只有全系統鎖定狀態可用。<!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>如果選取了特定群組，則只能使用該群組的可用狀態</p> </li> 
      </ul> <p>如需有關核准程式如何使用狀態的資訊，請參閱文章<a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">核准程式概觀</a>中的<a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">核准程式如何依賴狀態</a>一節。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">階段名稱</td> 
      <td>（選擇性）輸入描述路徑第一階段的名稱。 如果您未指定階段名稱，預設名稱為<b>階段1</b>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">核准者</td> 
      <td> <p>開始輸入您想要指定為此階段核准者的使用者、專案團隊或工作角色名稱，然後按一下該名稱出現在下拉式清單中。 您只能新增作用中使用者、工作角色和團隊。 </p>

   <p><b>提示</b>：</p>

   <p>將使用者新增為核准者時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。 使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。</p>
      <p>您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱<a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">授予使用者存取權</a></p>。

   <p><b>附註</b>：

   將使用者、團隊或角色新增為核准者，並不會自動授予他們與該核准相關聯的物件許可權。 他們會在觸發核准步驟時獲得物件的許可權。 否則，物件必須先與他們共用，他們才能做出核准決定。 </p>
   <p>您也可以指定個人的角色，將個人指定為核准者。 例如，您可以將專案所有者、專案贊助者、Portfolio所有者、方案所有者或經理指派為核准者。 當您開始輸入時，這些選項會自動顯示。</p> 
      <p><b>重要</b>：  
      <ul> 
      <li> 當您將核准指派給「專案贊助者」，且沒有指定任何人員作為專案的贊助者時，核准將重新指派給「專案所有者」。 如果未指定任何人為專案的所有者，則會將核准指派給Workfront管理員。 </li> 
      <li> 當您將核准指派給角色且選項<b>核准者不需要位於專案團隊</b>中時已停用，但專案團隊中沒有符合核准角色的角色，核准將重新指派給專案所有者。 如需核准設定的相關資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">設定全域核准設定</a>。
      </li> 
      <li>當您將核准指派給專案所有者，且沒有人被指定為專案的所有者時，核准將重新指派給主要Workfront管理員，如設定區域的客戶資訊區段中所述。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">設定您系統的基本資訊</a>。</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>當您指派工作角色作為核准者時，與該工作角色相關聯且同樣位於專案團隊中的所有使用者都可以對核准做出決定。 </p> 
      <p>當您將團隊指派為核准者時，該團隊中的任何使用者都可以對核准做出決定。 </p> 
      <p>如需有關專案團隊的詳細資訊，請參閱<a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">專案團隊概述</a>。 如需核准工作的詳細資訊，請參閱<a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">核准工作</a>。</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">僅需要一個決策</td> 
      <td>（只有在您將多個核准者新增至階段時才會顯示）如果階段上的任何核准者可以在此階段核准或拒絕工作專案，請選取此選項。 此動作允許工作專案離開階段。  
      <p>如果未選取此選項，則所有已識別的核准者必須在專案離開階段之前，以任何順序核准或拒絕階段。 如果任一核准者拒絕該階段，則程式會中斷並重新開始，以便進行所需的變更。 然後核准者可以再次核准或拒絕階段。</p> 
      <p>當團隊被指定為核准者時，團隊的任何成員都可以授予或拒絕階段。</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">新增階段</p> </td> 
      <td>（可選）使用以上三列所述的選項，將另一個階段新增至路徑。 您可以視需要為路徑新增多個階段。</td> 
     </tr>
     <tr> 
      <td role="rowheader"> 選擇核准被拒絕時會發生的情況</td> 
      <td> <p>選取工作專案在路徑的任何階段遭到拒絕時要採取的動作：</p> 
      <ul> <li><strong>建立問題</strong>： （僅適用於專案與任務核准程式）在執行核准程式的專案或任務中建立問題。 任務的預設已指派資源，或專案的所有者已指派給問題。 依預設，建立的問題名稱為<strong>已拒絕核准（專案或任務名稱）</strong>。 這是「拒絕問題」，根據發生拒絕的核准程式，在任務或專案下輸入。</li> 
      <li> <p><strong>將狀態設定為</strong>：選擇下列其中一項：</p> 
      <ul> <li><strong>先前的狀態</strong>：拒絕的專案、任務或問題回覆成啟動核准程式之前的狀態。</li> 
      <li> <p><strong>清單中的任何其他狀態</strong>：拒絕的物件會移至您選擇的狀態，例如「保留」。 您可以選擇其中一個預設狀態，或新增至Workfront系統的自訂狀態。</p> <p>如果您選擇與核准流程關聯的狀態作為核准路徑的拒絕狀態，則被拒絕的物件將移動到所選狀態，並將標籤為「待核准」。</p>
      <p>例如，如果您選擇等候接聽對於拒絕狀態和等候接聽status與核准流程相關聯，被拒絕的物件置於「狀態」暫停 — 待核准」，需要核准。</p>    <p>對於系統範圍的核准流程，僅可使用系統範圍的狀態。</p> <p>針對群組特定的核准程式，所有群組狀態皆可使用。 這包括群組管理員專門為群組建立的任何自訂狀態，以及任何系統範圍的狀態。 </p> <p>如需有關核准程式如何使用狀態的資訊，請參閱文章<a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">核准程式概觀</a>中的<a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">核准程式如何依賴狀態</a>一節。</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）按一下&#x200B;**新增路徑**，參照上一步驟中的選項清單，將另一個路徑新增至核准程式。

   新路徑必須與另一個狀態相關聯。 專案更新以顯示此狀態時會觸發路徑。 相同狀態不能有兩個路徑。

1. 按一下「**儲存**」。
1. （可選）執行下列任一項作業：

   * 將核准程式與整個系統中的特定專案、任務或問題建立關聯，如[將新的或現有的核准程式與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)中所述。
   * 在Workfront外部，通知使用者核准流程可供他們與他們的專案、任務或問題建立關聯，如[將新的或現有的核准流程與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)中所述。
   * 建立另一個核准流程，如果此核准流程遭拒絕，而專案處於另一個狀態，則會觸發此流程。 這可讓您將核准流程連結在一起。
