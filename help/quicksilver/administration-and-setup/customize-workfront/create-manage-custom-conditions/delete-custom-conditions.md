---
title: 刪除自訂條件
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 您可以刪除自訂條件。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# 刪除自訂條件

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

## 刪除自訂條件

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **專案偏好設定** > **條件**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. 選擇對象類型的頁簽(**專案**, **任務**，或 **問題**)，您要刪除的條件位於的位置。

1. 將滑鼠指標暫留在您要刪除的條件上，然後按一下 **刪除** 圖示 ![](assets/delete.png) 在最右邊。
1. 在顯示的確認訊息中，按一下 **刪除條件**.

1. 在 **刪除條件** 框中，針對使用您正在刪除的條件的所有項目，在下拉清單中選擇新條件。

   只有當自訂條件與您要刪除的相同內建條件相等時，才可在下拉式清單中使用。 例如，如果您刪除等於「風險」的條件，則只能選擇同樣等於「風險」的自訂條件。

1. 按一下 **刪除條件**.

>[!NOTE]
>
>您無法刪除內建條件，這些條件在Target上、有風險且有問題。 不過，您可以變更其名稱和顏色。

如需自訂條件的相關資訊，請參閱 [自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
