---
product-area: projects
navigation-topic: update-work-in-a-project
title: 檢視並更新任務的完成百分比
description: 您可以更新任務的完成百分比，以指出完成任務的進度。
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# 檢視並更新任務的完成百分比

您可以更新任務的完成百分比，以指出完成任務的進度。

## 存取需求

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具有下列存取權才能手動更新任務：

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。


## 您可以更新任務完成百分比的區域

您可以在下列任一區域中更新任務的完成百分比：

* **在工作清單中**：當顯示「完成百分比」欄時，您可以更新任務的完成百分比。\
  如需內嵌編輯的詳細資訊，請參閱 [在Adobe Workfront中內嵌編輯清單中的專案](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **在里程碑檢視中**：在專案清單或專案報告上使用里程碑檢視時，您可以更新任務的完成百分比。 如需詳細資訊，請參閱 [使用里程碑檢視](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **當您更新任務時**：將更新新增至任務時，您可以更新任務的完成百分比選項。

  >[!IMPORTANT]
  >
  >只有在啟用「顯示完成百分比」選項後，才會顯示此選項。\
  >若要啟用任務的完成百分比更新列，請執行下列動作：
  >
  >1. 前往 **主要** menu>您的名稱>**更多** 圖示加以存取>**編輯** >選取 **顯示更新狀態的完成百分比**.\
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >

* **在任務標題中**：您可以在任務標題中更新任務的完成百分比。 如需詳細資訊，請參閱 [編輯任務](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)


## 更新任務完成百分比的考量事項

* 當您將任務標示為100%完成時，任務「狀態」會更新為「完成」。
* 父系任務存在下列情況：
   * 當專案的「摘要完成模式」設定為「自動」且子任務未完成時，您無法將父系任務的完成百分比更新為100%。
   * 當專案的「摘要完成模式」設定為「手動」，且子作業已完成或不完成時，您可以將父系作業的完成百分比更新為100%。

  如需詳細資訊，請參閱 [編輯專案](../manage-projects/edit-projects.md).

## 更新任務的完成百分比

1. 前往Workfront中的下列任一區域：

   * 工作清單
   * 專案清單和應用里程碑檢視
   * 任務，透過存取任務頁面
1. 找到 **完成百分比** 您要更新其完成百分比之任務的欄位。
1. 按一下完成百分比欄位，然後輸入介於0到100之間的數字

   或

   按一下並拖曳 **完成百分比** 列至必要的數字，以指出您完成了多少工作。

   >[!NOTE]
   >
   >當您指出所有的工作都已完成時，工作的狀態也會更新為「完成」。


1. 在鍵盤上按Enter鍵以儲存完成百分比。

