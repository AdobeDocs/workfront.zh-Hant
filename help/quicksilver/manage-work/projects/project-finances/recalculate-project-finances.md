---
title: 重新計算項目財務
product-area: projects
navigation-topic: financials
description: 當項目記錄的小時數或用於計算成本和收入的費率發生變化時，將在項目上計算財務。
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1590'
ht-degree: 0%

---

# 重新計算項目財務

當項目記錄的小時數或用於計算成本和收入的費率發生變化時，將在項目上計算財務。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對項目和財務資料的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>使用管理財務的權限管理項目的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 關於Adobe Workfront財務計算的思考

在Enhanced Analytics中，會以下列方式計算財務：

* 您可以使用項目上的「重新計算財務」選項，人工重新計算項目的成本和收入。
* 此外，有些動作會觸發自動重新計算。

當使用者或角色的比率在專案期間變更時，可能會發生下列情況：

* 進行變更時，會從該點開始使用更新後的比率，作為記錄小時數並計算財務資訊。 變更比率不會影響進行變更前的項目計算方式。 對於記錄的所有現有小時數，舊費率用於計算財務資訊。
* 您可以使用「重新計算財務」選項，強制Adobe Workfront對迄今記錄的所有小時使用新費率進行追溯。 這將迫使Workfront根據新費率資訊追溯重新計算所有以前輸入的小時數、計畫成本和收入。

>[!CAUTION]
>
>在手動重新計算指定項目的財務資料之前，您可能希望保留以前費率計算的任何財務資料。 建議僅在您確定不對現有資訊進行更改，或僅在需要更改時使用「重新計算財務」選項。

## 保留現有小時的任務的財務資料 {#preserve-financial-data-for-tasks-with-existing-hours}

重新計算項目的財務資料時，Workfront會根據任何新的或更新的財務資訊，追溯地重新計算所有先前記錄的小時數、計畫、實際成本以及計畫和實際收入。

