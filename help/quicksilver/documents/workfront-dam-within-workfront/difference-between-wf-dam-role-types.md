---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Adobe Workfront授權角色型別與Adobe Workfront DAM角色型別的比較
description: Adobe Workfront管理員會使用存取層級來決定使用者可在應用程式中執行的動作。
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 2%

---

# Adobe Workfront授權角色型別與Adobe Workfront DAM角色型別的比較

Adobe Workfront管理員會使用存取層級來決定使用者可在應用程式中執行的動作。

* 在Workfront中，授權會決定使用者的存取層級。
* 在Workfront DAM中，角色型別會定義使用者對DAM中資產的存取權。

因為授權型別和角色型別不可互換，在一個應用程式中具有存取層級並不意味著在另一個應用程式中具有存取權。 例如，在Workfront中擁有工作授權的使用者，不會在Workfront DAM中自動獲派貢獻者角色。

## Workfront 授權類型

作為Workfront管理員，您可以透過指派授權型別來定義使用者擁有的存取層級。 每個授權都隨附一組預設存取功能，您可以在將授權指派給使用者之前修改這些功能。 

您使用授權可決定使用者在Workfront中可以檢視和執行的操作。 Workfront提供五種授權型別：

* 計劃
* 工作
* 檢閱
* 請求
* 外部

如需Workfront中不同授權型別的說明，請參閱[舊版授權概觀](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)。

## Workfront DAM角色型別

身為Workfront DAM Workfront管理員，您可以指派角色型別給使用者，以定義使用者對資產的存取權。 此外，角色型別會指定使用者可在DAM中工作的區域。

建立使用者存取許可權時，角色型別可與群組搭配使用。 群組可控制使用者對資料夾及資產本身的存取權。 角色型別會決定使用者對資產可採取的動作。 所有DAM使用者必須至少與一個群組相關聯。 若要深入瞭解角色型別和存取設定，請參閱Workfront DAM的說明。

Workfront DAM中有四種不同的角色型別可用：

### Brand Portal

具有此角色型別的使用者只能存取DAM中的Brand Connect入口網站。 在入口網站中，使用者可以檢視和下載他們有權使用的資產。

Brand Portal使用者可以透過建立和共用燈箱與其他人共同作業。

### 一般使用者

具有此角色型別的使用者可以從Workfront DAM和Brand Connect入口網站檢視及下載資產。

一般使用者也可以藉由建立和共用燈箱來與其他使用者共同作業。

### 貢獻者

具有此角色型別的使用者可存取Workfront DAM和Brand Connect入口網站。

貢獻者可以檢視、下載、上傳、編輯、移動和刪除其有權存取的資產和資料夾。 此外，貢獻者可以透過建立和共用燈箱與其他人共同作業。 

### 管理員

Workfront管理員可存取Brand Connect入口網站和Workfront DAM中的所有專案，包括已過期或處於非使用中狀態的資產。

若要擁有管理員存取權，具有「管理員」角色型別的使用者必須在「管理員群組」中。
