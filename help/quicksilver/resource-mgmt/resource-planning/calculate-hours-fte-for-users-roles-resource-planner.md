---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: 計算資源規劃工具中使用者和角色的時數和FTE的概要
description: 計算資源規劃工具中使用者和角色的時數和FTE的概觀
author: Lisa
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 0%

---

# 計算資源規劃工具中使用者和角色的時數和FTE的概觀

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

您可以依時數、約當全職人數或成本，在「資源規劃工具」中顯示資源的配置與可用性。\
如需有關計算資源規劃工具中成本的詳細資訊，請參閱[計算資源規劃工具中的成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)。

「FTE」代表全時工作。 這是時間測量值，代表使用者或工作角色在一天或一週內專用於實際工作的時數。

下列資源資訊集合在「資源規劃工具」中的計算方式不同：

* 可用時數或FTE值是根據系統管理員在系統中設定資源管理偏好設定的方式計算的。\
  如需有關如何計算可用時數和FTE值的詳細資訊，請參閱[計算資源規劃工具中使用者和工作角色的可用時數或FTE](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner)。\
  如需定義Adobe Workfront系統之資源管理喜好設定的詳細資訊，請參閱[設定資源管理喜好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

* 所有其他FTE值都是根據「系統預設」排程進行計算。\
  如需有關使用FTE時所有其他值如何顯示在「資源規劃工具」中的詳細資訊，請參閱本文的[計算資源規劃工具](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner)中使用者和工作角色的所有其他時數和FTE值一節。

請務必瞭解您每個使用者及其工作角色的FTE，以便在您指派他們工作時，準確管理您的資源。

## 計算資源規劃工具中使用者和工作角色的可用時數或FTE {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [計算資源規劃工具中使用者的可用時數和FTE](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [計算資源規劃工具中工作角色的可用時數和FTE](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [計算資源規劃工具中使用者的可用時數和FTE （範例）](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### 計算資源規劃工具中使用者的可用時數和FTE {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

Workfront管理員在「設定」的「資源管理」區域中，選取使用下列其中一項，以決定如何計算使用者的可用時間：

* 系統的「預設排程」和使用者的FTE。
* 使用者的排程。

![使用者排程的系統設定](assets/setup-resource-mgmt.png)

>[!NOTE]
>
>這會決定如何在系統層次計算資源可用性。 如需定義系統之資源管理喜好設定的詳細資訊，請參閱[設定資源管理喜好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

根據此設定的設定方式，使用下列方法計算資源規劃工具中使用者的可用性（時數以及FTE可用性）：

* **預設排程**：系統的預設排程和使用者FTE是用來決定資源規劃工具中使用者的可用時數和FTE值。 使用者的排程會被忽略。 在此案例中：

   * 資源規劃工具中的&#x200B;**可用時數**&#x200B;使用下列公式計算：

     `User Available Hours = Default Schedule Hours * User FTE value`

     例如，如果預設排程每週有40小時可供工作，且使用者FTE為0.5，則使用者可在資源規劃工具中每週工作20小時。

     如需排程的詳細資訊，包括預設排程，請參閱[建立排程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

   * 資源規劃工具中使用者的&#x200B;**可用FTE**&#x200B;與使用者設定中指定的使用者FTE相同。

     例如，如果使用者FTE在使用者設定中為0.5，則使用者的可用FTE在資源規劃工具中為0.5。 如需有關使用者FTE在使用者設定中所顯示值的詳細資訊，請參閱[編輯使用者的設定檔](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

* **使用者的排程**：使用者的排程是用來決定使用者在資源規劃工具中的可用性。 使用者FTE的值會被忽略。 在此案例中：

   * 資源規劃工具中的&#x200B;**可用時數**&#x200B;與使用者排程的時數相同。

     例如，如果使用者的排程每週有40小時可供工作，則使用者可在資源規劃工具中每週有40小時可供工作。

   * 資源規劃工具中的&#x200B;**可用FTE**&#x200B;由下列公式計算：

     `User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours`

     例如，如果使用者的排程有20小時可工作，而Workfront中的預設排程有40小時可工作，則使用者的FTE為0.5。

     如需排程的詳細資訊，包括預設排程，請參閱[建立排程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

>[!NOTE]
>
>如果使用者未與排程相關聯，則會使用預設排程來計算使用者的可用時數。

### 計算資源規劃工具中工作角色的可用時數和FTE {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

您首先必須計算使用者可用性，然後可以計算其每個職務角色的可用性。

資源規劃工具中工作角色的可用性會考慮使用者的總可用性，以及與使用者的每個角色相關聯的FTE可用性&#x200B;**百分比**。\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

如需將&#x200B;**FTE可用性百分比**&#x200B;值與使用者的工作角色產生關聯的詳細資訊，請參閱[編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

例如，如果使用者的「可用時數」值為40，且他們可以在75%的時間內完成一個主要角色，以及在25%的時間內完成一個「其他角色」，則資源規劃工具會顯示一週內主要角色的&#x200B;**可用時數**&#x200B;值為30小時，而「其他角色」的&#x200B;**可用時數**&#x200B;值為10小時。 在此案例中，主要角色的FTE為0.75，而其他角色的FTE為0.25。

>[!NOTE]
>
>使用者的總可用時間是透過本文中「資源規劃工具」的[計算使用者的可用時數和FTE ](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)」一節中所述的兩種方法之一計算的。

在「角色檢視」中檢視「資源規劃工具」時，一個工作角色的可用性是能夠履行該工作角色之所有使用者的可用性總計。\
如需資源規劃工具中資源可用性的詳細資訊，請參閱[資源規劃工具概觀](../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

### 計算資源規劃工具中使用者的可用時數和FTE （範例） {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

下表說明如何在「資源規劃工具」中為使用者計算「可用時數」與「可用FTE」，這取決於系統管理員在「資源管理偏好設定」中用於計算FTE的方法。

在此範例中，我們使用以下數字：

* 40小時的系統預設排程
* 20小時的使用者排程
* 使用者FTE為0.8

| FTE計算方法（系統設定） | 從使用者的排程&#x200B;**小時** | 從預設排程&#x200B;**小時** | **使用者FTE欄位** | 資源規劃工具中的&#x200B;**可用時數** | 資源規劃工具中的&#x200B;**可用FTE** |
|---|---|---|---|---|---|
| **預設排程** | 已忽略 | 40 | 0.8 | **32** （已計算） | **0.8** |
| **使用者的排程** | 20 | 40 | 已忽略 | **20** | **0.5** （已計算） |

排程例外和休假可能會影響計畫時數或FTE的數量。 如需詳細資訊，請參閱[設定資源管理喜好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

依使用者和時數的資源規劃工具檢視範例：

![資源規劃工具檢視（依使用者和時數）](assets/resource-planner-by-user-by-hours.png)

依使用者和FTE區分的資源規劃工具檢視範例：

![資源規劃工具檢視（依使用者和FTE）](assets/resource-planner-by-user-by-fte.png)

## 計算資源規劃工具中使用者和職位角色的所有其他時數和FTE值 {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

除了「可用時數」或FTE外，「資源規劃工具」中也會顯示下列時間資訊：

* 規劃時數
* 預算時數
* 小時差異
* 淨小時\
  如需這些值的詳細資訊，請參閱資源規劃工具專案和角色檢視中的[時數概觀、約當全職人數和成本資訊](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* 小時差異\
  如需此值代表的詳細資訊，請參閱資源規劃工具](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)的專案和角色檢視中的[時數概觀、約當全職人數和成本資訊。

您可以在「資源規劃工具」中顯示與FTE或時數相同的資訊。

Workfront使用以下公式，在資源規劃工具中將所有其他值顯示為FTE：

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>在資源規劃工具中計算所有值(可用(AVL) FTE值除外)的FTE時，使用者的排程會被忽略。 計算時只考慮「預設排程」。

此計算適用於下列值：

* 計畫FTE (PLN)
* 預算FTE （預算）
* FTE差額(VAR)
* 淨FTE
* FTE差異(DIF)
