---
title: 使用Adobe Workfront Planning時的授權型別概觀
description: 除了物件的許可權外，您對Adobe Workfront Planning的存取權還取決於您的授權型別。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# 使用Adobe Workfront Planning時的授權型別概觀

{{planning-important-intro}}

您的Adobe Workfront授權型別與您的Adobe Workfront Planning許可權搭配使用，以提供下列存取權：

* 檢視、貢獻或管理工作區
* 檢視或管理檢視。

如需Workfront Planning中物件的許可權相關資訊，請參閱[在Adobe Workfront Planning中共用許可權概觀](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

## Workfront授權型別與Workfront Planning許可權之間的關係

下表說明Adobe Workfront中使用者的授權型別之間的關係，以及您可以根據該授權授予他們給Adobe Workfront Planning物件的許可權等級。

將使用者許可權授予工作區也會授予他們記錄型別、記錄和欄位的許可權。


| Adobe Workfront授權型別* | Adobe Workfront Planning允許的最高許可權 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 新增：標準<br>或<br>目前：計畫 | 使用者可以管理工作區。 他們可以建立、編輯或刪除工作區、記錄型別、記錄和欄位。 <br>系統管理員擁有所有工作區的管理許可權，包括他們未建立的工作區。 |
| 新增：淺色、貢獻者<br>或<br>目前：工作、請求者、檢閱者 | 使用者可以檢視與他們共用的工作區，以及這些工作區的記錄型別、記錄和欄位。 <br>使用者無法建立、編輯或刪除工作區、記錄型別、記錄或欄位。 |

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

### 授權型別和工作區許可權

只有具有Standard （或Plan）授權的使用者才能擁有工作區的Contribute或管理許可權。 具有所有其他授權型別的使用者可以擁有與其共用之工作區的「檢視」許可權。

系統管理員可以檢視系統中的所有工作區，即使是他們未建立的工作區。

>[!INFO]
>
>**範例：**
>
>請求者（或根據新授權模型的共同作業人員）無法貢獻或管理工作區及其物件。
>
>共用方塊中會顯示當使用者擁有較低層級的授權時，由於這些許可權層級變暗，因此無法授予他們參與或管理工作區的許可權。
>
>![](assets/permissions-grayed-out-for-requestor-user.png)

### 授權型別和檢視許可權

只有擁有標準（或計畫）授權的使用者才能擁有檢視的管理許可權。 具有所有其他授權型別的使用者可以擁有與其共用檢視的檢視許可權。

>[!INFO]
>
>**範例：**
>
>共同作業人員（或請求者和檢閱者）無法管理檢視。 他們可以套用臨時篩選器、排序或分組到他們可以存取的檢視。
>
>共用方塊中會顯示當使用者擁有較低層級的授權時，無法授予他們管理檢視的許可權，因為這些許可權層級會變暗。
>
>![](assets/permissions-grayed-out-for-reviewer-user-on-a-view.png)


<!--Replace all of the above with this:

The table below describes the relationship between the license type of a user in Adobe Workfront and the level of permissions you can grant to them to Adobe Workfront Planning objects based on that license. 

Granting a user permissions to a workspace also grants them permissions to record types, records, and fields. 

You must grant view permissions separately from workspace permissions. 


| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | <ul><li>Users can contribute to or manage workspaces and they can manage views. They can create, edit, or delete workspaces, record types, records, fields, and views.</li> <li> System administrators have Manage permissions to all workspaces, including the ones they did not create.</li> <li> System administrators can only access views they created.</li></ul>                                                                                                                     |
|New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | <ul><li>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</li> <li>Users can access views shared with them and apply temporary filters, sorts, or groupings, but they cannot modify the views. </li><li> Users cannot create, edit, or delete workspaces, record types, records, fields, or views.</li></ul>|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->