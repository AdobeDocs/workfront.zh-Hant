---
title: 設定記錄型別商業規則
description: 您可以設定記錄型別商業規則，以根據欄位值對記錄強制執行特定動作。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: cafe52c228520becb66e2fa9d8121127223a8f71
workflow-type: tm+mt
source-wordcount: '1094'
ht-degree: 1%

---


# 設定記錄型別商業規則

{{planning-important-intro}}

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 在「預覽」版發行後，啟用的客戶每月可在「生產」環境中使用相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

您可以為Adobe Workfront Planning記錄型別設定商業規則，以指示在允許或阻止對該型別記錄的動作之前，需要某些欄位。

根據規則的制定方式，如果符合定義的商業規則，您可以允許對記錄進行下列動作：

* 編輯或不編輯記錄
* 刪除或不刪除記錄

## 存取權要求

+++ 展開以檢視存取需求，以執行本文中的步驟：  

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
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe計畫授權</p></td> 
   <td><p>規劃標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>擁有Workflow和Planning套件時，您必須將Workflow和Planning授權型別新增到存取層級</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區和記錄型別的許可權</p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定商業規則時的注意事項

* 商業規則會將條件附加至欄位變更或記錄刪除。 規則只會在經過審慎考慮的特定時刻生效：當欄位即將變更為您在規則中設定的欄位值時。

* 規則以純文字顯示如下：「編輯此記錄之前，行銷活動摘要欄位必須具有值」。

  如果欄位為空，記錄編輯會被封鎖，使用者會收到明確訊息，說明在繼續編輯之前需要解決的事項。 一旦他們更新必填欄位並重試，就允許變更。

* 規則不會阻止記錄建立。 使用者仍然可以建立記錄，但他們必須確定必填欄位不是空白或包含指定值。
* 規則不會自動編輯或刪除記錄。 變更必須由使用者蓄意並觸發。
* 規則不回溯套用：舊記錄不受影響。 規則檢查只會在下次有人嘗試編輯或刪除記錄時執行。
* 您無法將商業規則新增至其主要或次要工作區中的全域記錄型別。
* 您可以為商業規則建立條件，該條件會參考以下欄位型別以外的所有欄位型別：
  * 公式欄位
  * 查詢欄位
  * 參考欄位
* 規則適用於可以編輯或刪除記錄的所有人。
* 記錄型別可以有多個商業規則。 <!--Syuzanna is checking this because it should be just ONE rule per action: one per edit and one per delete - see this: https://workfront.slack.com/archives/C0BHWEUSJCU/p1788281638322049?thread_ts=1787924876.280359&cid=C0BHWEUSJCU; I also logged a bug for this because it released with more than one per action - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/6a99add600001e9aa90435ec181dec3e/overview-->

  所有規則會同時檢查在一起。<!-- I have asked Syuzanna and Norayr multiple times HOW are the rules run/ prioritized and I got no answers; when I know, I will update here-->

## 設定商業規則

1. 移至記錄型別頁面。
1. 從任何檢視中，按一下記錄型別名稱右邊的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**商業規則**。

   「商業規則」表格頁面隨即開啟。
1. 按一下&#x200B;**新商業規則**。
1. 在&#x200B;**新企業**&#x200B;規則方塊中，在第一個可用欄位中為企業規則新增名稱。 這是必填欄位
1. （選用）新增說明以定義商業規則，然後按一下[儲存]。****

   「商業規則設定」表單隨即開啟。

   ![商業規則設定表單](assets/business-rule-setup-form.png)

1. 在商業規則設定表單的&#x200B;**If**&#x200B;區段中，根據特定規則選擇要限制或允許哪些動作。 從下列專案中選擇： <!--check UI text-->
   * **記錄編輯**：如果符合此規則中定義的條件，將允許使用者編輯或不編輯記錄。
   * **刪除記錄**：如果符合此規則中定義的條件，則允許使用者刪除或不刪除記錄。
     <!--add screen shot when UI text is final-->
