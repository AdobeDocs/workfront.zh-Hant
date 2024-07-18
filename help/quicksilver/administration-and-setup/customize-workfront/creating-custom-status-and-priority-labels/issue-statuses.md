---
title: 存取系統問題狀態清單
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 您可以使用問題的狀態來顯示系統中在指定時間問題處於哪個開發階段的使用者。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# 存取系統問題狀態清單

您可以使用問題的狀態來顯示系統中在指定時間問題處於哪個開發階段的使用者。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 存取問題狀態

您可以存取及修改系統層級的問題狀態。 您可以編輯一些關於預設系統狀態的資訊，也可以建立新的自訂狀態。 如需建立自訂狀態或編輯系統狀態的詳細資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

若要存取系統層級問題狀態：

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**專案偏好設定** > **狀態**。

1. 按一下&#x200B;**問題**&#x200B;索引標籤，檢視Workfront中可用的問題狀態。

   ![](assets/issue-status.png)

## 系統問題狀態

Workfront附帶10個原始問題狀態。 下表中的前4個為必要專案，這表示您可以解除鎖定、重新命名及重新排序，但無法隱藏或刪除它們。

您可以新增自訂問題狀態以符合組織中的需求。 如需詳細資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

對於使用者而言，變更問題狀態通常是手動流程。 但是，在某些情況下，當問題的狀態根據系統中發生的其他因素自動變更時，如下表所述。

