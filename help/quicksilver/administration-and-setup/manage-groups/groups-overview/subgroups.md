---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: 子群組概述
description: 您最多可以在一個群組下建立14層子群組。 在這些層級的任一層級上，您可以建立不限數量的平行子群組。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# 子群組概述

您最多可以在一個群組下建立14層子群組。 在這些層級的任一層級上，您可以建立不限數量的平行子群組。 如需指示，請參閱[建立子群組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。

如需群組的相關資訊，請參閱[群組概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md)。

## 子群組會繼承哪些內容？

子群組會繼承其父群組的成員資格。 因此，子群組中的使用者和群組對於所有物件的可見度、許可權和存取權，與屬於他們共用之父群組的使用者和群組相同。

此外，子群組會自動繼承其最上層群組的群組管理員，但您也可以指派子群組的成員擔任其群組管理員。

>[!TIP]
>
>有時候，您可能會想要使用子群組將多位使用者新增至現有群組，以便讓他們存取所需的物件。
>
>例如，假設您有一組服務檯技術人員和另一組IT主管。 服務檯群組擁有特定請求佇列的許可權。 您想要將IT主管新增至服務檯群組，讓他們也能擁有請求佇列的許可權。 如果沒有子群組功能，您必須手動將IT主管新增到服務檯群組，這樣可能會效率低下，而且難以管理。 如果您將IT主管群組作為子群組新增至服務檯群組，只需一次變更即可更快速地完成這項工作。

>[!NOTE]
>
>如果將使用者分別新增至子群組及其父群組，則從其中一個群組移除使用者並不會將該使用者從另一個群組移除。 如果您不想讓使用者擁有父群組的允許存取權，您必須將使用者從子群組和父群組中移除。

## 公開和私人子群組

對於公用群組，任何擁有編輯使用者存取許可權的使用者（在群組內或群組外），都可以將該群組新增到其他使用者的設定檔中。 他們無法為私人群組執行此操作。

您只能在具有多個層級的群組階層中的頂層父群組上編輯此選項。 父群組的所有子群組都會繼承其設定。

如果您在公開群組下建立子群組，預設情況下該子群組也是公開的。 如需建立群組及公開群組的詳細資訊，請參閱[建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)。 如需編輯使用者所需存取許可權的詳細資訊，請參閱[授予使用者存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

您新增至現有群組的任何群組都會自動變成子群組，而不再是主要群組。 但是，除了屬於新父群組的所有專案、任務和問題狀態之外，子群組會保留其現有使用者，以及與專案、問題和任務的任何關聯。

## 子群組的群組管理員

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

建立或編輯子群組時，您可以將子群組成員指派為子群組的群組管理員。 如需指示，請參閱文章[建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的[&#128279;](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create)。

或者，您也可以將子群組的管理權交給群組管理員，由他們指定給該子群組之上的群組。 建立子群組時，上方群組的群組管理員擁有管理子群組的自動存取權。

>[!NOTE]
>
>如果您將使用者新增至子群組，並且該使用者是該子群組上任何位置的群組管理員，則該使用者具有管理該子群組的管理許可權，即使未被指派為該子群組的群組管理員。

若要瞭解哪些動作適用於管理Workfront系統的Adobe Workfront管理員、管理最上層群組的群組管理員以及管理子群組的群組管理員，請參閱[不同型別的管理員允許的動作](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md)。