1. 在&#x200B;**公式欄位**&#x200B;中，新增商業規則。 從右側面板的&#x200B;**公式運算式**&#x200B;區段中，為您的規則選擇一個運運算元。

   例如，您可以從&#x200B;**Other**&#x200B;欄位區段選擇&#x200B;**IF**，或開始輸入「IF」，然後在建議清單中顯示時按一下它。

   >[!TIP]
   >
   >建議您從建議清單中選取欄位和運運算元，以保持規則的語法正確。
1. 選擇您要設為強制性的欄位，以允許編輯或刪除此記錄型別的記錄。

   例如，您可以輸入下列陳述式，讓&#x200B;**行銷活動摘要**&#x200B;欄位成為必要欄位：

   ```
      IF(ISBLANK({Campaign summary}),"Campaign summary is a required field. You cannot edit this record without a value for the Campaign summary field.")
   ```

   >[!IMPORTANT]
   >
   >強烈建議您在規則公式中加入下列資訊，讓使用者更容易瞭解他們嘗試在記錄上執行的動作何時不適用：
   >
   >* 適用於設定規則的確切欄位。
   >* 不符合規則時的確切結果。

   當欄位或運算式錯誤時，**公式**&#x200B;欄位中有指標。 <!--add screen shot?-->

   在商業規則的&#x200B;**Then**&#x200B;區段中，您可以檢視規則功能的說明。

1. 按一下[啟動]****&#x200B;以啟用此記錄型別的規則，然後按一下[儲存]****。

   規則會在您啟動後立即套用，而所有有權編輯或刪除所選記錄型別中記錄的使用者都必須遵循這些規則。
1. （選用且建議使用）按一下頁首中&#x200B;**Business rules**&#x200B;左側的返回箭頭，以顯示記錄型別頁面，並移至表格檢視或開啟記錄頁面，然後嘗試編輯或刪除記錄，以測試您剛才建立的規則。

## 管理商業規則

您可以編輯、刪除或停用現有的商業規則。

編輯現有規則不會變更現有記錄。 編輯的規則僅適用於有人嘗試編輯或刪除現有記錄時。

1. 返回記錄型別的&#x200B;**商業規則**&#x200B;表格頁面。
1. 尋找您要變更的規則。
1. 將游標暫留在規則名稱上，然後按一下&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下下列其中一個選項：

   * **編輯**：這會開啟商業規則設定頁面，您可以編輯商業規則的相關資訊。
   * **停用**： <!--check this in the UI: right now, it says Disable-->這會停止規則觸發，但會保留以備將來使用。
   * **刪除**：已刪除規則的所有相關資訊。 已刪除的規則無法復原。

   已編輯的規則或規則的停用僅適用於未來的記錄，且不會回溯套用。

   <!--add NEW screen shot below if UI is fixed with Deactivate at release; it was fixed in devTest-->

   <!--![Business rule more menu expanded](assets/business-rule-more-menu-in-table-expanded.png)-->

<!--

***********FROM CLAUDE - BELOW - MUST EDIT*******************


### What business rules actually do

Business rules attach a condition to a **status change**. Instead of enforcing complete data the moment someone creates a record (which would slow everyone down), the rule only kicks in at one specific, deliberate moment: when a status is about to change to a status you've configured.

A rule looks like this in plain language:

> "Before a record can move to **Ready for Execution**, the field **Brand** must have a value."

If the field is empty, the status change is blocked and the person gets a clear message telling them what to fix. Once they fill it in and try again, the change goes through.

A few important things this is *not*:

* **It doesn't block record creation.** People can still create a new record instantly and fill it in over time, exactly like today. 
* **It doesn't auto-fill anything or auto-change statuses.** A person always has to make the status change themselves.
* **It doesn't retroactively flag old records.** Records that are already sitting in the target status aren't affected — the check only runs the next time someone tries to move a record *into* that status.

### Step 1: Open the business rules configuration area

Business rules live alongside your other admin setup — you won't need to hunt for a separate "Planning" panel. From your workflow setup area:

1. Go to the main **workflow setup / admin configuration** area for your workspace.
2. Look for the **business rules** section for the record type you want to configure (for example, "Materials" or "Campaigns").


### Step 2: Choose the record type

