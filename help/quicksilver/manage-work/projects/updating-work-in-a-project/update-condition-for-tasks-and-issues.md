---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新任務和問題的條件
description: 任務或問題的條件是在其上放置的標籤，以指示其進行的方式。 這與工作項的狀態不同，該狀態指示了項目開發的當前階段。
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# 更新任務和問題的條件

任務或問題的條件是在其上放置的標籤，以指示其進行的方式。 這與工作項的狀態不同，該狀態指示了項目開發的當前階段。

您可以自動或手動設定任務或問題的條件。

Adobe Workfront管理員可以建立您環境的自訂條件，如 [建立或編輯自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## 存取需求 {#access-requirements}

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   
   For the current licenses:
   <ul><li><p>Standard for tasks</p></li>
   <li><p>Contributor or higher for issues</p></li></ul>


   For legacy licenses:
   <ul><li><p>Work or higher for tasks</p></li>
   <li><p>Request or higher for issues</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to projects</p> <p>Edit access to tasks and issues </p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on tasks and issues to view their Condition</p>
   <p>Manage permissions on tasks and issues to update the Condition</p>
    <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或更高</p>
   <p>請求或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視或更高的專案存取權</p> <p>編輯對任務和問題的存取 </p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看任務和問題的或更高權限以查看其條件</p>
   <p>管理任務和問題的權限以更新條件</p>
    <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 找出工作和問題的條件

條件會顯示為與工作或問題相關聯的標幟。 它們也可以與可顯示在報表中而非標籤的數字相關聯。 有關將條件與數字關聯的詳細資訊，請參閱 [建立或編輯自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

您可以在下列區域找到工作和問題的條件：

* 將您分配給任務或問題時，在更新內的「任務和問題更新」區域。
* 在「檢視」或「分組」中顯示「條件」欄位時，會顯示報表和清單。

>[!NOTE]
>
>當「條件」字詞顯示在「日記帳分錄」報表的「欄位名稱」欄位中時，這表示已更新項目的條件。 在「日記帳分錄」報表中跟蹤「條件」欄位時，「新編號」和「舊編號」值將顯示與條件相關聯的編號，而非其名稱。 如果最初沒有為任務或問題定義條件，而您稍後更新了該條件，則捕獲該更新的日記帳分錄將將「條件」欄位的「舊編號值」顯示為–2,147,483,648。

## 更新狀態以自動更新條件

當您被分配任務或問題時，按一下 **努力** 、「開始任務」或「開始問題」，或更新其狀態，任務或問題的條件將自動更改為與關聯的預設條件 **順利進行**.

如需使用自訂條件作為預設條件的相關資訊，請參閱文章  [將自訂條件設為工作和問題的預設值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) 和 [將自訂條件設為專案的預設值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

有關更改任務狀態的資訊，請參閱 [更新任務狀態](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

有關更改問題狀態的資訊，請參閱 [更新問題狀態](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

有關將Work On It按鈕設定為Start Task或Start Issue按鈕的資訊，請參閱 [將「Work On It（工作完成）」按鈕替換為「Start（開始）」按鈕](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## 手動更新條件

您必須被指派給任務或問題，或擁有任務或問題的「管理」權限，才能設定該任務或問題的「條件」。

更新任務或問題的條件會因您是否被指派給任務或問題而有所不同：

* 您可以在「更新」索引標籤中，或指派給任務或問題清單中更新條件。
* 如果您沒有被指派給任務或問題，但有這些任務或問題的「管理」權限，則只能在任務或問題清單中更新條件。 在這種情況下，無法更新任務或問題的「更新」頁簽中的「條件」。

要手動設定任務或問題的條件，請執行以下操作：

1. 轉到要為其設定條件的任務或問題。

   或

   移至您擁有「管理」權限但未指派給您的任務或問題清單。

1. 更改問題或任務的條件，如下所示：

   * 如果您被指派給任務或問題，並且擁有該任務或問題的「管理」權限，則 **更新** 按一下 **開始新更新**，請選取 **條件** 這最能反映工作的進行方式，請在 **開始新更新** 區域（選用），然後按一下 **更新**.

      ![](assets/change-condition-update-comment-350x141.png)

      >[!NOTE]
      >
      >您可以根據您的環境自訂條件，因此在您的環境中可能會找到三個以上的「條件」選項。 條件的名稱可能與上述名稱不同。 如需在Workfront中自訂條件的相關資訊，請參閱 [建立或編輯自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

      有關更新工作項時可用的其他功能的資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
