---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 使用自訂狀態作為預設狀態
description: 當自訂狀態設為預設狀態時，系統會以各種方式使用新的預設狀態。 其使用方式取決於其設定為預設系統級別狀態還是預設的組級別狀態。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# 使用自訂狀態作為預設狀態

當自訂狀態設為預設狀態時，系統會以各種方式使用新的預設狀態。 其使用方式取決於其設定為預設系統級別狀態還是預設的組級別狀態。

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

## 自定義預設系統級狀態

當您將自定義狀態設定為預設系統狀態時，系統中建立的任何新組都將繼承該狀態。

設定新預設系統狀態時已存在的組不會自動繼承它。

例如，假設已在您的Adobe Workfront環境中建立兩個群組（行銷和銷售）。 您可以建立與「當前」相等的新自定義狀態，並調用「正在處理」狀態。 現在，您將建立一個名為「工程」的新組。 在此情況下，工程組會繼承新的預設狀態；行銷和銷售群組則否。

## 自訂預設群組層級狀態

您設定為預設群組狀態的自訂狀態會用於下列情況：

* **當Workfront系統自動選擇狀態時，會使用預設群組狀態：** 當Workfront系統自動將狀態指派給物件時，會使用您設定為預設群組狀態的自訂狀態。

   例如，任務可以配置為當完成百分比達到100%時自動更改為完成狀態。 如果您建立等於「完成」的自訂狀態，並將該自訂狀態設為預設狀態，則Workfront會將任務的狀態變更為新的預設狀態。

   自訂狀態只能用於與任務或問題相關聯的組狀態。 對於與專案相關聯的狀態，無法以此方式使用自訂狀態。

* 此 **項目狀態由與項目關聯的組確定**:如果與指定項目關聯的組發生更改，則項目的狀態會根據為組定義的預設狀態而改變。 （在編輯專案時，群組可透過「群組」欄位與專案相關聯。）

   如果該組更改，則如果新組定義的預設狀態與項目的當前狀態相等，則項目的狀態將更改。

   例如，一個項目可以與市場營銷組關聯，並且項目的狀態設定為Planning。 項目經過編輯，現在與「銷售」組關聯。 Sales組的自定義預設組狀態稱為Thinking（此狀態相當於Planning）。 由於項目組已更改，項目的狀態現在變為Thinking。

如果您是群組管理員，請參閱 [將狀態設定為組的預設狀態](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## 問題狀態

如果自訂狀態為「問題」狀態，則必須為其啟用所有四種問題類型（錯誤報告、變更順序、問題和請求）。 例如，在下面顯示的問題狀態中，無法將狀態重新開啟用作預設狀態，因為未選擇更改單問題類型：

![](assets/all-4-issue-types-enabled.png)

## 將自訂狀態設為預設狀態

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).
1. 在左側面板中，按一下 **專案偏好設定** > **狀態**.
1. （條件性）如果要設定組的預設狀態，請開始在右上角的功能表中鍵入組的名稱，然後在顯示時選擇該名稱。
1. 開啟 **專案**, **工作**，或 **問題** 頁簽，具體取決於要設定為預設狀態的狀態類型。
1. 按一下 **設定預設狀態** 下拉式功能表。
1. 在顯示的下拉式區域中，在您要設定預設狀態的狀態旁，選取您要的預設狀態。
1. 按一下&#x200B;**儲存**。
1. 將項目與狀態所在的組關聯。

   >[!NOTE]
   >
   >如果您要設定群組的自訂狀態，而您稍後將專案指派給其他群組，專案狀態會重新載入，且可能會變更。

   1. 前往您要使用自訂狀態的專案。
   1. 按一下「更多」功能表 ![](assets/more-icon.png)，然後按一下 **編輯**.
   1. 在 **編輯專案** 框中 **群組** 欄位 **專案關聯**，請選擇狀態所在的組。
   1. 按一下 **儲存變更**.
