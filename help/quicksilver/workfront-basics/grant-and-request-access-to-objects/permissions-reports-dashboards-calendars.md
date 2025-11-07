---
title: 共用報告、儀表板和行事曆
content-type: reference
product-area: user-management;reports;dashboards;calendars
navigation-topic: grant-and-request-access-to-objects
description: 當使用者指派存取層級時，您的Adobe Workfront管理員會授予他們檢視或編輯報告、儀表板和行事曆的存取權。 如需授與報表、控制面板和行事曆存取權的詳細資訊，請參閱授與報表、控制面板和行事曆的存取權。
author: Courtney
feature: Get Started with Workfront
exl-id: c2dac54b-6506-41b0-a7f2-6fafab12c2d1
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# 共用報告、儀表板和行事曆

當使用者指派存取層級時，您的Adobe Workfront管理員會授予他們檢視或編輯報告、儀表板和行事曆的存取權。 如需授與報告、儀表板和行事曆存取權的詳細資訊，請參閱[授與報告、儀表板和行事曆的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。

除了授予使用者的存取層級之外，您還可以授予他們檢視或管理您有權存取共用之特定報告、儀表板或行事曆的許可權。 如需授與使用者共用物件許可權的相關資訊，請參閱[共用物件許可權簡介](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

許可權專屬於Workfront中的一個專案，可定義使用者可對該專案執行的動作。

如需有關每個存取層級中的使用者可以對問題執行的資訊，請參閱文章[每個物件型別可用的功能](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports)中的[報告](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)小節。

## 關於共用報表、儀表板或行事曆的考量事項

除了下列考量事項外，另請參閱[物件共用許可權概觀](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

>[!NOTE]
>
>Workfront管理員可以新增或移除系統中所有使用者的任何專案許可權，而無需擁有這些專案。

* 報表、控制面板或行事曆的建立者預設擁有管理許可權。
* 共用報告、控制面板和行事曆類似於在Workfront中共用任何其他物件。

  如需有關如何在Workfront中共用物件的詳細資訊，請參閱[共用物件](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

  另請參閱下列文章以瞭解如何共用報告、控制面板和行事曆：

   * [在Adobe Workfront中共用報告](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [共用儀表板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [共用行事曆報告](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* 您可以個別共用報表和控制面板，也可以大量共用。

  您只能個別共用行事曆。 您無法大量共用它們。

* 您無法共用內建的系統報告。 您只能共用自訂報表。

  如需將系統報告儲存為新的自訂報告的詳細資訊，請參閱[建立報告復本](../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

* 您可以授予報表、控制面板和行事曆下列許可權：

   * 檢視
   * 管理

* 當您共用控制面板時，使用者預設擁有控制面板上所有報告、行事曆和外部頁面的檢視許可權。
* 擁有請求授權的使用者無法檢視系統範圍的報告。 請求者需要檢視報表時，必須個別與請求者共用報表。
* 如果報表有提示且您公開共用，則存取該報表的使用者必須登入Workfront，才能使用提示執行報表。 如果他們無法登入Workfront，將會看到未套用提示的報告。\
  如需有關共用具有提示之報表的限制的詳細資訊，請參閱文章[新增提示至報表](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports)中的[共用提示之報表的限制](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)小節。

* 您可以從報告或行事曆移除繼承的許可權。

  如需有關移除物件繼承許可權的詳細資訊，請參閱[移除物件許可權](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)。

* 您也可以公開或全系統共用報表或行事曆。

  您無法公開共用儀表板，但可以在系統內共用。

  >[!CAUTION]
  >
  >建議您將包含機密資訊的物件與外部使用者共用時務必謹慎。 這可讓他們檢視資訊，而不需要身為Workfront使用者或屬於您的組織。
