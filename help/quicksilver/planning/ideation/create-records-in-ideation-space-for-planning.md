---
title: 從創意空間摘要建立計畫記錄
description: 使用Adobe Workfront Planning的新功能Ideation Space，您可以將簡報轉換為Planning記錄。 匯出的摘要會建立新記錄或更新現有記錄。 本文說明如何使用Ideation空間建立或編輯現有Planning記錄。
role: User, Admin
author: Alina
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 0%

---


# 從創意空間摘要建立Planning記錄

<!--
Will this release JUST to preview? If not - hide the preview portion below
-->

<!--
I started with this under Records first but what if Ideation will be added to other products and it will generate record types in those products? keep it here so it can be moved, if needed, to a standalone product one day?
-->

<!--
*********************** IMPORTANT ***************
THIS ARTICLE HAS 2 DRAFTS IN 2 SEPARATE AREAS FROM CLAUDE - THEY WERE CREATED AT DIFFERENT TIMES - WHICH ONE WOULD YOU KEEP OR MERGE THEM INTO ONE ARTICLE
-->

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它只能做為&#x200B;**創意空間Beta**&#x200B;程式的一部分。</span>

<span class="preview">如需詳細資訊，請參閱[開始使用Adobe Workfront Planning的構思空間](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)。</span>

{{planning-important-intro}}

使用Adobe Workfront Planning的新功能Ideation Space，您可以將簡報轉換為Planning記錄。 匯出的摘要會建立新記錄或更新現有記錄。

本文說明如何使用Ideation空間建立或編輯現有Planning記錄。

## 存取權要求

+++ 展開以檢視本文中功能的存取需求。 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<ul> 
<li><p>具有Planning套件的任何Workfront或工作流程</p></li>
或
<li><p>以獨立產品形式購買時的任何Planning套件</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>其他產品</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe工作流程授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe計畫授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> 
   <ul>
   <li><p>擁有Workflow和Planning套件時，您必須將Workflow和Planning授權型別新增到存取層級</p>   </li>
   <li><p>必須取消選取存取層級中的停用創意空間設定</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p>提供或更高許可權給您要新增記錄的工作區和記錄型別 </p>
      <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
      <p>檢視Workfront物件的許可權，以將它們新增至摘要 <!--not sure if this is available--></p>
      <p>創意力空間的編輯器許可權以建立簡報</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing使用者角色</p></td> 
   <td><p><ul><li>存取行銷活動、產品和角色的任何GenStudio使用者角色</li>
   <li>用於存取啟用的GenStudio系統管理員 <!--and Events--></li></ul>
   如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">使用者角色和許可權</a>。 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++  

## 使用創意力空間建立記錄的相關考量事項

* 在建立或編輯記錄時，您只能從Workfront Planning啟動創意力空間。 Workfront Planning之外沒有創意力空間。
* 若要存取創意力空間，您必須在Workfront Planning中擁有工作區和記錄型別。
* 新記錄一律以預留位置內容開始，無論您如何建立它們。
* 當您刪除連結至創意力簡述的Planning記錄時，簡述會保留在創意力空間中，且創意力空間中的相關畫布不會被刪除。
* 同步資訊只會從創意空間到Workfront Planning。 從Planning記錄到Ideation space brief沒有反向同步或自動同步。
* 在Workfront Planning中建立、編輯或移除欄位時，會發生下列情況：

  * 連結至創意力簡報的記錄所建立的新欄位，每天都會新增至簡報。 新欄位在創意力簡報中顯示為空白。
  * 移除的欄位會保留在摘要中並保留其先前的值。
  * 重新命名欄位會更新摘要中的名稱。
* 您可以將檔案新增為創意空間中的卡片。 這也包括影像。

  支援的檔案型別如下：PDF、Excel、CSV、PNG （和其他影像格式）、Word、PowerPoint。 不支援影片。

  所有上傳的檔案都會在後端轉換為PDF以供處理。
* 您可以直接將記錄從Workfront Planning拖放至空間，其顯示方式與手動上傳檔案相同。

## 使用創意力空間建立記錄

1. 在Workfront Planning登陸頁面中，按一下您可管理之工作區的卡片。
1. 按一下可新增記錄的記錄型別卡片。
1. 執行下列任一項作業來建立記錄：

   * 從任何記錄型別頁面的檢視，按一下頁面右上角的&#x200B;**新增記錄**，並在&#x200B;**選擇新增記錄的方式**&#x200B;方塊中，按一下&#x200B;**開啟創意空間**，然後按一下&#x200B;**繼續**。
   * 捲動到記錄表底部，按一下&#x200B;**新增列**，然後按一下&#x200B;**開啟創意空間**。

     >[!TIP]
     >
     >選取&#x200B;**不要顯示**&#x200B;會永久關閉未來的提示。 按一下「關閉」圖示&#x200B;**X**&#x200B;可關閉此方塊，但下次您新增內嵌記錄時，它將會重新出現。

   ![具有開啟創意空間按鈕的新記錄方塊](assets/new-record-creation-picker-with-ideation.png)

   創意力空間會在新標籤中開啟，並帶有空白提示。

   記錄會立即以預留位置文字建立。

