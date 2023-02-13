---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: 子組概述
description: 在一個組下最多可以建立14個子組級別。 在任一級別上，可以建立不限數量的並行子組。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# 子組概述

在一個組下最多可以建立14個子組級別。 在任一級別上，可以建立不限數量的並行子組。 如需指示，請參閱 [建立子組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

如需群組的相關資訊，請參閱 [群組概觀](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## 子組會繼承什麼？

子組將繼承其父組的成員資格。 因此，子組中的用戶和組與屬於它們共用的父組的用戶和組具有相同的可見性、權限和對所有對象的訪問權限。

此外，子組會自動繼承其頂級組的組管理員，但您也可以分配子組的成員作為其組管理員。

>[!TIP]
>
>有時候，您可能會想要使用子組向現有組添加多個用戶，以便他們可以訪問他們需要的對象。
>
>例如，假設您有一組服務台技術人員和一組單獨的IT主管。 服務台組具有特定「請求隊列」的權限。 您想要將IT控制器添加到幫助台組，以便它們也擁有「請求隊列」的權限。 如果沒有子組功能，您必須手動將IT控制器添加到幫助台組中，這可能會效率低下且難以管理。 如果將IT控制器組添加到幫助台組中作為子組，則只需更改一次即可更快地完成此任務。

>[!NOTE]
>
>如果將用戶分別添加到子組和其父組，則從其中一個組中刪除該用戶並不會從另一個組中刪除該用戶。 如果您不希望用戶具有父組的訪問權限，則必須同時從子組和父組中刪除該用戶。

## 公共和私有子組

對於公用群組，任何具有編輯使用者存取權的使用者（進入或退出群組）都可將群組新增至其他使用者的設定檔。 他們無法為私人群組執行此操作。

您只能在具有多個層級之群組階層的上層父群組上編輯此選項。 父組的所有子組都會繼承其設定。

如果在公用的組下建立子組，預設情況下，該子組也為公用。 如需建立群組並將其公開的詳細資訊，請參閱 [建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 如需編輯使用者所需存取權的詳細資訊，請參閱 [授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

添加到現有組的任何組都會自動成為子組，不再是主組。 但是，除了屬於新父組的所有項目、任務和發放狀態之外，子組還保留其現有用戶以及與項目、問題和任務的任何關聯。

## 子組的組管理員

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

在建立或編輯子組時，可以將子組成員作為組管理員分配給該子組。 如需指示，請參閱 [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) 在文章中 [建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

或者，您也可以將子組的管理保留給分配給上面組的組管理員。 建立子組時，其上的組的組管理員可以自動訪問管理子組。

>[!NOTE]
>
>如果向子組添加用戶，並且該用戶是子組上方某個組的組管理員，則該用戶具有管理子組的管理權限，即使未被分配為該子組的組管理員。

要了解管理Workfront系統的Adobe Workfront管理員、管理頂級組的組管理員和管理子組的組管理員可以執行哪些操作，請參閱 [允許對不同類型的管理員執行的操作](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
