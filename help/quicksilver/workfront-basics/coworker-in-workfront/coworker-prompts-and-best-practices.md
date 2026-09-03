---
title: CX Co-worker提示和最佳作法
content-type: reference
description: 瞭解在Workfront中使用同事的最佳實務，並檢視提示範例清單。
author: Becky
feature: Get Started with Workfront
source-git-commit: 01de260893e5bbf7a228479df2f3fc6a1337d31d
workflow-type: tm+mt
source-wordcount: '2247'
ht-degree: 1%

---

# CX Co-worker提示和最佳作法

&lt;！ — 不要使用這個 — 請改為連結到MCP範例提示文章，確定它已更新為最新的MCP版本 — >

>[!IMPORTANT]
>
>CX Co-worker目前不適用於醫療、金融或其他具有敏感資料產業的組織使用。 AI助理可供這些組織使用。 如需詳細資訊，請參閱[AI助理概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。

有了CX Co-worker，您可以使用自然語言與Workfront Workflow和Workfront Planning互動。

同事是Adobe Experience Cloud Agent Orchestrator的一部分。

如需Agent Orchestrator的詳細資訊，請參閱[Adobe Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/zh-hant/docs/experience-cloud-ai/experience-cloud-ai/agents/agent-orchestrator)。

## 存取權要求

<!--Add info about how to qualify for agent orchestrator stuff-->

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>選取、Prime或Ultimate </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準或淺色</p>
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td><p>若要使用基本技能以外的任何功能，貴組織必須已購買Adobe Agent Orchestrator。</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td><p>您必須擁有適當的許可權，才能透過Co-worker與任何物件互動。</p> <p>例如，若要透過「同事」接收專案的相關資訊，您至少必須擁有該專案的「檢視」許可權。</p></td>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

* 您的Workfront管理員必須為貴組織啟用AI助理。

  如需詳細資訊，請參閱AI助理總覽一文中的[ AI助理的必要條件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)。
* 您的Workfront管理員必須為您的存取層級啟用AI助理。

  如需詳細資訊，請參閱[啟用或停用AI助理](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

## 考量事項

使用CX Co-worker時，請考量下列限制：

### 可回覆

某些動作可以還原。 例如，如果建立了物件，該建立可以反轉。

但是，某些動作（例如物件刪除）無法&#x200B;**回覆**。 透過同事對您的資料執行動作時，建議您將此謹記在心。

### 資料/物件涵蓋範圍限制

* 對自訂欄位的查詢和報告處於早期階段，並且某些技能（如基於API的查詢協助程式）尚未處理用於彙總和篩選的任意自訂欄位。

### 互動/UX限制

* CX Co-worker目前不會從個別使用者的風格或偏好設定中長期「學習」。 每次聊天都只使用目前的交談和產品知識。
* 交談內容會保留在單一交談工作階段中。 開啟新頁面或關閉助理會重設交談記錄。
* 如果核准程式位於外部應用程式（如Confluence或SharePoint）中，且僅透過URL欄位連結，Co-worker目前不會擷取並推斷這些頁面。

### 資料儲存/客戶管理的金鑰

* 由於CX Co-worker是Adobe Experience Platform Agent Orchestrator的一部分，您與Co-worker互動的資料會儲存在Adobe Experience Platform中，而非Workfront中。 因此，Workfront客戶自控金鑰(BYOK)合約不涵蓋這些資料。

## 一般用途的基礎AI技能

>[!IMPORTANT]
>
>這些一般使用功能適用於其組織已在檔案中簽署Adobe AI合約的所有使用者。

如需這些一般使用技能的最佳實務和提示，請參閱[AI助理提示和最佳實務](/help/quicksilver/workfront-basics/ai-assistant/ai-prompts-best-practices.md)。

<!--Follow up with Oznur-->

### 產品知識

CX Co-worker可提供從Workfront檔案取得的指示或參考資訊。

如需有關從Workfront檔案提取資訊的詳細資訊，請參閱[從AI助理取得說明](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md)。

範例：如何變更任務期間型別？

### 專案、任務和問題摘要

CX Co-worker可摘要說明已上傳至Workfront的專案、任務或問題<!--, or documents-->。

如需有關專案、任務和問題摘要的詳細資訊，請參閱[使用AI助理摘要](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md)。

範例：摘要說明名為「秋季促銷活動2026」的專案。

<!--

### Locate work items

CX Coworker can find work items like projects, tasks, and issues

Example: Find all tasks assigned to me that are due this week.

For more information on using AI Assistant to locate project, tasks, and issues, see [se AI Assistant to work with projects, tasks, and issues](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

-->

<!--

Follow up on this to see if it's going away or what

### Catch Me Up 

Catch Me Up summarizes updates, uploaded documents, and other notable changes that have about your projects that have occurred in the last 24 hours, 3 days, or 7 days.  

For more information on Catch me up, see [Catch up on work in Priorities](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).

-->

<!--

### Smart filters

You can use natural language filters in Priorities to replace status, pre-built views to help you filter your work.

For more information on using Smart Filters, see [Filter your work with Smart filters](/help/quicksilver/workfront-basics/priorities/filter-group-work-priorities.md) in the article Filter and group your work with Priorities.

-->

## Workfront中的CX Co-worker

* [專案、任務和問題資訊](#project-task-and-issue-information)
* [專案和工作管理](#project-and-work-management)
* [內容與核准](#content-and-approvals)

### 專案、任務和問題資訊

CX Co-worker可提供專案、任務和問題的相關資訊，包括摘要和專案狀況。

請參閱以下區域的檔案和資產核准提示範例：

* [尋找有關專案、任務或問題的資訊](#find-information-about-projects-tasks-or-issues)
* [概述專案、任務或問題](#summarize-projects-tasks-or-issues)
* [顯示專案、計畫或投資組合的專案狀況](#show-project-health-for-projects-programs-or-portfolios) <!--remove any mention of project health-->

#### 尋找有關專案、任務或問題的資訊

* 專案
  * 顯示品牌行銷團隊的所有作用中專案
  * 需要「數位」類別下的第4季行銷活動組合中的專案清單。
  * 顯示由Creative Services公司中身為專案經理的使用者所管理的專案。
* 任務
  * 將指派給Joan Harris的所有任務交給我。
  * 顯示指派給UX團隊的「設計」類別中的任務。
  * 我需要在「假日行銷活動」方案中指派給撰稿人的工作。
* 問題
  * 在「技術」類別下顯示「網站重新設計」專案中的所有問題。
  * 給我問答群組報告的所有未解決問題。
  * 我需要將問題指派給全球技術公司的開發人員。

#### 概述專案、任務或問題

* &quot;摘要本專案&quot;
* 「總結此專案的最後一週」

#### 顯示專案、計畫或投資組合的專案健康情況

>[!NOTE]
>
>您的組織必須註冊Project Health測試版才能使用此功能。

* 「顯示我作用中專案的健康情況」
* 「顯示這個程式的健康情況」

### 專案和工作管理

您可以使用CX Co-worker來建立和管理專案，包括任務和指派。

請參閱以下區域的專案和工作管理範例提示：

* [建立、更新或刪除專案](#create-update-or-delete-projects)
* [根據使用者提示識別正確的專案範本](#identify-the-right-project-template-based-on-user-prompt)
* [新增、編輯或自訂專案中的任務](#add-edit-or-customize-tasks-in-a-project)
  <!--* [Create, update, or delete assignments](#create-update-or-delete-assignments)-->
  <!--* [Recommend best matching user assignments for the task based on users' job role and availability](#recommend-best-matching-user-assignments-for-the-task-based-on-users-job-role-and-availability)-->

#### 建立、更新或刪除專案

您可以從頭開始建立專案，或從範本建立專案、更新專案及刪除專案。

* 從3月10日起至4月30日止，建立名為「第2季創新沙箱」的空白專案。 將我設為擁有者。
* 使用整合式行銷活動範本，建立名為Lucent AI Launch - NA的專案。 從2月5日開始，並將其設定為目前。
* 自3月1日起至6月15日止，建立名為「網站重新設計 — EMEA」的專案。 這項優先服務由EMEA行銷部門所擁有，由行銷部門的VP提供贊助，預算為25萬美元，預計約1,200小時，著重於歐洲，目標是提高轉換率。
* 針對Lucent AI Launch - NA專案，將其移至第2季，將目標變更為推動免費試用，將完成日期推進至4月中旬，將預算增加至15萬美元，並標籤為緊急。
* 顯示於第2季完成的所有目前行銷專案（高優先順序或緊急優先順序），以最早的結束日期排序。

#### 新增或編輯任務

您可以在專案中新增或編輯任務，也可以自訂用來建立專案的範本任務清單。

* 將稱為登陸頁面QA的新任務新增到專案，並排程從4月22日至4月26日。
* 更新「設計評論」任務，使其在4月18日完成，並將其指派給創意團隊。
* 從專案移除列印資產生產任務。
* 顯示此專案中未完成且排程在4月1日至4月30日之間開始的所有任務。
* 將「合法核准」設定為「行銷活動啟動」任務的前置任務。
* 新增名為「最終復本拋光版」的新任務，此任務排程從4月15日到4月16日，將「復本檢閱」任務移至4月10日，移除「額外檢閱」輪次任務，並將「最終復本拋光版」設定為「電子郵件建置」的前置任務。
* 在專案建立期間，請嘗試儘可能多地提供有關交付專案（最好應成為專案下的任務）的資訊。

#### 建立、更新或刪除指派

您可以建立、更新及刪除使用者或工作角色指派。

* 針對「產品上市的設計登陸頁面」專案，請為所有目前未指派的任務識別適當的職務角色和建議計畫時數。
* 我有數項未指派的工作，包括「對行銷活動網站實作GA4追蹤」、「設定轉換事件」和「驗證分析資料」。 您可以為每個人建議合適的工作角色和估計時數嗎？
* 對於創意工作「為EMEA顯示廣告建立3個橫幅變體」、「套用修訂版本」和「匯出最終資產」，請指派最佳工作角色並估計每個工作所需的精力。
* 在專案「第2季產品上市」、「網站重新設計 — EMEA」和「付費媒體行銷活動 — NA」中，識別所有未指派的工作並為每個工作角色指派具有建議計畫時數的適當工作角色。

<!--

#### Identify the right project template based on user prompt

* We're launching a new product feature with a landing page, emails, paid ads, and social posts. Which project template should we use?
* Create a project for a global marketing campaign with multiple channels and regional rollouts. (should suggest a template if provided more info)
* For Website Redesign – EMEA project, recommend and attach the correct project template.

-->

<!--

#### Recommend best matching user assignments for the task based on users' job role and availability

* Who is the best available user to assign to 'Design Landing Page Hero', considering who still has capacity today?
* Who should be assigned to 'Backend API integration for campaign reporting', considering engineering role alignment?
* For all unassigned tasks in this project, recommend the best users based on job role match and daily availability.
* Recommend users for the tasks 'QA testing for website launch' and 'Content review', prioritizing users whose job roles match and who are not over-allocated today.

-->

### 內容與核准

CX Co-worker可協助管理Workfront中的檔案和資產核准。

處理檔案和資產核準時，請考慮下列事項：

* 您必須先為您的組織啟用內容核准，才能在同事中使用此功能。
* AI無法代表人類核准或拒絕。 除了Workfront AI檢閱者外，決策依賴使用者。

  如需Workfront AI檢閱者的詳細資訊，請參閱[開始使用Workfront AI檢閱者](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)。
* 此功能存在於Workfront中，無法用於與外部工具或檔案提供者互動。
* 為獲得最佳體驗，請將此功能與整合式核准體驗搭配使用。

  如需整合式核准的詳細資訊，請參閱[整合式核准總覽](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)。

請參閱以下區域的檔案和資產核准提示範例：

* [新增或移除核准參與者](#add-or-remove-approval-participants)
* [提醒專案關係人單一資產正在等候檢閱](#remind-stakeholders-of-a-single-asset-waiting-for-review)
* [新增、更新或套用單一資產的核准範本](#add-update-or-apply-approval-templates-for-a-single-asset)

#### 新增或移除核准參與者

* 將Sarah Chen和Miguel Alvarez新增為目前檔案的核准者。
* 從此核准中移除Jennifer Otto。
* 移除尚未做出核准決定的任何人。
* 在spring-campaign.pdf中新增一個稱為「最終稽核」的新階段。
* 在winter-campaign.pdf的第二階段新增Mark和Sarah作為核准者，Phil作為檢閱者
* 對於winter-campaign.pdf，請將第一階段的截止日期設為今天下午5點，而最終稽核的截止日期設為明天下午5點
* 在fall-campaign.png中新增Final check stage （最後檢查階段），截止時間為星期四下午5點，並加入Jim和Pam作為核准者，以及Oscar作為檢閱者
* 將Mark Jones新增至fall-campaign.png作為檢閱者的第一個和最後一個階段。
* 我們將針對fall-campaign.png建立多階段核准，包含3個階段、1個設計2個撰稿和3個法律檔案。 每個階段只需要一個決定。 將Mike、Sally、Jane加入設計，將Chris、Richard、Mark加入撰寫，將Phil、Tom和Sarah加入法律。

#### 提醒專案關係人單一資產正在等候檢閱

* 傳送提醒給資產「Spring Campaign影片」上尚未回應的核准者。
* 提醒所有尚未核准此資產的人「春季行銷活動影片」。
* 誰尚未針對「PDF品牌指引」資產作出決定？ 提醒他們。

#### 新增、更新或套用單一資產的核准範本

* 將「行銷啟動」核准範本套用至名為「春季行銷活動影片」的資產。
* 建立具有3個階段的新核准範本：Creative稽核、法律及最終核准。
* 將Julia Santos和Shane Baker加入階段1。
* 編輯「產品啟動」範本，將Elizabeth Peterson新增至最終核准階段。
* 建立一個名為「緊急稽核」的範本，並包含一個階段，然後指派給Olivia Kim。
* 移除Rick Kuvec並將Karen Sterling新增至階段2，以更新「Creative Review」範本。


## Workfront中的CX同事Planning

### 使用Planning記錄

* [建立、刪除、複製或還原記錄](#create-delete-duplicate-or-restore-records)
* [將記錄連結至其他記錄](#link-records-to-other-records)
* [編輯、更新或附加欄位到記錄](#edit-update-or-append-a-field-to-a-record)
* [存取記錄變更記錄](#access-record-change-history)

#### 建立、刪除、複製或還原記錄

* 建立名為「2026年夏季優惠」的新行銷活動記錄
* 新增名為Widget Pro且價格為$299的新產品記錄
* 您可以為John Smith建立新的潛在客戶記錄嗎？
* 刪除名為「舊促銷」的行銷活動記錄
* 移除我剛才建立的測試記錄
* 您可以刪除記錄ID Rc123abc456嗎？
* 複製第1季行銷活動記錄
* 您可以複製此行銷活動以建立新行銷活動嗎？
* 製作假日促銷活動副本
* 還原我意外刪除的行銷活動
* 您可以復原已刪除的專案記錄嗎？
* 我意外刪除了記錄，您可以還原它嗎？

#### 將記錄連結至其他記錄

* 將夏季行銷活動記錄連結至第2季計畫
* 您可以將此產品連結至相關的行銷活動嗎？
* 我需要將這三個銷售機會與企業帳戶記錄建立關聯

#### 編輯、更新或附加欄位到記錄

* 將夏季行銷活動中的預算欄位更新為$75,000
* 您將此專案記錄的狀態變更為「已完成」嗎？
* 將John Doe新增至此方案的團隊成員欄位

#### 存取記錄變更記錄

* 顯示夏季行銷活動記錄的變更記錄
* 您可以顯示誰修改了此專案以及變更了哪些內容？
* 我需要檢視上週對此記錄所做的所有更新

### 在Workfront Planning中使用系統Designer

* [建立及設定工作區](#create-and-configure-workspaces)
* [定義記錄型別](#define-record-types)
* [設計欄位和公式欄位](#design-fields-and-formula-fields)
* [建置自訂檢視](#build-custom-views)


#### 建立及設定工作區

* 建立名為「2026年行銷活動」的全新規劃工作區
* 更新我的產品規劃工作區以將顏色變更為藍色並新增說明
* 顯示我有權存取的所有Planning工作區

#### 定義記錄型別

* 在我的Planning工作區中建立稱為「行銷活動」的新記錄型別
* 更新方案記錄型別以變更其圖示和說明
* 顯示行銷計畫工作區中的所有記錄型別

#### 設計欄位和公式欄位

* 新增預算欄位至具有貨幣型別的規劃行銷活動記錄型別
* 在Planning中建立公式欄位，以計算行銷活動結束日期前的剩餘天數
* 更新我的Planning工作區中的「優先順序」欄位，以新增更多下拉式清單選項

#### 建置自訂檢視

* 在「計畫」中建立時間表檢視，以按開始和結束日期檢視我的行銷活動排程
* 新增表格檢視至我的Planning方案，該檢視只會篩選作用中狀態
* 複製我的Planning作用中行銷活動檢視並修改排序。
