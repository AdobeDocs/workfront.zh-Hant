---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 使用自訂狀態作為群組的預設狀態
description: 作為群組管理員，您可以將自訂狀態設定為您管理的群組或子群組的預設狀態。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: fb555df123701c62e9a0f2d451ad6dcd16586595
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 1%

---

# 使用自訂狀態作為群組的預設狀態

作為群組管理員，您可以將自訂狀態設定為您管理的群組或子群組的預設狀態。 當系統需要自動將Workfront狀態指派給專案、任務或問題時，這將很有用。 專案、任務或問題一律會顯示您設定為預設狀態的自訂狀態，而不是顯示其所對應的Workfront狀態。

您設定的狀態可以是針對群組建立的任何自訂狀態、繼承自群組上方的群組，或繼承自系統層級。

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

>[!INFO]
>
>**範例：**&#x200B;您可以建立名為「已完成」的自訂狀態，並將其設定為等同於Workfront狀態「完成」的預設狀態。
>
>然後，對於將任務設定為變更到狀態完成當它們達到100%，狀態顯示為完成而不是完成。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 問題狀態

如果自訂狀態是問題狀態，則必須為其啟用所有四種問題型別（錯誤報告、變更順序、問題和請求）。 例如，在下方顯示的問題狀態中，由於未選取「變更單」問題型別，因此「重新開啟」狀態無法作為預設狀態：

![所有問題型別已啟用](assets/all-4-issue-types-enabled.png)

## 將自訂狀態設定為群組的預設狀態

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)，然後按一下您要建立或自訂狀態的群組名稱。
1. 在左側面板中，按一下&#x200B;**狀態** ![齒輪設定圖示](assets/gear-icon-settings.png)。
1. 視您要設定為預設狀態的狀態型別而定，開啟&#x200B;**專案**、**任務**&#x200B;或&#x200B;**問題**&#x200B;標籤。
1. 按一下右上角附近的&#x200B;**設定預設狀態**。
1. 在顯示的下拉式區域中，在您要設定預設狀態的狀態旁邊，選取您要設定的預設狀態。
1. 按一下「**儲存**」。

   該狀態現在可作為預設狀態，用於與群組關聯的專案。

1. 將自訂狀態與您要使用它的專案建立關聯。

   您可以將狀態所在的群組與專案建立關聯，藉此將狀態與專案建立關聯。 只有當狀態所在的群組與專案相關聯時，使用者才能使用自訂狀態。

   >[!NOTE]
   >
   >如果您將專案指派給不同的群組，專案狀態將會重新載入並可能變更。

   1. 前往您要使用自訂狀態的專案。
   1. 按一下[更多]功能表![更多圖示](assets/more-icon.png)，然後按一下[編輯]****。
   1. 在顯示的&#x200B;**編輯專案**&#x200B;方塊中，在&#x200B;**專案關聯**&#x200B;下的&#x200B;**群組**&#x200B;欄位中，選取自訂狀態關聯的群組。

   1. 按一下「**儲存變更**」。

## 群組繼承預設狀態設定

Workfront管理員將自訂狀態設定為預設狀態後，建立的新群組將繼承該設定。

同樣地，群組管理員將自訂狀態設為預設狀態後，直接在群組下方建立的新子群組會繼承該設定。

如需詳細資訊，請參閱[群組如何繼承狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md)。

## 當預設狀態為隱藏時

如果您隱藏預設狀態(透過為其啟用「隱藏狀態」(Hide status)選項)，系統會嘗試將另一個同等型別的狀態設定為預設值。

如果沒有同等型別的可用狀態，則狀態型別會顯示為&#x200B;**隱藏**，且不適用於工作專案。

![沒有可用的狀態](assets/when-hide-default-status-no-equivalent.png)
