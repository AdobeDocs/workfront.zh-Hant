---
title: 主群組概觀
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: 主群組會在使用者的設定檔中指派。 所有使用者都必須有「主群組」。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# 主群組概觀

主群組會在使用者的設定檔中指派。 所有使用者都必須有「主群組」。 一個使用者可以屬於多個群組，但他們只能有一個主群組。 如需群組的詳細資訊，請參閱[群組概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md)。

雖然系統中的任何現有群組都可以指派為使用者的「主群組」，我們建議您建立和指派代表大型組織單位的新群組。

建立主群組時，請考量您的組織如何劃分Adobe Workfront使用者。 以下提供一些建議，可決定應該使用哪一種型別的群組作為主群組：

* 代表部門的群組，例如IT或行銷
* 由不同預算管理的群組
* 位於不同區域或區域的群組
* 群組由屬於相同成本中心的多個團隊組成

>[!NOTE]
>
>如果您需要重新組織主群組為組織單位，您需要>
>1. 建立新群組，如[建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中所述。
>1. 如[編輯使用者設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)中所述，將新群組重新指派為使用者的主群組。
>

## 配置範本管理

將版面配置範本指派給群組時，所有將該群組指派為其主群組的使用者都可以看到版面配置範本中指定的設定。

如果版面配置範本指派給主群組，則只有指派給該主群組的使用者會看到它。

如需詳細資訊，請參閱[建立和管理配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中的[建立和管理配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

## 授權管理

每個使用者只能指派給一個主群組，這讓管理授權計數變得更加容易。

Workfront管理員可選擇設定主群組的授權數量上限。

設定最大授權數量可讓Workfront管理員防止業務單位使用為其他業務單位購買的Workfront授權。

如需詳細資訊，請參閱[管理您系統中的可用授權](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)。
