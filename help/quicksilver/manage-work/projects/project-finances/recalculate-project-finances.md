---
title: 重新計算專案財務
product-area: projects
navigation-topic: financials
description: 當專案記錄的時數或用於計算成本和收入的費率發生變更時，在專案上計算財務。
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: bfe77796863bb2d7d324901721fda7fa045c2c0b
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 0%

---

# 重新計算專案財務

當專案記錄的時數或用於計算成本和收入的費率發生變更時，在專案上計算財務。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案與財務資料的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理具有管理財務之許可權的專案許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 在Adobe Workfront中計算財務的考量事項

增強型分析中的財務計算方式如下：

* 您可以使用專案上的「重新計算財務」選項，手動重新計算專案的成本和收入。
* 此外，某些動作會觸發自動重新計算。

當使用者或角色的速率在專案存留期內變更時，可能會出現下列情況：

* 進行變更時，會從該時間點開始使用更新的費率，因為會記錄時數並計算財務資訊。 變更速率不會影響進行變更前的運算方式。 對於記錄的所有現有時數，使用舊比率來計算財務資訊。
* 您可以使用「重新計算財務」選項，強制Adobe Workfront回溯使用目前為止記錄之所有時數的新費率。 這可強制Workfront根據新的費率資訊，回溯重新計算所有先前輸入的時數、計畫成本和收入。

>[!CAUTION]
>
>手動重新計算指定專案的財務之前，您可能想要保留已使用先前費率計算的任何財務資料。 建議您僅在確定未變更現有資訊或需要變更時，才使用重新計算財務選項。

## 保留具有現有時數的任務的財務資料 {#preserve-financial-data-for-tasks-with-existing-hours}

重新計算專案的財務資料時，Workfront會根據任何新或更新的財務資訊，回溯重新計算所有先前記錄的時數、計畫、實際成本以及計畫和實際收入。

