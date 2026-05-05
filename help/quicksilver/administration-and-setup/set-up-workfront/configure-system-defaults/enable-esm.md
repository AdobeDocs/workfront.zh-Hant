---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 為您的組織啟用Adobe企業儲存空間
description: 您可以為貴組織啟用Adobe企業儲存，以便針對所有Adobe產品使用統一的儲存解決方案。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 48b581c7-a21a-45de-95c5-eafb0713b42e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b3c8559ddac934cc41461f88503b2fa71abaf452
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 5%

---

# 為您的組織啟用Adobe企業儲存空間

Adobe企業儲存是適用於所有Adobe產品的統一儲存解決方案。 這是雲端型儲存解決方案，可作為Adobe企業產品中資產的中央存放庫。

新客戶預設會啟用Adobe企業儲存，現有客戶也可以在續約時啟用。

如需Adobe企業儲存的詳細資訊，請參閱[Adobe企業儲存概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td><p>任何Workflow封裝</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p> <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是Workfront管理員。 </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 為您的組織啟用Adobe企業儲存空間

若要為貴組織啟用Adobe企業儲存空間：

{{step-1-to-setup}}

1. 在左側導覽中選取&#x200B;**系統**，然後選取&#x200B;**偏好設定**。
1. 向下捲動至&#x200B;**儲存偏好設定**&#x200B;區段。
1. 在「預設」下拉式功能表中，選取&#x200B;**Adobe企業儲存空間**。
1. （選擇性）如果要使用Adobe企業儲存裝置和舊版Workfront儲存裝置的組合，請選取&#x200B;**允許使用者選取儲存裝置提供者**&#x200B;核取方塊。

   >[!NOTE]
   >
   >啟用此選項可讓使用者在建立新專案時選取儲存提供者。 企業儲存體標示為「新專案」，因為它是預設的儲存提供者。 舊版Workfront儲存空間標示為「舊版專案」。
   >
   >![新專案和舊版專案選項](assets/new-esm-project.png)

1. 在「套用至」下拉式功能表中，選擇下列其中一個選項：

   - **整個組織**：此選項會將預設儲存提供者套用至您的整個Workfront環境。 每當使用者建立新專案時，都會使用預設的儲存提供者。
   - **特定群組**：此選項只會將預設儲存提供者套用至您組織內的特定群組。 每當指定群組中的使用者建立新專案時，都會使用預設的儲存提供者

1. 按一下「**儲存**」。

   >[!NOTE]
   >
   >現有專案會保留建立該專案的儲存模式。 例如，使用Adobe企業儲存空間的專案會在您變更預設儲存偏好設定後，繼續使用Adobe企業儲存空間。
