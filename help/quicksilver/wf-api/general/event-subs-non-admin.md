---
content-type: api
navigation-topic: general-api
title: 以非管理員使用者身分管理事件訂閱
description: 如果您的Workfront存取權允許，則可以在您的許可權和系統設定允許的範圍內建立、檢視和刪除事件訂閱。
author: Courtney
feature: Workfront API
role: Developer
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 5%
---

# 以非管理員使用者身分管理事件訂閱

如果您的Workfront存取權允許，您可以從設定區域建立、檢視和刪除事件訂閱。 但是，您的存取權僅限於您的角色及您組織的系統設定所授權的訂閱和動作。

並非每位使用者都能使用此功能，Workfront管理員也一樣。 具有必要存取許可權的使用者只能在授予他們的範圍內管理事件訂閱。

例如，您的許可權可讓您僅管理已定義作品集的特定物件型別、事件型別或訂閱。 您不能在存取和設定允許的範圍之外管理事件訂閱。

如需管理員管理的設定，請參閱[在Workfront中設定事件訂閱](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)。

如需Event Subscription API的相關資訊，請參閱[Event Subscription API](/help/quicksilver/wf-api/general/event-subs-api.md)。

>[!NOTE]
>
>使用者只能在其許可權及組織的系統設定允許的範圍內管理事件訂閱。 存取權並不自動等同於管理員存取權。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront 封裝</td>
   <td>任何</td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront授權</td>
   <td>
    <p>標準</p>
    <p>規劃</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">存取層級設定</td>
   <td>
    <p>您必須有適當的存取權才能管理事件訂閱。</p>
    <p>您的存取權僅限為您的許可權所允許的訂閱和動作，以及您組織的系統設定。</p>
   </td>
  </tr>
 </tbody>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用事件訂閱

{{step-1-to-setup}}

1. 在左側導覽面板中，按一下&#x200B;**系統**，然後按一下&#x200B;**事件訂閱**。
1. 檢閱您可用的訂閱。
1. 僅建立、檢視或刪除屬於您授權範圍內的訂閱。

如果您沒有看到預期的選項，或無法建立或管理訂閱，請聯絡Workfront管理員，確認您的存取權是否受到角色、許可權或系統設定的限制。

## 相關文章

* [在Workfront中設定事件訂閱](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)
* [事件訂閱API](/help/quicksilver/wf-api/general/event-subs-api.md)
