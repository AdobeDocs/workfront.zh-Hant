---
content-type: overview
product-area: timesheets
navigation-topic: timesheets-navigation-topic
title: 時程表總覽
description: 您可以使用時程表來追蹤您花在工作上的時間。 如需Adobe Workfront中時程表配置的相關資訊，請參閱瞭解時程表配置。
author: Alina
feature: Timesheets
exl-id: 2174a879-4a19-4a0f-803a-f19a8909f227
source-git-commit: 48f46abab1958325aba6832b85247dc2c80f4e80
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# 時程表總覽

您可以使用時程表來追蹤在Adobe Workfront中工作所花費的時間。

身為Workfront或群組管理員，您可以建立時程表並將其與使用者建立關聯。 如需關於建立時程表的資訊，請參閱 [建立和管理時程表](../create-and-manage-timesheets/create-and-manage-timesheets.md).

時程表是類似格線的表格，會顯示工作專案與行事曆區域。 您可以記錄專案的時間，並將其與工作的執行日期建立關聯。 這會追蹤您在Workfront中的實際工作時間。 時程表中也有一個區域，可供您記錄非工作相關專案的時間，例如會議、訓練或外出時間。

如需Adobe Workfront中時程表配置的相關資訊，請參閱 [瞭解時程表配置](../../timesheets/timesheets/timesheet-layout.md).

![](assets/timesheet-example.png)

您可以在Workfront中以多種方式記錄時間，通常是在專案、任務或執行工作問題的層級。 對照任務、問題和專案記錄的時間也會顯示在您的時程表中。

您也可以在「一般時數」底下記錄非專案工作的時間。 一般小時時間只能在您的時程表中記錄。

如需可以在Workfront中記錄時間位置的詳細資訊，請參閱 [記錄時間](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!TIP]
>
>Workfront行動應用程式也可讓您發佈更新、變更記錄時間、輸入註解及關閉時程表。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須擁有時程表的管理存取權。 </p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者管理特定區域的存取權</a>.</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。


## 瞭解專案時間與非專案時間

時程表為使用者提供追蹤專案和非專案工作時間的簡單方式：

* **專案時間：** 直接從您要追蹤時間的任務或專案。

  透過時程錶針對任務、問題和專案記錄的小時與各自的工作專案產生關聯，以準確表示在專案和任務上所花費的精力。 如果沒有準確的時間輸入，如果您的資料用於計費目的，可能會不準確。

  此外，當資源直接在任務上記錄時數時，當使用者存取時程表時，問題和專案會自動出現。 這是假設時程表日期範圍跨越記錄時數的日期。

* **非專案時間：** 直接在使用者時程表上。 如需如何在Workfront中追蹤時間的詳細資訊，請參閱   [記錄時間](../../timesheets/create-and-manage-timesheets/log-time.md).

  在時程表中，資源可以記錄休假時數、病假時數、運輸時數、維修或維護裝置時數，或您希望建立的任何一般管理費用時數型別。

## 存取時程表區域中的時程表

如需可記錄時間之Workfront所有區域的詳細資訊，請參閱 [記錄時間](../../timesheets/create-and-manage-timesheets/log-time.md).

若要存取時程表：

1. 按一下 **主要功能表** 圖示 ![](assets/dots-main-menu.png) 位於右上角，或 **主要功能表** 圖示 ![](assets/lines-main-menu.png) 在Workfront的左上角（如果有的話），按一下「時程表」。

   依預設，會顯示時程表區域，以及屬於您或您有權檢視的所有時程表顯示。

   ![](assets/all-timesheets-list-nwe-350x68.png)

1. 按一下右上角的以下選項之一，以顯示有限數量的時程表：

   * **我的時間表** 以僅顯示您的時間表。

   ![](assets/my-timesheets-list-various-statuses-nwe-350x60.png)

   * **我的時程表核准** 以僅顯示您核准的時程表。

     ![](assets/timesheets-i-approve-list-with0filters-new-nwe-350x61.png)

   此時會顯示經篩選的時程表清單。

1. （選用）更新時程表清單頂端的檢視、篩選和群組。 如需詳細資訊，請參閱 [報表元素：篩選器、檢視和群組](../../reports-and-dashboards/reports/reporting-elements/reporting-elements-overview.md).

1. 按一下 **日期範圍** 時程表以將其開啟。

   每個時程表都會顯示您已記錄時間的所有任務、問題和專案。 時程表也會顯示最多45個指派給您的任務、問題或專案，其日期在時程表的時間範圍內，但您可能尚未記錄時間。

   如需詳細資訊，請參閱 [設定時程表和小時偏好設定](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).



