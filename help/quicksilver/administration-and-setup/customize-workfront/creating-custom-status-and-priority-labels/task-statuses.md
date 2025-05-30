---
title: 存取系統工作狀態清單
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 您可以使用任務的狀態來向使用者顯示任務在指定時間處於哪個開發階段。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2cdedc67-b7b0-4e83-a446-d71e3afe255c
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# 存取系統工作狀態清單

您可以使用任務的狀態來向使用者顯示任務在指定時間處於哪個開發階段。

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
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 存取任務狀態

如需有關編輯系統狀態或建立新自訂狀態的資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

{{step-1-to-setup}}

1. 按一下&#x200B;**專案偏好設定** > **狀態**。

1. 按一下「**任務**」標籤。

   此標籤會列出Workfront中可用的工作狀態。

   ![任務狀態](assets/task-status.png)

   如需每個內建系統工作狀態的詳細資訊，請參閱[系統工作狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-task-statuses.md)。

## 關於建立自訂任務狀態

身為Workfront管理員，您可以新增自訂系統任務狀態至Workfront。

身為群組擁有者，您可以為群組新增自訂任務狀態。

當您建立自訂任務狀態時，必須始終將新狀態與現有系統狀態等同。 您必須瞭解系統狀態的行為，才能知道哪個狀態適合將您的自訂狀態等同於。 選取相等狀態後，便無法變更此選取專案。

如需建立自訂狀態、編輯系統狀態，或選取工作的新預設狀態的詳細資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。
