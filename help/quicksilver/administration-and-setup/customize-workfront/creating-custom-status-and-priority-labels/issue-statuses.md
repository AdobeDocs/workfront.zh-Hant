---
title: 訪問系統問題狀態清單
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 您可以使用問題的狀態，來顯示系統中使用者在指定時間的開發階段和問題。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# 訪問系統問題狀態清單

您可以使用問題的狀態，來顯示系統中使用者在指定時間的開發階段和問題。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 訪問問題狀態

您可以訪問和修改系統級問題狀態。 您可以編輯一些關於預設系統狀態的資訊，也可以建立新的自訂狀態。 有關建立自定義狀態或編輯系統狀態的詳細資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

要訪問系統級問題狀態，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **專案偏好設定** > **狀態**.

1. 按一下 **問題** 頁簽，查看Workfront中可用的問題狀態。

   ![](assets/issue-status.png)

## 系統問題狀態

Workfront提供10種原始發行狀態。 下表中的前4個是必填項，這表示您可以解除鎖定、重新命名和重新排序這些項目，但無法隱藏或刪除這些項目。

您可以新增自訂問題狀態，以符合組織的需求。 如需詳細資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

對使用者而言，變更問題狀態通常是手動程式。 不過，在下列清單中列出的某些情況下，系統中發生的其他因素會導致問題狀態自動變更。

