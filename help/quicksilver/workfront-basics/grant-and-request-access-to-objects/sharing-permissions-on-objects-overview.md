---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: 對象共用權限概述
description: 您可以共用或移除您所建立物件或已共用給您的物件的權限。
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: 4644edd2aac8c77508e940ec42c597aa702c4df1
workflow-type: tm+mt
source-wordcount: '1156'
ht-degree: 0%

---

# 對象共用權限概述

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->

您不必是Adobe Workfront管理員，就能共用您有權存取之物件的權限，但物件的權限可在Workfront管理員設定的存取層級內運作。

您可以共用或移除您所建立物件或已共用給您的物件的權限。 當您不是對象的建立者時，除了對對象的「共用」權限之外，還必須對要在訪問級別共用的對象具有「共用」訪問權限。 有關訪問級別的資訊，請參見 [新訪問級別概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) 或 [存取層級概觀](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Workfront管理員可以為所有使用者新增或移除系統中任何項目的權限，而不是這些項目的擁有者。

## 可在Workfront中共用的物件

您可以在Workfront中與其他使用者共用下列物件：

* **專案**:如需詳細資訊，請參閱 [在Adobe Workfront中共用專案](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **範本**:如需詳細資訊，請參閱 [共用專案範本](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfolio**:如需詳細資訊，請參閱 [共用產品組合](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

* **方案**:如需詳細資訊，請參閱 [共用方案](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **工作**:如需詳細資訊，請參閱 [共用任務](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **問題**:如需詳細資訊，請參閱 [共用問題](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **檔案**:如需詳細資訊，請參閱 [共用檔案](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **文檔資料夾**:如需詳細資訊，請參閱 [共用文檔資料夾](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **校樣**:如需詳細資訊，請參閱 [在Workfront校樣中共用校樣](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

* **報表、控制面板和日曆**:如需詳細資訊，請參閱 [共用報表、控制面板和日曆](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md). 此外，請參閱下列文章：

   * [在Adobe Workfront中共用報表](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [共用控制面板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [共用日曆報表](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **篩選器、檢視和群組**:如需詳細資訊，請參閱 [共用篩選、檢視或分組](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **計畫**:如需詳細資訊，請參閱 [在方案計畫器中共用計畫](../../scenario-planner/share-a-plan.md).

   這需要額外的授權。

* **目標**:如需詳細資訊，請參閱 [在Workfront目標中共用目標](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

   這需要額外的授權。

## 共用物件的考量事項

* 您只能共用您對物件擁有的相同層級或較低層級權限。

   例如，如果您對物件擁有Contribute權限，則無法授予其他使用者對該物件的「管理」權限。

* 不能共用權限級別高於用戶訪問級別的對象。 例如，如果使用者在其存取層級有「檢視」專案的存取權，則您無法授予他們專案的「管理」權限。
* 具有至少「檢視」物件權限的使用者可與其他人共用該物件。
* 您可以與作用中使用者、工作角色、團隊、群組或公司共用物件。

   >[!NOTE]
   >
   >您只能與其他作用中使用者共用計畫或目標。 這需要額外的授權。
   >
   >
   >如需詳細資訊，請參閱：
   >
   >* [在方案計畫器中共用計畫](../../scenario-planner/share-a-plan.md)
   >* [在Workfront目標中共用目標](../../workfront-goals/workfront-goals-settings/share-a-goal.md)


## 共用限制

您最多可以與100個實體（使用者、團隊、群組、工作角色、公司）共用物件。 建議您將物件共用給群組、團隊或公司（而非個別使用者），以避免此限制。

## 共用對象的權限

下表說明了共用對象時可以選擇的權限級別。 並非所有對象都有這些設定可用。 您可以授予其他實體權限來檢視或管理物件。 如果您共用專案、任務或問題，您也可以授予Contribute的權限。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">檢視</td> 
   <td> <p>您可以對物件執行下列動作：</p> 
    <ul> 
     <li>檢視物件</li> 
     <li>向對象添加文檔</li> 
     <li>查看有關對象的財務資訊</li> 
     <li> <p>共用物件<br></p> <p>當您共用對象時，您可以授予其他用戶您在對象上僅擁有的相同權限級別，而不是更高級別的權限。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">參與</td> 
   <td> <p>您可以對物件執行下列動作：</p> 
    <ul> 
     <li>檢視它</li> 
     <li>包含在「查看」權限中的所有操作。</li> 
     <li>添加費用</li> 
     <li>新增問題（如果是任務或專案）</li> 
     <li>新增任務（如果是專案）</li> 
     <li>編輯上的自訂Forms</li> 
     <li>登錄對象的時數</li> 
     <li>在其中進行分配</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">管理</td> 
   <td> <p>您可以對物件執行下列動作：</p> 
    <ul> 
     <li>檢視它</li> 
     <li>檢視和Contribute權限中包含的所有動作</li> 
     <li>刪除它</li> 
     <li>管理其中的財務資訊</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">將此項目公開給外部使用者</td> 
   <td> <p>沒有Workfront帳戶的任何人都可以按一下物件的連結來檢視該物件。 並非所有對象都可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">設為於系統範圍中可見</td> 
   <td> <p>在搜尋中可找到物件，且擁有Workfront帳戶的任何人都能檢視該物件。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 了解繼承的權限和對象的層次結構

* [從父對象繼承的權限](#permissions-inherited-from-parent-objects)
* [通過組織成員獲得的權限](#permissions-acquired-through-organizational-memberships) 

### 從父對象繼承的權限 {#permissions-inherited-from-parent-objects}

Workfront的權限是依階層繼承。 這表示，如果您授予某個用戶對父對象的權限，預設情況下，這些用戶對與其關聯的子對象獲得相同的權限。

例如，如果您為使用者授予專案的Contribute權限，則使用者擁有與該專案相關聯之所有工作和問題（子物件）的Contribute權限。

繼續上述範例，您無法限制子物件的權限。 如果您不希望用戶具有與項目關聯的子對象的Contribute權限，則必須手動從對象中刪除「繼承的權限」，然後調整單個用戶的權限，包括任何「高級設定」。 

如需Workfront中物件的階層和相依性的詳細資訊，請參閱區段 [對象的相互依存和層次](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [了解Adobe Workfront中的物件](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>您的Workfront管理員可以停用您存取層級中檔案的繼承權限。 有關禁用訪問級別中文檔的繼承權限的詳細資訊，請參見 [建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### 通過組織成員獲得的權限  {#permissions-acquired-through-organizational-memberships}

如果您授予某個對象的一組用戶「管理」權限，並且授予該組中的單個用戶對同一對象的「查看」權限，則該用戶具有通過該對象的組成員資格授予的最高級別權限（「管理」）。 

如果您想要將較低權限授予已屬於某個組織單位（群組、團隊、工作角色或公司）且具有較高權限級別的使用者，則必須從組織單位移除權限，並以較低權限級別個別新增使用者。

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

如需如何共用物件的相關資訊，請參閱 [共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## 從對象中刪除權限

有關如何從對象中刪除權限的資訊，請參見 [從對象中刪除權限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## 請求對象權限

當某人向您發送一個指向您沒有查看權限的對象的連結，或者您對某個對象具有較低權限，並且您想要請求更高級別的權限時，您可以請求該對象的權限。 

您可以向對對象具有「共用」權限的任何人請求對對象的訪問權限。 

如需向物件要求權限的詳細資訊，請參閱 [請求對對象的訪問](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
