---
product-area: programs
navigation-topic: Create and manage programs
title: 刪除和停用計畫
description: 方案代表共用跨專案界限的共同策略、目標或目標的專案集合。 計畫是投資組合的細分，它們不能存在於投資組合之外。 計畫通常與同一投資組合中的其他計畫共用相同的資源。 您可以在程式變得無關時將其刪除或停用。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 605d1ec5-ca2e-4ff0-87e1-fa53d8ac4a95
TQID: https://experienceleague.adobe.com/nXFATsZ0uMLsgS-q4VlSQxL1Zh29QSCSAWTHxEGBgMw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 464
ht-degree: 1%

---

# 刪除和停用程式

方案代表共用跨專案界限的共同策略、目標或目標的專案集合。 計畫是投資組合的細分，它們不能存在於投資組合之外。 計畫通常與同一投資組合中的其他計畫共用相同的資源。

當方案變得無關時，您可以執行下列其中一項作業，以防止使用者將專案與方案建立關聯：

* 停用：現有專案仍與方案及其個別投資組合相關聯。 使用者嘗試將新專案與方案建立關聯時，不再將方案視為選項。
* 刪除它：現有專案會失去與方案的關聯，而直接在投資組合下移動。 使用者嘗試將其未來的專案與方案建立關聯時，不再將方案視為選項。

我們建議您停用投資組合，而不是刪除投資組合，以保留您專案的歷史資訊。 但是，有時可能必須刪除計畫。

## 存取權要求

+++ 展開以檢視存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 封裝</td>

<td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>[!UICONTROL 標準]</p><p>[!UICONTROL 計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>[!UICONTROL Edit]對投資組合和計畫的存取權 </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>投資組合的[!UICONTROL Manage]許可權</p> <p>建立方案後，預設情況下您擁有[!UICONTROL 管理]許可權。</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 刪除計畫

{{step1-to-programs}}

1. 按一下計畫名稱以開啟。
1. 按一下程式名稱右邊的&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**刪除程式**。
1. 按一下&#x200B;**是，刪除**&#x200B;以進行確認。

   程式會遭到刪除，且會發生下列情況：

   * 現有專案會失去與方案的關聯，而直接在投資組合下方移動。
   * 使用者嘗試將其未來的專案與方案建立關聯時，不再將方案視為選項。

## 停用計畫

{{step1-to-programs}}

1. 按一下計畫名稱以開啟。
1. 執行下列其中一項：

   * 按一下程式名稱右邊的&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**停用程式**。
   * 按一下程式右側的&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**編輯**

     或

     按一下左側面板中的&#x200B;**程式詳細資料**&#x200B;區段，然後取消勾選&#x200B;**使用中**&#x200B;方塊。

   程式會立即停用，且會發生下列情況：

   * 現有專案仍與方案及其個別投資組合相關聯。
   * 使用者嘗試將新專案與方案建立關聯時，不再將方案視為選項。
