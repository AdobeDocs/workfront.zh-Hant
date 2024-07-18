---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: 物件許可權共用概觀
description: 您可以共用或移除您所建立之物件或與您共用之物件的許可權。
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 1%

---

# 物件許可權共用概觀

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
與系統中的某人共用物件時，您可以授予收件者下列任何許可權：檢視、貢獻和管理。

您不必是Adobe Workfront管理員，即可共用您有權存取之物件的許可權，但您對物件的許可權可在Workfront管理員設定的存取層級內運作。

您可以共用或移除您所建立之物件或與您共用之物件的許可權。 當您不是物件的建立者時，除了物件的「共用」許可權之外，您還必須對要在存取層級中共用的物件擁有「共用」存取許可權。 如需存取層級的資訊，請參閱[新的存取層級總覽](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)或[存取層級總覽](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)。

>[!NOTE]
>
>Workfront管理員可以新增或移除系統中所有使用者的任何專案許可權，而無需擁有這些專案。

## 可在Workfront中共用的物件

您可以在Workfront中與其他使用者共用下列物件：

* **專案**：如需詳細資訊，請參閱[在Adobe Workfront中共用專案](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。

* **範本**：如需詳細資訊，請參閱[共用專案範本](../../manage-work/projects/create-and-manage-templates/share-project-template.md)。

* **Portfolio**：如需詳細資訊，請參閱[共用投資組合](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md)。

* **程式**：如需詳細資訊，請參閱[共用程式](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md)。

* **工作**：如需詳細資訊，請參閱[共用工作](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)。

* **問題**：如需詳細資訊，請參閱[共用問題](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)。

* **檔案**：如需詳細資訊，請參閱[共用檔案](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md)。

* **檔案資料夾**：如需詳細資訊，請參閱[共用檔案資料夾](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)。

* **校訂**：如需詳細資訊，請參閱[在Workfront中共用校訂](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)。

* **報告、儀表板和行事曆**：如需詳細資訊，請參閱[共用報告、儀表板和行事曆](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)。 此外，請參閱下列文章：

   * [在Adobe Workfront中共用報表](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [共用儀表板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [共用行事曆報告](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **篩選器、檢視和群組**：如需詳細資訊，請參閱[共用篩選器、檢視或群組](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)。

* **計畫**：如需詳細資訊，請參閱[在Scenario Planner中共用計畫](../../scenario-planner/share-a-plan.md)。

  這需要額外的授權。

* **目標**：如需詳細資訊，請參閱[在Workfront目標中共用目標](../../workfront-goals/workfront-goals-settings/share-a-goal.md)。

  這需要額外的授權。

## 關於共用物件的考量事項

* 您只能共用您對物件的相同層級或更低層級的許可權。

  例如，如果您擁有物件的Contribute許可權，則無法授予其他使用者該物件的「管理」許可權。

* 您無法共用許可權層級高於使用者存取層級的物件。

  例如，如果使用者擁有其存取層級中專案的檢視存取權，您無法將專案的管理許可權授予他們。
* 至少擁有檢視物件許可權的使用者可以與其他人共用該物件。
* 您可以與作用中使用者、工作角色、團隊、群組或公司共用物件。

  >[!NOTE]
  >
  >您只能與其他使用中的使用者共用計畫或目標。 這需要額外的授權。
  >
  >
  >如需詳細資訊，請參閱：
  >
  >* [在情境規劃工具中共用計畫](../../scenario-planner/share-a-plan.md)
  >* [在Workfront目標中共用目標](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

## 共用限制

您最多可以與100個實體（使用者、團隊、群組、工作角色、公司）共用物件。 建議您與群組、團隊或公司共用物件，而非與個別使用者共用，以避免此限制。

## 共用物件的許可權

下表說明您可在共用物件時選取的許可權等級。 並非所有物件都有這些設定可供使用。 您可以將其他實體許可權授予「檢視」或「管理物件」。 如果您要共用專案、任務或問題，也可以授與Contribute的許可權給它。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>檢視</strong></td> 
   <td> <p>您可以對物件執行下列動作：</p> 
    <ul> 
     <li><p>檢視物件</p></li> 
     <li><p>將檔案新增至物件</p></li> 
     <li><p>檢視物件的財務資訊</p></li> 
     <li> <p>共用物件<br></p> <p>當您共用物件時，您可以授予其他使用者與您僅擁有物件之許可權層級的相同許可權，而不是更高的層級。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>參與</strong></td> 
   <td> <p>您可以對物件執行下列動作：</p> 
    <ul> 
     <li>檢視許可權所包含的所有動作。</li> 
     <li>新增費用</li> 
     <li>新增問題（如果它是任務或專案）</li> 
     <li>新增任務（若為專案）</li> 
     <li>編輯其上的自訂Forms</li> 
     <li>在物件上記錄時數</li> 
     <li>在其中進行指派</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>管理</strong></td> 
   <td> <p>您可以對物件執行下列動作：</p> 
    <ul> 
     <li>檢視和Contribute許可權所包含的所有動作</li> 
     <li>刪除它</li> 
     <li>管理其中的財務資訊</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>將此設為對外部使用者公開</strong></td> 
   <td> <p>沒有Workfront帳戶的任何人都可以按一下物件的連結來檢視該物件。 並非所有物件皆可使用此選項。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>設為於系統範圍中可見</strong></td> 
   <td> <p>擁有Workfront帳戶的任何人都可以在搜尋中找到和檢視物件。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 瞭解繼承的許可權和物件的階層

### 從父物件繼承的許可權 {#permissions-inherited-from-parent-objects}

Workfront中的許可權是階層式繼承的。 這表示如果您授予使用者對父物件的許可權，預設情況下，這些使用者會獲得與其相關聯之子物件的相同許可權。

例如，如果您將專案的Contribute許可權授予使用者，則該使用者擁有與該專案相關聯的所有任務和問題（子物件）的Contribute許可權。

繼續上述範例，您無法將許可權限制在子物件。 如果您不希望使用者擁有與專案相關聯之子物件的Contribute許可權，您必須手動從物件中移除繼承許可權，然後調整個別使用者的許可權，包括任何進階設定。 

如需Workfront中物件的階層與相依性的詳細資訊，請參閱[Adobe Workfront物件概觀](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)一文中的[物件相依性和階層](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects)一節。

>[!NOTE]
>
>您的Workfront管理員可以停用存取層級中檔案的繼承許可權。 如需有關停用存取層級中檔案的繼承許可權的詳細資訊，請參閱[建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

### 透過組織成員資格取得的許可權  {#permissions-acquired-through-organizational-memberships}

如果您將「管理」許可權授與物件的使用者群組，並將「檢視」許可權授與相同物件之該群組中的個別使用者，則使用者會透過物件的群組成員資格獲得最高層級的許可權（管理）。 

如果您想要將較低許可權授予已經屬於具有較高許可權層級之組織單位（群組、團隊、工作角色或公司）的使用者，您必須從組織單位中移除許可權，並個別新增具有較低許可權層級的使用者。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;</p> <note type="note">
&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;
</note>
<p>To remove permissions from objects consider the following:&nbsp;</p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:&nbsp;</p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.&nbsp;</li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;</li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;</li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>&nbsp;mark next to <strong>Inherited Permission</strong>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.&nbsp;</li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;</p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.&nbsp;</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## 共用物件

如需如何共用物件的詳細資訊，請參閱[共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

## 移除物件的許可權

如需有關如何從物件移除許可權的資訊，請參閱[從物件移除許可權](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)。

## 要求物件的許可權

當有人將您無權檢視的物件的連結傳送給您時，或當您對物件有較低許可權而您想要請求更高層級的許可權時，您可以請求物件的許可權。 

您可以向擁有物件「共用」許可權的任何人請求物件的存取權。 

如需有關要求物件許可權的詳細資訊，請參閱[要求存取物件](../../workfront-basics/grant-and-request-access-to-objects/request-access.md)。
