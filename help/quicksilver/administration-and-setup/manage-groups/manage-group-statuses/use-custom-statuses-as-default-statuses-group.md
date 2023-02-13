---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 使用自訂狀態作為群組的預設狀態
description: 作為組管理員，您可以將自定義狀態配置為所管理的組或子組的預設狀態。 當系統需要自動將Workfront狀態指派給專案、任務或問題時，這個功能會很實用。 專案、任務或問題一律會顯示您設為預設狀態的自訂狀態，而非顯示相等的Workfront狀態。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# 使用自訂狀態作為群組的預設狀態

作為組管理員，您可以將自定義狀態配置為所管理的組或子組的預設狀態。 當系統需要自動將Workfront狀態指派給專案、任務或問題時，這個功能會很實用。 專案、任務或問題一律會顯示您設為預設狀態的自訂狀態，而非顯示相等的Workfront狀態。

您配置的狀態可以是為組建立的任何自定義狀態、從組上方的組繼承的狀態，或從系統級別繼承的狀態。

如果您管理的群組上方有任何群組，其管理員也可以對您的群組執行此動作。 Workfront管理員（適用於任何群組）也是如此。

>[!INFO]
>
>**範例：** 您可以建立稱為「已完成」的自訂狀態，並將其設為與Workfront狀態「完成」相等的預設狀態。
>
>接著，對於設為在達到100%時變更為「完成」狀態的任務，狀態會顯示為「已完成」而非「完成」。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 問題狀態

如果自訂狀態為「問題」狀態，則必須為其啟用所有四種問題類型（錯誤報告、變更順序、問題和請求）。 例如，在下面顯示的問題狀態中，無法將狀態重新開啟用作預設狀態，因為未選擇更改單問題類型：

![](assets/all-4-issue-types-enabled.png)

## 將自訂狀態設定為群組的預設狀態

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).
1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png)，然後按一下您要建立或自訂狀態的群組名稱。
1. 在左側面板中，按一下 **狀態** ![](assets/gear-icon-settings.png).
1. 開啟 **專案**, **工作**，或 **問題** 頁簽，具體取決於要設定為預設狀態的狀態類型。
1. 按一下 **設定預設狀態** 在右上角。
1. 在顯示的下拉式區域中，在您要設定預設狀態的狀態旁，選取您要設定的預設狀態。
1. 按一下&#x200B;**儲存**。

   該狀態現在可作為預設狀態，以用於與群組相關聯的專案。

1. 將自訂狀態與您要使用它的專案建立關聯。

   通過將狀態所在的組與項目關聯，可將狀態與項目關聯。 只有狀態所在的群組與專案相關聯時，使用者才能使用自訂狀態。

   >[!NOTE]
   >
   >如果將專案指派給其他群組，專案狀態會重新載入，且可能會變更。

   1. 前往您要使用自訂狀態的專案。
   1. 按一下「更多」功能表 ![](assets/more-icon.png)，然後按一下 **編輯**.
   1. 在 **編輯專案** 框中 **群組** 欄位 **專案關聯**，選擇與自訂狀態相關聯的群組。

   1. 按一下 **儲存變更**.

## 組繼承預設狀態配置

Workfront管理員將自訂狀態設定為預設狀態後，建立的新群組會繼承該設定。

同樣，在組管理員將自定義狀態設定為預設狀態後，在組正下面建立的新子組將繼承該配置。

如需詳細資訊，請參閱 [組如何繼承狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## 隱藏預設狀態時

如果隱藏預設狀態（通過為其啟用「隱藏狀態」選項），系統將嘗試將等效類型的另一個狀態設定為預設狀態。

如果沒有對等類型的可用狀態，則狀態類型顯示為 **隱藏** 和不適用於工作項目。

![](assets/when-hide-default-status-no-equivalent.png)
