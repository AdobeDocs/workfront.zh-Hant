---
title: 使用Adobe Workfront Planning時的授權型別概觀
description: 除了物件的許可權外，您對Adobe Workfront Planning的存取權還取決於您的授權型別。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# 使用Adobe Workfront Planning時的授權型別概觀

{{maestro-important-intro}}

您的Adobe Workfront授權型別會與您的Adobe Workfront Planning許可權搭配使用，提供您檢視、貢獻或管理工作區的存取權。 <!--add more objects here when we can grant other object-specific permissions-->

擁有所有授權型別的使用者可以檢視、建立、編輯或管理Workfront Planning檢視。

本文說明Workfront中所需的授權型別，以及根據每種授權型別授予Workfront Planning中工作區的許可權。

當使用Workfront規劃功能時，具有較低層級授權型別的使用者已限制對工作區的許可權。

>[!INFO]
>
>**範例：**
>
>請求者（或根據新授權模型的共同作業人員）無法貢獻或管理工作區及其物件。
>
>共用方塊中會顯示當使用者擁有較低層級的授權時，無法授予他們貢獻或管理工作區的許可權。
>
>![](assets/permissions-grayed-out-for-requestor-user.png)


如需Workfront Planning中物件許可權的相關資訊，請參閱 [在Adobe Workfront Planning中共用許可權的概觀](/help/quicksilver/maestro/access/sharing-permissions-overview.md).

## Workfront授權型別與Workfront Planning許可權之間的關係

下表說明Adobe Workfront中使用者的授權型別之間的關係，以及您可以根據該授權授予他們給Adobe Workfront Planning物件的許可權等級。

將使用者許可權授予工作區也會授予他們記錄型別、記錄和欄位的許可權。


| Adobe Workfront授權型別* | Adobe Workfront Planning中允許的許可權 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 新增：標準 <br> 或 <br>目前：計畫 | 使用者可以建立和管理工作區、記錄型別和記錄。<br> 系統管理員擁有所有工作區的管理許可權，包括他們未建立的工作區。 |
| 新增：淺色 <br> 或 <br>目前：工作 | 使用者可以貢獻並檢視與他們共用的工作區，以及該工作區的記錄型別和記錄。 <br> 使用者擁有貢獻許可權，可在工作區中建立、編輯、刪除記錄。 |
| 新增：投稿人 <br> 或 <br>目前：檢閱者或要求者 | 使用者可以檢視與其共用的工作區，以及這些工作區的記錄型別和記錄。 <br> 使用者無法建立、編輯或刪除記錄型別或記錄。 |

*如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).