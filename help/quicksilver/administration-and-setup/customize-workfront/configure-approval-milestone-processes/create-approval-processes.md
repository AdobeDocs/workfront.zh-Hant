---
title: 建立工作專案的核准流程
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 您可以建立使用者可附加至工作專案（專案、任務、問題、範本或範本任務）、檔案或校訂的核准流程。 核准程式可確保物件上的指定受指派人在物件在系統中進行之前稽核某些變更。
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '2193'
ht-degree: 1%

---

# 為工作項目建立核准流程

<!-- Audited: 12/2023 -->

<!--see below the "hidden" content for the redesigned tabs - August 2023-->

您可以建立使用者可附加至工作專案（專案、任務、問題、範本或範本任務）、檔案或校訂的核准流程。 核准程式可確保物件上的指定受指派人在物件在系統中進行之前稽核某些變更。

本文說明如何建立工作專案（專案、任務、問題、範本或範本任務）的系統層級或群組層級全域核准流程。

如需與檔案或校樣相關之核准的資訊，請參閱下列文章：

* [要求檔案核准](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [自動化工作流程總覽](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>使用者也可對其擁有管理許可權的專案、任務、問題、範本或範本任務建立單次使用核准流程。
>
>本文使用「全域核准流程」一詞來區分單次使用核准流程。 全域核准流程可重複使用。
>
>在群組層級，全域核准程式僅限於屬於群組的工作專案與狀態。
>
>如需單一使用核准程式的資訊，請參閱[核准程式概述](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md)和[將新的或現有的核准程式與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td><p>系統層級或單一使用核准程式：任何</p>
   <p>群組層級核准流程： Prime或Ultimate</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準 </p>
 <p>或</p> 
<p>目前：計畫 </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>如果您是系統管理員或您擁有核准流程的管理存取權，則可以為特定群組建立系統層級核准流程，或群組層級核准流程。</p> 
   <p>如果您是群組管理員，您可以為您管理的群組建立群組層級核准流程。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立工作專案的系統層次或群組層次全域核准程式

{{step-1-to-setup}}

1. （視條件而定）如果您正在建立系統層級的核准程式，請按一下左側面板中的&#x200B;**程式** > **核准**。

   或

   如果您正在建立群組層級的核准程式，請按一下&#x200B;**群組** ![群組圖示](assets/groups-icon.png)，按一下群組名稱，然後按一下&#x200B;**核准**。

   <!--hidden for the new tab redesign - August 2023: 
   ![Approvals area in setup](assets/approvals-area-in-setup-processes.png)
   -->

1. 選擇&#x200B;**專案核准**、**任務核准**&#x200B;或&#x200B;**問題核准**&#x200B;索引標籤。

1. 按一下&#x200B;**新增核准程式**。
1. 在顯示的方塊中指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">核准流程名稱</td> 
      <td><p>輸入核准流程的描述性名稱。 將核准程式套用至物件時，使用者可以看到此名稱，如<a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">將新的或現有的核准程式與工作建立關聯</a>中所述。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td><p>輸入核准流程的說明。 這會顯示在核准程式名稱旁的<b>設定</b>區域中的<b>核准</b>區段。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">為作用中</td> 
      <td> <p>如果您希望其他使用者能夠將核准流程附加到他們建立的專案、任務和問題，請將此選項保持啟用。 </p> <p>此選項預設為啟用。</p> <p> 提示：當您的組織不再需要使用核准流程，但您想要保留其使用的相關歷史資訊時，將核准流程標籤為非使用中會很有用。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">此核准流程能由以下人員使用 </td> 
      <td> <p>如果您希望專案、任務、問題和範本的核准流程只屬於特定群組，請開始輸入群組的名稱，然後在其出現時選取名稱：</p> 
       <ul> 
       <li>如果您是系統管理員或您擁有核准流程的管理存取權，則當您鍵入群組名稱時，可以在系統中看到任何群組。 <b>預設會選取所有群組</b>。 </li> 
       <li>如果您是群組管理員，沒有核准程式的管理許可權，則可以在輸入核准程式名稱時，將核准程式指定給您管理的任何群組。 <b>所有群組</b>選項無法使用。</li> 
       </ul> 
       <p>此選項不適用於單次使用的核准流程。</p> 
       <p><b>警告</b>：當您變更群組特定核准程式時，已經與工作專案關聯的現有核准程式可能會變更。 如需這些變更的相關資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">群組和核准流程變更如何影響指派的核准流程</a>。</p> 
       <p>如需從群組頁面列出和管理群組核准流程的資訊，請參閱<a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">群組層級核准流程</a>。 </p> 
       <p>如需有關核准程式之管理存取許可權的資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者對特定區域的管理存取許可權</a>。</p> </td> 
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
       <li> 如果選取<b>所有群組</b>，則只能使用系統範圍狀態
       <li> <p>如果選取了特定群組，則只能使用該群組的可用狀態</p> </li> 
       </ul> <p>如需有關核准程式如何使用狀態的資訊，請參閱文章<a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">核准程式概觀</a>中的<a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">核准程式如何依賴狀態</a>一節。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">階段名稱</td> 
      <td>（選擇性）輸入描述路徑第一階段的名稱。 如果您未指定階段名稱，預設名稱為<b>階段1</b>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">核准者</td> 
      <td> <p>開始輸入您想要指定為此階段核准者的使用者、專案團隊或工作角色名稱，然後按一下該名稱出現在下拉式清單中。 您只能新增作用中使用者、<span>工作角色</span>和團隊。 </p>

   <p><b>提示</b>：</p>

   <p>將使用者新增為核准者時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。 使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。</p>
      <p>您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱<a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">授予使用者存取權</a>。 </p>

   <p><b>附註</b>：

   將使用者、團隊或角色新增為核准者，並不會自動授予他們與該核准相關聯的物件許可權。 他們會在觸發核准步驟時獲得物件的許可權。 否則，物件必須先與他們共用，他們才能做出核准決定。 </p> <p>您也可以指定個人的角色，將個人指定為核准者。 例如，您可以將專案所有者、專案贊助者、Portfolio所有者、方案所有者或經理指派為核准者。 當您開始輸入時，這些選項會自動顯示。</p>

   <p><b>重要</b>：  
       <ul> 
       <li> <p>當您將核准指派給「專案贊助者」，且沒有指定任何人員作為專案的贊助者時，核准將重新指派給「專案所有者」。 如果未指定任何人為專案的所有者，則會將核准指派給Workfront管理員。 </p> </li> 
      </ul> 
       <ul> 
       <li> <p>當您將核准指派給角色，且<b>核准者不需要位於專案團隊中（對於包含角色的核准程式）</b>已停用，但專案團隊中沒有符合核準時角色的角色時，核准將重新指派給專案所有者。 如需核准設定的相關資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">設定全域核准設定</a>。</p> </li> 
       </ul> 
       <ul> 
       <li> <p>當您將核准指派給專案所有者，且沒有人被指定為專案的所有者時，核准將重新指派給主要Workfront管理員，如設定區域的客戶資訊區段中所述。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">設定您系統的基本資訊</a>。  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>您可以重複此程式，將多個核准者新增至階段。 單一階段可包含使用者、團隊和職務角色作為核准者的組合。 您可以新增到階段的核准者數量沒有限制。</p> <p><b>重要</b>：  <p>當您指派工作角色作為核准者時，與該工作角色相關聯且同樣位於專案團隊中的所有使用者都可以對核准做出決定。 </p> <p>當您將團隊指派為核准者時，該團隊中的任何使用者都可以對核准做出決定。 </p> <p>如需有關專案團隊的詳細資訊，請參閱<a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">專案團隊概述</a>。 如需核准工作的詳細資訊，請參閱<a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">核准工作</a>。</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">只需要一個決定<br> <br>（只有在您將多個核准者新增到階段時才會顯示） </td> 
      <td> <p>如果階段中的任何一位核准者可以在此階段核准或拒絕工作專案，請選取此選項。 此動作允許工作專案離開階段。 </p> <p>如果未選取此選項，則所有已識別的核准者必須在專案離開階段之前，以任何順序核准或拒絕階段。 如果任一核准者拒絕該階段，則程式會中斷並重新開始，以便進行所需的變更。 然後核准者可以再次核准或拒絕階段。</p> <p>當團隊被指定為核准者時，團隊的任何成員都可以授予或拒絕階段。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">新增階段</p> </td> 
      <td><p>（可選）使用以上三列所述的選項，將另一個階段新增至路徑。 您可以視需要為路徑新增多個階段。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">選擇核准被拒絕時會發生的情況</p> </td> 
      <td> <p>選取工作專案在路徑的任何階段遭到拒絕時要採取的動作：</p> 
       <ul> 
       <li><b>建立問題</b>： （僅適用於專案與任務核准程式）在執行核准程式的專案或任務中建立問題。 任務的預設已指派資源，或專案的所有者已指派給問題。 依預設，建立的問題名稱為<b>已拒絕核准（&lt;專案或任務名稱&gt;）</b>。 這是「拒絕問題」，根據發生拒絕的核准程式，在任務或專案下輸入。</li> 
       <li> <p><b>將狀態設定為</b>：選擇下列其中一項：</p> 
       <ul> 
       <li><b>先前的狀態</b>：拒絕的專案、任務或問題回覆成啟動核准程式之前的狀態。</li> 
       <li><p><b>清單中的任何其他狀態</b>：拒絕的物件會移至您選擇的狀態，例如「保留」。 您可以選擇其中一個預設狀態，或新增至Workfront系統的自訂狀態。</p>
       <p>如果您選擇與核准流程關聯的狀態作為拒絕狀態，則被拒絕的物件將移動到所選狀態，並將標籤為「待核准」。</p> 
       <p> 例如，如果您選擇等候接聽對於拒絕狀態和等候接聽status與核准流程相關聯，被拒絕的物件置於「暫停 — 待核准」狀態，需要核准。</p>

   </tr> 
    </tbody> 
   </table>

1. （選擇性）按一下&#x200B;**新增路徑**，參照上一步驟中的選項清單，將另一個路徑新增至核准程式。

   新路徑必須與另一個狀態相關聯。 專案更新以顯示此狀態時會觸發路徑。 相同狀態不能有兩個路徑。

1. 按一下「**儲存**」。
1. 現在核准流程已建立，請繼續下列任一項作業：

   * 將核准程式與整個系統中的特定專案、任務或問題建立關聯，如[將新的或現有的核准程式與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)中所述。
   * 在Workfront外部，通知使用者核准流程可供他們與他們的專案、任務或問題建立關聯，如[將新的或現有的核准流程與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)中所述。
   * 建立另一個核准流程，如果此核准流程遭拒絕，而專案處於另一個狀態，則會觸發此流程。 這可讓您將核准流程連結在一起。

如需有關編輯核准流程的資訊，請參閱[編輯核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md)。

## 將核准流程與工作專案建立關聯

當您想要建立工作專案（專案、任務或問題）的核准流程時，

1. 先建立核准流程
1. 建立工作專案
1. 將核准流程與工作專案建立關聯

如需將核准程式與工作專案產生關聯的指示，請參閱[將新的或現有的核准程式與工作產生關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。

>[!NOTE]
>
>任何對專案、任務或問題具有管理許可權的Workfront使用者都可以建立一次性使用核准流程，以僅用於建立該流程的物件。 如需詳細資訊，請參閱[將新的或現有的核准程式與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。

## 允許使用者修改單一工作專案的全域核准流程

根據預設，擁有專案、任務和問題管理許可權的使用者可以對其建立單一使用核准流程。 如需新增單一使用核准流程至專案、任務和問題的相關資訊，請參閱[將新的或現有的核准流程與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)一文中的[將單一使用核准流程與專案、任務、問題、範本或範本任務建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process)小節。

使用者也可以變更與工作專案相關聯之全域核准流程的設定。 這些變更只會影響與系統層級核准流程關聯的專案、任務或問題。 如需詳細資訊，請參閱文章[將新的或現有的核准程式與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)中的[修改用於特定物件的全域核准程式](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process)一節。
