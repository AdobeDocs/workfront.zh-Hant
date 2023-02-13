---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 移動或刪除的群組中的自訂狀態
description: 本文說明移動或刪除群組時，群組自訂狀態會發生什麼事。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# 移動或刪除的群組中的自訂狀態

本文說明移動或刪除群組時，群組自訂狀態會發生什麼事。

## 已移動的群組中的自訂狀態

請考慮下列案例，說明將一個群組移至另一個群組下的新位置時，群組自訂狀態會發生什麼事。

如需移動群組的相關資訊，請參閱 [移動組](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">將組移到其他組下時 </td> 
   <td> <p>移動的群組的所有狀態都會保留在其中。 它們不會新增至群組新父群組的狀態。</p> <p>但移動的組繼承組或組中所有鎖定的狀態，這些狀態現在在其層次結構中更高。 此外，從現在開始，如果管理員鎖定層次結構中較高的狀態，則移動的組將繼承該狀態。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">當兩個群組中的狀態具有相同的索引鍵但不同屬性時</td> 
   <td> <p>假設兩個不同的子組從父組繼承相同的解鎖狀態。 然後，2個群組的群組管理員會以不同方式自訂其群組的狀態。</p> <p>之後，兩個群組中的一個會移至另一個群組下。 現在，兩者都具有具有相同索引鍵的狀態，但兩個群組中卻有不同的屬性。</p> <p>在此情況下，以下其中一項是true:</p> 
    <ul> 
     <li>如果新父組中的狀態處於解鎖狀態，則移動組中的狀態將保留其屬性，不受移動的影響。</li> 
     <li>如果新父組中的狀態被鎖定，則父組中狀態的屬性將覆蓋移動組中的狀態屬性。</li> 
    </ul> <p>如需狀態索引鍵的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>移動的組具有從其前一個父組繼承的狀態時 </td> 
   <td> <p>從上一個父組繼承的所有自訂狀態都會隨移動的組一起出現，並成為自己的自訂狀態。 它們不再與前一個父組連接。</p> 
    <ul> 
     <li>如果前一個父組在移動後編輯鎖定的自定義狀態，則更改不會影響移動的子組的狀態。</li> 
     <li>如果前一個父組鎖定的自定義狀態在組移動時已解除鎖定，則移動的子組的狀態不會鎖定。</li> 
     <li>已移動的群組現在可解除鎖定從先前的父群組繼承時鎖定的狀態。</li> 
    </ul> 
     <p><b>範例：</b><p> 
     <p>Marketing群組的群組管理員Olivia為群組建立兩種狀態。 她用鍵ABC將一個First Review命名為，然後鎖上。 她用密鑰XYZ給另一個Final Review取名，但不鎖定它。</p> 
     <p>她也會在行銷群組下建立一個子群組，稱為產品行銷。 建立時，它會自動繼承「行銷」群組的「首次檢閱」和「最終檢閱」。</p> 
     <p>之後，Olivia將產品營銷子組移到產品組下。 「首次審閱」和「最終審閱」都與產品市場營銷組一起到產品組下的新位置。</p> 
     <p>雖然移動前已鎖定「首次檢閱」，但產品行銷群組管理員現在可以編輯它，因為它不再是由其來源的上層群組控制的繼承狀態。</p> 
     <p>「最終審閱」已解除鎖定，並且可以按原樣編輯。</p> 
     <p>對於市場營銷組，Olivia更改了「首次審核」和「最終審核」的顏色，並將它們重新命名為「首次審核 — 編輯」和「最終審核 — 編輯」。 她還鎖定了最終審核編輯。 同時，在「產品行銷」群組中，狀態「首次檢閱」和「最終檢閱」的顏色和名稱不會變更。</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 已刪除的組中的自定義狀態

刪除組或子組時，您會將與其關聯的資訊（包括其自定義狀態）重新分配給其他組或子組。 已刪除群組的狀態會新增至目的地群組的狀態。

如果目標組也使用已刪除組的其中一種狀態（兩個組中的狀態具有相同的鍵），並且目標組以不同方式自定義了狀態，則目標組版本的設定將覆蓋已移動組版本的設定。

>[!INFO]
>
>**範例：**
>
>組A的組管理員將更名其組的未鎖定系統級別狀態。 組B的組管理員也會更名其組的狀態。 雖然狀態在兩個群組中的名稱不同，但有相同的鍵值。
>
>之後， A組被刪除，其所有資訊被重新分配給B組。
>
>* 狀態的B組版本名稱將覆蓋A組版本的名稱。
>* 如果在刪除組之前，組A中的某個人將該狀態應用於某個對象，則該對象上的狀態名稱將更新為組B使用的狀態名稱。
>
>如需狀態索引鍵的相關資訊，請參閱本文章中的表格，位於 [建立或編輯自訂狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [建立或編輯群組的狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>如需刪除群組的詳細資訊，請參閱 [刪除群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
