---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 刪除自訂狀態
description: 如果自訂系統狀態對您的組織不再有用，您可以將其刪除。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 2%

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

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>系統管理員</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 刪除自訂系統狀態

{{step-1-to-setup}}

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
