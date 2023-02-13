---
content-type: reference
product-area: projects
navigation-topic: convert-issues
title: 解析和可解析對象概述
description: 可解析對象是解析度與解析對象綁定的問題。 解決對象是項目、任務或其他問題。
author: Alina
feature: Work Management
exl-id: 2ff034ec-6116-42af-a55f-1fb24fc12b2f
source-git-commit: cd0adf2bd44a5c9f093e005b5af54b54ad019e34
workflow-type: tm+mt
source-wordcount: '1732'
ht-degree: 1%

---

# 解析和可解析對象概述

可解析對象是解析度與解析對象綁定的問題。 解決對象是項目、任務或其他問題。

將問題轉換為任務或項目時，該問題將成為任務或項目的可解析對象。

您也可以手動將問題連結至「解決物件」，這可以是任務、專案或問題。 如需詳細資訊，請參閱 [手動將問題的解決與其他問題、任務或專案關聯](../../../manage-work/issues/convert-issues/manually-tie-resolution-of-issue-to-ptis.md).

在此情境中，原始問題成為任務、項目或問題的可解析對象。

## 設定Adobe Workfront以處理可解析的對象 {#set-up-adobe-workfront-to-handle-resolvable-objects}

作為Workfront管理員或組管理員，您可以決定要如何處理系統或組中的可解析對象。

在將可解析對象轉換為任務或項目時，可以選擇保留該對象，或在建立任務或項目後將其刪除。 您可以選取允許在轉換問題的過程中變更這些設定，讓轉換問題的使用者可以選擇保留或刪除轉換問題時的問題。

>[!NOTE]
>
>可解析對象始終是問題，其解析度和狀態取決於與其關聯的解析對象的解析度和狀態。 解決對象可以是問題、任務或項目。

有關設定處理可解析對象的首選項的資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Note: drafted and just pointed the user to the article linked above)&nbsp;</p>
<p>To establish the system default for what happens to the issue as it is being converted to a task or a project:</p>
<ol>
<li value="1">Log in to Workfront as a Workfront administrator <span>or group administrator.</span></li>
<li value="2"> <p>  From the main menu, click <strong>Setup</strong>. </p> <p> <img src="assets/qs-main-menu-expanded-with-menu-highlight-350x521.png" style="width: 350;height: 521;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Expand <strong>Project Preferences</strong>.</li>
<li value="4">Click <strong>Tasks & Issues</strong>.</li>
<li value="5">Go to the <strong>Issues</strong> area of the setup.<br><img src="assets/qs-setup-project-preferences-issues-area-350x214.png" style="width: 350;height: 214;"><br>Consider editing any of the following settings:
<ul>
<li><p><strong>Automatically update Resolvable Issue status when the status of the Resolving Object changes:</strong> Select this option to tie the resolution of the original issue to the resolution of its Resolving Object. In order for this setting to have any effect, the options to <strong>Keep the original issue and tie its resolution to the task</strong> or<strong>project</strong> must be selected.</p>
<ul>
<li>When this setting is enabled, you can create custom statuses with the same key for both issues and projects or tasks. When the project or task (as a resolvable object) turns into the custom status, the change also reflects on the status of the issue. The status key must be the same for the issue and project or task statuses.</li>
<li><p>When this setting is disabled, resolving object statuses are automatically set to the default status, instead of the custom ones. For more information about the default statuses, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p><note type="note">
The default status of the issue is controlled by the status of the project or task, regardless of whether this option is selected or not.
</note></li>
</ul></li>
<li><strong>When converting an issue to a TASK...:</strong> The settings in this section determine what happens during the conversion process from issue to task:
<ul>
<li><strong>Keep the original issue and tie its resolution to the task:</strong> When converting the issue, it remains visible as an issue until the task is complete. The status of the issue automatically changes to Closed when the task completes.</li>
<li><strong>Allow Primary Contact to have access to the task:</strong> Gives the primary contact (issue creator) access to the task to review the task, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a task. </li>
</ul></li>
<li><strong>When converting an issue to a PROJECT...:</strong> The settings in this section determine what happens during the conversion process from issue to project:
<ul>
<li><strong>Keep the original issue and tie its resolution to the project:</strong> When converting the issue, it remains visible as an issue until the project is complete. The status of the issue automatically changes to Closed when the project completes.</li>
<li><strong>Allow Primary Contact to have access to the project:</strong> Gives the primary contact (issue creator) access to the project to review the project, make updates, and stay informed of its progress.</li>
<li><strong>Allow these settings to be changed during conversion:</strong> Allows the user who is converting the issue to change these options during the conversion of an issue to a project. </li>
</ul></li>
</ul></li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## 在轉換為項目或任務期間處理可解析對象

根據Workfront或組管理員配置系統或組級別問題首選項的方式，在將問題轉換為項目或任務期間，您可能可以處理可解析的對象。

存在下列情況：