您的Workfront執行個體提供下列問題狀態：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>系統問題狀態</th> 
   <th>如何使用狀態</th> 
   <th>狀態中會發生什麼</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>新增（必要狀態）</td> 
   <td>這是每個新建立問題的預設狀態。</td> 
   <td>如果問題位於處於「當前」狀態的項目上，則問題會顯示在分配給該問題的用戶的「工作請求」頁簽中。 使用者現在可以開始處理問題。</td> 
  </tr> 
  <tr> 
   <td>正在進行（必需狀態）</td> 
   <td> <p>您可以在此狀態中放置問題，以指出已開始處理該問題。</p> <p>如果問題的解決連接到另一個對象（任務、項目或其他問題），則當將解決對象的狀態更改為「正在處理」時，問題狀態將自動更改為「正在處理」。 </p> <p>有關解析對象的詳細資訊，請參閱 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>.</p> </td> 
   <td> <p>如果問題出現在狀態為「目前」的專案上，則問題會顯示在指派給問題之使用者的「工作中」索引標籤中。</p> <p>當問題正在進行中時，問題會顯示實際開始日期的值。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>已關閉（必要狀態）</td> 
   <td> <p>完成問題時，您可以手動將問題標示為「已關閉」。 </p> <p>如果問題的解決連接到另一個對象（任務、項目或其他問題），則當將解決對象的狀態更改為「已關閉」時，問題狀態將自動更改為「已關閉」。</p> <p>有關解析對象的詳細資訊，請參閱 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>.</p> </td> 
   <td> <p>當問題關閉時，該問題將從受託人的「工作時間」清單中刪除。 在這種情況下，問題會顯示實際完成日期的值。 </p> <p>完成所有任務並關閉項目上的問題後，即可完成項目。</p> </td> 
  </tr> 
  <tr> 
   <td>暫掛（必需狀態）</td> 
   <td> <p>您可以手動將問題標示為「暫掛」，以指出完成問題時發生延遲。 </p> </td> 
   <td> <p>如果問題出現在狀態為「目前」的專案上，則問題會顯示在指派給問題之使用者的「工作中」索引標籤中。 </p> <p>如果項目上的所有任務都已完成，但項目上至少存在一個「暫掛」問題，則無法完成項目。 </p> </td> 
  </tr> 
  <tr> 
   <td>重新開啟（等於進行中）</td> 
   <td> <p>您可以在此狀態中放置一個問題，以指出問題之前關閉時，該問題的工作尚未完成，因此需要重新開啟它才能完成工作。</p> </td> 
   <td> <p>如果問題位於處於「當前」狀態的項目上，則問題會顯示在分配給該問題的用戶的「工作請求」頁簽中。 使用者現在可以開始處理問題。</p> <p>此狀態在報表中很重要，可區分第一次開啟的問題（通常為「新」狀態），以及之前關閉之後開啟的問題（通常為「重新開啟」狀態）。 </p> </td> 
  </tr> 
  <tr> 
   <td>等待反饋（等於暫掛）</td> 
   <td>您可以在此狀態中放置問題，以表示您正在等待反饋（通常來自主聯繫人），然後才能繼續處理問題。 </td> 
   <td> <p>如果問題出現在狀態為「目前」的專案上，則問題會顯示在指派給問題之使用者的「工作中」索引標籤中。</p> <p>如果問題為等待反饋，則無法完成項目。</p> <p>此狀態在報表中很重要，可區分目前開啟但正在處理的問題（通常在「進行中」狀態中）和目前開啟但未處理的問題，因為完成這些問題需要更多意見（通常處於「等待意見」狀態）。</p> </td> 
  </tr> 
  <tr> 
   <td>無法複製（等於已關閉）</td> 
   <td>您可能會在此狀態中放置問題，以表示您正在關閉問題，但您無法看到觸發開啟問題的問題。 問題可能仍然存在，但無法在指定時間複製。 </td> 
   <td> <p>此狀態在報告中非常重要，可區分已完成的問題和已解決的問題（通常處於「已關閉」狀態），以及在指定時間無法顯示的問題（通常處於「無法複製」狀態）。</p> <p>當問題標示為「無法複製」時，該問題將從受託人的「工作時間」清單中移除。 在這種情況下，問題將顯示Actual CompletionDate的值。</p> <p>如果項目上的所有任務都已完成，並且某些問題處於「無法複製」狀態，則項目可以完成。</p> </td> 
  </tr> 
  <tr> 
   <td>已解決（等於關閉）</td> 
   <td>您可以在此狀態中放置問題，以指出您正在關閉問題，而建立問題的問題實際上已解決。</td> 
   <td> <p>此狀態在報表中很重要，可區分以或不以解決方案關閉的問題（通常為「已關閉」狀態），以及以實際解決方案關閉的問題（通常為「已解決」狀態）。</p> <p>將問題標示為「已解決」時，該問題將從受託人的「工作時間」清單中移除。 在這種情況下，問題會顯示實際完成日期的值。</p> <p>如果項目上的所有任務都已完成，並且至少有一個問題處於「已解決」狀態，則項目可以完成。 </p> </td> 
  </tr> 
  <tr> 
   <td>驗證完成（等於關閉）</td> 
   <td>您可以在此狀態中放置問題，以表示您正在關閉問題，並且您已驗證已解決產生問題的問題。</td> 
   <td> <p>當問題標籤為「已驗證完成」時，該問題將從受託人的「工作時間」清單中刪除。 在這種情況下，問題會顯示實際完成日期的值。</p> <p>如果項目上的所有任務都已完成，並且某些問題處於「已驗證的完成」狀態，則項目可以完成。</p> </td> 
  </tr> 
  <tr> 
   <td>無法解決（等於關閉）</td> 
   <td>您可以在此狀態中放置問題，以表示您正在關閉問題，但無法解決已產生問題的問題。</td> 
   <td> <p>在報表中，此狀態非常重要，可區分以或不以解決方案關閉的問題（通常為「已關閉」狀態），以及未以實際解決方案關閉的問題（通常為「不解決」狀態）。</p> <p>當問題標籤為「不解決」時，該問題將從受託人的「工作時間」清單中刪除。 在這種情況下，問題會顯示實際完成日期的值。</p> <p>如果項目上的所有任務都已完成，並且至少有一個問題處於「無法解決」狀態，則項目可以完成。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂問題狀態

Workfront管理員可將系統層級和群組層級問題狀態新增至Workfront，並變更使用者看到的順序。 如需詳細資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

群組管理員可以新增一個群組專屬的自訂狀態。 如需詳細資訊，請參閱 [建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