1. （選擇性）按一下提示方塊中的&#x200B;**使用現有的簡介**，以瀏覽並新增現有檔案，創意空間將用來建立簡介和未來記錄。

   ![空的創意力簡短提示](assets/empty-ideation-prompt.png)

1. （選擇性）按一下提示方塊右上角的&#x200B;**開啟先前的畫布** <!--accurate??-->圖示![開啟現有的簡介圖示](assets/open-existing-briefs-icon.png)以開啟現有的簡介

1. 在&#x200B;**您正在處理什麼工作？** 提示方塊，說明您要建立哪種記錄。

   您分享的詳細資訊越多，構思空間提供的資訊就越有用。 例如，輸入您計畫之行銷活動的說明：「返回行銷機構的學校行銷活動」。

1. 按一下&#x200B;**開始構思**。

   創意空間在建立您的創意時會透過下列步驟運作： <!--check some of these in the UI - there might have been UI text changes-->

   1. 瞭解您的目標與內容
   2. 檢閱您的分享空間與選取的材料
   3. 從檔案、網頁和資料收集證據
   4. 將發現綜合成研究摘要
   5. 建立和調整包含引文的卡片

   在此過程中，您會看到Ideation Space主動搜尋已連線的Workfront Planning資料或網頁上可用的資訊。

   例如，它可能會搜尋現有的計畫、產品、角色或區域，以及線上提供的類似概念。<!--check on this with Et-->

   構思完成後，下列專案會新增至構思空間：

   * AI結果的摘要，已連結至數張卡片，其中包含有關要考慮的事項的詳細資訊。 詳細資訊卡會顯示在新的區段中。 聯結器會指出哪個卡區段屬於哪個摘要。

   * 位於創意力空間左下角的&#x200B;**Brief**&#x200B;檔案。 摘要是未來記錄的草稿，會顯示為記錄的「詳細資訊」頁面。

   ![含分支的創意力卡](assets/ideation-card-with-branched-off-additional-cards.png)

1. 繼續將資訊新增至創意力空間，以完成建立您的簡報。

1. （視條件而定）簡介完成時，請按一下左下角的預覽影像，然後按一下下列其中一項：

   * **匯出至檔案**&#x200B;以建立檔案
   * **匯出至Workfront Planning**&#x200B;以建立Planning記錄

   如需有關新增專案到簡介並匯出的資訊，請參閱[在構思空間建立簡介](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)。

   這樣會使用其他資訊完成記錄的建立，並將其新增到您最初選取的記錄型別。

## 編輯創意力空間中的現有記錄

您可以從現有記錄中開啟創意空間以更新它們。

您無法大量編輯創意空間中的記錄。

1. 前往Workfront Planning中的現有記錄，並開啟其詳細資訊頁面。

1. 按一下&#x200B;**在創意力空間**&#x200B;中開啟。 這會在新標籤中開啟「構思」空間。

   如果記錄的構思已存在，則會開啟該空間。

   如果沒有創意力存在，則會建立創意力空間與摘要。

   >[!TIP]
   >
   >無法使用創意力空間大量編輯記錄。

   <!-- 
    I don't think these steps are still valid but the environment was not available to test: 
    - If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
    - If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.
    -->