Rules are configured per record type, so pick the one you want to add a rule to. For example, if you want to make sure every Materials record has key fields filled in before execution, select **Materials**.

### Step 3: Create a new rule

For each rule, you'll specify three things:

| What you set | Example |
|---|---|
| **Record type** | Materials |
| **Target status** | Ready for Execution |
| **Required field** | Brand |

In other words: "When a Materials record's status is changed to **Ready for Execution**, the field **Brand** must have a value."

You can add more than one rule for the same status. For example, you might require Brand, Therapeutic Area, Indication, and Estimated Launch Date all to be filled in before a record can move to "Ready for Execution" — each is its own rule, and all of them are checked together.

**What fields can you require?**

* Connected record fields (e.g., a linked Brand or Indication record) — the rule passes as soon as at least one record is linked.
* Standard text fields (single-line or paragraph) — the rule passes once there's any value.
* Date fields — the rule passes once a date is set.

**What you can't use yet:** formula fields and lookup fields aren't supported as rule targets in this release, since they're calculated in the background rather than filled in directly by a person.

### Step 4: Write the message people will see

When you create a rule, you'll also provide the message that shows up if someone tries to make the change without the field filled in. Keep it specific and actionable — something like:

> "Brand is required."

You don't need to worry about formatting a whole error banner — the system handles combining messages if multiple rules are violated at once (see below).

### Step 5: Save the rule

Once saved, the rule takes effect **immediately** for everyone in the workspace — no need to log out, refresh, or wait for a deployment. The very next time anyone tries to move a record into that status, the rule is checked.

### What your team will actually experience

Here's what changes for the people using Planning day to day, once a rule is live.

#### If a required field is empty

1. A planner opens a record and changes the status to the gated status (say, "Ready for Execution").
2. The system checks all rules tied to that status.
3. If a required field is empty, the change is **rejected** — the status reverts back to what it was.
4. A toast message appears, naming exactly which field(s) are missing:
   > *"Status change blocked: 'Brand' and 'Estimated Launch Date' must be populated before moving to 'Ready for Execution.'"*
5. The planner fills in the missing field(s) and tries the status change again.
6. This time, the rule passes, and the status updates normally.

#### If everything is already filled in

Nothing changes. The status updates instantly, with no extra steps or popups. Business rules are invisible until they're actually needed.

#### If several fields are missing at once

All the violated rules are checked together, and the message lists every missing field in one go — planners don't have to fix one field, try again, get told about the next one, and repeat.

### Step 6: Edit or remove a rule later

Rules aren't set in stone. To make changes:

1. Go back to the business rules configuration area for the record type.
2. Find the rule you want to change.
3. Edit the required field, target status, or message — or delete the rule entirely.
4. Save. The change applies immediately to future status changes.

Keep in mind: editing or deleting a rule **only affects transitions going forward.** Records that already made it into the target status before the change aren't reevaluated.
3## A few things worth knowing

* **This is separate from locking records after a status change.** Business rules (as described here) only check field completeness *before* a status change goes through. A different, related feature governs whether a record becomes fully locked from edits/deletion once it reaches a certain status — that's not what's covered here.
* **Bulk status changes** (changing status on many records at once) aren't fully defined yet for how they interact with business rules — if your team relies heavily on bulk actions, check with your Adobe contact on current behavior.
* **If a rule can't be evaluated** due to a system error, the transition is blocked rather than silently allowed through — you'll never end up with an incomplete record slipping past a rule because of a backend hiccup.
* **Turning the feature off** doesn't delete your configured rules — they're just paused. Turning it back on restores them exactly as they were, no reconfiguration needed.

### Quick reference: setting up your first rule

1. Confirm the feature is enabled for your tenant.
2. Go to workflow setup → business rules for your record type.
3. Choose the record type (e.g., Materials).
4. Create a rule: target status + required field.
5. Write a clear, specific error message.
6. Save — it's live immediately.
7. Repeat for each field you want to require.
8. Test it yourself: try changing a record's status with the field empty, confirm you see the expected message, fill in the field, and confirm the status change now goes through.

That's it — from here on, anyone converting a record forward will get a clear nudge if something's missing, instead of a downstream project quietly showing up incomplete.

-->