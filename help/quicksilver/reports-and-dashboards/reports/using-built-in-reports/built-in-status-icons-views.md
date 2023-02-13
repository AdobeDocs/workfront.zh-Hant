---
product-area: reporting
navigation-topic: using-built-in-reports
title: 檢視中的內建狀態圖示
description: 檢視中的內建狀態圖示
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1291'
ht-degree: 2%

---

# 檢視中的內建狀態圖示

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.) </p>
-->

您可以在檢視中將內建的「狀態圖示」欄位新增為欄，以增強對象關鍵點的可見性。 使用「狀態圖示」，您可在下列條件存在時一覽：

* 對象附加了文檔
* 對象與批准過程相關聯
* 對象具有與其關聯的附加註釋
* 費用是可計費或可償還的
* 任務位於關鍵路徑上
* 使用者屬於公司、團隊，或位於不同時區

「狀態表徵圖」欄位中的大多數指示符是指向實際對象或其表示的對象區域的快速連結。

如果對象中缺少表徵圖所表示的任何項，則表示缺失項的表徵圖將作為大綱顯示在「狀態表徵圖」列中，而不是完整影像。\
![task_status_icons.png](assets/task-status-icons.png)\
如需詳細資訊，請參閱 [狀態圖示和標幟概述](#overview-of-status-icons-and-flags) 一節。\
在某些情況下， **狀態表徵圖** 欄位已命名 **標幟** 或 **查看表徵圖**.\
您無法自訂「狀態表徵圖」欄位中表徵圖的外觀和風格。

## 存取需求

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
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取，以新增欄至報表</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理現有檢視的權限</p> <p>管理報表的權限以新增欄</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 將「狀態表徵圖」欄位添加到視圖

有些內建檢視和報表已包含「狀態圖示」欄位。

您無法將「狀態圖示」欄位新增至所有檢視。

若要將「狀態圖示」欄位新增至您從頭建立的自訂檢視：

1. 轉到下列任一對象的清單：

   * 任務
   * 問題
   * 專案
   * 範本任務
   * 範本
   * 費用
   * 文件
   * 使用者\
      只有這些物件具有 **狀態表徵圖** 欄位。\
      有關對象清單的資訊，請參見 [開始使用Adobe Workfront中的清單](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. 從 **檢視** 下拉式功能表，選取 **新建視圖**.

1. 按一下 **添加列**.
1. 在 **顯示在此列中** 框中，開始鍵入以下任何欄位名稱，然後在清單中出現時選擇它：

   * *狀態圖示*
   * *標誌*
   * *查看表徵圖*（僅在文檔視圖中）。

   內建圖示會列在任一名稱下。\
   範本檢視包含 **狀態表徵圖** 和 **標幟** 欄位。 在此情況下，兩欄包含相同的圖示。\
   文檔視圖包含 **查看表徵圖** 欄位。

1. 按一下 **保存視圖**.
1. （選用）為檢視指定新名稱，然後按一下 **保存視圖**.\
   這會新增 **狀態表徵圖** 欄。
1. （選用）將滑鼠移至圖示上方，即可了解其代表什麼。
1. （可選）按一下圖示，前往所代表之物件的區域。\
   並非所有圖示都是物件的連結。\
   如需每個圖示的完整屬性清單，請參閱 [狀態圖示和標幟概述](#overview-of-status-icons-and-flags) 區段。

## 狀態圖示和標幟概述 {#overview-of-status-icons-and-flags}

下表列出Workfront中可用的所有狀態圖示、可與其關聯的物件類型，以及按一下後會發生的情況。

您必須具有至少「查看對象」的權限，才能按一下以下某些表徵圖並訪問這些對象。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>狀態表徵圖或標籤</strong> </th> 
   <th><strong>說明</strong> </th> 
   <th><strong>物件</strong> </th> 
   <th>按一下</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">或 <img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon__in_trouble.png" style="width: 29;height: 26;"> 或 <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_risk.png" style="width: 27;height: 28;"> 或 <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>指出專案的條件為「On Target」（綠色）、「In Failue」（紅色）或「At Risk」（黃色）。<br>如需專案條件的相關資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">專案條件和條件類型概觀</a>.</td> 
   <td>專案</td> 
   <td>按一下以開啟專案的工作清單。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>指示對象在「更新」頁簽中有注釋（更新）。</td> 
   <td> <p>專案<br>工作<br>問題<br>範本<br>模板任務</p> </td> 
   <td> <p>按一下以開啟對象的「更新」(Updates)頁簽。 </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">或 <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>指示對象已附加文檔。 </td> 
   <td> 專案<br>工作<br>問題<br>範本<br>模板任務 </td> 
   <td>按一下以開啟對象的「文檔」(Documents)頁簽。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issu_icon.png" style="width: 34;height: 36;">或 <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>表示項目或任務上存在未結問題。</td> 
   <td> 專案<br>工作 </td> 
   <td>按一下以開啟物件。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="approval_icon.png" style="width: 42;height: 38;"> 或 <img src="assets/new-approval-icon-33x35.png" alt="new_approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>表示對象上有批准。</td> 
   <td> 專案<br>工作<br>問題<br>範本<br>模板任務 </td> 
   <td>按一下以開啟物件。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="expenses_icon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>您可以在視圖中添加「費用」表徵圖列以顯示此表徵圖。 這表示項目或任務具有與它們關聯的費用。</p> </td> 
   <td> <p>專案</p> <p>任務</p> </td> 
   <td>按一下以開啟項目或任務的「費用」頁簽。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>指示任務的「進度狀態」為以下任務之一：</p> 
    <ul> 
     <li>開啟時間（綠方）</li> 
     <li>延遲（紅色圓形）</li> 
     <li>風險（藍色鑽石）</li> 
     <li>後面（黃色三角形）</li> 
    </ul> <p>有關任務的進度狀態的資訊，請參見 <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任務進度狀態概述</a>.</p> </td> 
   <td>任務</td> 
   <td>按一下以開啟任務。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_critical_path_icon.png" style="width: 36;height: 35;"> 或 <img src="assets/new-critical-path-icon-34x34.png" alt="new_critical_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>指示任務當前位於關鍵路徑上。 <br>有關項目關鍵路徑上的任務的資訊，請參見 <a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">項目關鍵路徑概述</a>.</td> 
   <td>任務</td> 
   <td>按一下以開啟任務。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>指示任務與里程碑相關聯。 您的系統管理員可以自訂環境中菱形的顏色。<br>如需里程碑的資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">建立里程碑路徑</a>.</td> 
   <td>任務</td> 
   <td>按一下以開啟任務。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>連結至問題的來源物件。 問題的來源物件是記錄問題的物件。 任務或項目可以是問題的源對象。 </td> 
   <td>問題</td> 
   <td>按一下以開啟問題的源對象（任務或項目）。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resoling_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>指出有一個可最終解決問題的解決對象。 在此情況下，您無法完成問題。 解析對象完成後，將完成它。 <br>有關解析對象的資訊，請參見 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>.</td> 
   <td>問題</td> 
   <td>按一下以開啟問題的解決物件。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>查看文檔。</td> 
   <td>文件</td> 
   <td>按一下以下載文檔。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>下載檔案。</td> 
   <td>文件</td> 
   <td>按一下以下載文檔。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>指示文檔的類型。</td> 
   <td>文件</td> 
   <td>按一下以下載文檔。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_telles_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>指出使用者與公司相關聯。 </td> 
   <td>使用者</td> 
   <td>不可用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>指示用戶與某個團隊關聯。</td> 
   <td>使用者</td> 
   <td>按一下以開啟使用者設定檔。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>使用者的「配置」索引標籤的捷徑。 </td> 
   <td>使用者</td> 
   <td>按一下以開啟使用者的「配置」索引標籤，並了解指派給使用者的工作項目。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>指出使用者所在的時區與系統不同。</td> 
   <td>使用者</td> 
   <td>不可用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_expense_icon.png" style="width: 44;height: 45;"> </td> 
   <td>指明費用是可開單的。<br>有關費用的資訊，請參閱 <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理項目費用 </a>.</td> 
   <td>費用</td> 
   <td>不可用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="expense_recommendable_icon.png" style="width: 44;height: 45;"> </td> 
   <td> 指明費用是可償還的。<br>有關費用的資訊，請參閱 <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理項目費用 </a>.</td> 
   <td>費用</td> 
   <td>不可用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="revercated_expense_icon.png" style="width: 44;height: 43;"></td> 
   <td> 表示已報銷費用。<br>有關費用的資訊，請參閱 <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理項目費用 </a>.</td> 
   <td>費用</td> 
   <td>不可用</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
