---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 移動或刪除的群組中的自訂狀態
description: 本文說明當您移動或刪除群組時，群組自訂狀態會發生什麼情況。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# 群組中已移動或刪除的自訂狀態

本文說明當您移動或刪除群組時，群組自訂狀態會發生什麼情況。

## 移動之群組中的自訂狀態

請考量下列案例，說明將群組移至另一個群組下的新位置時，群組自訂狀態會發生什麼事。

如需關於移動群組的資訊，請參閱[移動群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md)。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">將群組移動到另一個群組下時 </td> 
   <td> <p>所有已移動群組的狀態都會保留下來。 它們不會新增至群組的新父級群組的狀態。</p> <p>但是，移動的群組會繼承群組中的所有鎖定狀態，或繼承其階層中較高位置的群組。 從現在開始，如果管理員在階層中鎖定較高的狀態，則移動的群組會繼承該狀態。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">當兩個群組中的狀態具有相同的鍵但不同的屬性時</td> 
   <td> <p>假設兩個不同的子群組從父群組繼承相同的解除鎖定狀態。 然後，這2個群組的群組管理員會以不同方式自訂其群組的狀態。</p> <p>之後，兩個群組中的一個會移至另一個群組下方。 現在，兩者的狀態具有相同的索引鍵，但其在兩個群組中具有不同的屬性。</p> <p>在此案例中，下列其中一個為true：</p> 
    <ul> 
     <li>如果新父群組中的狀態已解鎖，則已移動群組中的狀態會保留其屬性，不受移動影響。</li> 
     <li>如果新父群組中的狀態已鎖定，則父群組中狀態的屬性會覆寫已移動群組中狀態的屬性。</li> 
    </ul> <p>如需有關狀態金鑰的資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>當移動的群組具有繼承自其先前父群組的狀態時 </td> 
   <td> <p>從先前的父群組繼承的所有自訂狀態都會隨移動的群組一起出現，並成為其自己的自訂狀態。 它們不再與先前的父群組連線。</p> 
    <ul> 
     <li>如果先前的父群組在移動後編輯鎖定的自訂狀態，則變更不會影響已移動子群組的狀態。</li> 
     <li>如果前一個父群組鎖定自訂狀態，而該自訂狀態在群組移動時已解鎖，則已移動子群組的狀態不會鎖定。</li> 
     <li>移動的群組現在可以解鎖從先前的父群組繼承而鎖定的狀態。</li> 
    </ul> 
     <p><b>範例：</b><p> 
     <p>行銷群組的群組管理員Olivia會為群組建立兩種狀態。 她用金鑰ABC命名一個「First Review」，並加以鎖定。 她用金鑰XYZ為另一個最終評論命名，而且沒有鎖定。</p> 
     <p>她也會在行銷群組下建立稱為產品行銷的子群組。 在建立時，會自動繼承行銷群組的「首次檢閱」和「最終檢閱」。</p> 
     <p>稍後，Olivia將產品行銷子群組移至產品群組下方。 首次檢閱和最終檢閱都會隨產品行銷群組移至其產品群組下的新位置。</p> 
     <p>雖然「首次檢閱」已在移動前鎖定，但「產品行銷群組」管理員現在可以編輯它，因為它不再是繼承狀態，且由它所來自的父群組控制。</p> 
     <p>「最終稽核」會如往常一樣解除鎖定並可編輯。</p> 
     <p>對於行銷群組，Olivia會變更「首次稽核」和「最終稽核」的顏色，並將其重新命名為「首次稽核編輯」和「最終稽核編輯」。 她也會鎖定「最終稽核 — 已編輯」。 同時，在產品行銷群組中，狀態「首次檢閱」和「最終檢閱」的顏色和名稱不會變更。</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 已刪除群組內的自訂狀態

刪除群組或子群組時，將與其相關的資訊（包括其自訂狀態）重新指派給另一個群組或子群組。 已刪除群組的狀態會新增至目的地群組的狀態。

如果目的地群組也使用了其中一個已刪除群組的狀態（兩個群組中的狀態具有相同的索引鍵），且目的地群組以不同的方式自訂了狀態，則目的地群組版本的設定會覆寫移動群組版本的設定。

>[!INFO]
>
>**範例：**
>
>A群組的群組管理員會重新命名其群組的解除鎖定系統層級狀態。 群組B的群組管理員也會重新命名其群組的狀態。 雖然狀態在兩個群組中的名稱不同，但鍵是相同的。
>
>之後，群組A被刪除，其所有資訊被重新指派給群組B。
>
>* 狀態為群組B版本的名稱會覆寫群組A版本的名稱。
>* 如果群組A中的某個人在刪除該群組之前將狀態套用至物件，則物件上的狀態名稱會更新為群組B使用的狀態名稱。
>
>如需有關狀態索引鍵的資訊，請參閱本文中[建立或編輯自訂狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [建立或編輯群組](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create)的狀態下的表格。
>
>如需有關刪除群組的資訊，請參閱[刪除群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)。
