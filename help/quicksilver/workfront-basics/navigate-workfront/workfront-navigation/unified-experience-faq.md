---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Adobe Unified Experience常見問題集
description: '[!DNL Workfront]和Adobe Experience Cloud之間的幾項功能不同，當您將[!DNL Workfront]執行個體移轉至統一體驗時，可能會有一些問題。'
author: Courtney
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/Axlk02Ilq5Y-jNBpEx76gNmZ3mF04sh4JNJpcx-DcQw'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 3da69fe6ab5bdb843e17bd5ae2ffa985bf2b5cc4
workflow-type: tm+mt
source-wordcount: '48'
ht-degree: 2%
---
# [!DNL Adobe Unified Experience]常見問題集

<!--Remove me January 2027-->

>[!NOTE]
>
>由於所有Workfront組織現在都會使用Adobe Unified Experience來存取Workfront，因此本文已移除。

<!--

The [!DNL Adobe Unified Experience] for [!DNL Workfront] allows you to manage all of your [!DNL Adobe] applications in one place with a single login. The [!DNL Adobe] navigation area is integrated seamlessly with [!DNL Workfront]. A few features are different, and you might have some questions as your [!DNL Workfront] instance is migrated to the unified experience.

For information about how to log in to the [!DNL Adobe Unified Experience], see [[!DNL Adobe Unified Experience] for [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Comparison of [!DNL Adobe Unified Experience] and [!DNL Workfront only] experience

Only customers using the [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] can access the [!DNL Adobe Unified Experience]. Customers who have not yet migrated will see the [!DNL Workfront only] experience, without the ability to switch between [!DNL Adobe] applications.

This table describes some features that differ between the two experiences.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] only experience |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Main Menu] is on the left ![Main Menu](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Main Menu] is on the right ![Main Menu](assets/main-menu-icon.png) |
| A single login URL is available for all [!DNL Adobe Experience Cloud] applications | Log in to [!DNL Workfront] with a custom [!DNL Workfront] URL |
| An "organization switcher" allows you to move between [!DNL Workfront] organizations and environments | The "organization switcher" is not available |
| Navigation includes a top level navigation area for [!DNL Adobe] products, [!DNL Adobe] notifications, help, and your user profile, in addition to the [!DNL Workfront] navigation bar | Navigation includes the [!DNL Workfront] navigation bar only |
| Help is accessible via the [!UICONTROL Main Menu] and top navigation area | Help is accessible via the [!UICONTROL Main Menu] and [!DNL Workfront] navigation bar |
| The proofing viewer opens in a new tab | The proofing viewer opens inside Workfront |
| URL used to access Workfront is `experience.adobe.com` | URL used to access Workfront is `(CompanyName).my.workfront.adobe.com` |
| Date format (such as MM/DD/YYYY) is based on Unified Experience language settings. If the user has not updated their language settings, `en-US` settings are used. | Date format (such as MM/DD/YYYY) is based on browser preferences |

{style="table-layout:auto"}

## Frequently asked questions

### How do I determine whether I am using Adobe Unified Experience or Adobe Workfront?

To determine whether your organization is on the Adobe Unified Experience, examine the URL that you use to access Workfront.

| URL | Adobe Experience|
|------------|------------|
| (CompanyName).my.workfront.com | Workfront experience |
| experience.adobe.com | Adobe Unified Experience |

### How can I learn more about the [!DNL Adobe Admin Console]?

For information about the [!DNL Admin Console], review these articles:

