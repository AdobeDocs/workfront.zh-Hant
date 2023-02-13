---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: 使用Workfront目標的需求
description: 您的Adobe Workfront管理員必須先確定符合某些條件，您才能存取Adobe Workfront目標。
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 4298659c6eaf7c0370d8d88454e54aeba70f48cf
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# 使用Workfront目標的需求

您的Adobe Workfront管理員必須先確定符合下列所有條件，您才能存取Adobe Workfront目標：

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* 貴組織必須購買正確的Workfront目標授權。 如需詳細資訊，請參閱 [取得Workfront Target組織存取權](#obtain-workfront-goals-organization-access)這篇文章。

* 為您指派正確的Workfront授權類型。 有關分配許可證類型和訪問級別的資訊，請參閱 [更新許可證類型和訪問級別設定](#update-license-types-and-access-level-settings) 這篇文章。

>[!NOTE]
>
>具有外部授權類型的使用者無法存取Workfront Goals。

* 授予您存取層級中目標的存取權。 如需詳細資訊，請參閱 [授予Adobe Workfront目標的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* 為您指派「配置範本」，其中包含「主功能表」中的「目標」區域。

   如需詳細資訊，請參閱 [將Workfront目標新增至版面範本](#add-workfront-goals-to-a-layout-template) 這篇文章。

* 如果您必須修改您未自行建立的目標，則目標建立者必須與您共用目標，並為目標授予您管理權限。

   如需詳細資訊，請參閱 [與其他使用者共用個別目標](#share-individual-goals-with-other-users) 這篇文章。

## 取得Workfront Target組織存取權 {#obtain-workfront-goals-organization-access}

<!--drafted for P&P release: 

If your company has a current Workfront plan, you must have one of the following:

* An Ultimate Workfront plan. Workfront Goals are included in this plan. 
* A Select or higher Workfront plan and a separate Workfront Goals license. -->

<!-- drafted for P&P - add this to the sentence below at release: 

If your company has a legacy Workfront plan, -->

您的組織除了Workfront授權外，還必須購買額外的授權，才能讓您的使用者存取Workfront Targets。 貴組織購買其他授權後，Workfront會為您的帳戶啟用Workfront Targets。 如需購買Workfront Target授權的相關資訊，請聯絡您的Workfront客戶經理。

## 更新許可證類型和訪問級別設定  {#update-license-types-and-access-level-settings}

<!--drafted for P&P release: 
If your company has the current access level model, your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

* Contributor
* Light
* Standard-->

<!--drafted for P&P release: add this to the first sentence: 
If your company has the legacy access level model, -->

您的Workfront管理員必須授予您下列其中一種Workfront授權類型，才能存取Workfront目標：

* 計劃
* 工作
* 檢閱
* 請求

在您的Workfront管理員授予您其中一種授權類型後，這些授權類型也必須授予您存取層級中的目標存取權。 如需存取目標的相關資訊，請參閱 [授予Adobe Workfront目標的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

身為Workfront管理員，您可以檢閱系統中的Workfront Target授權數量，並了解目前已啟用的數量。 如需詳細資訊，請參閱 [管理系統中的可用許可證](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront可讓您指派已購買的更多Workfront Target授權。 不過，當您指派的授權數超過Workfront目標合約允許的數量時，Workfront客戶經理會聯絡您，告知您已超出合約編號。

## 將Workfront目標新增至版面範本 {#add-workfront-goals-to-a-layout-template}

您的Workfront或群組管理員必須為您指派版面範本，其中包含主功能表中的「目標」區域，您才能存取Workfront目標。

![](assets/layout-template-align-highlighted-350x220.png)

您的Workfront管理員或群組管理員也可將下列項目新增至您的配置範本，以便輕鬆存取Workfront目標：

* 固定頁簽
* 將目標區域設為您的登陸頁面

如需更新「版面範本」的相關資訊，請參閱下列文章：

* [建立和管理版面範本](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [使用版面範本自訂主功能表](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [使用版面範本自訂已固定的頁面](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [使用版面範本自訂登錄頁面](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [將使用者指派至版面範本](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## 與其他使用者共用個別目標 {#share-individual-goals-with-other-users}

依預設，在其存取層級中至少擁有「檢視」目標存取權的所有使用者，都可以檢視Workfront中的所有目標。

任何具有「編輯」目標存取權的使用者皆可建立目標，且會自動取得其所建立目標的「管理」存取權。 如果他們必須編輯其他使用者的目標，則具有這些目標之「管理」權限的人必須與他們共用他們未建立的目標。

如需與使用者共用目標及給予使用者管理權限的相關資訊，請參閱 [在Workfront目標中共用目標](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