* 如果Workfront或群組管理員 **保留原始問題，並將其解決方案與任務掛鈎** 和 **保留原始問題，並將其解決方案與項目掛鈎** 已選取， **允許在轉換期間變更這些設定** 取消選取「 」，您將無法變更這些設定，因為您將問題轉換為工作或專案。\
   ![](assets/qs-setup-project-preferences-issues-area-some-boxes-unselected-350x217.png)

* 如果Workfront或群組管理員 **保留原始問題，並將其解決方案與任務掛鈎** 和 **保留原始問題，並將其解決方案與項目掛鈎** 已選取或未選取，且 **允許在轉換期間變更這些設定** 若選取，您將可在將問題轉換為任務或專案時變更這些設定。\
   ![](assets/qs-options-to-keep-issue-when-coverting-it-inside-the-issue-350x113.png)

如需將問題轉換為工作和專案的詳細資訊，請參閱 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Tie the resolution of an issue to a project, task or </h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: created new article for this section; draft when the article is live and see if you need to make a link from this one to the new article) </p>
<div>
<p>You can manually tie the resolution of an issue to the resolution of a project, task, or issue without converting the issue. The issue becomes one of the Resolvable Objects of the project, task, or issue you select. When you do this, a change in the status of the project, task, or issue triggers a change in the status of the original issue, so you cannot manually edit the status of the original issue. <br>For more information about how the status of the Resolving Object affects the Resolvable Object, see <a href="#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object" class="MCXref xref">Synchronize the Status of the Resolvable Object with that of the Resolving Object</a>.</p>
<p>You must have Manage permissions on the original issue and View permissions on the project, task, or issue to do this. </p>
<p>To tie the resolution of an issue to the resolution of a project, task, or issue:</p>
<ol>
<li value="1">Navigate to an issue whose resolution you want to tie to a task or a project.</li>
<li value="2"> <p>  Click the <strong>Issue Details</strong> > <strong>Overview</strong> area. </p> <p> <img src="assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png" style="width: 350;height: 462;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> in the upper-right corner of the Issue Details section. </p> </li>
<li value="4">At the bottom of the form,  click in the <strong>Resolved By</strong> field,  and select from the following types of resolving objects:
<ul>
<li><strong>Project</strong></li>
<li><strong>Task</strong></li>
<li><p><strong>Issue</strong></p></li>
</ul><p>The field for the resolving object displays. </p></li>
<li value="5">After selecting the object, start typing the name of a specific project, task, or issue in the available field and select it when it appears in the drop-down list. </li>
<li value="6">Click <strong>Save</strong>&nbsp;<strong>Changes</strong>.<br>The original issue becomes the Resolvable Object for the project, task, or issue you selected in step 4 and 5.<br><note type="note">
One project, task, or issue may have multiple issues as Resolvable Objects.
</note></li>
</ol>
</div>
</div>
-->

## 將可解析對象的狀態與解析對象的狀態同步 {#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object}

