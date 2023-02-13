---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Adobe Workfront授權角色類型與Adobe Workfront DAM角色類型的比較
description: Adobe Workfront管理員使用存取層級來決定使用者可在應用程式中執行的動作。
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 2%

---

# Adobe Workfront授權角色類型與Adobe Workfront DAM角色類型的比較

Adobe Workfront管理員使用存取層級來決定使用者可在應用程式中執行的動作。

* 在Workfront中，授權會決定使用者的存取層級。
* 在Workfront DAM中，角色類型會定義使用者對DAM中資產的存取權。

由於許可證類型和角色類型不可互換，因此在一個應用程式中具有訪問級別並不意味著在另一個應用程式中具有訪問權限。 例如，在Workfront中具有工作授權的使用者不會在Workfront DAM內自動獲派貢獻者角色。

## Workfront 授權類型

身為Workfront管理員，您可以指派授權類型來定義使用者擁有的存取層級。 每個許可證都附有一組預設訪問功能，您可以先修改這些功能，然後再將許可證分配給用戶。 

您可以透過授權來判斷使用者在Workfront中可以看到和執行的動作。 Workfront提供五種授權類型：

* 計劃
* 工作
* 檢閱
* 請求
* 外部

請參閱 [Adobe Workfront授權概觀](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) 以取得Workfront中不同授權類型的說明。

## Workfront DAM角色類型

身為Workfront DAM Workfront管理員，您可以將角色類型指派給使用者，以定義使用者對資產的存取權。 此外，角色類型會指定DAM中使用者可以工作的區域。

建立使用者存取權限時，角色類型可與群組搭配使用。 群組可控制使用者對資料夾和資產本身的存取權。 角色類型決定使用者可對資產採取的動作。 所有DAM使用者都至少必須與一個群組相關聯。 若要進一步了解角色類型和存取設定，請參閱Workfront DAM的說明。

Workfront DAM提供四種不同的角色類型：

### Brand Portal

具有此角色類型的使用者只能存取DAM中的Brand Connect入口網站。 在入口網站中，使用者可以檢視並下載擁有權限的資產。

Brand Portal使用者可以透過建立和共用燈箱來與他人共同作業。

### 一般使用者

具有此角色類型的使用者可從Workfront DAM和Brand Connect入口網站檢視和下載資產。

一般使用者也可以建立和共用燈箱，與他人共同作業。

### 投稿人

具有此角色類型的使用者可存取Workfront DAM和Brand Connect入口網站。

貢獻者可以檢視、下載、上傳、編輯、移動及刪除他們有權存取的資產和資料夾。 此外，貢獻者可以建立和共用燈箱，與他人共同作業。 

### 管理員

Workfront管理員可存取Brand Connect入口網站和Workfront DAM中的所有項目，包括過期或狀態非作用中的資產。

為了具有管理員訪問權限，具有管理員角色類型的用戶必須位於管理員組中。
