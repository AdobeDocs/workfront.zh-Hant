---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Adobe Workfront和Workfront Proof之間的使用者同步
description: 使用者資訊會從Adobe Workfront同步至Workfront Proof，而不會從Workfront Proof同步至Workfront。 因此，無論您何時建立或修改使用者，都必須在Workfront中進行這些變更。 您無法在Workfront Proof中變更使用者。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Adobe Workfront與Workfront Proof之間的使用者同步

使用者資訊會從Adobe Workfront同步至Workfront Proof，而不會從Workfront Proof同步至Workfront。 因此，無論您何時建立或修改使用者，都必須在Workfront中進行這些變更。 您無法在Workfront Proof中變更使用者。

以下小節提供有關從Workfront到Workfront Proof的使用者同步資訊：

## 已同步的資訊

Workfront會將下列使用者資訊同步至Workfront Proof：

* 名稱（使用者的名字和姓氏）
* 電子郵件地址

## 同步發生時

在下列情況下，使用者資訊會從Workfront同步至Workfront Proof：

* 使用者資訊會在Workfront中更新
* 在Workfront中建立使用者

根據Workfront Proof中是否存在具有相同電子郵件地址的使用者，會發生以下任一情況：

* **如果Workfront Proof中沒有具有相符電子郵件的使用者，則**

   * **已為使用者啟用校訂：**&#x200B;使用者是在Workfront Proof中建立為使用者。
   * **未針對使用者啟用校訂：**&#x200B;使用者是在Workfront Proof中建立為連絡人。

* **如果具有相符電子郵件的使用者存在於Workfront Proof中：**&#x200B;已在Workfront中為該使用者啟用校訂（如果尚未啟用），且兩個使用者之間的資訊會同步化。

  如需詳細資訊，請參閱[設定使用者的校訂存取權](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md)中的[設定使用者的校訂存取權](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md)。

  >[!IMPORTANT]
  >
  >當具有相符電子郵件的使用者存在時、在其自身或其他校訂環境中，Workfront會透過將使用者的帳戶ID新增為其電子郵件的尾碼來建立別名電子郵件地址。 例如，*username+accountid@domain.com*。 如果別名電子郵件已建立，使用者仍會收到校訂通知。
