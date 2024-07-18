---
title: 停用新授權計畫上未付費使用者的自動升級選項
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 存取，層級，系統，管理員，標準，輕量，參與者
navigation-topic: access-levels
description: 每位使用者都必須具備存取層級，才能登入及在Workfront中工作。 您可以使用存取層級來控制使用者可以檢視特定Workfront物件與區域的內容，以及對這些物件與區域執行的動作。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 58c76187-fc74-4ab4-80e8-c3e296a84f27
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 1%

---

# 停用新授權計畫上未付費使用者的自動升級選項

新計畫的所有未付費Workfront授權校訂和檔案決定受限。 當使用者達到其分配數量的決定時，他們會依預設升級至輕度授權。

您可以從設定區域停用自動升級選項。 若要深入瞭解自動升級如何運作，請參閱[非付費使用者的有限檔案與校訂決定概覽](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)。

>[!IMPORTANT]
>
>一旦停用，任何超過分配數量決定的非付費使用者都不會自動升級。

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
   <td>新計畫：標準
   <p>或</p>
   <p>目前計畫：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p></td> 
  </tr> 
 </tbody> 
</table>

## 停用非付費使用者的自動升級

{{step-1-to-setup}}

1. 展開左側導覽中的&#x200B;[!UICONTROL **系統**]，然後按一下&#x200B;[!UICONTROL **偏好設定**]。
1. 在&#x200B;[!UICONTROL **一般偏好設定**]&#x200B;區段中，勾選&#x200B;[!UICONTROL **停用存取層級內的自動升級**]&#x200B;方塊。
1. 按一下「[!UICONTROL **儲存**]」。
