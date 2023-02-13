---
title: 建立工作項的審批流程
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 您可以建立一個批准流程，用戶可以將該流程附加到工作項目（項目、任務、問題、模板或模板任務）、文檔或校樣。 批准過程確保對象上指定的受分配者在對象在系統中前進之前審閱某些更改。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '2201'
ht-degree: 1%

---

# 建立工作項的審批流程

您可以建立一個批准流程，用戶可以將該流程附加到工作項目（項目、任務、問題、模板或模板任務）、文檔或校樣。 批准過程確保對象上指定的受分配者在對象在系統中前進之前審閱某些更改。

本文介紹如何為工作項（項目、任務、問題、模板或模板任務）建立系統級或組級全局審批流程。

有關與文檔或校樣關聯的批准的資訊，請參閱以下文章：

* [請求文檔批准](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [自動化工作流程概觀](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>使用者也可以為具有「管理」權限的專案、任務、問題、範本或範本任務建立單一用途的核准程式。
>
>本文使用「全域核准程式」一詞，以區別於單一使用的核准程式。 可重複使用全域核准程式。
>
>在組層，全局審批流程僅限於屬於組的工作項目和狀態。
>
>如需單次使用核准程式的相關資訊，請參閱 [核准流程概述](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) 和 [將新審批流程或現有審批流程與工作關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>如果您是Workfront管理員，或您有核准程式的管理存取權，您可以為特定群組建立系統層級核准程式或群組層級核准程式。</p> 
   <p>如果您是群組管理員，您可以為您管理的群組建立群組層級的核准程式。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 為工作項建立系統級或組級全局審批流程

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. （條件性）如果您要建立系統層級的核准程式，請按一下 **程式** > **核准** 中。

   或

   如果您要建立群組層級的核准流程，請按一下 **群組** ![](assets/groups-icon.png)，按一下群組名稱，然後按一下 **核准**.

1. 按一下 **專案核准**, **任務批准**，或 **核准** 頁簽，具體取決於您要建立的審批流程類型。

1. 按一下 **新批准流程**.
1. 在顯示的方塊中指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">核准流程名稱</td> 
      <td>為審批流程鍵入描述性名稱。 將核准程式套用至物件時，使用者會看到此名稱，如 <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">將新審批流程或現有審批流程與工作關聯</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>鍵入審批流程的說明。 這會顯示在 <b>核准</b> 區段 <b>設定</b> 區域。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">活動</td> 
      <td> <p>如果您希望其他使用者能夠將核准程式附加至其建立的專案、工作和問題，請保留此選項為啟用。 </p> <p>預設會啟用此選項。</p> <p> 如果您的組織不再需要使用核准程式，但您想要保留其使用的相關歷史資訊，將核准程式標示為非作用中即可使用。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">此核准流程能由以下人員使用 </td> 
      <td> <p>如果希望審批流程僅適用於特定組的項目、任務、問題和模板，請開始鍵入組的名稱，然後在出現時選擇該名稱：</p> 
       <ul> 
       <li>如果您是系統管理員或您擁有審批流程的管理訪問權限，則在鍵入組名稱時，可以在系統中看到任何組。 <b>所有群組</b> 預設為選取。 </li> 
       <li>如果您是組管理員，無管理權限訪問批准流程，則可以在鍵入其名稱時將批准流程分配給您管理的任何組。 此 <b>所有群組</b> 選項無法使用。</li> 
       </ul> 
       <p>此選項不適用於單次使用的核准程式。</p> 
       <p><b>警告</b>:當您對組特定審批流程進行更改時，已與工作項目關聯的現有審批流程可能會更改。 如需這些變更的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">組和審批流程更改如何影響分配的審批流程</a>.</p> 
       <p>如需從群組頁面列出及管理群組核准程式的相關資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">組級審批流程</a>. </p> 
       <p>有關對批准流程的管理訪問的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 使用下列選項，設定核准程式的路徑。

   路徑是您指定核准程式中需要執行的動作。 您可以在路徑中建立階段，以指出誰需要進行核准工作，以及依序進行。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">開始核准流程 - 當狀態設定為</p> </td> 
      <td> <p>選擇將觸發工作項目審批流程的狀態。 當某人將工作項更新為此狀態時，其批准過程將開始。 </p> <p>無法為多個批准流程路徑選擇相同的狀態。</p> <p>可用的狀態是根據在選項下選取的項目而定 <b>此核准可供</b> （見上表）:</p> 
       <ul> 
       <li> 若 <b>所有群組</b> 已選取，則僅系統範圍的狀態可用
       <li> <p>如果選取了特定群組，則只有該群組可用的狀態可供使用</p> </li> 
       </ul> <p>有關批准流程如何處理狀態的資訊，請參閱 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">審批流程如何依賴狀態</a> 在文章中 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">核准流程概述</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">階段名稱</td> 
      <td>（選用）輸入描述路徑第一階段的名稱。 如果未指定階段名稱，則預設名稱為 <b>第1階段</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">核准者</td> 
      <td> <p>開始鍵入要指定為此階段的批准者的用戶、團隊或作業角色的名稱，然後在名稱出現在下拉清單中時按一下該名稱。 只能添加活動用戶， <span>工作角色</span>和團隊。 </p>

   <p><b>筆尖</b>:</p>

   <p>將使用者新增為核准者時，請注意頭像、使用者的主要角色或其電子郵件地址，以區分名稱相同的使用者。 用戶必須至少與一個作業角色關聯，才能在添加時查看該角色。</p>

   <p><b>附註</b>:

   將使用者、團隊或角色新增為核准者時，不會自動將權限授予與該核准相關聯的物件。 觸發核准步驟時，使用者會收到物件的權限。 否則，必須先與對象共用，才能做出批准決策。 </p> <p>您也可以指定個人的角色，將個人指定為核准者。 例如，您可以將項目責任人、項目發起人、Portfolio責任人、項目負責人或經理指派為審批人。 開始鍵入時，這些選項會自動顯示。</p>

   <p><b>重要</b>:  
       <ul> 
       <li> <p>當您為項目發起人分配了批准，並且沒有人被指定為項目的發起人時，批准將重新分配給項目責任人。 如果未指定任何人為專案的擁有者，則會將核准指派給Workfront管理員。 </p> </li> 
      </ul> 
       <ul> 
       <li> <p>當您將核准指派給角色，且 <b>不需要核准者加入專案團隊（用於包含角色的核准程式）</b> 已禁用，但項目團隊中沒有與批准時的角色匹配的角色，則會將批准重新分配給項目所有者。 如需核准設定的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局批准設定</a>.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>當您為項目所有者分配了批准，並且沒有人被指定為項目的所有者時，該批准將重新分配給主Workfront管理員，如「設定」區域的「客戶資訊」部分所示。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">配置系統的基本資訊</a>.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>您可以重複此過程，將多個批准者添加到舞台。 單個階段可以包括用戶、團隊和作業角色的組合，作為批准者。 可添加到階段的批准者數量沒有限制。</p> <p><b>重要</b>:  <p>當您將作業角色分配為批准者時，與該作業角色關聯的所有用戶（也位於項目組中）都可以對批准做出決策。 </p> <p>當您將團隊指派為核准者時，該團隊中的任何使用者都可以對核准做出決策。 </p> <p>如需專案團隊的詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">專案團隊概觀</a>. 有關批准工作的詳細資訊，請參閱 <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">核准工作 </a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">僅需要一個決策</td> 
      <td> <p>（僅當將多個批准者添加到此階段時才顯示）如果此階段中的任何一個批准者可以批准或拒絕工作項目，則選擇此選項。 此操作允許工作項離開舞台。 </p> <p>如果未選擇此選項，則所有已標識的批准者必須在物料離開階段之前（按任意順序）批准或拒絕階段。 如果任何一個批准者拒絕該階段，則進程會中斷並重新開始，以便進行所需的更改。 然後批准者可以再次批准或拒絕該階段。</p> <p>將團隊指定為批准者時，團隊的任何成員都可以授予或拒絕階段。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">新增階段</p> </td> 
      <td>（選用）使用上述三列中說明的選項，將另一個階段新增至路徑。 您可以視需要將多個階段新增至路徑。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">選擇拒絕批准時會發生什麼</p> </td> 
      <td> <p>如果路徑的任何階段拒絕工作項，請選擇要執行的操作：</p> 
       <ul> 
       <li><b>建立問題</b>:（僅適用於項目和任務審批流程）在運行審批流程的項目或任務中建立問題。 任務上的預設分配資源或項目所有者被分配給問題。 依預設，所建立問題的名稱為 <b>已拒絕批准(&lt;project or="" task="" name=""&gt;)</b>. 這是在任務或項目下輸入的拒絕問題，具體取決於發生拒絕的審批流程。</li> 
       <li> <p><b>將狀態設定為</b>:選擇以下選項之一：</p> 
       <ul> 
       <li><b>上一狀態</b>:被拒絕的項目、任務或問題在激活審批流程的狀態之前回復為狀態。</li> 
       <li><p><b>清單中的任何其他狀態</b>:被拒絕的對象將移至您選擇的狀態，如「暫掛」。 您可以選擇您新增至Workfront系統的其中一種預設狀態或自訂狀態。</p>
       <p>如果您選擇與審批流程關聯的狀態作為拒絕狀態，則被拒絕的對象將移動到選定狀態，並且它將標籤為「待批准」。</p> 
       <p> 例如，如果為拒絕狀態選擇「暫掛」，並且「暫掛」狀態與審批流程關聯，則被拒絕的對象將處於「暫掛 — 待審批」狀態，需要審批。</p>

   </tr> 
    </tbody> 
   </table>

1. （選用）按一下 **新增路徑** 若要新增其他路徑至核准程式，請參考上一步驟中的選項清單。

   新路徑必須與另一個狀態相關聯。 更新項目以顯示此狀態時，路徑就會觸發。 同一狀態不能有兩個路徑。

1. 按一下&#x200B;**儲存**。
1. 現在已建立核准程式，請繼續下列任一步驟：

   * 將核准流程與整個系統中的特定項目、任務或問題相關聯，如 [將新審批流程或現有審批流程與工作關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * 在Workfront以外，通知使用者核准程式可供他們建立其專案、工作或問題的關聯，如 [將新審批流程或現有審批流程與工作關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * 建立在拒絕此審批流程且項目處於另一個狀態時觸發的另一個審批流程。 這可讓您將核准程式連結在一起。

如需編輯核准程式的相關資訊，請參閱 [編輯核准程式](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

## 將審批流程與工作項目關聯

如果要為工作項目（項目、任務或發放）建立審批流程，請先建立審批流程，然後建立工作項目，然後您和用戶可以將審批流程與工作項目關聯。

有關將審批流程與工作項目關聯的說明，請參閱 [將新審批流程或現有審批流程與工作關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>任何擁有專案、任務或問題管理權限的Workfront使用者都可以建立單一使用的核准程式，以便僅用於建立專案、任務或問題的物件。 如需詳細資訊，請參閱 [將新審批流程或現有審批流程與工作關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## 使用戶能夠修改單個工作項的全局批准流程

依預設，擁有專案、工作和問題管理權限的使用者，可以對其建立單一使用的核准程式。 如需將單一使用的核准程式新增至專案、工作和問題的相關資訊，請參閱區段 [將一次性審批流程與項目、任務、問題、模板或模板任務關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) 在文章中 [將新審批流程或現有審批流程與工作關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

用戶還可以更改與工作項關聯的全局批准進程的設定。 這些更改只影響與系統級審批流程關聯的項目、任務或問題。 如需詳細資訊，請參閱 [修改全局批准流程以用於特定對象](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process) 在文章中 [將新審批流程或現有審批流程與工作關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md))。
