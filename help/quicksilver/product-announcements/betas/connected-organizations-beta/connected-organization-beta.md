---
product-area: betas
title: 連線組織功能Beta計畫
description:
author: Alina
feature: Product Announcements
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 8f8f4e7962bfde525470842caecd49f03b758b29
workflow-type: tm+mt
source-wordcount: '2241'
ht-degree: 1%
---
# 連線組織功能測試版計畫

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

## 端對端工作流程

本節說明參與此整合之雙方的工作流程。

我們以使用者端及提供者工作流程為例。

工作流程包含下列步驟：

1. [建立執行個體連線](#1-create-an-instance-connection)
1. [認可連線](#2-acknowledge-the-connection)
1. [與連線的組織共用請求表單](#3-share-a-request-form-with-the-connected-organization)
1. [提交請求](#4-submit-a-request)
1. [檢閱請求並建立專案](#5-review-the-request-and-create-a-project)
1. [在跨公司交談中共同作業](#6-collaborate-in-the-cross-company-conversation)

### 開始之前

* 您必須是系統管理員，才能完整存取兩個執行個體中的&#x200B;**安裝程式**&#x200B;區域。
* 請求執行個體需要接收執行個體的唯一客戶&#x200B;**GUID**。
* 必須發佈您要共用的表單。

### &#x200B;1. 建立執行個體連線

在請求的執行個體（使用者端）中設定下列專案：

1. 登入使用者端的環境，然後前往&#x200B;**設定** > **執行個體連線**。 此頁面列出所有連線，如果還沒有連線，則為空白。
1. 按一下&#x200B;**建立連線**。
1. 在&#x200B;**建立連線**&#x200B;方塊中，新增&#x200B;**接收執行個體GUID**。 這是必填欄位。
1. （選擇性）設定&#x200B;**到期日**。 連線在此日期之後停止運作。
1. 按一下&#x200B;**建立連線**。

   新連線會顯示在狀態為&#x200B;**擱置中**&#x200B;的連線清單中。
1. 選取新連線以檢視其詳細資料。

   >[!TIP]
   >
   >擱置中的連線不共用任何內容。 接收執行個體必須先確認它。


### &#x200B;2. 認可連線

在接收執行環境（提供者）中設定下列專案：

1. 登入提供者的執行個體並移至&#x200B;**主要功能表** > **安裝程式** > **執行個體連線**。
1. 按一下名稱以開啟來自接收執行個體的連線。 橫幅會顯示下列訊息： **執行個體想要連線到您的執行個體。 請至少選擇一個符合資格的收件者，然後確認連線。 在您執行之前，不會共用任何專案。**
1. 在&#x200B;**合格收件者**&#x200B;底下，開啟&#x200B;**搜尋群組和使用者**&#x200B;清單，並選擇可從請求執行個體接收工作的使用者。 您可以挑選群組和個別使用者。<!--asking Anna K if this should be teams and users, instead of groups; it's groups in the UI-->
1. 按一下&#x200B;**認可**&#x200B;接受連線，或按一下下列其中一項：

   * **拒絕**&#x200B;以拒絕連線。
   * **關閉**&#x200B;以保留擱置中。

   出現「已儲存變更」訊息，且連線狀態變更為&#x200B;**作用中**。 清單現在會顯示合格的收件者、建立日期和到期日。

   >[!TIP]
   >
   >**認可**&#x200B;在您選擇至少一個符合資格的收件者之前，會保持暗灰色。

### &#x200B;3. 分享請求組織的請求表單

從使用者端的Workfront執行個體：

1. 移至&#x200B;**主功能表** > **要求**，然後按一下&#x200B;**要求表單**。
1. 開啟您要共用的已發佈表單。
1. 按一下&#x200B;**共用**。

   請注意&#x200B;**共用**&#x200B;方塊內的下列標籤：

   * **內部共用**
   * **公開共用**
   * **連線的組織**
1. 開啟&#x200B;**連線的組織**&#x200B;標籤。
1. 在&#x200B;**組織**&#x200B;欄位中，選取連線提供者的執行個體。
1. 在&#x200B;**使用者和群組**&#x200B;欄位中，選擇該組織中可以使用表單的使用者。 新增使用者和群組。
1. 按一下「**儲存**」。

**您的變更已成功儲存**&#x200B;訊息確認共用。<!--need to submit a UI text change - remove "successfully"-->

### &#x200B;4. 提交請求

以使用者端例項中的使用者身分，執行下列操作提交請求：

1. 登入使用者端的Workfront執行個體，然後前往&#x200B;**主功能表** > **要求**。

   **提交新請求**&#x200B;頁面會列出最近的表單，包括您剛共用的表單。

   頂端的附註會顯示&#x200B;**跨公司請求：透過此表單提交的請求對連線的組織可見。**
1. 手動填寫表單，或使用&#x200B;**填寫表單**&#x200B;讓AI為您執行。
1. （可選）若要使用「填色」表單，請執行下列動作：

   1. 按一下&#x200B;**填寫表單**。
   1. 描述您的要求、貼上相關電子郵件，或按一下&#x200B;**附加檔案**&#x200B;以上傳檔案。 AI會尋找相關詳細資料，並將其套用至表單。
   1. 按一下&#x200B;**套用至表單**。 產生欄位值時，進度列顯示&#x200B;**正在填寫您的表單**。
   1. 若要略過AI步驟，請按一下&#x200B;**略過**。
1. 檢閱產生的值，並編輯任何需要變更的專案。
1. 按一下&#x200B;**提交**&#x200B;以提交要求。

   已成功提交的&#x200B;**要求**&#x200B;訊息會顯示有&#x200B;**檢視您的要求**&#x200B;連結。

   新要求已新增到要求清單中，使用者端及提供者的執行個體上的表單名稱和&#x200B;**New**&#x200B;狀態皆為。

   >[!TIP]
   >
   >AI回應可能不準確。 提交前，請務必仔細檢查填入的值。

   建立的請求在提供者的執行個體上是唯讀的。

### &#x200B;5. 檢閱請求並建立專案

1. 登入提供者的Workfront執行個體並移至&#x200B;**主要功能表** > **要求**。

傳入的請求會顯示在清單中。

請求的&#x200B;**Type**&#x200B;已標示為&#x200B;**外部： &lt;使用者端執行個體的名稱>**，這會將其標示為來自連線的組織。

1. 開啟請求。 標題旁會顯示&#x200B;**共用對象： &lt;使用者端執行個體的名稱>**&#x200B;徽章，而註解面板會顯示下列&#x200B;**跨公司交談**&#x200B;通知： **此討論會對&lt;使用者端組織的名稱>.**&#x200B;可見
1. 檢閱請求資訊和表單答案。
1. 按一下要求名稱右側的&#x200B;**更多**&#x200B;功能表，然後&#x200B;**建立物件**。
1. 在&#x200B;**建立物件**&#x200B;對話方塊中，更新下列欄位：
   * **動作**：從功能表選取動作。 例如，**建立單一專案**
   * **專案範本**：選取可用的範本。
   * **專案所有者**：新增專案所有者。
   * **模組**：選擇顯示物件的產品。 如果您選擇&#x200B;**工作流程**，則會在Workfront的提供者執行個體中建立專案。
   * **自訂表單**：如有需要，請附加自訂表單。
   * **Portfolio**&#x200B;和&#x200B;**方案**：新增新專案的投資組合或方案。
1. 按一下「**建立**」。

   提供者執行個體中的要求現在連結到新專案，而且如果專案處於[目前]狀態，要求的狀態會變更為&#x200B;**進行中**。 使用者端的請求執行個體會在自己的請求副本上看到狀態變更。

### &#x200B;6. 在跨公司交談中共同作業

兩個組織中的使用者都可以評論其個別請求。 **跨公司交談**&#x200B;橫幅提醒您，其他組織可以看見此處所寫的所有內容。

執行下列其中一項：

1. 若要從使用者端執行個體要求更新：

   1. 開啟要求並移至&#x200B;**註解**&#x200B;面板。
   1. 按一下&#x200B;**新註解**，輸入您的訊息，然後按一下&#x200B;**提交**。

1. 若要更新來自提供者執行個體的要求：

   1. 開啟請求。 新註解會以&#x200B;**新**&#x200B;標籤強調顯示。
   1. 按一下&#x200B;**回覆**，撰寫回覆，然後按一下&#x200B;**提交**。

1. 若要從使用者端執行個體進行後續追蹤：

   1. 開啟請求。 提供者的回覆會顯示在原始註解下方。
   1. 按一下&#x200B;**贊**&#x200B;以認可它，或按一下&#x200B;**新增回覆**&#x200B;以繼續討論。




<!--
### Client's workflow

As a requestor in the client's organization, you can do the following:  

1. Create or ask an administrator to create a request form, publish it, and share it with the connected provider's organization.

2. Open the published form from the Requests area, enter a prompt, and attach any files.

3. Review how the content maps to the form fields, accept, and submit.

### Provider's workflow

As a work manager in the provider's organization, do the following: 

1. Receive the request in your Requests area as a read-only copy.

2. Discuss the request through comments until both sides are aligned, then accept it.

3. Convert the request into a project, choosing the portfolio, program, and template, if needed.

4. Choose which project fields are mirrored back to the client's request. 

5. Answer status questions in comments, or generate a draft status update, review it, and publish to your request. It will also display on the client's original request. 

    From that point on, the request on the provider's side acts as a replica of the client's original request, so comments and agreed-upon data stay in sync.
-->

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