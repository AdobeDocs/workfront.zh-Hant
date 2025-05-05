---
product-area: reporting
navigation-topic: using-built-in-reports
title: 檢視中的內建狀態圖示
description: 您可以將內建的狀態圖示欄位新增為檢視中的欄，以增進物件關鍵點的可見度。
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: 0022892cabb9a44fb21e33d88148b098c937f388
workflow-type: tm+mt
source-wordcount: '1213'
ht-degree: 3%

---

# 檢視中的內建狀態圖示

<!-- Audited: 11/2024 -->

<!--(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.)-->

您可以將內建的狀態圖示欄位新增為檢視中的欄，以增進物件關鍵點的可見度。 使用「狀態圖示」，您可以一眼就看到下列情況：

* 物件已附加檔案
* 物件與核准流程相關聯
* 物件具有與其相關的其他附註
* 費用為可記帳或可償還
* 任務在關鍵路徑上
* 使用者屬於公司、團隊或位於不同時區的個人

請考量下列事項：

* 「狀態圖示」欄位中的大多數指示器都是快速連結，可快速連結到實際物件或它們所代表的物件區域。

* 如果物件中遺漏了圖示所代表的任何專案，則代表遺漏專案的圖示會在「狀態圖示」欄中顯示為灰色，而非彩色影像。

  ![task_status_icons.png](assets/task-status-icons.png)

  如需詳細資訊，請參閱本文中的[狀態圖示與旗標概觀](#overview-of-status-icons-and-flags)一節。

* 在某些檢視中，**狀態圖示**&#x200B;欄位命名為&#x200B;**旗標**&#x200B;或&#x200B;**檢檢視示**。\
  您無法自訂包含在狀態圖示欄位中的圖示外觀。

* 您無法編輯狀態圖示欄位中的圖示數。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>投稿人或以上</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>要求或更高版本</p></li>
         </ul>
   </td>
  </tr>
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯對報告、儀表板、行事曆的存取權以新增欄到報告</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理現有檢視的許可權</p> <p>管理報表的許可權以新增欄</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將狀態圖示欄位新增到檢視

有些內建檢視和報告已包含狀態圖示欄位。

您無法將狀態圖示欄位新增到所有檢視。

若要將狀態圖示欄位新增至您從頭開始建立的自訂檢視：

1. 移至下列任一物件的清單：

   * 任務
   * 問題
   * 專案
   * 範本任務
   * 範本
   * 費用
   * 文件
   * 使用者\
     只有這些物件有&#x200B;**狀態圖示**&#x200B;欄位可用。\
     如需物件清單的相關資訊，請參閱[開始使用Adobe Workfront中的清單](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

1. 從&#x200B;**檢視**&#x200B;下拉式功能表中，選取&#x200B;**新增檢視**。

1. 按一下「**新增欄**」。
1. 在&#x200B;**顯示在此欄**&#x200B;方塊中，開始輸入下列任何欄位名稱，然後在其出現在清單中時選取它：

   * *狀態圖示*
   * *標幟*
   * *檢檢視示* （僅在檔案檢視中）。

   內建圖示會列在任一名稱下。\
   範本檢視同時包含&#x200B;**狀態圖示**&#x200B;和&#x200B;**旗標**&#x200B;欄位。 在這種情況下，兩欄包含相同的圖示。\
   檔案檢視包含&#x200B;**檢檢視示**&#x200B;欄位。

1. 按一下「**儲存視圖**」。
1. （選擇性）指定檢視的新名稱，然後按一下[儲存檢視]。**&#x200B;**\
   這會將&#x200B;**狀態圖示**&#x200B;欄新增至您的檢視。
1. （選用）將滑鼠移至圖示上方，瞭解其代表的意義。
1. （選擇性）按一下圖示，移至該圖示所代表的物件區域。\
   並非所有圖示都是物件的連結。\
   如需每個圖示的完整屬性清單，請參閱[狀態圖示與旗標概觀](#overview-of-status-icons-and-flags)區段。

## 狀態圖示與旗標概要 {#overview-of-status-icons-and-flags}

下表列出Workfront中可用的所有「狀態圖示」、可與其關聯的物件型別，以及按一下它們時會發生什麼事情。

您必須至少擁有檢視物件的許可權，才能按一下下列某些圖示並存取這些物件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>狀態圖示或旗標</strong> </th> 
   <th><strong>說明</strong> </th> 
   <th><strong>物件</strong> </th> 
   <th>按一下</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">或<img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon__in_trouble.png" style="width: 29;height: 26;">或<img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_risk.png" style="width: 27;height: 28;">或 <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>表示專案狀況為達成目標（綠色）、存在問題（紅色）或處於風險（黃色）。<br>如需有關專案狀況的資訊，請參閱<a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">專案狀況與狀況型別概觀</a>。</td> 
   <td>專案</td> 
   <td>按一下以開啟專案的任務清單。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>表示物件在「更新」(Updates)標籤中有註釋（更新）。</td> 
   <td> <p>專案<br>任務<br>問題<br>範本<br>範本任務</p> </td> 
   <td> <p>按一下以開啟物件的「更新」標籤。 </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">或 <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>表示物件已附加檔案。 </td> 
   <td> 專案<br>任務<br>問題<br>範本<br>範本任務 </td> 
   <td>按一下以開啟物件的「檔案」標籤。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issu_icon.png" style="width: 34;height: 36;">或 <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>表示專案或任務有未完成的問題。</td> 
   <td> 專案<br>任務 </td> 
   <td>按一下以開啟物件。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="approval_icon.png" style="width: 42;height: 38;"> 或 <img src="assets/new-approval-icon-33x35.png" alt="new_approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>表示物件上有核准。</td> 
   <td> 專案<br>任務<br>問題<br>範本<br>範本任務 </td> 
   <td>按一下以開啟物件。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="expenses_icon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>您可以在檢視中新增「費用圖示」欄，以顯示此圖示。 這表示專案或任務具有與其關聯的費用。</p> </td> 
   <td> <p>專案</p> <p>任務</p> </td> 
   <td>按一下以開啟專案或任務的「費用」標籤。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>指出任務的進度狀態為下列其中一項：</p> 
    <ul> 
     <li>準時（綠色方塊）</li> 
     <li>延遲（紅色圓形）</li> 
     <li>有風險（藍色菱形）</li> 
     <li>後方（黃色三角形）</li> 
    </ul> <p>如需有關任務進度狀態的資訊，請參閱<a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任務進度狀態總覽</a>。</p> </td> 
   <td>任務</td> 
   <td>按一下以開啟工作。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_critical_path_icon.png" style="width: 36;height: 35;"> 或 <img src="assets/new-critical-path-icon-34x34.png" alt="new_critical_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>指出任務目前位於關鍵路徑。 <br>如需有關專案關鍵路徑上任務的資訊，請參閱<a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">專案關鍵路徑概觀</a>。</td> 
   <td>任務</td> 
   <td>按一下以開啟工作。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>表示任務與里程碑相關聯。 您的系統管理員可以在您的環境中自訂鑽石的顏色。<br>如需里程碑的相關資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">建立里程碑路徑</a>。</td> 
   <td>任務</td> 
   <td>按一下以開啟工作。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>問題的來源物件的連結。 問題的來源物件是記錄問題的物件。 任務或專案可以是問題的來源物件。 </td> 
   <td>問題</td> 
   <td>按一下以開啟問題的來源物件（任務或專案）。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolving_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>表示有解決物件可最終解決問題。 在這種情況下，您無法完成問題。 解析物件完成時它會完成。 <br>如需解析物件的相關資訊，請參閱<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析物件概述</a>。</td> 
   <td>問題</td> 
   <td>按一下以開啟問題的解決物件。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>檢視檔案。</td> 
   <td>文件</td> 
   <td>按一下以下載檔案。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>下載檔案。</td> 
   <td>文件</td> 
   <td>按一下以下載檔案。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>指示檔案的型別。</td> 
   <td>文件</td> 
   <td>按一下以下載檔案。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_belists_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>表示使用者與公司相關聯。 </td> 
   <td>使用者</td> 
   <td>無法使用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>表示使用者與團隊相關聯。</td> 
   <td>使用者</td> 
   <td>按一下以開啟使用者設定檔。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>使用者的「配置」索引標籤的捷徑。 </td> 
   <td>使用者</td> 
   <td>按一下以開啟使用者的「配置」標籤，並瞭解指派給使用者的工作專案。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>表示使用者與系統的時區不同。</td> 
   <td>使用者</td> 
   <td>無法使用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_expense_icon.png" style="width: 44;height: 45;"> </td> 
   <td>表示費用可記帳。<br>如需費用相關資訊，請參閱<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理專案費用</a>。</td> 
   <td>費用</td> 
   <td>無法使用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="expense_refelemable_icon.png" style="width: 44;height: 45;"> </td> 
   <td> 表示費用是可償還的。<br>如需費用相關資訊，請參閱<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理專案費用</a>。</td> 
   <td>費用</td> 
   <td>無法使用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="replaced_expense_icon.png" style="width: 44;height: 43;"></td> 
   <td> 表示費用已償還。<br>如需費用相關資訊，請參閱<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理專案費用</a>。</td> 
   <td>費用</td> 
   <td>無法使用</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
