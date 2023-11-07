---
content-type: api
product-area: user-management
navigation-topic: general-api
title: 透過API停用使用者
description: 透過API停用使用者
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b06cce-4622-4739-b9f3-2edb9101c099
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# 透過API停用使用者

當使用者離開您的組織時，您可以停用使用者，將其Adobe Workfront授權提供給其他使用者使用，並防止他們不慎指派工作。 透過停用使用者，您可以保留其工作歷史記錄，包括其工作指派及其與附註、時數及檔案的關聯。

若要深入瞭解如何停用使用者，請參閱&quot; [停用或重新啟用使用者](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

如需使用核心API的相關資訊，請參閱 [API基本概念](../../wf-api/general/api-basics.md).

若要透過API停用使用者：

1. 使用以下API請求產生API金鑰：

```
<domain>.my.workfront.com/attask/api/v15.0/user?action=generateApiKey&username=`username`&password=`password`&method=PUT`
```

1. 找到您要停用之使用者的GUID。

   1. 使用以下API請求為系統中的所有使用者擷取GUID，請注意 **isActive** 欄位顯示 **true** 適用於目前使用中和 **false** 針對已停用的使用者：

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/search?fields=isActive
```

1. 找到您要停用之使用者的GUID，使用下列專案 **PUT** 要求變更使用者的 **isActive** 欄位值至 **false**：

```
<domain>`.my.workfront.com/attask/api/v15.0/USER/`<user's GUID>`?updates={"isActive":"false"}&method=put&apiKey=`<apiKey>`&fields=isActive
```

1. 回應會顯示 **isActive** 欄位值已從 **true** 至 **false**&#x200B;表示使用者已停用：

<!-- [Copy](javascript:void(0);) -->
<pre><code>{<br>&nbsp;&nbsp;&nbsp;&nbsp;data:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ID:&nbsp;"592125e60089b88fae8b51c08383e144",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;name:&nbsp;"Tyler Reid",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objCode:&nbsp;"USER",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;isActive:&nbsp;false&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}<br>}<br></code></pre>
