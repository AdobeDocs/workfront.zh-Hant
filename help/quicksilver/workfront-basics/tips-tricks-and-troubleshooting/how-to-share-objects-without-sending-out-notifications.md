---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 如何共用物件而不產生通知
description: 瞭解如何共用物件及防止傳送有關此變更的通知。 當您大量共用物件時，這會特別有用。
author: Alina
feature: Get Started with Workfront
source-git-commit: b14dd633edec3e9746f7f1412445b74bcd37a676
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 4%

---


# 如何共用物件而不產生通知

<!--Audited: 12/2024-->

當您在Adobe Workfront中共用物件時，您要共用物件的人員會收到有關共用的電子郵件通知。

有人與您共用物件時收到電子郵件通知是瞭解此變更的重要事項。 但是，太多的通知可能會讓使用者感到過於困惑。 如果您想一次與使用者共用大量物件，暫時停用通知將有助於避免混淆。

同時啟用下列設定時，人員會收到電子郵件通知：

* 系統或群組層級會啟用下列一或兩項事件通知：

   * 將分享物件的資訊發給使用者
   * 「物件共用至團隊」可在系統或群組層級啟用。
* 使用者設定檔中已啟用下列其中一項或兩項電子郵件通知：

   * 有人與我分享了一個物件
   * 有人與我的團隊分享了一個物件

如果您需要與多個人員（大量）共用多個物件，但您不希望他們收到有關此變更的電子郵件通知，請執行以下操作：

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能共用物件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>新授權： Standard</p> 
   或
   <p>目前授權：計畫</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視您要共用之物件的存取許可權或以上許可權</p>
   <p>編輯使用者的存取權</p>
   <p><b>附註</b></p>
   <p> 您必須是系統或群組管理員，才能檢查系統或群組的事件通知狀態</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視您要共用之物件的許可權或更高的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共用物件而不產生通知

1. 確定系統或群組層級已啟用下列&#x200B;**事件通知**：

   * **物件共用給使用者**
   * 系統或群組層級&#x200B;**已啟用**&#x200B;與Team共用物件。

   如需詳細資訊，請參閱[設定系統中每個人的事件通知](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

   如果未啟用這些事件通知，則不會將有關共用物件的通知傳送給使用者。 如果已啟用其中一項或兩項功能，請繼續下列步驟。

{{step-1-to-users}}

1. 在清單中選取多個使用者，然後按一下&#x200B;**通知** > **雜項**。
1. 停用下列一或兩個通知（視系統或群組層級啟用哪些通知而定）：

   * **有人與我共用一個物件**
   * **有人與我的團隊共用一個物件**

   在停用通知之前，請確定所有選取的使用者都已選取這些通知。 如此一來，您可以在共用物件後，為全部的物件大量重新啟用它們。

1. 按一下「**儲存變更**」。
1. 前往您要共用的物件清單，並選取物件，然後按一下清單頂端的&#x200B;**共用**&#x200B;圖示。

   如需大量共用物件的相關資訊，請參閱[共用物件](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

1. 返回您為其停用通知的使用者清單，並選取相同的使用者。
1. 在清單中選取相同的使用者，然後按一下&#x200B;**通知** > **雜項**。
1. 啟用下列通知之一或兩者（視系統或群組層級所啟用的通知而定）：

   * **有人與我共用一個物件**
   * **有人與我的團隊共用一個物件**

1. 按一下「**儲存變更**」。

   這些物件已與選取的使用者共用，他們中沒有收到有關此變更的任何電子郵件通知。






