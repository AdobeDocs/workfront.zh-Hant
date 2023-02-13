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

狀態是鎖定還是解除鎖定將決定系統中所有組的狀態是否被刪除：

* 刪除當前鎖定的系統狀態時，系統中所有組的狀態都將被刪除，無論組是否已更名。
* 反之，如果刪除當前已解鎖的系統狀態，則系統中所有組的狀態都會保持不變。


>[!NOTE]
>
>您無法刪除下列項目：
>
>* 系統批准進程中使用的鎖定或解鎖系統狀態，當前正在等待系統中至少一個對象的批准。
>
>  但是，您可以刪除單次使用或當前正在等待批准的組級別批准流程中使用的未鎖定系統狀態。
>
>  您可以運行報告來查找對象並解析掛起的批准，然後重試以刪除狀態。 如需指示，請參閱 [使用特定狀態列出具有待批准進程的對象](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* 在審批流程中使用的狀態，這些狀態當前是系統中至少一個對象的待審批狀態。


有關刪除組狀態的說明，請參閱 [刪除組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

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

## 刪除自定義系統狀態

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **專案偏好設定** > **狀態**.

1. 若要刪除整個系統的狀態（包括個別群組的狀態），請將滑鼠移至狀態上方，按一下 **編輯**，然後確定 **鎖定所有組** 中所有規則的URL。 按一下&#x200B;**儲存**。

   或

   要刪除系統狀態，但將其保留給各個組，請將滑鼠移到該狀態上，按一下 **編輯**，然後確定 **鎖定所有組** 未選取。 按一下&#x200B;**儲存**。

1. 暫留在您要刪除的狀態上，然後按一下 **刪除**.
1. 在顯示的訊息中，按一下 **刪除狀態**.
1. 在 **刪除狀態** 框中，在標籤為的欄位中選擇狀態 **將當前處於此狀態的所有項目設定為**.

   使用您正在刪除的狀態的專案會設為您選取的狀態。

   狀態等於您要刪除的狀態時，才可在下拉式清單中使用。

   例如，如果您刪除等於「目前」的狀態，則只能選擇同樣等於「目前」的狀態。

1. 按一下 **刪除狀態**.
