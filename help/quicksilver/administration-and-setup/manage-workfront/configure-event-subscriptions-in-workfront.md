---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: 在Workfront中設定事件訂閱
description: 身為Adobe Workfront管理員，您可以從設定區域建立、檢視和刪除事件訂閱，以將Workfront事件傳送至外部端點。
feature: System Setup and Administration
role: Admin
author: Courtney
source-git-commit: 5a44679115dcfda871e2fe40c0c8443649fc43cf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 5%
---

# 在Workfront中設定事件訂閱

{{highlighted-preview-article-level}}

身為Adobe Workfront管理員，您可以從設定區域建立、檢視和刪除事件訂閱。 事件訂閱會在指定事件發生時，將Workfront事件資訊傳送至外部端點。

您可以在Workfront中建立和刪除事件訂閱，但無法編輯現有訂閱。 如果您需要變更訂閱，請刪除它並建立新的訂閱。

如需有關活動訂閱的詳細資訊，請參閱[活動訂閱](/help/quicksilver/wf-api/api/event-subscriptions.md)下的文章。

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
   <td>您必須是Workfront管理員。</td>
  </tr>
 </tbody>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立事件訂閱

{{step-1-to-setup}}

1. 在左側導覽面板中，按一下&#x200B;**系統**，然後按一下&#x200B;**事件訂閱**。
1. 按一下&#x200B;**新增事件訂閱**。
1. 在&#x200B;**物件**&#x200B;欄位中，選取您要監視的Workfront物件。
1. 在&#x200B;**事件型別**&#x200B;欄位中，選取您是否要讓事件訂閱在建立、更新、刪除或共用物件時觸發。
1. 在&#x200B;**Webhook URL**&#x200B;欄位中，輸入應該接收事件裝載的端點。
1. 在&#x200B;**驗證Token**&#x200B;欄位中，輸入用來驗證端點之要求的權杖。
1. 如果您希望Workfront在傳送裝載前先進行編碼，請啟用以Base64傳送裝載的選項。
1. 如有需要，請新增一或多個篩選器，以限制會觸發訂閱的事件。 可用的濾鏡是根據選取的物件。
1. 按一下「**建立**」。

如需端點需求的資訊，請參閱[事件訂閱傳遞需求](/help/quicksilver/wf-api/general/setup-event-sub-endpoint.md)。

## 檢視事件訂閱

{{step-1-to-setup}}

1. 在左側導覽面板中，按一下&#x200B;**系統**，然後按一下&#x200B;**事件訂閱**。

在「事件訂閱」頁面中，您可以檢閱為您的環境設定的訂閱。 您也可以檢視貴組織擁有的訂閱總數，以及其中有效、停用或凍結的訂閱數。

* **已停用的訂閱**：由於多次傳送失敗，這些訂閱已自動停用。
* **凍結的訂閱**：由於傳送問題，這些訂閱已暫時凍結。

## 刪除事件訂閱

{{step-1-to-setup}}

1. 在左側導覽面板中，按一下&#x200B;**系統**，然後按一下&#x200B;**事件訂閱**。
1. 選取您要移除的事件訂閱。
1. 按一下&#x200B;**刪除**。
