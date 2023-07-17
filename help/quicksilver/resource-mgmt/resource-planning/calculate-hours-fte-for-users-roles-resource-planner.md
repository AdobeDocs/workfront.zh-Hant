---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: 計算資源規劃工具中使用者和角色的時數和FTE的概觀
description: 計算資源規劃工具中使用者和角色的時數和FTE的概觀
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 4331917d133c52cf727f148b75a213853c1e5679
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# 計算資源規劃工具中使用者和角色的時數和FTE的概觀

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

您可以依時數、約當全職人數或成本，在「資源規劃工具」中顯示資源的配置與可用性。\
如需有關在資源規劃工具中計算成本的詳細資訊，請參閱 [在資源規劃工具中計算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

「FTE」代表全時同等。 這是時間測量值，代表使用者或工作角色在一天或一週內專用於實際工作的時數。

下列資源資訊集在「資源規劃工具」中的計算方式不同：

* 可用時數或FTE值是根據系統管理員在系統中設定資源管理偏好設定的方式計算的。\
  如需有關如何計算可用時數和FTE值的詳細資訊，請參閱 [計算資源規劃工具中使用者和職務角色的可用時數或FTE](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  如需為Adobe Workfront系統定義資源管理偏好設定的詳細資訊，請參閱 [設定資源管理喜好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* 所有其他FTE值都是根據系統預設排程來計算。\
  如需使用FTE時所有其他值在資源規劃工具中如何顯示的詳細資訊，請參閱區段 [計算資源規劃工具中使用者和職務角色的所有其他時數和FTE值](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) 本文章內容。

請務必瞭解每個使用者及其職位角色的FTE是什麼，以便在您指派他們工作時，準確地管理您的資源。

## 計算資源規劃工具中使用者和職務角色的可用時數或FTE {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [計算資源規劃工具中使用者的可用時數和FTE](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [計算資源規劃工具中工作角色的可用時數和FTE](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [計算資源規劃工具中使用者的可用時數和FTE （範例）](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### 計算資源規劃工具中使用者的可用時數和FTE {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

Workfront管理員在「設定」的「資源管理」區域中選取使用下列其中一項，以決定如何計算使用者的可用時間：

* 系統的預設排程和使用者的FTE。
* 使用者的排程。

如需詳細資訊，請參閱 [設定資源管理喜好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><br></p>
<p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p>
<p>(NOTE: The determines how to calculate resource availability at the system level.For more information about defining the Resource Management preferences for the system, see Configure Resource Management preferences.)</p>
<p>Based on how this setting is configured, the availability of the users in the Resource Planner (hours as well as FTE availability) is calculated by using the following methods: </p>
<ul>
<li><strong>The Default Schedule</strong>: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the Resource Planner. The Schedule of the user is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE value</code> <span style="color: #dc143c;">( NOTE: this is the correct value. If this shows as a division in other articles, that is wrong. It's a multiplication between these 2 values).</span><br>For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Resource Planner.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a></li>
<li style="font-weight: normal;"> The <strong>Available FTE</strong> for the user in the<strong>Resource Planner</strong> is the same as the user FTE specified in the user settings. <br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner. For more information about the value of the user FTE as it displays in the user settings, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><strong>The User's Schedule</strong>: The Schedule of the user is used to determine the availability of the user in the Resource Planner. The value of the user FTE is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the Resource Planner. </li>
<li> The <strong>Available FTE</strong> in the<strong>Resource Planner</strong> is calculated by the following formula:<br><em><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul></li>
</ul> <note type="note">
If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note>
</div>
-->

### 計算資源規劃工具中工作角色的可用時數和FTE {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

您首先必須計算使用者可用性，然後可以計算其每個職務角色的可用性。

「資源規劃工具」中工作角色的可用性會考慮使用者的總可用性，以及 **FTE可用性百分比** 與使用者的每個角色相關聯。\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

如需建立關聯的詳細資訊 **FTE可用性百分比** 具有使用者工作角色的值，請參閱 [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

例如，如果使用者的「可用時數」值為40，且他們可以在75%的時間中履行一個「主要角色」，並在該時間的25%時間內履行一個「其他角色」，則「資源規劃工具」會顯示 **可用時數** 「主要角色」一週的值為30小時，而 **可用時數** 「其他角色」的值為10小時。 在此情況下，主要角色的FTE為0.75，而其他角色的FTE為0.25。

>[!NOTE]
>
>使用者的總可用時間是以下文所述的兩種方法之一計算的 [計算資源規劃工具中使用者的可用時數和FTE](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) 章節。

在「角色檢視」中檢視「資源規劃工具」時，一個工作角色的可用性是能夠履行該工作角色之所有使用者的可用性總計。\
如需「資源規劃工具」中資源可用性的詳細資訊，請參閱 [資源規劃工具概觀](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### 計算資源規劃工具中使用者的可用時數和FTE （範例） {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

下表說明如何針對「資源規劃工具」中的使用者計算「可用時數」與「可用FTE」，這取決於系統管理員在「資源管理偏好設定」中用於計算FTE的方法。

在此範例中，我們使用以下數字：

* 40小時的系統預設排程
* 20小時的使用者排程
* 使用者FTE為0.75

| FTE計算方法（系統設定） | **來自使用者排程的小時** | **預設排程的時數** | **使用者FTE欄位** | **資源規劃工具中的可用時數** | **資源規劃工具中的可用FTE** |
|---|---|---|---|---|---|
| **預設排程** | 已忽略 | 40 | 0.75 | **30** （計算） | **0.75** |
| **使用者的排程** | 20 | 40 | 已忽略 | **20** | **0.5** （計算） |

排程例外和休假可能會影響計畫時數或FTE的數量。 如需詳細資訊，請參閱 [設定資源管理喜好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 計算資源規劃工具中使用者和職務角色的所有其他時數和FTE值 {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

除了「可用時數」或FTE之外，「資源規劃工具」中也會顯示下列時間資訊：

* 計畫小時
* 預算時數
* 小時差異
* 淨小時\
  如需這些值的詳細資訊，請參閱 [資源規劃工具的「專案」與「角色」檢視中的時數、約當全職人數及成本資訊概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* 小時差異\
  如需有關此值代表的詳細資訊，請參閱 [資源規劃工具的「專案」與「角色」檢視中的時數、約當全職人數及成本資訊概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

您可以在「資源規劃工具」中顯示與FTE或時數相同的資訊。

Workfront會使用以下公式，在資源規劃工具中將所有其他值顯示為FTE：

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>在計算「資源規劃工具」中可用(AVL) FTE值以外的所有值的FTE時，會忽略使用者的排程。 計算時只會考慮「預設排程」。

此計算適用於下列值：

* 計畫FTE (PLN)
* 預算FTE (BDG)
* FTE差額(VAR)
* 淨FTE
* FTE差異(DIF)
