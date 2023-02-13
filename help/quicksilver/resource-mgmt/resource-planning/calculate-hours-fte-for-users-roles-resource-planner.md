---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: 在資源計畫員中計算用戶和角色的小時數和FTE的概覽
description: 在資源計畫員中計算用戶和角色的小時數和FTE的概覽
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# 在資源計畫員中計算用戶和角色的小時數和FTE的概覽

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

您可以按小時數、FTE或成本在資源計畫員中顯示資源的分配和可用性。\
有關在資源計畫器中計算成本的詳細資訊，請參閱 [在資源計畫器中計算成本](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

「FTE」代表「全職」等值。 這是一種時間測量，代表使用者或工作角色在一天或一週內用於實際工作的小時數。

在資源計畫器中，以下資源資訊集的計算方式不同：

* 「可用小時數」或「FTE」值的計算方式取決於系統管理員在系統中配置「資源管理」首選項的方式。\
   有關如何計算可用小時數和FTE值的詳細資訊，請參閱 [計算資源計畫員中用戶和任務職責的可用小時數或FTE](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
   有關定義Adobe Workfront系統的資源管理首選項的詳細資訊，請參閱 [配置資源管理首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* 所有其他FTE值則根據「系統預設」計畫計算。\
   有關使用FTE時在資源計畫器中顯示所有其他值的詳細資訊，請參閱：部分 [計算資源計畫員中用戶和任務職責的所有其他小時值和FTE值](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) 這篇文章。

了解每個用戶及其職務的FTE是什麼，在您將資源分配給工作時準確管理資源非常重要。

## 計算資源計畫員中用戶和任務職責的可用小時數或FTE {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [計算資源計畫員中用戶的可用小時數和FTE](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [在資源計畫員中計算任務職責的可用小時數和FTE](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [計算資源計畫員中用戶的可用小時數和FTE（示例）](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### 計算資源計畫員中用戶的可用小時數和FTE {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

Workfront管理員通過在「設定」的「資源管理」區域中選擇使用以下選項之一，來確定如何計算用戶的可用時間：

* 系統的預設計畫和用戶的FTE。
* 使用者的排程。

如需詳細資訊，請參閱 [配置資源管理首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

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

### 在資源計畫員中計算任務職責的可用小時數和FTE {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

首先必須計算用戶可用性，然後才能計算每個作業角色的可用性。

Oracle Resource Planner中任務角色的可用性考慮用戶的總可用性，以及 **FTE可用性百分比** 與使用者的每個角色相關聯。\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

如需關於關聯 **FTE可用性百分比** 具有使用者工作角色的值，請參閱 [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

例如，如果用戶的「可用小時數」值為40，並且他們可以在75%的時間內完成一個主要職責，在25%的時間內完成一個其他職責，則資源計畫器會顯示 **可用小時數** 主要角色一週的值為30小時，且 **可用小時數** 其他角色的值為10小時。 在這種情況下，主要角色的FTE為0.75，而其他角色的FTE為0.25。

>[!NOTE]
>
>使用者的可用時間總計是根據 [計算資源計畫員中用戶的可用小時數和FTE](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) 一節。

在「角色視圖」中查看資源計畫員時，一個任務職責的可用性是所有可履行該任務職責的用戶的可用性總和。\
有關資源計畫器中資源可用性的詳細資訊，請參閱 [資源計畫員概覽](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### 計算資源計畫員中用戶的可用小時數和FTE（示例） {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

下表說明了如何為資源計畫員中的用戶計算可用小時數和可用FTE，具體取決於系統管理員在資源管理首選項中用於FTE計算的方法。

在此範例中，我們使用下列數字：

* 40小時的系統預設計畫
* 20小時的用戶計畫
* 用戶FTE為0.75。

| FTE計算方法（系統設定） | **距離用戶計畫的小時數** | **預設排程的小時數** | **用戶FTE欄位** | **資源計畫員中的可用小時數** | **資源計畫員中的可用FTE** |
|---|---|---|---|---|---|
| **預設排程** | 已忽略 | 40 | 0.75 | **30** （計算） | **0.75** |
| **使用者的排程** | 20 | 40 | 已忽略 | **20** | **0.5** （計算） |

計畫例外和休假時間可能會影響計畫小時數或FTE的數量。 如需詳細資訊，請參閱 [配置資源管理首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 計算資源計畫員中用戶和任務職責的所有其他小時值和FTE值 {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

除了可用小時數或FTE外，下列時間資訊還顯示在資源計畫器中：

* 計畫小時
* 預算時數
* 小時差異
* 淨小時數\
   如需這些值的詳細資訊，請參閱 [資源計畫員的「項目」和「職責」視圖中的小時數、FTE和成本資訊概覽](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* 小時差\
   如需此值代表哪些內容的詳細資訊，請參閱 [資源計畫員的「項目」和「職責」視圖中的小時數、FTE和成本資訊概覽](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

您可以在資源計畫員中顯示與FTE或小時相同的資訊。

Workfront使用以下公式將資源計畫員中的所有其他值顯示為FTE:

```
FTE = Resource Planner Hours/ Default Schedule Hours
```

>[!NOTE]
>
>計算資源計畫員中除「可用(AVL)FTE」值外的所有值的FTE時，將忽略用戶的計畫。 計算時只考慮預設計畫。

此計算適用於下列值：

* 計畫FTE(PLN)
* 預算的FTE(BDG)
* FTE差異(VAR)
* 淨FTE
* FTE差異(DIF)
