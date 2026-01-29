---
title: 連線記錄概觀
description: 在記錄型別之間建立連線後，可以將個別記錄彼此連線。 本文說明在Adobe Workfront Planning中連線記錄時，您必須考慮的事項。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: be51023c-8e11-42e7-aa4f-34484c30eb03
source-git-commit: 11d856aeee3bd9edcdc1dbca3964f37bdf83bd00
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# 連線記錄概觀

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

您可以將Adobe Workfront Planning記錄彼此連線，或從其他應用程式連線至物件。

本文說明在Workfront Planning中連線記錄時，您必須考慮的事項。

如需如何將記錄連結至彼此或另一個物件的詳細資訊，請參閱[連結記錄](/help/quicksilver/planning/records/connect-records.md)。

## 先決條件

您必須先連線下列專案，才能在Workfront Planning中連線記錄：

* 兩種記錄型別
* 含有來自其他應用程式的物件的記錄型別

如需詳細資訊，請參閱[連線記錄型別概觀](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。


## 有關連線記錄的考量事項

* 在您連線記錄型別之後，連線的記錄型別會以連線欄位的形式顯示在它們連結的記錄型別表格中，以及記錄頁面上。
* 您可以從連結記錄欄位中瀏覽並新增連結記錄的記錄和物件以及物件型別。
* 您可以在連結的記錄型別表格中，新增連結的記錄型別的欄位（查詢欄位）。

  此外，您也可以在您連結的記錄型別表格中，新增您正在連結的記錄型別的欄位（查詢欄位）。

  例如，如果您從促銷活動的記錄型別連結產品的記錄型別，則可以顯示促銷活動的產品欄位，以及產品的促銷活動欄位。
* 您無法手動更新您連結之記錄中的查閱欄位值。

  查詢欄位的值會在原始記錄或物件上更新後，自動填入您正在連結的Workfront Planning記錄。

* 有權存取Workfront Planning和「檢視」或對工作區和記錄型別擁有更高許可權的每個人，都可以看到您在記錄之間或記錄與其他應用程式物件之間建立的連線。 無論連線至應用程式的許可權為何，使用者都可以檢視連線的記錄和物件。
* 如果您擁有工作區的「管理」許可權以及連線記錄的記錄型別，則可以檢視及編輯其他人的連線。
* 您可以將一個記錄連線到另一個應用程式的一或多個物件。視您在連線記錄型別時選取的連線型別而定。 如需詳細資訊，請參閱文章[連線記錄型別概觀](/help/quicksilver/planning/architecture/connect-record-types-overview.md)中的「連線型別」一節。
* 當連線的記錄型別屬於階層的一部分時，您可以從記錄的頁面存取階層內的任何物件型別。 如需詳細資訊，請參閱[階層與階層連結概觀](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)。
* 當連線的記錄型別是階層的一部分時，您可以從子記錄型別連線一個記錄，到從父記錄型別連線最多10個記錄。 如需詳細資訊，請參閱[階層與階層連結概觀](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)。

## 您可以連線記錄的區域

您可以在Workfront中手動或自動連線記錄。

### 手動連線記錄

您可以在下列區域中，手動將記錄連線到其他記錄，或從其他應用程式連線到物件：

* 您可以在Workfront Planning記錄的下列區域中，將記錄連結至Workfront物件、Experience Manager Assets物件或GenStudio Brands：

   * Planning中記錄型別的表格檢視中的已連線記錄欄位。
   * 記錄的預覽或詳細資訊頁面中的已連線記錄欄位。
   * 記錄的「連線記錄」頁面上的記錄預覽或詳細資訊頁面。

* 您可以在Workfront的下列區域中，將Workfront物件連結至Workfront Planning記錄：

   * Workfront物件的「規劃」區段。
   * Workfront物件自訂表單上的Planning連線欄位。

  如需詳細資訊，請參閱[管理來自Workfront物件的記錄連線](/help/quicksilver/planning/records/manage-records-in-planning-section.md)。

### 自動連線記錄

將記錄型別連線到另一個或記錄型別連線到另一個應用程式的物件型別之後，您可以以下列方式自動連線記錄和物件：

* 使用自動化

  您可以從設定自動化的Planning記錄中建立記錄或Workfront物件。

  當您定義的條件符合時，系統就會建立記錄或物件，並自動連線至您觸發自動處理的記錄。

  如需詳細資訊，請參閱[設定Adobe Workfront規劃自動化](/help/quicksilver/planning/records/configure-automations-to-create-records.md)。

* 使用請求表單建立記錄

  您可以在提交Planning請求時建立記錄。 請求和記錄會自動連線。

  >[!NOTE]
  >
  >您無法中斷記錄與其原始請求的連線。

  如需詳細資訊，請參閱[提交Adobe Workfront Planning要求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)。
