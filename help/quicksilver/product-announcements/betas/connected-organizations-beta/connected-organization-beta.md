---
product-area: betas
title: 開始使用連線組織功能
description:
author: Alina
feature: Product Announcements
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 1eaa497ba7e446f7fdf978f369205f309bbe231f
workflow-type: tm+mt
source-wordcount: '1428'
ht-degree: 0%
---
# 開始使用連線組織功能

>[!IMPORTANT]
>
>「連線組織」功能目前處於封閉測試階段，且僅開放少數客戶使用。
>
>Beta版將持續至2026年底。
>
>如有疑問，請聯絡您的Adobe Beta版計畫管理員。

連線組織功能可讓公司及其合作夥伴在組織都已購買Adobe Workfront時進行工作上的共同作業。

例如，客戶公司可能會向其提供者公司提交完成工作的請求。

每個公司都可以利用自己的使用者、許可權和工作流程，繼續使用自己的Workfront例項。

工作物件會在兩個執行個體之間映象，只有雙方同意共用的資料才會同步。

結果會產生請求、狀態和決策的共用檢視，而不會有額外的訪客登入、重複授權或長電子郵件執行緒。

## 今日多組織工作流程概觀

當兩家公司都投資於Workfront時，他們應該能夠在不支付兩次費用或進入另一個系統的情況下進行合作。

現在，當兩家公司使用兩個不同的系統時，他們的共同作業可能包括以下一些工作流程：

* 請求和簡報會透過難以遵循的電子郵件對話串進行。

* 移交是手動進行的，可稽核度很低。

* 在另一個公司的系統中工作意味著訪客登入、額外的授權，或兩者皆有。

* 檔案會循環多份，沒有人確定這是真實來源。

* 狀態很難追蹤，因此客戶經理會花時間建置平台及排程更新會議。

## 連線組織解決方案概觀

當您使用「連線」組織功能時，兩家公司會繼續使用兩個不同的系統，其共同作業將包含下列部分工作流程：

* 這兩個組織都不會存取另一個例項中的物件。
* 物件（例如來自使用者端組織的請求）會複製並發佈至提供者的執行個體。
* 只有為同步設定的中繼資料才會在兩個副本之間保持最新。
* 每個公司都管理其自己的使用者、許可權，以及該物件之外的工作流程。

指導原則是共用完成工作所需的最低限度，並保密其他所有內容。

<table>
<tbody>
<tr class="odd">
<td><strong>共用的內容</strong></td>
<td><strong>哪些專案會維持私密狀態</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>簡報和請求詳細資料</p></li>
<li><p>商定的截止日期和里程碑</p></li>
<li><p>審閱評論</p></li>
<li><p>核准決策</p></li>
<li><p>最終核准的資產</p></li>
</ul></td>
<td><ul>
<li><p>與其他客戶或其他代理商的關係</p></li>
<li><p>財務狀況、費率，以及對使用者端收費的專案</p></li>
<li><p>資源規劃與產能</p></li>
<li><p>內部專案結構、任務及未選取要共用的任何欄位</p></li>
</ul></td>
</tr>
</tbody>
</table>

## Beta版中可用的功能

Beta版計畫的第一階段可讓您連線兩個執行個體並開始工作。

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **功能** | **它的作用** |
| **連線的組織** | 連結兩個組織之間的兩個Workfront執行個體。 在Beta版期間，Adobe會設定連線。 自助式設定目前正在開發中。 |
| **要求表單** | 客戶公司會建立請求表單、發佈它，並透過表單的「共用」設定與提供者公司共用。 |
| **AI輔助要求錄取** | 使用者端的請求者可使用AI表單填寫功能來輸入提示並附加檔案，而非填寫長表單。 系統會將該內容對應至表單欄位，並顯示該對應以供檢閱。 請求者接受結果並提交表單。 |
| **映象要求** | 提交的請求會以唯讀副本的形式顯示在提供者公司的「請求」區域中，包括自訂欄位值。 |
| **請求到專案轉換** | 提供者將請求轉換為專案，並選取投資組合、方案和範本以開始工作。 提供者執行個體中的新物件會連結回使用者端的原始要求。 請求公司看不到提供者端實際工作的詳細資訊。 |
| **雙向註解** | 雙方都能看到請求的評論，而且幾乎立即送達，因此雙方可以在一個地方達成一致意見。 |
| **要求接受** | 雙方同意後，提供者就會接受要求，使用者端就會看到要求已被接受。 |
| **AI草擬的狀態更新** | 當請求者在評論中要求狀態時，提供者可以使用AI指令快速且一致地產生草稿回覆。<br> 草稿包含連線到請求的物件資訊，例如計畫完成日期、條件和根據計畫時數記錄的時數。<br> 這是最重要資訊的摘要，而不是逐欄匯出。 在將回應傳送給使用者端之前，人員會稽核並編輯該回應。 |