1. 繼續編輯簡報，如本文中[使用創意空間](#create-records-using-the-ideation-space)建立記錄一節中所述。






<!-- this is from Claude, but rephrased and included most of this above: 

## Step 5: Open the Workfront Planning Records panel

To bring real Workfront Planning records into your canvas (rather than just AI-generated ideas), click the **records icon** in the left-hand toolbar (third icon down). This opens the **Workfront Planning Records** panel, listing all **Connected Record types** available in your Planning environment — for example:

- Products
- Regions
- Personas
- Channels
- Activations
- Project
- Test Record
- Experience Manager Assets

## Step 6: Drag real records onto the canvas

Search or browse within a record type (e.g., **Products** or **Personas**), then drag the record you want directly onto the canvas. In the example, an existing **Nike product** record and a **Deep testing** persona record were both dragged in and positioned near the relevant concept cards.

This lets you visually connect your AI-generated ideas to the actual records that already exist in Workfront Planning, grounding the ideation in real data rather than hypothetical entities.


![Dragging a persona record onto the canvas](images/05_drag_persona_record.png)

---

## Step 7: Refine with follow-up prompts

Use the **Ask anything** box in the bottom-right corner at any time to refine the canvas — for example, typing `regenerate` against a specific card to have Catalyze redo that section using updated context. Catalyze will re-run its reasoning steps (searching, synthesizing, citing) and update the affected cards in place.

---

## Step 8: Review the full canvas

Zoom out to see the complete picture: your original campaign goal, all AI-generated concept cards with citations, the real Workfront Planning records you've pulled in (Products, Personas, etc.), and a **Campaign Brief** summary card in the corner pulling it all together.



![Full canvas overview](images/06_full_canvas_overview.png)

---

## Tips

- **Be specific in Step 2** — richer campaign descriptions produce more relevant, better-grounded cards.
- **Check citations** before trusting a generated fact — click **Sources** on any card.
- **Mix AI cards with real records** — dragging in actual Products, Personas, Regions, etc. keeps the canvas tied to your real Planning data, not just AI speculation.
- Responses are AI-generated and may be inaccurate — always verify against the linked sources before finalizing a record.

***************SECOND DRAFT FROM CLAUDE*******************
# Creating and Managing Records with Catalyze Ideation

> This workflow reflects the Closed Beta experience and is expected to evolve before Open Beta and GA. Confirm current behavior before publishing to customers.

This guide explains how to create and ideate on records using Catalyze within Workfront Planning. It covers all entry points, system behavior, data sync rules, and file-upload support.

## Before you start

- You must have access to a record list within Workfront Planning.
- Catalyze always opens in a **new browser tab** — this is consistent across every entry point.
- Any record created through Catalyze starts with **placeholder text** until you begin ideating.

## Option 1: Create a record via the top-level "New Record" button

1. Navigate to your record list in Workfront Planning.
2. Click the **New Record** button at the top of the page.
3. From the dropdown menu, select **Ideate in Catalyze**.
4. A new browser tab opens automatically, launching the Catalyze canvas.
5. A new record is created in Workfront Planning with placeholder text.
6. Begin ideation directly in Catalyze.

**Additional access from the record view:** Open the newly created record and, in its detail modal, click **Ideate in Catalyze**. This opens Catalyze in a new tab (same behavior as above).

## Option 2: Create a record via inline record creation (bottom of table)

1. Scroll to the bottom of the record table.
2. Click **New Record**.
3. The record is created immediately with placeholder text.
4. A pop-up appears with these options:
   - **Open Catalyze** — launches Catalyze in a new browser tab
   - **Don't Show Again** — permanently dismisses the future prompt
   - **X (Close)** — closes the pop-up; it will reappear next time
5. Click **Open Catalyze** to begin ideation.

## Working with existing records

**Contextual actions (bottom selection bar)**
- **Single record selected:** an "Ideate in Canvas" / "Open in Canvas" action appears.
  - If a canvas already exists, it opens that canvas.
  - If no canvas exists, it creates a new one.
- **Multiple records selected:** the Ideate/Open in Canvas action is **not available** — bulk ideation is not supported.

**Record detail panel**
- If no canvas is connected, an **Ideate in Catalyze** button appears in the record header.
- If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
- If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.

**When can you create a canvas for a record?**
A canvas can be created for a record that is in Workfront Planning and still in **draft** state (not yet marked "ready").

## Record deletion behavior

If a Planning record linked to a Catalyze canvas is deleted:
- The canvas remains intact in Catalyze.
- No data is removed from Catalyze.

## Data synchronization rules

**Sync direction:** One-way only, from Catalyze → Workfront Planning. There is no reverse or automatic sync from Planning back to Catalyze.

**Export process:**
1. In Catalyze, click **Export to Planning**.
2. Data is pushed to the connected Workfront Planning record.
3. The export **overwrites all existing field data** in the record.

**Important notes:**
- Changes made directly in Workfront Planning do **not** sync back to Catalyze.
- Data refresh in Workfront Planning is manual only (Beta behavior) — there is no scheduled/automatic sync.
- Schema updates do sync one direction: once connected, Planning schema changes propagate to Catalyze daily — added fields appear empty, removed fields keep their prior values, and renamed fields update in place.

## Uploading documents into the Catalyze canvas

- Files can be added as a "document card" on the canvas — this works the same whether the file is an image or another document type.
- You can drag and drop files directly from Workfront Planning onto the canvas, and they appear the same way as manually uploaded files.
- All uploaded documents are converted to PDF on the backend for processing.
- Supported file types (as of the Aug 2026 beta): **PDF, Excel, CSV, PNG (and likely other image formats), Word, PowerPoint.**
- **Not supported:** video files.
- You can include images directly in a prompt and Catalyze will recognize their content, though small-format legibility is still being refined.

## Key takeaways

- Use **Ideate in Catalyze** to connect records to the AI-assisted ideation workflow.
- Catalyze always launches in a separate browser tab.
- New records always start with placeholder content, regardless of entry point.
- Data flow between Catalyze and Planning is manual and one-directional (Catalyze → Planning).
- Deleting a Planning record does not delete its associated Catalyze canvas.

-->


<!--
Internal info: 

## The Ideation space and Adobe GenStudio

Adobe GenStudio for Performance Marketing is Adobe's end-to-end content supply chain solution, spanning five stages:

1. Strategy and Ideation
2. Workflow and Planning
3. Asset Management
4. Creation and Production
5. Delivery and Activation

The Ideation space fits in the **Strategy and Ideation** stage — the front door of the content supply chain — and is designed to work natively with the rest of GenStudio, so the briefs and strategic direction it generates flow directly into Workfront Planning for execution.
-->