* [保留項目收入](#preserve-project-revenue)
* [保留項目成本](#preserve-project-cost)

### 保留項目收入  {#preserve-project-revenue}

收入率可在專案存留期內變更。

如需帳單費率和收入的詳細資訊，請參閱文章 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

收入率可在下列層級變更：

* 系統級別（用於作業角色）\
   有關在系統層使用計費費率建立職務職責的詳細資訊，請參閱文章 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* 使用者層級\
   有關更改用戶計費率資訊的詳細資訊，請參閱文章 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 公司層級（針對職務）\
   如需詳細資訊，請參閱 [在公司層改寫職務開單費率](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* 專案層級（針對作業角色）\
   有關在項目級改寫職務職責費率的詳細資訊，請參閱文章 [改寫任務職責開單費率和計算項目收入概覽](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

例如，在項目過程中，用戶的計費費率從每小時50美元更改為75美元，您希望所有現有資料保持以舊費率（50美元和小時）計算。 但是，當重新計算項目財務時，已經擁有現有財務資料的任務將更新收入，以反映新的開單率（每小時75美元）。

* [建立開單記錄以保留項目收入](#preserve-project-revenue-by-creating-a-billing-record)
* [使用多個開單率改寫保留項目收入](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### 建立開單記錄以保留項目收入 {#preserve-project-revenue-by-creating-a-billing-record}

當在上述任何層更改開單費率時，您可以通過避免使用人工重新計算財務選項，或將項目上記錄的使用舊費率計算的時間鎖定到狀態為「已開單」的開單記錄中，來保留已在項目上計算的現有收入。

當您不重新計算項目上的財務或將記錄到計費開單記錄的小時數鎖定時，費率更改後記錄的小時數將使用新費率計算，而成本費率更改前記錄的小時數仍按舊費率計算。

有關建立計費記錄的詳細資訊，請參閱文章 [建立計費記錄](../../../manage-work/projects/project-finances/create-billing-records.md).

#### 使用多個開單率改寫保留項目收入 {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

當項目層任務職責的開單費率發生更改時，您可以使用多個在指定時間範圍內鎖定的開單費率改寫來保留項目上已計算的現有收入。

有關使用多個計費費率改寫的詳細資訊，請參閱文章 [改寫任務職責開單費率和計算項目收入概覽](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>這隻適用於在項目層更改的職務職責開單費率。

### 保留項目成本 {#preserve-project-cost}

成本率可在以下層次變動：

* 系統級別（用於作業角色）\
   有關在系統級別使用成本費率建立職務職責的詳細資訊，請參閱文章 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* 使用者層級\
   有關更改用戶成本率資訊的詳細資訊，請參閱文章 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

當在上述任何層更改開單費率時，您可以通過將項目上記錄的時間鎖定在狀態為「已開單」的開單記錄中，並使用舊費率計算，來保留已在項目上計算的現有成本。 有關建立計費記錄的詳細資訊，請參閱文章 [建立計費記錄](../../../manage-work/projects/project-finances/create-billing-records.md).

如果您不想建立開單記錄（如一節中所述），也可以避免使用人工重新計算財務選項 [人工重新計算項目的財務](#manually-recalculate-finances-for-a-project) 這篇文章。

當您不重新計算項目上的財務或將記錄到計費開單記錄的小時數鎖定時，費率更改後記錄的小時數將使用新費率計算，而成本費率更改前記錄的小時數仍按舊費率計算。

## 人工重新計算項目的財務 {#manually-recalculate-finances-for-a-project}

如果您的費率在項目期間發生更改，並且希望成本和收入計算反映新費率，則必須人工重新計算項目的財務。

>[!NOTE]
>
>按照部分中的步驟人工重新計算財務時，您可以阻止更新收入值以反映新費率 [保留現有小時的任務的財務資料](#preserve-financial-data-for-tasks-with-existing-hours) 這篇文章。 在人工重新計算項目的財務時，系統始終會更新成本值以反映新費率。

您可以從項目頁或項目清單或報表重新計算Workfront中項目的財務。

您可以在批量編輯財務時重新計算這些財務。 如需詳細資訊，請參閱 [在「編輯項目」框中手動重新計算財務](#manually-recalculate-finances-in-bulk-in-the-edit-projects-box) 一節。

1. 轉到要重新計算財務的項目，然後按一下 **更多** 圖示 ![](assets/qs-more-icon-on-an-object.png) 項目名稱的右側

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   前往專案清單或報表，選取一或多個專案，然後按一下 **更多** 圖示 ![](assets/qs-more-icon-on-an-object.png) 清單頂端。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >根據項目的複雜性，我們建議在大量重新計算其財務時不要選擇大量項目以確保最佳效能。 有些項目可能太複雜，可能是多個相依性或指派，或是大量自訂欄位。

1. 按一下 **重新計算財務**.

   系統會使用任何新資訊重新計算項目上的所有計畫成本和收入。

   您應會在瀏覽器頂端收到確認，確認專案的財務狀況已成功重新計算。\
   現有成本值和某些尚未鎖定的收入值會更新以反映新費率。

## 在「編輯項目」框中手動重新計算財務 {#manually-recalculate-finances-in-bulk-in-the-edit-projects-box}

您可以通過批量編輯多個項目來手動重新計算其財務。 這會導致項目上的收入重新計算。

>[!IMPORTANT]
>
>按照部分中的步驟人工重新計算財務時，您可以阻止更新收入值以反映新費率 [保留現有小時的任務的財務資料](#preserve-financial-data-for-tasks-with-existing-hours) 這篇文章。 在人工重新計算項目的財務時，系統始終會更新成本值以反映新費率。

要人工重新計算多個項目的財務，請執行以下操作：

1. 前往專案清單。
1. 在清單中選取數個專案，然後按一下 **編輯**.

   >[!TIP]
   >
   >根據專案的複雜度，我們建議在大量編輯專案時不要選取大量專案，以確保提供最佳效能。 有些項目可能太複雜，可能是多個相依性或指派，或是大量自訂欄位。

1. 按一下 **設定**，然後選取 **重新計算成本和收入**.

1. 按一下 **儲存變更**.

## 觸發自動重新計算財務的操作

下列動作會觸發Workfront中專案的財務重新計算：

* 更改任務狀態
* 將具有小時的任務移動到另一個項目
* 將項目狀態從「完成」更改為「活動」狀態

>[!NOTE]
>
>變更專案狀態時，只會重新計算計畫值。

您也可以在 **更多** 功能表 ![](assets/qs-more-menu.png) 在專案層級，按一下 **重新計算財務**.
