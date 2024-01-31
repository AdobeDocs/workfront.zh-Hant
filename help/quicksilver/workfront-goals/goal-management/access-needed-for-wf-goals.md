---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: 使用Workfront目標的需求
description: 在存取Adobe Workfront目標之前，您的Adobe Workfront管理員必須確定已符合某些條件。
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 使用Workfront目標的需求

在存取Adobe Workfront目標之前，您的Adobe Workfront管理員必須確認下列所有條件皆已符合：

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* 您的組織必須購買正確的Workfront目標授權。 如需詳細資訊，請參閱區段 [取得Workfront目標組織存取權](#obtain-workfront-goals-organization-access)本文章內容。

* 指派正確的Workfront授權型別。 有關指派許可證型別和存取層級的資訊，請參閱區段 [更新授權型別和存取層級設定](#update-license-types-and-access-level-settings) 本文章內容。

>[!NOTE]
>
>具有外部授權型別的使用者無法存取Workfront目標。

* 讓您存取存取存取層級中的目標。 如需詳細資訊，請參閱 [授予Adobe Workfront目標的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* 指派包含主功能表中目標區域的版面配置範本。

  >[!NOTE]
  >
  >必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「目標」區域。

  如需詳細資訊，請參閱區段 [將Workfront目標新增至版面配置範本](#add-workfront-goals-to-a-layout-template) 本文章內容。

* 如果您必須修改您未自行建立的目標，則目標建立者必須與您共用目標，並授予您管理目標的許可權。

  如需詳細資訊，請參閱區段 [與其他使用者共用個別目標](#share-individual-goals-with-other-users) 本文章內容。

## 取得Workfront目標組織存取權 {#obtain-workfront-goals-organization-access}

<!--drafted for P&P release: 

If your company has a current Workfront plan, you must have one of the following:

* An Ultimate Workfront plan. Workfront Goals are included in this plan. 
* A Select or higher Workfront plan and a separate Workfront Goals license. -->

<!-- drafted for P&P - add this to the sentence below at release: 

If your company has a legacy Workfront plan, -->

除了Workfront授權外，您的組織還必須購買額外授權，使用者才能存取Workfront目標。 貴組織購買額外授權後，Workfront會為您的帳戶啟用Workfront目標。 如需購買Workfront目標授權的相關資訊，請聯絡您的Workfront客戶經理。

## 更新授權型別和存取層級設定  {#update-license-types-and-access-level-settings}

<!--drafted for P&P release: 
If your company has the current access level model, your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

* Contributor
* Light
* Standard-->

<!--drafted for P&P release: add this to the first sentence: 
If your company has the legacy access level model, -->

您的Workfront管理員必須授予您下列其中一種Workfront授權型別，才能存取Workfront目標：

* 計劃
* 工作
* 檢閱
* 請求

在您的Workfront管理員授予您其中一種授權型別後，他們還必須授予您存取層級中目標的存取權。 如需有關存取目標的資訊，請參閱 [授予Adobe Workfront目標的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

身為Workfront管理員，您可以檢視系統中的目標Workfront授權數量，並瞭解目前啟用的數量。 如需詳細資訊，請參閱 [管理系統中的可用授權](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront可讓您指派更多已購買的Workfront Goals授權。 但是，當您指派的授權超過Workfront目標合約所允許的數量時，Workfront客戶經理會聯絡您，告知您已超出合約數量。

## 將Workfront目標新增至版面配置範本 {#add-workfront-goals-to-a-layout-template}

您的Workfront或群組管理員必須指派包含主要功能表中目標區域的版面配置範本，您才能存取Workfront目標。

![](assets/layout-template-align-highlighted-350x220.png)

您的Workfront管理員或群組管理員也可以將以下專案新增到您的版面配置範本，讓您能夠輕鬆存取Workfront目標：

* 釘選索引標籤
* 讓目標區域成為您的登陸頁面

如需有關更新版面配置範本的資訊，請參閱下列文章：

* [建立及管理版面範本](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [使用版面配置範本自訂主功能表](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [使用版面配置範本自訂釘選頁面](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [使用版面配置範本自訂登入頁面](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [將使用者指派至版面配置範本](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## 與其他使用者共用個別目標 {#share-individual-goals-with-other-users}

根據預設，所有至少擁有存取層級中目標檢視存取許可權的使用者，都可以在Workfront中檢視所有目標。

任何擁有目標編輯存取許可權的使用者都可以建立目標，且他們會自動獲得對其所建立目標的「管理」存取許可權。 如果他們必須編輯其他使用者的目標，擁有這些目標管理許可權的人必須與他們分享他們未建立的目標。

如需關於與使用者共用目標及給予他們管理許可權的資訊，請參閱 [在Workfront目標中共用目標](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
