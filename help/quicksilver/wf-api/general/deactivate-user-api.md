---
content-type: api
product-area: user-management
navigation-topic: general-api
title: 透過API停用使用者
description: 透過API停用使用者
author: Becky
feature: Workfront API
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# 透過API停用使用者

當使用者離開您的組織時，您可以停用該使用者、讓其Adobe Workfront授權可供其他使用者使用，並防止他們不慎被指派工作。 通過停用用戶，您可以保留其工作歷史記錄，包括其工作分配以及其與筆記、小時和文檔的關聯。

若要進一步了解停用使用者，請參閱 [停用或重新啟用使用者](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

如需使用核心API的詳細資訊，請參閱 [API基本介紹](../../wf-api/general/api-basics.md).

若要透過API停用使用者：

1. 使用下列API請求產生API金鑰：

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. 找出要停用之使用者的GUID。

   1. 使用下列API請求來擷取系統中所有使用者的GUID，請注意 **isActive** 欄位顯示 **true** 適用於目前使用中和 **false** 已停用的使用者：

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. 找到要停用的用戶的GUID，請使用以下 **PUT** 請求變更使用者的 **isActive** 欄位值 **false**:

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. 回應會顯示 **isActive** 欄位值已從 **true** to **false**&#x200B;表示用戶已停用：

<!-- [Copy](javascript:void(0);) -->
<pre></pre>
