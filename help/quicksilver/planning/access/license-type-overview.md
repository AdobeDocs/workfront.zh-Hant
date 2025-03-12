---
title: 使用Adobe Workfront Planning時的授權型別概觀
description: 除了物件的許可權外，您對Adobe Workfront Planning的存取權還取決於您的授權型別。 並非組織中的所有使用者都有相同的存取權和許可權來使用Adobe Workfront Planning。 本文說明使用者對Adobe Workfront Planning的存取層級。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---


# 使用Adobe Workfront Planning時的授權型別概觀

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

您的Adobe Workfront授權型別與您的Adobe Workfront Planning許可權搭配使用，以提供下列存取權：

* 檢視、貢獻或管理工作區<!--<span class="preview">or record types</span>-->
* 檢視或管理檢視。

如需Workfront Planning中物件的許可權相關資訊，請參閱[在Adobe Workfront Planning中共用許可權概觀](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

如需有關存取Workfront Planning的資訊，請參閱[Adobe Planning存取總覽](/help/quicksilver/planning/access/access-overview.md)。

## Workfront授權型別與Workfront Planning許可權之間的關係

下表說明Adobe Workfront中使用者的授權型別之間的關係，以及您可以根據該授權授予他們給Adobe Workfront Planning物件的許可權等級。

將使用者許可權授予工作區也會授予他們記錄型別、記錄和欄位的許可權。

除了使用者擁有的工作區許可權外，您還必須授予使用者各別的檢視許可權，才能存取和管理檢視。


<div class="preview">

使用記錄型別許可權時，請考慮下列事項：

* 使用者會自動從工作區繼承記錄型別許可權。
* 當使用者具有工作區的管理許可權，他們無法擁有記錄型別的較小存取許可權。
* 使用者對記錄型別的許可權不能超過他們對該記錄型別所屬的工作區的許可權。

</div>

| Adobe Workfront授權型別* | Adobe Workfront Planning允許的最高許可權 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 標準 | <p>使用者可以管理工作區<span class="preview">、記錄型別、</span>和檢視。 他們可以建立、編輯或刪除工作區、記錄型別、記錄、欄位和檢視。</p> <br> <p>系統管理員擁有所有工作區的管理許可權，包括他們未建立的工作區。</p> |
| 輕度或貢獻者 | <p>使用者可以檢視與他們共用的工作區，以及這些工作區的記錄型別、記錄和欄位。</p> <br> <p>使用者可以檢視與他們共用的檢視，但無法建立自己的檢視。 </p><br> <p>使用者無法建立、編輯或刪除工作區、記錄型別、記錄或欄位。</p> |

*舊版Workfront授權無法使用Workfront規劃。
如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


<!--OLD 

| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

### 授權型別和工作區許可權

只有擁有標準授權的使用者才能擁有工作區<span class="preview">和記錄型別</span>的Contribute或Manage許可權。 擁有所有其他授權型別的使用者可以擁有工作區<span class="preview">的檢視許可權，以及與其共用的記錄型別</span>。

系統管理員可以檢視系統中的所有工作區，即使是他們未建立的工作區。

<!--does the shot below need to be replaced for record types??-->

>[!INFO]
>
>**範例：**
>
>貢獻者或輕度授權使用者無法貢獻或管理工作區及其物件。
>
>共用方塊中會顯示當使用者擁有較低層級的授權時，由於這些許可權層級變暗，因此無法授予他們參與或管理工作區的許可權。
>
>![參與者使用者在工作區上的許可權顯示為灰色](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### 授權型別和檢視許可權

只有具有Standard授權的使用者才能擁有檢視的管理許可權。 具有所有其他授權型別的使用者可以擁有與其共用檢視的檢視許可權。

>[!INFO]
>
>**範例：**
>
>貢獻者或輕度授權使用者無法管理檢視。 他們可以套用臨時篩選器、排序或分組到他們可以存取的檢視。
>
>共用方塊中會顯示當使用者擁有較低層級的授權時，無法授予他們管理檢視的許可權，因為這些許可權層級會變暗。
>
>![檢視共用](assets/permissions-grayed-out-for-light-user.png)上輕度使用者的許可權顯示為灰色