## 端對端工作流程

本節說明在相關組織的Workfront執行個體連線後，參與此整合的兩方的工作流程。

我們以使用者端及提供者工作流程為例。

### 使用者端的工作流程

作為使用者端組織中的請求者，您可以執行以下操作：

1. 建立或要求管理員建立請求表單、發佈它，並與連線的提供者組織共用。

2. 從「請求」區域開啟已發佈的表單，輸入提示並附加任何檔案。

3. 檢閱內容如何對應至表單欄位、接受和提交。

### 提供者的工作流程

身為提供者組織中的工作管理員，請執行下列動作：

1. 在您的請求區域中以唯讀副本的形式接收請求。

2. 透過註解討論請求，直到兩側對齊為止，然後接受它。

3. 將請求轉換為專案，視需要選擇投資組合、計畫和範本。

4. 選擇將哪些專案欄位映象回使用者端的請求。

5. 回答評論中的狀態問題，或產生草稿狀態更新、稽核並發佈到您的請求。 它也會顯示在使用者端的原始請求上。

   從那時起，提供者端的請求就會成為使用者端原始請求的復本，因此評論和議定的資料會保持同步。

## 安全性與治理

保護每個組織的資料是核心設計需求。

我們希望Beta版建立的基準之一，就是IT和安全性團隊核准及管理執行個體之間連線的難易程度。

以下是連線組織工作流程的優點：

* **無跨執行個體存取**：您的執行個體中不需要來自夥伴組織的使用者，因此沒有訪客登入及額外的授權。

* **最低必要共用**：僅共用為同步設定的資料。 其他所有專案都會保留在其原始執行個體中。

* **獨立控制項**：每個組織都會保留自己的使用者、許可權和工作流程。

* **團隊層級範圍**：請求旨在使用現有的Workfront存取控制項，僅聯絡為該使用者端設定的代理團隊。

## 藍圖展望

以下階段說明我們目前的開發和發行計畫。 排序可能會根據我們在Beta版階段中學到的知識而改變。 後續階段不是承諾。

<table>
<tbody>
<tr class="odd">
<td><strong>階段</strong></td>
<td><strong>焦點與規劃的功能</strong></td>
<td><strong>狀態</strong></td>
</tr>
<tr class="even">
<td><strong>階段1</strong></td>
<td>連線執行個體並開始工作：請求表單、AI輔助接收、映象請求、專案轉換、評論和狀態草稿。</td>
<td>Beta版</td>
</tr>
<tr class="odd">
<td><strong>階段2</strong></td>
<td><ul>
<li><p>使用框架及整合式檢閱和核准體驗來檢閱和核准</p></li>
<li><p>無論利害相關者如何運作，待決審查都會出現在Workfront或框架中</p></li>
<li><p>註解會與工作檔案維持繫結，讓創意團隊能在一個地方看到意見反應</p></li>
</ul></td>
<td>已規劃</td>
</tr>
<tr class="even">
<td><strong>階段3</strong></td>
<td><ul>
<li><p>除了請求之外，以任務為基礎的工作指派</p></li>
<li><p>更多自動化狀態，透過共用或非共用欄位告知</p></li>
<li><p>新的交付專案物件型別，其中包含簡報期間定義的中繼資料，並由最終核准的資產繼承</p></li>
<li><p>將核准的最終資產直接傳送至品牌的AEM，減少手動輸入中繼資料</p></li>
</ul></td>
<td>已規劃</td>
</tr>
<tr class="odd">
<td><strong>階段4</strong></td>
<td><ul>
<li><p>合作夥伴間的共用內容</p></li>
<li><p>檢閱前使用Adobe Brand Intelligence <!--by the agency-->，存取權由團隊控制</p></li>
<li><p>上下文相關的功能，例如預估</p></li>
</ul></td>
<td>長期</td>
</tr>
</tbody>
</table>

