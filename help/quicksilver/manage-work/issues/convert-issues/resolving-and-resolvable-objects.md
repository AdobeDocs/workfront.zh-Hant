---
content-type: reference
product-area: projects
navigation-topic: convert-issues
title: 解析與可解析物件的概觀
description: 可解析物件是其解析繫結至解析物件的問題。 解決物件是專案、任務或其他問題。
author: Alina
feature: Work Management
exl-id: 2ff034ec-6116-42af-a55f-1fb24fc12b2f
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1760'
ht-degree: 1%

---

# 解析與可解析物件的概觀

<!-- Audited: 08/2025 -->

可解析物件是其解析繫結至解析物件的問題。 解決物件是專案、任務或其他問題。

將問題轉換為任務或專案時，問題會成為任務或專案的可解析物件。

您也可以手動將問題連結至解決物件，可以是任務、專案或問題。 如需詳細資訊，請參閱[手動將問題的解決連結到其他問題、任務或專案](../../../manage-work/issues/convert-issues/manually-tie-resolution-of-issue-to-ptis.md)。

在此案例中，原始問題會成為任務、專案或問題的可解析物件。

## 設定Adobe Workfront以處理可解析物件 {#set-up-adobe-workfront-to-handle-resolvable-objects}

身為Workfront管理員或群組管理員，您可以決定如何處理系統中或群組的可解析物件。

您可以選取在將「可解析物件」轉換為任務或專案時將其保留，或在任務或專案建立後將其刪除。 您可以選擇允許在轉換問題的過程中變更這些設定，這可讓轉換問題的使用者在轉換問題時選擇是保留還是刪除問題。

>[!NOTE]
>
>可解析物件永遠是問題，其解析度和狀態取決於與其關聯的解析物件的解析度和狀態。 解析物件可以是問題、任務或專案。

如需設定處理可解析物件的偏好設定的相關資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

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

## 在轉換為專案或任務期間處理可解析物件

根據Workfront或群組管理員設定系統或群組層級問題偏好設定的方式，您或許可以在問題轉換為專案或任務期間處理可解析物件。

存在下列情況：

* 如果Workfront或群組管理員擁有「保留原始問題，並將其解決方案連結至任務」和「保留原始問題，並將其解決方案連結至選取的專案」，且未選取「允許在轉換期間變更這些設定」，則您將問題轉換為任務或專案時無法變更這些設定。\
  ![專案偏好設定問題區域](assets/qs-setup-project-preferences-issues-area-some-boxes-unselected-350x217.png)

* 如果Workfront或群組管理員擁有「保留原始問題，並將其解決方案連結至任務」和「保留原始問題，並將其解決方案連結至專案」（選取或未選取），以及「允許在轉換期間變更這些設定」選項，則當您將問題轉換為任務或專案時，您將能夠變更這些設定。\
  ![保留問題的選項](assets/qs-options-to-keep-issue-when-coverting-it-inside-the-issue-350x113.png)

如需將問題轉換為任務和專案的詳細資訊，請參閱[在Adobe Workfront中轉換問題的總覽](../../../manage-work/issues/convert-issues/convert-issues.md)。

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
<li value="2"> <p>  Click the <strong>Issue Details</strong> > <strong>Overview</strong> area. </p>  </li>
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

## 將可解析物件的狀態與解析物件的狀態同步 {#synchronize-the-status-of-the-resolvable-object-with-that-of-the-resolving-object}

