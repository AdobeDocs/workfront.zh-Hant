---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 使用自訂狀態作為預設狀態
description: 當自訂狀態設定為預設狀態時，新的預設狀態會以各種方式在整個系統中使用。 其使用方式取決於其設定為預設系統層級狀態，還是預設群組層級狀態。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# 使用自訂狀態作為預設狀態

當自訂狀態設定為預設狀態時，新的預設狀態會以各種方式在整個系統中使用。 其使用方式取決於其設定為預設系統層級狀態，還是預設群組層級狀態。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td>
     <p>新增：標準</p>
     <p>或</p>
     <p>目前：計畫</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自訂預設系統層級狀態

當您設定自訂狀態為預設系統狀態時，系統中建立的任何新群組都會繼承該狀態。

當您設定新的預設系統狀態時已經存在的群組不會自動繼承它。

例如，假設已在您的Adobe Workfront環境中建立兩個群組（行銷和銷售）。 您可以建立等同於「目前」的新自訂狀態，並呼叫「處理中」狀態。 您現在會建立名為「工程」的新群組。 在此案例中，「工程」群組會繼承新的預設狀態；「行銷」和「銷售」群組則不會。

## 自訂預設群組層級狀態

在下列情況下，將使用您設定為預設群組狀態的自訂狀態：

* **當Workfront系統自動選擇狀態時，會使用預設群組狀態：**&#x200B;當Workfront系統自動指派狀態給物件時，會使用您設定為預設群組狀態的自訂狀態。

  例如，一項任務可設定為當完成百分比達到100%時自動變更為完成狀態。 如果您建立等同於完成的自訂狀態，並將該自訂狀態設定為預設狀態，Workfront會將任務的狀態變更為新的預設狀態。

  自訂狀態僅能用於與任務或問題相關聯的群組狀態。 自訂狀態無法以這種方式用於與專案關聯的狀態。

* 專案的&#x200B;**狀態是由與專案關聯的群組所決定**：如果與指定專案關聯的群組變更，則專案狀態會根據為群組定義的預設狀態而變更。 （編輯專案時，群組可透過「群組」欄位與專案相關聯。）

  若該群組變更，則若新群組已定義與專案目前狀態相等的不同預設狀態，則專案狀態會變更。

  例如，專案可與行銷群組相關聯，且專案狀態設為「計畫」。 專案經過編輯，現在會與銷售群組產生關聯。 「銷售」群組具有名為「思考」的自訂預設群組狀態（此狀態等於「計畫」）。 由於專案群組已變更，專案狀態現在變更為「思考」。

如果您是群組管理員，請參閱[將狀態設定為群組](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md)的預設狀態。

## 問題狀態

如果自訂狀態是問題狀態，則必須為其啟用所有四種問題型別（錯誤報告、變更順序、問題和請求）。 例如，在下方顯示的問題狀態中，由於未選取「變更單」問題型別，因此「重新開啟」狀態無法作為預設狀態：

![所有問題型別已啟用](assets/all-4-issue-types-enabled.png)

## 將自訂狀態設定為預設狀態

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**專案偏好設定** > **狀態**。
1. （視條件而定）如果您正在設定群組的預設狀態，請在右上角的選單中開始輸入群組的名稱，然後在其出現時選取它。
1. 視您要設定為預設狀態的狀態型別而定，開啟&#x200B;**專案**、**任務**&#x200B;或&#x200B;**問題**&#x200B;標籤。
1. 按一下&#x200B;**設定預設狀態**&#x200B;下拉式功能表。
1. 在顯示的下拉式區域中，在您要設定預設狀態的狀態旁邊，選取您想要的預設狀態。
1. 按一下「**儲存**」。
1. 將專案與狀態所在的群組建立關聯。

   >[!NOTE]
   >
   >如果您設定群組的自訂狀態，且稍後將專案指派給其他群組，則專案狀態將會重新載入並可能變更。

   1. 前往您要使用自訂狀態的專案。
   1. 按一下[更多]功能表![更多圖示](assets/more-icon.png)，然後按一下[編輯]****。
   1. 在顯示的&#x200B;**編輯專案**&#x200B;方塊中，在&#x200B;**專案關聯**&#x200B;下的&#x200B;**群組**&#x200B;欄位中，選取狀態所在的群組。
   1. 按一下「**儲存變更**」。