## 參與測試版

洽詢您的Adobe測試版計畫經理以參與測試版。

### 我們對參與者的要求

* 加入每週回饋通話。

* 每週約有一小時由您自行進行實際測試。 隨叫隨到的即時工作階段是一個選項。

* 儘可能將合作夥伴的觀點帶入會議。

* 識別要連線的Workfront環境，並為少數Adobe工程師布建管理員帳戶，以便他們驗證連線。

### 我們想要瞭解的

* 映象物件並僅同步所選資料是否為正確的共用模型？ 每一面是否都有足夠的彈性？

* 階段順序正確嗎？還是應該更早提供後續功能？

* 共同作業中缺少哪些接觸點？

* 兩個執行個體之間的欄位命名和對應應該如何運作？

  現在，表單和請求由使用者端擁有，並且提供者透過使用者端的欄位名稱將它們視為唯讀。

* IT需要什麼來核准和管理連線？




<!--

Original pdf from team:

**ADOBE WORKFRONT | BETA PROGRAM**

**Agency Brand Connectors**

Product overview for beta participants

# **Overview**

Agency Brand Connectors lets a brand and its agency collaborate on work when both organizations run Adobe Workfront. Each side keeps working in its own Workfront instance, with its own users, permissions, and workflows. Work objects are mirrored between the two instances, and only the data both sides agree to share is synchronized.

The result is a shared view of requests, status, and decisions without guest logins, duplicate licenses, or long email threads.

# **The challenge this addresses**

When a brand and an agency are both invested in Workfront, they should be able to work together without either one paying twice or moving into the other's system. Today the collaboration usually looks like this:

  - Requests and briefs travel through email threads that are hard to follow.

  - Handoffs are manual, with little auditability.

  - Working inside a partner's system means guest logins, extra licenses, or both.

  - Multiple copies of files circulate, and no one is sure which is the source of truth.

  - Status is hard to see, so producers and account managers spend time building decks and scheduling update meetings.

# **How it works: the sharing model**

Neither organization accesses an object in the other's instance. Instead, an object such as a request is duplicated and published into the partner's instance, and only the metadata configured for sync is kept up to date between the two copies. Each side manages its own users, permissions, and workflows downstream of that object.

The guiding principle is to share the minimum needed to get the work done, and to keep everything else confidential.

<table>
<tbody>
<tr class="odd">
<td><strong>What is shared</strong></td>
<td><strong>What stays private</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Briefs and request details</p></li>
<li><p>Agreed deadlines and milestones</p></li>
<li><p>Review comments</p></li>
<li><p>Approval decisions</p></li>
<li><p>Final approved assets</p></li>
</ul></td>
<td><ul>
<li><p>Relationships with other clients or other agencies</p></li>
<li><p>Financials, rates, and what is charged to the client</p></li>
<li><p>Resource planning and capacity</p></li>
<li><p>Internal project structure, tasks, and any fields not selected for sharing</p></li>
</ul></td>
</tr>
</tbody>
</table>

# **Features available in the beta**

The first phase of the beta covers connecting two instances and kicking off work.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Feature**                       | **What it does**                                                                                                                                                                                                                                                                                                                      |
| **Connected organizations**       | Links a brand instance and an agency instance. During the beta, Adobe configures the connection. A self-serve setup is being worked on.                                                                                                                                                                                               |
| **Request forms**                 | The brand creates a request form, publishes it, and shares it with a connected organization from the form's Share settings.                                                                                                                                                                                                           |
| **AI-assisted request intake**    | The requester types a prompt and attaches files instead of filling out a long form. The system maps that content to the form fields and shows the mapping for review. The requester accepts the result and submits. This uses Workfront's existing form-filling technology.                                                           |
| **Mirrored requests**             | The submitted request appears in the agency's request area as a read-only copy, including custom field values.                                                                                                                                                                                                                        |
| **Request-to-project conversion** | The agency converts the request into a project and selects the portfolio, program, and template. The new object is linked back to the request. Downstream work on the agency side is not visible to the brand.                                                                                                                        |
| **Two-way comments**              | Comments on the request are visible on both sides and arrive almost immediately, so both parties can work toward agreement in one place.                                                                                                                                                                                              |
| **Request acceptance**            | Once both sides agree, the agency accepts the request and the brand sees that it has been accepted.                                                                                                                                                                                                                                   |
| **AI-drafted status updates**     | When a brand asks for status in a comment, the agency can use a slash command to generate a draft reply. The draft draws on connected objects, such as planned completion date, condition, and hours logged against hours planned. It is a summary, not a field-by-field export, and a person reviews and edits it before publishing. |