* [Prepare for the [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Platform-based administration differences ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] overview](https://helpx.adobe.com/tw/enterprise/using/admin-console.html)

### What do I as a customer need to do to facilitate the migration?

Existing customers will be contacted to schedule migrations. The migration team support colleagues will walk customers through the process, advise on [!DNL Admin Console] setup, and provide links to documentation needed to make the move as simple and hassle-free as possible. Review the [[!DNL Adobe Business Platform] and [!DNL Admin Console] FAQ](https://experienceleague.adobe.com/zh-hant/docs/support-resources/adobe-support-tools-guide/workfront/faq) for more information.

### How are you handling [!DNL Adobe Admin Console] for companies that already have this enabled for federated IDs differently than [!DNL Workfront] SSO is set up?

[!DNL Adobe Admin Console] has the option to include [!DNL Workfront], replacing SSO with Adobe's Identity Management System (IMS). All user provisioning happens in the [!DNL Admin Console], and users will see the [!DNL Adobe] login screen to get to [!DNL Experience Cloud] where they will see [!DNL Workfront] as an option (if they are granted access to it).

### How does this impact customers that already have the AEM admin panel for [!DNL Adobe Assets] – but the SSO is configured differently than [!DNL Workfront?]

Once [!DNL Workfront] is added as an [!DNL Admin Console] application, you should not have to do anything else for [!DNL Workfront] to leverage the existing SSO setup you have for [!DNL Adobe Assets].

### How does this affect those that are set up with SSO?

SSO is set up in the [!DNL Admin Console] and inherited by the [!DNL Workfront] application.

### Is SSO with our internal [!DNL Active Directory] still going to be an option with Adobe's Identity Management System (IMS)?

IMS is a replacement for SSO and functions mostly the same. All user permissions are granted and provisioned in [!DNL Adobe Admin Console], and the user will see the [!DNL Adobe] login screen where they can choose "[!UICONTROL Personal Account]" or "[!UICONTROL Company Account]" to log in (if you have [!DNL Active Directory], most will log in with a company account).

### For those that are not using SSO, does the [!DNL Workfront] login URL change?

The login URL will change; however, the old URL will redirect to the new login URL, so you should retrain your users where to go.

### Will aliases we have set up still work, or are the [!DNL Workfront] links changing with this migration?

[!DNL Workfront] redirects/aliases are available to get to the homepage.

### Will there be a time when the redirects are disabled? Or will we always be able to type in my.company.workfront.com?

You'll always be able to use any custom URLs. After you click any of those links, it will direct you to [!DNL Workfront] and show a different URL. However, it is a better [!DNL experience] to log in to experience.adobe.com, and bookmark links from within [!DNL Experience Cloud]. Less redirecting equals less lag time/loading time.

### Will direct links to request queues be broken?

All direct links should redirect to the new URL patterns. However, if you have distributed links to people, you should send an update to leverage the direct link and prevent delays in getting to the expected page.

### Will we migrate to [!DNL Experience Cloud] globally or can we select for certain users (not all our users even use other Adobe products)?

The entire [!DNL Workfront] customer account will be migrated. It cannot be done on a user-by-user basis.

### Will all [!DNL Workfront] users have to log in via [!DNL Experience Cloud]? Or just administrators?

Yes, all users will log in via [!DNL Experience Cloud]. The Adobe Identity Management System (IMS) login will replace SSO. It's a very similar experience, just a different login screen.

### Will users have to link their [!DNL Adobe] accounts to their [!DNL Workfront] accounts if they already have both?

Yes, there is a process for this, and more details will be provided when it's time for your organization to move to IMS.

### What happens to the [!DNL Workfront] users who don't have an [!DNL Adobe] account?

Users who haven't been granted access in [!DNL Adobe Admin Console] to get into [!DNL Workfront] must create a "[!UICONTROL personal account]" or an [!DNL Adobe] ID account to be able to log in. This sends an email to the administrator to approve or reject their request, and it additionally enables the admin to configure what type of access that user has. When they log in, they will go to experience.adobe.com, enter their email address, and choose [!UICONTROL Personal Account]. From there, they will be able to access [!DNL Workfront].

### What if we don't have any [!DNL Adobe] products other than [!DNL Workfront?]

It is still recommended that your organization migrate to the [!DNL Adobe Unified Experience]. You will receive an [!DNL Adobe] ID along with the benefits listed above.

### We have external users included in our [!DNL Workfront] instance. We wouldn't want them to have access to any other products included in [!DNL Adobe]. How would we limit their access within the console?

[!DNL Admin Console] gives admins a lot of control over what users can and cannot access. Whenever an external user wants access, they need to create an [!DNL Adobe] ID, which sends an email to the administrator. The administrator can then accept or reject access to a product and define what they can/cannot access for products owned by that organization. Then, the [!DNL Workfront] System Administrator can go into the [!UICONTROL Users] area of [!DNL Workfront] to make any more granular permissions for the external user.

### Group Admins are used to create people in [!DNL Workfront]. With the move to [!DNL Experience Cloud], will group admins still be able to create people?

Yes, user creation is still possible through [!DNL Workfront]. Those users can be added to [!DNL Experience Cloud] automatically. You can also set up your group admins as product owners in the [!DNL Admin Console] to allow them to assign [!DNL Workfront] to users.

### What is the deadline to switch over to [!DNL Experience Cloud]?

There is no deadline currently to move to [!DNL Adobe Experience Cloud]. We're working with customers to let them choose when they're ready to make the move.

### Will our support team need to do anything for this change?

If the support team is responsible for creating new users, then they will need to become familiar with the [!DNL Admin Console] interfaces used to create users and assign an entitlement to Workfront. Otherwise, there is likely no significant change for your internal support team.

### How does this impact integrations we have through the API function?

The existing URL path will continue to be available for API traffic. You should not need to do anything to update the endpoints in your integrations. However, direct login through username and password will not be supported – you must use an API key, with the exception being [!DNL Workfront Fusion] connectors.

### What about [!DNL Creative Cloud] users? How does the migration affect them? Are there any advantages for them?

There is no impact to [!DNL Creative Cloud] users with the migration to [!DNL Adobe Unified Experience].

### Will logins change for [!DNL Workfront] mobile users?

[!DNL Workfront] mobile users should not be affected by the migration to [!DNL Adobe Unified Experience].

### JumpSeat is not working with the [!DNL Adobe Unified Experience], how can I resolve this? 

JumpSeat works with the [!DNL Adobe Unified Experience], but requires a configuration update. Using the JumpSeat admin panel, change the application URL from `workfront.com` to end with `.workfront.adobe.com`

-->