* [當「解決對象」是問題時，同步狀態](#synchronize-statuses-when-the-resolving-object-is-an-issue)
* [當「解析對象」是任務或項目時同步狀態](#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project)

### 當「解決對象」是問題時，同步狀態 {#synchronize-statuses-when-the-resolving-object-is-an-issue}

如果問題手動與另一個問題系結，則第二個問題的狀態（解決物件）會觸發第一個問題的狀態（可解決物件）的變更。 第一個問題的狀態與第二個問題變更為的狀態相符。 這適用於預設和自訂問題狀態。

### 當「解析對象」是任務或項目時同步狀態 {#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project}

當問題是任務或項目的「可解析對象」時，任務和項目狀態的更改將觸發問題狀態的更改。 預設狀態的觸發方式與自訂狀態不同，在此案例中為。

* [將解析對象的預設狀態與可解析對象的預設狀態同步](#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object)
* [將解析對象的自定義狀態與可解析對象的自定義狀態同步](#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object)

#### 將解析對象的預設狀態與可解析對象的預設狀態同步 {#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object}

無論是否選擇「在解析對象的狀態更改時自動更新可解決的問題狀態」選項，每當解析對象（項目或任務）上的預設狀態更改時，可解決的對象（問題）的狀態就會相應地更改。 只有預設狀態已對應以觸發此類變更。

將問題設定為任務的解決對象時，任務的以下預設狀態將觸發問題的預設狀態中的以下更改：

| **任務狀態** | **問題狀態** |
|---|---|
| 新增 | 新增 |
| 進行中 | 進行中 |
| 已完成 | 已關閉 |

將問題設定為項目的「可解析對象」時，項目的以下預設狀態將觸發問題的預設狀態中的以下更改。 有些專案狀態不會觸發問題狀態的變更。 問題仍會維持在專案變成以下其中一個狀態之前的狀態：

| **專案狀態** | **問題狀態** |
|---|---|
| 計畫 | 新增 |
| 目前 | 進行中 |
| 保留 | 保留 |
| 已請求 | 不會觸發問題狀態的變更 |
| 已核准 | 不會觸發問題狀態的變更 |
| 已拒絕 | 不會觸發問題狀態的變更 |
| 構想 | 不會觸發問題狀態的變更 |
| 廢棄 | 已關閉 |
| 已完成 | 已關閉 |

>[!NOTE]
>
>問題的狀態變為「已結」（由於關閉任務或項目）後，無論任務或項目在關閉後更改為什麼狀態，問題都保持「已結」。

#### 將解析對象的自定義狀態與可解析對象的自定義狀態同步 {#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object}

將任務或項目的狀態更改為自定義狀態時，問題的狀態將更改為自定義問題狀態，只有在滿足以下兩個條件時：

* 選擇「在解決對象的狀態更改時自動更新可解決的問題狀態」選項。 如需如何啟用此設定的詳細資訊，請參閱 [設定Adobe Workfront以處理可解析的對象](#set-up-adobe-workfront-to-handle-resolvable-objects).

* 項目或任務的自定義狀態與問題的自定義狀態具有相同的三個字母代碼。

您可以針對問題和專案或工作，使用相同的鍵值建立自訂狀態。 當項目或任務（作為解決對象）更改為自定義狀態時，更改也會反映問題的狀態。 對於問題和項目或任務狀態，狀態鍵必須相同。

例如，建立名為「已啟動」的專案自訂狀態，並使用三個字母代碼「LCD」，相當於「目前」。 此外，建立名為「Project Launched」的問題自訂狀態，並加上字母代碼「LCD」，等於「In Progress」。 當您將專案標示為「已啟動」時，問題會自動將狀態變更為「已啟動專案」。 如果未啟用「Automatical****s set issue statusses to match the resolavable object using the Status keys（自動設定問題狀態以使用狀態鍵匹配可解析對象）」設定，則問題狀態將更改為「In Progress（正在進行）」（預設狀態）。

如需建立自訂狀態的詳細資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## 將解析對象的完成百分比與可解析對象的完成百分比同步

如果問題由任務或項目解決，則問題完成百分比會在發生下列任何情況時更新可解決的問題： 

* 當某人保存任務或項目的更改時。
* 系統會重新計算專案的時間軸。

如果和問題已由其他問題解決，當其中一個問題更新時，完成百分比就會更新。

## 在任務或項目上查找可解析對象

對於任務和項目，查找解析對象的位置相同。

1. 導航至您通過將問題轉換為項目或任務而建立的項目或任務。
1. 按一下 **專案詳細資料** 或 **任務詳細資訊** 圖示並按一下以展開。
1. 按一下 **概述**.
1. 在索引標籤底部，找到 **此解析** 欄位：此欄位中列出了項目或任務的可解析對象問題。

   >[!NOTE]
   >
   >問題無法轉換為其他問題，但可手動與「解決問題」建立關聯。 項目、任務或問題可以有多個問題作為可解析對象。 項目、任務或問題解決後，可解析對象（問題）也解決。 即使重新開啟已解決的項目、任務或問題，「可解決的問題」仍然處於關閉狀態。

## 識別清單中解決物件的問題

在問題清單中，您可以在 **狀態表徵圖** 或 **標幟** 欄：

![](assets/ro1.png)

## 在報表中查看可解析和可解析的對象資訊

您可以在項目、任務或問題的視圖或報告中顯示關於可解析對象或可解析對象的資訊。\
下表顯示您可以顯示哪些欄位，以及可顯示哪些檢視：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>視圖中的欄位</strong> </th> 
   <th><strong>問題檢視</strong> </th> 
   <th><strong>任務檢視</strong> </th> 
   <th><strong>專案檢視</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>有可解析項</strong>:顯示 <strong>True</strong> 值（如果項目或任務具有與它們關聯的可解決問題），以及 <strong>False</strong> 值。</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td><strong>原始發行名稱、原始發行錄入日期、創始人名稱</strong>:顯示原始問題的名稱和登入日期，以及在文字模式自訂檢視中建立問題的使用者名稱。<br>有關為項目或任務報告或清單建立文本模式自定義視圖以顯示有關原始問題的資訊的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md" class="MCXref xref">查看：顯示任務和項目清單的原始問題資訊</a>.<br></td> 
   <td> </td> 
   <td> ✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>應收賬款：</strong> 以文本模式為項目或任務報表或清單顯示所有可解析對象的自定義視圖清單。</p> <p>如需有關建立此檢視的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-resolvable-objects-task-project-report.md" class="MCXref xref">查看：任務或項目報表中的可解析對象</a></p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><strong>已轉換的發行創始者</strong>:顯示有關最初記錄問題（後來已轉換為任務）的用戶的資訊。 </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>解決專案</strong>:顯示有關已從原始問題轉換或手動指定為問題解決對象的解決項目的資訊。</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>解析任務</strong>:顯示有關「解決任務」的資訊，該任務是從原始問題轉換的，或手動指定為問題的「解決對象」。</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>解決問題</strong>:顯示有關「解決問題」的資訊，該資訊已手動指定為問題的「解決對象」。</td> 
   <td> ✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