# **End-to-end workflow**

## **Brand side**

1.  Create a request form, publish it, and share it with the connected agency.

2.  Open the published form, enter a prompt, and attach any files.

3.  Review how the content maps to the form fields, accept, and submit.

## **Agency side**

1.  Receive the request in the request area as a read-only copy.

2.  Discuss the request through comments until both sides are aligned, then accept it.

3.  Convert the request into a project, choosing the portfolio, program, and template.

4.  Choose which project data is mirrored back to the brand.

5.  Answer status questions in comments, or generate a draft status update, review it, and publish.

From that point on, the request on the agency side acts as a replica of the request on the brand side, so comments and agreed data stay in step.

# **Security and governance**

Keeping each organization's data protected is a core design requirement, and one of the baselines we want the beta to establish is how easily IT and security teams can approve and administer a connection between instances.

  - **No cross-instance access.** No users from the partner organization are needed in your instance, so there are no guest logins and no additional licenses.

  - **Minimum necessary sharing.** Only the data configured for sync is shared. Everything else stays in the originating instance.

  - **Independent controls.** Each organization keeps its own users, permissions, and workflows.

  - **Team-level scoping.** Requests are intended to reach only the agency teams set up to work on that brand, using existing Workfront access controls.

# **Roadmap**

The phases below describe our current plan. Sequencing may change based on what we learn in the beta, and later phases are not commitments.

<table>
<tbody>
<tr class="odd">
<td><strong>Phase</strong></td>
<td><strong>Focus and planned capabilities</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>Phase 1</strong></td>
<td>Connect instances and kick off work: request forms, AI-assisted intake, mirrored requests, project conversion, comments, and status drafting.</td>
<td>In beta</td>
</tr>
<tr class="odd">
<td><strong>Phase 2</strong></td>
<td><ul>
<li><p>Review and approval using Frame and the unified review and approval experience</p></li>
<li><p>Pending reviews appear in Workfront or Frame, wherever the stakeholder works</p></li>
<li><p>Annotations stay tied to the working file so creative teams see feedback in one place</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="even">
<td><strong>Phase 3</strong></td>
<td><ul>
<li><p>Task-based work assignment in addition to requests</p></li>
<li><p>More automated status, informed by shared or unshared fields</p></li>
<li><p>A new deliverable object type, with metadata defined during briefing and inherited by the final approved asset</p></li>
<li><p>Direct delivery of approved final assets into the brand's AEM, reducing manual metadata entry</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="odd">
<td><strong>Phase 4</strong></td>
<td><ul>
<li><p>Shared context between brand and agency</p></li>
<li><p>Use of Adobe Brand Intelligence by the agency before review, with access controlled by team</p></li>
<li><p>Context-informed capabilities such as estimating</p></li>
</ul></td>
<td>Longer term</td>
</tr>
</tbody>
</table>

# **Participating in the beta**

## **What we ask of participants**

  - Join a weekly feedback call.

  - Set aside about one hour per week for hands-on testing. Live working sessions on the call are an option if time is tight.

  - Bring both the brand and the agency perspective where possible.

  - Identify the Workfront environments to connect, and provision admin accounts for a small number of Adobe engineers so they can validate the connection.

## **What we want to learn**

  - Is mirroring an object and syncing only selected data the right sharing model, and is it flexible enough for each side?

  - Is the phase sequencing right, or should a later capability come sooner?

  - What touchpoints are missing from the collaboration?

  - How should field naming and mapping work between brand and agency instances? Today, the form and request are owned by the brand, and the agency sees them read-only with the brand's field names.

  - What does IT need to approve and administer a connection?

The beta runs through the end of the year. For questions or blockers, contact your Adobe beta program manager.


-->