* 當解析物件為問題時[同步狀態](#synchronize-statuses-when-the-resolving-object-is-an-issue)
* [當解析物件是任務或專案時同步狀態](#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project)

### 當解析物件為問題時同步狀態 {#synchronize-statuses-when-the-resolving-object-is-an-issue}

當問題手動繫結到另一個問題時，第二個問題（解決物件）的狀態會觸發第一個問題（可解決物件）的狀態變更。 第一個問題的狀態與第二個問題的變更目標狀態相符。 這適用於預設和自訂問題狀態。

### 當解析物件是任務或專案時同步狀態 {#synchronize-statuses-when-the-resolving-object-is-a-task-or-a-project}

當問題為任務或專案的可解析物件時，任務狀態的變更和專案會觸發問題狀態的變更。 在此案例中，預設狀態的觸發方式與自訂狀態不同。

當專案的自訂狀態等於未觸發問題狀態變更的預設狀態時，專案狀態的變更未觸發問題的狀態變更。

* [將解析物件的預設狀態與可解析物件的預設狀態同步](#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object)
* [將解析物件的自訂狀態與可解析物件的自訂狀態同步](#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object)

#### 將解析物件的預設狀態與可解析物件的預設狀態同步 {#synchronize-the-default-status-of-the-resolving-object-with-the-default-status-of-the-resolvable-object}

無論「解析物件狀態變更」選項是否選取「自動更新可解析問題」狀態時，每次解析物件（專案或任務）上的預設狀態變更時，可解析物件（問題）的狀態都會隨之變更。 只有預設狀態才能對應以觸發此類變更。

當問題設定為任務的解析物件時，以下預設任務狀態會觸發預設問題狀態的以下變更：

| **任務狀態** | **問題狀態** |
|---|---|
| 新增 | 新增 |
| 進行中 | 進行中 |
| 完成 | 已關閉 |

將問題設為專案的可解析物件時，下列預設專案狀態會觸發預設問題狀態的下列變更。 某些專案狀態不會觸發問題狀態的變更。 問題仍維持在專案變為以下狀態之一之前的狀態：

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
>在問題狀態變成「已關閉」（由於關閉任務或專案）後，無論任務或專案狀態在關閉後變更為何，問題仍為「已關閉」。

#### 將解析物件的自訂狀態與可解析物件的自訂狀態同步 {#synchronize-the-custom-status-of-the-resolving-object-with-the-custom-status-of-the-resolvable-object}

當您將任務或專案的狀態變更為自訂狀態時，問題狀態只有在滿足以下2個條件時才會變更為自訂問題狀態：

* 當已選取解析物件狀態變更選項時，自動更新可解析問題狀態。 如需詳細資訊，請參閱[設定Adobe Workfront以處理可解析物件](#set-up-adobe-workfront-to-handle-resolvable-objects)。

* 專案或任務的自訂狀態與問題自訂狀態具有相同的三個字母代碼。

您可以針對問題和專案或任務建立具有相同索引鍵的自訂狀態。 當專案或任務（作為解決物件）變更為自訂狀態時，變更也會反映在問題狀態上。 問題和專案或任務狀態的狀態索引鍵必須相同。

例如，假設您使用三個字母的程式碼LCD建立名為Launched的專案自訂狀態，這相當於Current。 接下來，您建立名為「已啟動專案」的問題自訂狀態，同時顯示字母代碼LCD，這相當於「進行中」。 當您將專案標籤為「已啟動」時，問題會自動將狀態變更為「已啟動專案」。 如果在解析物件變更設定的狀態未啟用時自動更新可解析問題狀態，則問題狀態將改為進行中。

如需建立自訂狀態的詳細資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

## 將解析物件的完成百分比與可解析物件的完成百分比同步

如果問題已由任務或專案解決，當以下任何情況發生時，可解決的問題會更新其完成百分比：

* 有人儲存任務或專案的變更時。
* 當重新計算專案的時間表時。

如果問題已由其他問題解決，當任一問題更新時，完成百分比會更新。

## 在任務或專案上尋找可解析物件

>[!NOTE]
>
>若要執行本節中的步驟，您至少必須擁有任務和專案的檢視存取權，以及包含您要檢視之可解析物件的任務或專案的檢視許可權。

對於任務和專案，找到相同的解析物件。

1. 導覽至您透過轉換問題建立的專案或任務。
1. 在頁面的左側，選取&#x200B;**任務詳細資料**&#x200B;或&#x200B;**專案詳細資料**&#x200B;標籤。
1. 在&#x200B;**總覽**&#x200B;區段的底部，找到&#x200B;**此已解析**&#x200B;欄位，其中顯示任務或專案的可解析物件。

   ![此解析欄位](assets/this-resolves-field.png)

   >[!NOTE]
   >
   >問題無法轉換為其他問題，但可以手動將其與正在解決的問題相關聯。 專案、任務或問題可以有多個問題作為可解析物件。 專案、任務或問題解決後，可解析物件（問題）也會解決。 即使解決可解決的問題重新開啟，可解決的問題仍保持關閉狀態。

## 識別清單中解析物件的問題

在問題清單中，您可以在&#x200B;**狀態圖示**&#x200B;或&#x200B;**旗標**&#x200B;欄中找出此圖示，藉此識別標示為透過狀態圖示解析物件的問題：

![解析物件](assets/resolving-icon.png)

## 在報告中檢視可解析物件和解析物件資訊

您可以在專案、任務或問題的檢視或報告中顯示有關可解析或解析物件的資訊。

下表顯示您可以顯示的欄位，以及您可以在哪些檢視中顯示欄位：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>檢視中的<strong>欄位</strong> </th> 
   <th><strong>問題檢視</strong> </th> 
   <th><strong>任務檢視</strong> </th> 
   <th><strong>專案檢視</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>有可解析專案</strong>：如果專案或任務有相關聯的可解析問題，則顯示True值，否則顯示False值。</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td><strong>原始問題名稱、原始問題輸入日期、建立者名稱</strong>：顯示原始問題的名稱和輸入日期，以及在文字模式自訂檢視中建立問題的使用者名稱。<br>如需詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md" class="MCXref xref">檢視：在任務或專案清單上顯示原始問題資訊</a>。<br></td> 
   <td> </td> 
   <td> ✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong>可解析專案：</strong>以文字模式自訂檢視顯示專案、工作報告或清單的所有可解析物件清單。</p> <p>如需詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-resolvable-objects-task-project-report.md" class="MCXref xref">檢視：任務或專案報告中的可解析物件</a></p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><strong>轉換的問題建立者</strong>：顯示最初記錄問題且後來轉換為任務之使用者的相關資訊。 </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>解決專案</strong>：顯示解決專案的資訊，該資訊已從原始問題轉換為問題或手動指定為問題的解決物件。</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>解決任務</strong>：顯示從原始問題轉換或手動指定為問題解決物件的解決任務的相關資訊。</td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>解決問題</strong>：顯示有關已手動指定為問題解決物件的解決問題的資訊。</td> 
   <td> ✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