您的Workfront執行個體會提供下列問題狀態：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>系統問題狀態</th> 
   <th>如何使用狀態</th> 
   <th>狀態中會發生什麼事</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>新增（必要狀態）</td> 
   <td>這是每個新建立問題的預設狀態。</td> 
   <td>如果問題是在狀態為「目前」的專案上，則問題會顯示在指派給問題的使用者的「工作請求」標籤中。 使用者現在可以開始處理問題。</td> 
  </tr> 
  <tr> 
   <td>進行中（必要狀態）</td> 
   <td> <p>您可以設定此狀態的問題，表示該問題的工作已開始。</p> <p>如果問題的解決連線到另一個物件（任務、專案或其他問題），當您將解決物件的狀態變更為進行中時，問題狀態會自動變更為進行中。 </p> <p>如需解析物件的詳細資訊，請參閱<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析物件概述</a>。</p> </td> 
   <td> <p>如果問題位於狀態為「目前」的專案上，則問題會顯示在受指派問題之使用者的「處理中」標籤中。</p> <p>當問題正在進行時，問題顯示實際開始日期的值。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>已關閉（必要狀態）</td> 
   <td> <p>當問題的工作完成時，您可以手動將問題標示為「已關閉」。 </p> <p>如果問題的解決連線到另一個物件（任務、專案或其他問題），則當您將解決物件的狀態變更為已關閉時，問題狀態會自動變更為已關閉。</p> <p>如需解析物件的詳細資訊，請參閱<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析物件概述</a>。</p> </td> 
   <td> <p>問題關閉時，該問題會從受指派人的工作清單中移除。 在此情況下，問題會顯示「實際完成日期」的值。 </p> <p>當專案中的所有任務完成並關閉問題時，專案就可以完成。</p> </td> 
  </tr> 
  <tr> 
   <td>保留（必要狀態）</td> 
   <td> <p>您可以手動將問題標示為「保留」，以指出完成問題時發生延遲。 </p> </td> 
   <td> <p>如果問題位於狀態為「目前」的專案上，則問題會顯示在受指派問題之使用者的「處理中」標籤中。 </p> <p>當專案上的所有任務都已完成，但專案上至少有一個保留問題時，專案便無法完成。 </p> </td> 
  </tr> 
  <tr> 
   <td>重新開啟（等於進行中）</td> 
   <td> <p>您可以將問題置於此狀態，以表示該問題的工作尚未在問題先前關閉時完全完成，需要重新開啟才能完成工作。</p> </td> 
   <td> <p>如果問題是在狀態為「目前」的專案上，則問題會顯示在指派給問題的使用者的「工作請求」標籤中。 使用者現在可以開始處理問題。</p> <p>此狀態在報告中很重要，可區分首次開啟的問題（通常在「新增」狀態中）和在關閉前開啟的問題（通常在「重新開啟」狀態中）。 </p> </td> 
  </tr> 
  <tr> 
   <td>等待回饋（等於保留）</td> 
   <td>您可以將問題置於此狀態，表示您正等待意見回饋（通常來自主要連絡人），然後才能繼續處理問題。 </td> 
   <td> <p>如果問題位於狀態為「目前」的專案上，則問題會顯示在受指派問題之使用者的「處理中」標籤中。</p> <p>如果問題正在等待意見反應，專案就無法完成。</p> <p>此狀態在報告中很重要，以區分目前未完成但正在處理的問題（通常處於進行中狀態）和目前未完成但並未處理的問題，因為需要更多意見才能完成它們（通常處於等待意見反應狀態）。</p> </td> 
  </tr> 
  <tr> 
   <td>無法複製（等於已關閉）</td> 
   <td>您可以將問題置於此狀態，表示您正在關閉問題，但您看不到觸發開啟問題的問題。 問題可能仍然存在，但無法在指定時間復寫。 </td> 
   <td> <p>此狀態在報告中很重要，以區分已完成的問題和已解決的問題（通常在「已關閉」狀態）和問題在特定時間不可見的問題（通常在「無法複製」狀態）。</p> <p>當問題被標籤為無法複製時，該問題會從受指派人的工作清單中移除。 在這種情況下，問題會顯示「實際CompletionDate」的值。</p> <p>如果專案上的所有任務已完成，且某些問題處於無法複製狀態，則專案可以完成。</p> </td> 
  </tr> 
  <tr> 
   <td>已解決（等於已關閉）</td> 
   <td>您可以將問題置於此狀態，以表示您正在關閉問題且建立問題的實際已解決。</td> 
   <td> <p>此狀態在報告中很重要，可區分使用解決方案關閉或未使用解決方案關閉的問題（通常在「已關閉」狀態）和使用實際解決方案關閉的問題（通常在「已解決」狀態）。</p> <p>當問題標籤為「已解決」時，該問題會從受指派人的工作清單中移除。 在此情況下，問題會顯示「實際完成日期」的值。</p> <p>如果專案上的所有任務已完成，且至少一個問題處於「已解決」狀態，則專案可完成。 </p> </td> 
  </tr> 
  <tr> 
   <td>已確認完成（等於已關閉）</td> 
   <td>您可以將問題置於此狀態，表示您正在關閉問題，且已驗證產生問題的問題已解決。</td> 
   <td> <p>當問題被標籤為「已驗證完成」時，該問題會從受指派人的工作清單中移除。 在此情況下，問題會顯示「實際完成日期」的值。</p> <p>如果專案上的所有任務已完成，且某些問題處於已驗證完成狀態，則專案可以完成。</p> </td> 
  </tr> 
  <tr> 
   <td>不會解析（等於已關閉）</td> 
   <td>您可以將問題置於此狀態，以表示您即將關閉問題，但無法解決產生問題的問題。</td> 
   <td> <p>此狀態在報告中很重要，以區分有解決方案或沒有解決方案關閉的問題（通常在「已關閉」狀態）和沒有實際解決方案關閉的問題（通常在「無法解決」狀態）。</p> <p>當問題標示為無法解決時，該問題會從受指派人的工作清單中移除。 在此情況下，問題會顯示「實際完成日期」的值。</p> <p>如果專案上的所有任務已完成，且至少一個問題處於無法解決狀態，則專案可以完成。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂問題狀態

Workfront管理員可以在Workfront中新增系統層級和群組層級問題狀態，並變更使用者看見這些問題的順序。 如需詳細資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

群組管理員可以新增一個群組的特定自訂狀態。 如需詳細資訊，請參閱[建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。
