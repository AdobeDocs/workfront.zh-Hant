---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 刪除自訂狀態
description: 如果自訂系統狀態對您的組織不再有用，您可以將其刪除。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# 刪除自訂狀態

如果自訂系統狀態對您的組織不再有用，您可以將其刪除。

狀態是鎖定還是解除鎖定會決定系統所有群組的狀態是否都已刪除：

* 當您刪除目前鎖定的系統狀態時，系統會移除系統中所有群組的狀態，無論群組是否已重新命名。
* 相反地，當您刪除目前解除鎖定的系統狀態時，系統中所有群組的狀態都會保留。


>[!NOTE]
>
>您無法刪除下列專案：
>
>* 系統核准程式中使用的已鎖定或已解除鎖定系統狀態，目前至少待核准系統中的一個物件。
>
>  不過，您可以刪除目前等待核准之單次使用或群組層級核准程式中使用的已解除鎖定系統狀態。
>
>  您可以執行報告以尋找物件並解析擱置核准，然後再次嘗試刪除狀態。 如需指示，請參閱[使用特定狀態列出具有未決核准流程的物件](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md)。
>
>* 核准流程中所使用的狀態，目前至少擱置核准系統中的一個物件。

如需刪除群組狀態的指示，請參閱[刪除群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md)。

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

## 刪除自訂系統狀態

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 在左側面板中，按一下&#x200B;**專案偏好設定** > **狀態**。

1. 若要刪除整個系統（包括個別群組）的狀態，請將滑鼠移到狀態上，按一下[編輯] ****，然後確定已選取[鎖定所有群組] ****。 按一下「**儲存**」。

   或

   若要刪除系統狀態但保留個別群組的狀態，請將滑鼠移到狀態上，按一下[編輯] ****，然後確定已取消選取[鎖定所有群組] ****。 按一下「**儲存**」。

1. 暫留在您要刪除的狀態上，然後按一下[刪除]。****
1. 在顯示的訊息中，按一下&#x200B;**刪除狀態**。
1. 在顯示的&#x200B;**刪除狀態**&#x200B;方塊中，在標示為&#x200B;**的欄位中選取狀態。將目前使用此狀態的所有專案設定為**。

   使用您要刪除之狀態的專案會設定為您選取的狀態。

   只有當狀態與您正在刪除的狀態相等時，下拉式清單中的狀態才可使用。

   例如，如果您要刪除與「目前」相等的狀態，則只能選取與「目前」相等的狀態。

1. 按一下&#x200B;**刪除狀態**。