* [保留專案收入](#preserve-project-revenue)
* [保留專案成本](#preserve-project-cost)

### 保留專案收入  {#preserve-project-revenue}

在專案存留期內，收入率可能會發生變化。

如需有關收費率和收入的詳細資訊，請參閱文章 [帳單與收入概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

收入率可在下列層次變更：

* 系統層級（適用於工作角色）\
  如需有關在系統層級使用計費率建立工作角色的詳細資訊，請參閱文章 [建立和管理職位角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* 使用者層級\
  如需有關變更使用者收費率資訊的詳細資訊，請參閱文章 [編輯使用者設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 公司層級（適用於職務角色）\
  如需詳細資訊，請參閱 [覆寫公司層級的工作角色收費率](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* 專案層級（適用於工作角色）\
  如需有關在專案層級覆寫工作角色費率的詳細資訊，請參閱文章 [覆寫工作角色帳單費率與計算專案收入的概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

例如，使用者的收費率在專案過程中從每小時$50變更為$75，而您想要所有現有資料保持以舊費率（$50和小時）計算。 但是，重新計算專案財務時，已有現有財務資料的任務將會更新收入，以反映新的計費率（每小時75美元）。

* [建立付費記錄以保留專案收入](#preserve-project-revenue-by-creating-a-billing-record)
* [使用多重記帳費率覆寫來保留專案收入](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### 建立付費記錄以保留專案收入 {#preserve-project-revenue-by-creating-a-billing-record}

當上述任何層級的帳單費率變更時，您可以保留已在專案上計算的現有收入，方法是避免使用手動「重新計算財務」選項，或是鎖定專案上記錄的時間，並使用舊費率計算至狀態為「已記帳」的帳單記錄中。

如果您未重新計算專案的財務，或您鎖定記錄到已記帳記帳記錄的時數，在費率變更之後記錄的時數將使用新費率計算，並且在成本費率變更之前記錄的時數仍按舊費率計算。

如需建立付費記錄的詳細資訊，請參閱文章 [建立付費記錄](../../../manage-work/projects/project-finances/create-billing-records.md).

#### 使用多重記帳費率覆寫來保留專案收入 {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

當專案層級的工作角色的計費率變更時，您可以使用在指定時間範圍內鎖定的多個計費率覆寫，來保留已在專案上計算的現有收入。

如需使用多個計費率覆寫的詳細資訊，請參閱文章 [覆寫工作角色帳單費率與計算專案收入的概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>這僅適用於在專案層級變更的工作角色收費率。

### 保留專案成本 {#preserve-project-cost}

成本費率可在下列層次變更：

* 系統層級（適用於工作角色）\
  如需有關以系統層級的成本費率建立職務角色的詳細資訊，請參閱文章 [建立和管理職位角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* 使用者層級\
  如需有關變更使用者成本費率資訊的詳細資訊，請參閱文章 [編輯使用者設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

當上述任何層級的計費率變更時，您可以鎖定專案上記錄的時間，並使用舊費率計算至狀態為「已記帳」的計費記錄中，以保留已在專案上計算的現有成本。 如需建立付費記錄的詳細資訊，請參閱文章 [建立付費記錄](../../../manage-work/projects/project-finances/create-billing-records.md).

如果您不想建立計費記錄，也可以避免使用手動重新計算財務選項，如一節所述 [手動重新計算專案的財務](#manually-recalculate-finances-for-a-project) 本文章內容。

如果您未重新計算專案的財務，或您鎖定記錄到已記帳記帳記錄的時數，在費率變更之後記錄的時數將使用新費率計算，並且在成本費率變更之前記錄的時數仍按舊費率計算。

## 手動重新計算專案的財務 {#manually-recalculate-finances-for-a-project}

如果您的費率在專案生命週期中變動，並且您想要成本和收入計算反映新的費率，則必須手動重新計算專案的財務。

>[!NOTE]
>
>當您手動重新計算財務時，可以按照一節中的步驟來防止更新收入值，以反映新的費率 [保留具有現有時數的任務的財務資料](#preserve-financial-data-for-tasks-with-existing-hours) 本文章節。 當您手動重新計算專案的財務時，成本值一律會更新以反映新的費率。

您可以從專案頁面或專案清單或報告，重新計算Workfront中專案的財務。

您可在大量編輯時重新計算財務。 如需詳細資訊，請參閱 [手動大量重新計算財務](#manually-recalculate-finances-in-bulk) 一節。

1. 前往您要重新計算財務的專案，然後按一下 **更多** 圖示 ![](assets/qs-more-icon-on-an-object.png) 專案名稱右側。

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   前往專案清單或報告，選取一或多個專案，然後按一下 **更多** 圖示 ![](assets/qs-more-icon-on-an-object.png) 在清單頂端。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >根據您專案的複雜性，我們建議不要在大量重新計算其財務時選取大量專案以確保最佳效能。 有些因素會導致專案過於複雜，包括多重相依性或指派，或大量自訂欄位。

1. 按一下 **重新計算財務**.

   專案的所有計畫成本和收入會使用任何新資訊重新計算。

   您應該會在瀏覽器頂端收到確認，表示已成功重新計算專案的財務。
現有成本值與某些尚未鎖定的收入值會更新以反映新的費率。

## 手動大量重新計算財務{#manually-recalculate-finances-in-bulk}

您可以手動重新計算數個專案的財務，方法是大量編輯專案。 這會導致專案上的收入回溯重新計算。

>[!IMPORTANT]
>
>當您手動重新計算財務時，可以按照一節中的步驟來防止更新收入值，以反映新的費率 [保留具有現有時數的任務的財務資料](#preserve-financial-data-for-tasks-with-existing-hours) 本文章節。 當您手動重新計算專案的財務時，成本值一律會更新以反映新的費率。

若要手動重新計算數個專案的財務：

1. 前往專案清單。
1. 在清單中選取數個專案，然後按一下 **更多** 圖示 ![](assets/qs-more-icon-on-an-object.png) 在清單頂端。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >根據您專案的複雜性，我們建議不要在大量編輯專案時選取大量專案，以確保最佳效能。 有些因素會導致專案過於複雜，包括多重相依性或指派，或大量自訂欄位。

1. 按一下 **重新計算財務**.

   所選專案的所有計畫成本和收入會使用任何新資訊重新計算。

   您應該會在瀏覽器頂端收到確認，表示已成功重新計算專案的財務。

## 觸發自動重新計算財務的動作

下列動作會觸發Workfront中專案的財務重新計算：

* 變更任務狀態
* 將具有時數的任務移動到另一個專案
* 將專案狀態從完成變更為使用中狀態

>[!NOTE]
>
>當您變更專案狀態時，只會重新計算計畫值。

您也可以在「 」下手動重新計算財務 **更多** 功能表 ![](assets/qs-more-menu.png) 在專案層級，按一下 **重新計算財務**.
