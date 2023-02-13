---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Adobe Workfront和Workfront Proof之間的使用者同步
description: 使用者資訊會從Adobe Workfront同步至Workfront Proof;不會從Workfront Proof同步至Workfront。 因此，每當您建立或修改使用者時，都必須在Workfront中進行這些變更。 您無法在Workfront Proof內變更使用者。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Adobe Workfront和Workfront Proof之間的使用者同步

使用者資訊會從Adobe Workfront同步至Workfront Proof;不會從Workfront Proof同步至Workfront。 因此，每當您建立或修改使用者時，都必須在Workfront中進行這些變更。 您無法在Workfront Proof內變更使用者。

以下小節提供使用者從Workfront同步至Workfront Proof的相關資訊：

## 已同步的資訊

Workfront會將下列使用者資訊同步至Workfront校樣：

* 名稱（使用者的名字和姓氏）
* 電子郵件地址

## 同步發生時

在下列情況下，使用者資訊會從Workfront同步至Workfront Proof:

* 使用者的資訊會在Workfront中更新
* 使用者是在Workfront中建立

根據Workfront Proof中是否存在具有相同電子郵件地址的使用者，會發生下列任一情況：

* **如果Workfront Proof和**

   * **已為用戶啟用校對：** 使用者會在Workfront Proof中建立為使用者。
   * **未為用戶啟用校對：** 使用者會在Workfront Proof中建立為連絡人。

* **如果使用者的電子郵件符合，Workfront Proof中就會：** 在Workfront中會為該使用者啟用校對（如果尚未啟用），且資訊會在這兩個使用者之間同步。

   如需詳細資訊，請參閱 [設定使用者的校對存取權](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [設定使用者的校對存取權](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

   >[!IMPORTANT]
   >
   >當具有相符電子郵件的使用者存在時（在其自己或其他校對環境中）,Workfront會將使用者的帳戶id新增為其電子郵件的尾碼，以建立別名電子郵件地址。 例如， *username+accountid@domain.com*. 使用者在建立別名電子郵件時仍會收到校樣通知。
