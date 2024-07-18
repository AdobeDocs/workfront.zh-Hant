---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 群組如何繼承狀態
description: 當您列出群組的可用狀態時，您會看到以下內容
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# 群組如何繼承狀態

當您列出群組的可用狀態時，您會看到以下內容

* 為群組建立的自訂狀態，如[建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)中所述。
* 如本文所述，狀態繼承自系統和群組階層中較高層級。

## 繼承狀態

當下列任一情況發生時，您的群組會繼承狀態：

* 您建立群組。
* 管理員會鎖定較高層級群組中的狀態。
* 管理員會刪除另一個群組，並選擇讓您的群組取代該群組。

下表逐一說明這些情況。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">當您建立群組時</td> 
   <td> <p>當您建立新群組時，它會自動繼承：</p> 
    <ul> 
     <li>如果新群組是子群組，則為群組上的一級解除鎖定狀態。</li> 
    </ul> 
    <ul> 
     <li>系統層級的鎖定狀態。</li> 
    </ul> 
     <b>範例：</b></span></span> 
     <p>假設一個稱為行銷的群組有2個稱為行銷通訊和品牌化的子群組。</p> 
     <p>行銷群組的群組管理員會建立稱為「探索」的新自訂狀態。</p> 
     <p>稍後，您在「行銷群組」下建立新的子群組，並將其稱為「Advertising」。</p> 
     <p>您的子群組會繼承「探索」狀態，因為您是在其他管理員建立解除鎖定的「探索」狀態之後才建立群組。</p> 
     <p>由於發生此情況時，子群組「行銷通訊」和「品牌推廣」已存在於「行銷群組」下方，因此不會繼承解鎖的「探索」狀態。</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">當管理員在更高層級鎖定狀態時</td> 
   <td> <p>當Workfront管理員在系統層級鎖定狀態時，您的群組會與系統中的所有其他群組一起繼承該狀態。</p> <p>同樣地，當管理員鎖定您群組之上某個群組的狀態時，您的群組會繼承該群組以及更高群組之下的任何其他子群組。</p> <p><b>注意</b>：稍後，如果系統管理員在系統層級或群組上方的群組中解除鎖定其中一個狀態，則您的群組會保留先前繼承的狀態。 現在這是狀態的獨立版本，您可以僅為群組自訂。</p> 
    <p><b>範例：</b></p>
    <p>行銷群組管理員會鎖定上述探索狀態，以確保所有3個子群組都具備該狀態。</p> 
    <p>行銷通訊和品牌群組現在與您的Advertising群組一樣，具有「探索」狀態。 當它鎖定在其上方的行銷群組時，他們就會繼承它。</p> 
    <p>行銷群組管理員接著會解除鎖定「探索」狀態，讓所有3個子群組都有自己的探索狀態版本。 現在，您和其他2個群組的管理員可以自訂「探索」狀態，以符合群組的需求。</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">當管理員刪除群組時</td> 
   <td> <p>當管理員刪除群組並選擇您的群組在系統中取代時，如果您的群組中沒有已刪除群組的自訂狀態，則您的群組會繼承已刪除群組的自訂狀態。</p> 
   <p><b>範例： </b></p>
     <p>名為傳訊的群組需要與您的Advertising群組合併，因此Workfront管理員會刪除傳訊群組並選擇您的群組取代該群組。</p> 
     <p>傳訊群組有一個唯一狀態，稱為「處理中」。 您的Advertising群組現在擁有該狀態可供使用。</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 繼承狀態設定

當您建立頂層群組時，它會從系統層級繼承下列組態。 建立子群組時，它會繼承下一個較高群組的下列組態。

* 預設狀態設定

  如需這些專案的相關資訊，請參閱[使用自訂狀態作為預設狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md)。

* 狀態顯示訂單組態

  如需這些專案的相關資訊，請參閱[重新排序系統層級和群組狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md)。

如果有人在建立群組後變更這些組態，其狀態則不受影響。
