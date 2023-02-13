---
title: 首頁群組概觀
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: 在使用者的設定檔中會指派「首頁群組」。 所有使用者都必須擁有首頁群組。 一個用戶可以屬於多個組，但只能有一個家庭組。 雖然系統中的任何現有群組都可指派為使用者的「首頁群組」，但建議您建立並指派代表較大組織單位的新群組。 建立首頁群組時，請考量您的組織如何劃分Adobe Workfront使用者。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 首頁群組概觀

在使用者的設定檔中會指派「首頁群組」。 所有使用者都必須擁有首頁群組。 一個用戶可以屬於多個組，但只能有一個家庭組。 如需群組的詳細資訊，請參閱 [群組概觀](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

雖然系統中的任何現有群組都可指派為使用者的「首頁群組」，但建議您建立並指派代表較大組織單位的新群組。

建立首頁群組時，請考量您的組織如何劃分Adobe Workfront使用者。 以下提供一些建議，以決定應將哪種類型的群組當作首頁群組使用：

* 代表部門的群組，例如IT或行銷
* 由不同預算管理的組
* 位於不同區域或區域的組
* 由屬於同一成本中心的多個團隊組成的組

>[!NOTE]
>
>如果您需要將家庭組重新組織為組織單位，則需要>
>1. 建立新群組，如 [建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).
>1. 將新組重新分配為用戶的主組，如 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>


## 版面範本管理

將「配置模板」指派給組時，所有將該組指定為其「主組」的用戶都可以查看「配置模板」中指定的設定。

如果「配置模板」被分配給「主組」，則只有分配給該「主組」的用戶才能看到該佈局模板。

如需詳細資訊，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) in [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## 授權管理

每個使用者只能指派給一個首頁群組，這可讓管理授權計數更輕鬆。

Workfront管理員可以選擇為首頁群組設定最大授權計數。

設定最大授權計數，可讓Workfront管理員防止業務單位使用為其他業務單位購買的Workfront授權。

如需詳細資訊，請參閱 [管理系統中的可用許可證](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
