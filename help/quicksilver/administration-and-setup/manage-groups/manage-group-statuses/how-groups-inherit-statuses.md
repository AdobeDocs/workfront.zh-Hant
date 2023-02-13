---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 組如何繼承狀態
description: 列出群組可用的狀態時，您會看到下列內容
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# 組如何繼承狀態

列出群組可用的狀態時，您會看到下列內容

* 為群組建立的自訂狀態，如 [建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* 從系統繼承的狀態和組層次結構中的較高級狀態，如本文所述。

## 繼承狀態

發生下列任一情況時，您的組會繼承狀態：

* 您會建立群組。
* 管理員鎖定較高級別組中的狀態。
* 管理員會刪除另一個群組，並選擇您的群組取代。

下表說明每種情況。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">建立群組時</td> 
   <td> <p>建立新組時，它會自動繼承：</p> 
    <ul> 
     <li>如果新組是子組，則在組中處於上一級的解除鎖定狀態。</li> 
    </ul> 
    <ul> 
     <li>系統層級的鎖定狀態。</li> 
    </ul> 
     <b>範例：</b></span></span> 
     <p>假設一個名為「行銷」的群組有2個名為「行銷通訊與品牌推廣」的子群組。</p> 
     <p>行銷群組的群組管理員會建立名為Discovery的新自訂狀態。</p> 
     <p>之後，您會在「行銷」群組下建立新的子群組，並將其命名為「廣告」。</p> 
     <p>您的子組會繼承發現狀態，因為您在其他管理員建立未鎖定的發現狀態後建立了該組。</p> 
     <p>因為當此情況發生時，「行銷通訊」和「品牌」子組已存在於「行銷」組之下，因此它們不會繼承未鎖定的「發現」狀態。</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">當管理員鎖定更高級別的狀態時</td> 
   <td> <p>當Workfront管理員鎖定系統級別的狀態時，您的組將繼承該狀態，並繼承系統中的所有其他組。</p> <p>同樣，當管理員鎖定組上方某組的狀態時，您的組將與較高組下的任何其他子組一起繼承該狀態。</p> <p><b>注意</b>:稍後，如果管理員在系統級別或組上方的組中解鎖其中一種狀態，則您的組將保留先前繼承的狀態。 現在，狀態是個別的版本，您可以只為群組自訂它。</p> 
    <p><b>範例：</b></p>
    <p>行銷群組管理員會鎖定上述的探索狀態，以確保所有3個子群組都具備該狀態。</p> 
    <p>與您的廣告群組一起，行銷通訊和品牌推廣群組現在具有探索狀態。 當鎖定在上方的行銷群組時，他們便繼承了它。</p> 
    <p>然後，行銷組管理員將解除鎖定「發現」狀態，以便所有3個子組都擁有自己版本的「發現」狀態。 現在，您和其他2個組的管理員可以自定義發現狀態以滿足組的需要。</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">管理員刪除群組時</td> 
   <td> <p>當管理員刪除組並選擇您的組在系統中的位置時，如果已刪除組中不存在，則組會繼承已刪除組的自定義狀態。</p> 
   <p><b>範例： </b></p>
     <p>名為「傳訊」的群組必須與您的廣告群組合併，因此，Workfront管理員會刪除「傳訊」群組，並選擇您的群組取代。</p> 
     <p>「消息」組具有名為「正在處理」的唯一狀態。 您的廣告群組現在擁有可供使用的狀態。</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 繼承狀態配置

建立頂級組時，它會從系統級繼承以下配置。 建立子組時，它會從下一個更高的組中繼承以下配置。

* 預設狀態配置

   如需這些項目的相關資訊，請參閱 [使用自訂狀態作為預設狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* 狀態顯示順序配置

   如需這些項目的相關資訊，請參閱 [重新排序系統級和組狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

如果在建立您的群組後有人變更這些設定，則其狀態不受影響。
