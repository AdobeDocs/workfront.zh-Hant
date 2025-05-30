---
title: 刪除自訂條件
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 您可以刪除自訂條件。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 刪除自訂條件

您可以刪除不再需要的自訂條件。

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

## 刪除自訂條件

{{step-1-to-setup}}

1. 按一下&#x200B;**專案偏好設定** > **條件**。

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. 選取您要刪除的條件所在之物件型別（**專案**、**任務**&#x200B;或&#x200B;**問題**）的標籤。

1. 暫留在您要刪除的條件上，然後按一下出現在最右邊的&#x200B;**刪除**&#x200B;圖示![刪除](assets/delete.png)。
1. 在出現的確認訊息中，按一下&#x200B;**刪除條件**。

1. 在出現的&#x200B;**刪除條件**&#x200B;方塊中，針對使用您要刪除條件的所有專案，在下拉式清單中選取新條件。

   自訂條件必須與您要刪除的內建條件相同，才可在下拉式清單中使用。 例如，如果您要刪除等同於「有風險」的條件，則只能選取等同於「有風險」的自訂條件。

1. 按一下&#x200B;**刪除條件**。

>[!NOTE]
>
>您無法刪除內建條件，這些條件已達目標狀態、有風險狀態及存在問題。 不過，您可以變更它們的名稱和顏色。

如需自訂條件的詳細資訊，請參閱[自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)。
