---
navigation-topic: financials
title: 建立付費記錄
description: 除了設定收入和追蹤費用外，您還可以在專案上建立付費記錄，以取得需要付費的資訊。
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 0%

---

# 建立付費記錄

除了設定收入和追蹤費用外，您還可以在專案上建立付費記錄，以取得需要付費的資訊。

您無法建立任務的付費記錄。 您只能為專案建立付費記錄。

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
   <td> <p>編輯專案與財務資料的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理具有管理財務之許可權的專案許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 付費記錄概觀

帳單記錄會建立為專案的附件，並包含專案的財務資料以及專案中任務的一些財務資訊。

計畫使用付費記錄時，請考量下列事項：

* 當您想要向外部供應商或合作夥伴開立與專案相關的金額帳單時，請建立帳單記錄。 除了開立固定金額帳單給外部來源外，有時您還需要開立帳單給外部承包商（從記錄時數）的專案工作金額，以及產生的費用或固定收入金額。 您可以在相同的付費記錄中包含所有這些資訊。
* 計費記錄一旦設定為Billed即無法編輯。

  >[!IMPORTANT]
  >
  >當您的費率不同，而且您想要鎖定專案的收入和費用資訊時，這一點很重要。 將其新增到記帳記錄並標籤為已記帳，可在您的系統中更新費率時防止其更新。

* 含有已標示為「已記帳」之記帳記錄的專案無法刪除。

## 建立付費記錄

1. 導覽至專案。
1. 按一下左側面板中的&#x200B;**記帳記錄**。

   此節可能位於&#x200B;**顯示更多**&#x200B;下。

1. 在左側面板中選取&#x200B;**記帳記錄詳細資料**，按一下&#x200B;**新增記帳記錄**。
1. 在顯示的&#x200B;**新付費記錄**&#x200B;方塊中，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>這是必填欄位。 指定付費記錄的描述，以反映此記錄的目的或目的。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">記帳狀態</td> 
      <td> <p>如果記錄尚未記帳，請選取<strong>未記帳</strong>。</p> <p>在記帳記錄時選取<strong>已記帳</strong>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計費日期</td> 
      <td>按一下行事曆圖示，選取對此付費記錄記帳的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">訂單號碼</td> 
      <td>如果有與此付費記錄關聯的採購單編號，請在此欄位中指定此資訊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">發票 ID</td> 
      <td>如果存在與此付費記錄相關聯的商業發票，請在此欄位中指定此資訊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">附加金額</td> 
      <td>輸入付費記錄的固定金額。 這是您針對此專案對外部客戶、承包商或合作夥伴開立帳單的金額。 記帳記錄的狀態變更為「已記帳」後，便無法修改此金額。</td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）在&#x200B;**自訂Forms**&#x200B;下，選取要新增至付費記錄的付費記錄自訂表單。

   您（或其他可存取自訂表單的使用者）必須先建立自訂表單的計費記錄，您才能在這裡選取它。 清單中只會顯示作用中的自訂表單。 如需建立自訂表單的相關資訊，請參閱[使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

   您可以重複此步驟，以新增付費記錄所需的其他自訂表格。

1. 按一下&#x200B;**儲存。**

   已建立付費記錄。 若要在計費記錄中包含可計費時數、費用與固定收入，請遵循下小節中概述的步驟。

## 在記帳記錄中包含可記帳小時、費用和固定收入

* [在記帳記錄中包含可記帳小時](#include-billable-hours-in-a-billing-record)
* [在記帳記錄中包含可記帳費用](#include-billable-expenses-in-a-billing-record)
* [在付費記錄中包含固定收入](#include-fixed-revenues-in-a-billing-record)

### 在記帳記錄中包含可記帳小時 {#include-billable-hours-in-a-billing-record}

您可以在帳單記錄中包含已登入任務、問題或專案的小時數。\
如果記錄時數的使用者或其主要工作角色與每小時計費率相關聯，則這些時數的收入會新增到計費記錄。

* [哪些小時可以新增至付費記錄](#what-hours-can-be-added-to-a-billing-record)
* [將時數新增至付費記錄](#add-hours-to-a-billing-record)

#### 可以向付費記錄新增哪些小時 {#what-hours-can-be-added-to-a-billing-record}

當滿足以下條件時，您可以新增時數到計費記錄：

* 任務、問題或專案已記錄時數。
* 所記錄時數的「時數型別」會標籤為收入。

  如需小時型別的詳細資訊，請參閱文章[管理小時型別](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md)。

* 如果為問題或專案記錄的所有小時記錄的使用者具有與他們或其主要工作角色關聯的每小時計費率，則可以將其新增到計費記錄。
* 如果時數記錄於任務上，則任務必須具有以下收入型別：

   * 收入型別不可設定為不可記帳。
   * 如果「收入型別」設定為「每小時使用者」，則記錄時間的使用者必須在他們的設定檔中設定每小時計費率。
   * 如果「收入型別」設定為「每小時角色」，則記錄時間之使用者的主要角色必須具有每小時收費率。

     >[!NOTE]
     >
     >您可以在專案層級覆寫職務角色的收費率。\
     >如需有關覆寫工作角色收費率的詳細資訊，請參閱文章[覆寫工作角色收費率和計算專案收入的概觀](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)中的「在專案層級覆寫工作角色收費率」一節。

* 如果在[專案設定]下核取&#x200B;**此專案需要核准時間**，則專案所有者必須核准記錄的時數。\
  如需有關專案時數要求核准的詳細資訊，請參閱文章[專案要求核准時間](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md)。

#### 將時數新增至付費記錄 {#add-hours-to-a-billing-record}

若要將可記帳時數新增至記帳記錄，請執行下列步驟：

1. 前往具有付費記錄的專案。
1. 按一下左側面板中的&#x200B;**記帳記錄**。

   此節可能位於&#x200B;**顯示更多**&#x200B;下。

1. 按一下付費記錄的&#x200B;**描述**&#x200B;以開啟&#x200B;**付費記錄詳細資料**&#x200B;標籤。

1. 按一下左側面板中的&#x200B;**可記帳小時**。
1. 如果帳單記錄中可能包含時數，請按一下&#x200B;**新增時數**。\
   **新增可記帳小時**&#x200B;方塊開啟。

   >[!NOTE]
   >
   >如果未記錄時數，或如果記錄的時數不符合新增至計費記錄所需的條件，則不會顯示&#x200B;**新增時數**&#x200B;按鈕。 如需有關哪些時數可記錄至付費記錄的詳細資訊，請參閱本文中[哪些時數可新增至付費記錄](#what-hours-can-be-added-to-a-billing-record)小節。

1. 選取要包含在付費記錄中的小時專案，然後按一下&#x200B;**新增小時**。\
   已將實際時數成本新增為&#x200B;**可記帳時數**&#x200B;金額至&#x200B;**記帳記錄總計**。

1. （選擇性）按一下&#x200B;**記帳記錄詳細資料**&#x200B;以檢閱&#x200B;**可記帳小時**&#x200B;和&#x200B;**記帳記錄總計**&#x200B;金額。 您也可以在記帳記錄的標題中檢視記帳記錄總計。

### 在記帳記錄中包含可記帳費用 {#include-billable-expenses-in-a-billing-record}

如果您要將「可記帳費用」新增到記帳記錄中，請確保將任務和專案上的費用標籤為「可記帳」。 未標籤為可記帳的費用無法新增到記帳記錄中。 如需有關新增費用的詳細資訊，請參閱文章[管理專案費用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。

若要將可記帳費用新增至記帳記錄，請執行下列步驟：

1. 前往具有付費記錄的專案。
1. 按一下左側面板中的&#x200B;**記帳記錄**。

   您可能需要按一下&#x200B;**顯示更多**，然後按一下&#x200B;**記帳記錄**。

1. 按一下付費記錄的&#x200B;**描述**&#x200B;以開啟&#x200B;**付費記錄詳細資料**&#x200B;標籤。

1. 按一下左側面板中的&#x200B;**可記帳費用**。
1. （視條件而定）如果您已將費用新增至您的任務或專案，並已將其標示為可記帳，請按一下&#x200B;**新增費用**。

   >[!NOTE]
   >
   >如果您有費用但未標籤為可記帳，則不會顯示&#x200B;**新增費用**&#x200B;按鈕。 只有實際金額大於零的可開立帳單費用才有資格納入帳單記錄中。

1. 選取可新增至記帳記錄的可記帳費用，然後按一下[新增費用]。****\
   將費用的實際金額新增為&#x200B;**可記帳費用**&#x200B;金額至&#x200B;**記帳記錄總計**。

1. （選擇性）按一下&#x200B;**記帳記錄詳細資料**&#x200B;以檢閱&#x200B;**可記帳費用**&#x200B;和&#x200B;**記帳記錄總計**&#x200B;金額。 您也可以在記帳記錄的標題中檢視記帳記錄總計。

### 在付費記錄中包含固定收入 {#include-fixed-revenues-in-a-billing-record}

如果您的任務有可用的固定收入，您可以將「固定收入」新增到記帳記錄。 沒有其他型別的任務或專案收入可新增到記帳記錄中。 如需有關收入型別的詳細資訊，請參閱[帳單和收入總覽](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)中的[帳單和收入總覽](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)區段。

若要將固定收入新增至付費記錄：

1. 前往具有付費記錄的專案。
1. 按一下左側面板中的&#x200B;**記帳記錄**。

   您可能需要按一下&#x200B;**顯示更多**，然後按一下&#x200B;**記帳記錄**。

1. 按一下付費記錄的&#x200B;**描述**&#x200B;以開啟&#x200B;**付費記錄詳細資料**&#x200B;標籤。

1. 選取「**固定收入**」標籤。
1. 如果您已將固定收入新增至工作，請按一下[新增固定收入]。****

   >[!NOTE]
   >
   >如果您在任務上有收入金額，但是金額未標籤為「固定」，則不會顯示&#x200B;**新增固定收入**&#x200B;按鈕。

1. 選取您要將其固定收入納入付費記錄中的任務，然後按一下[新增任務]。****\
   任務的&#x200B;**固定收入**&#x200B;金額已新增為&#x200B;**可記帳收入**&#x200B;金額至&#x200B;**記帳記錄總計**。

1. （選擇性）按一下&#x200B;**記帳記錄詳細資料**&#x200B;以檢閱&#x200B;**可記帳收入**&#x200B;和&#x200B;**記帳記錄總計**&#x200B;金額。 您也可以在記帳記錄的標題中檢視記帳記錄總計。

## 編輯付費記錄

建立付費記錄並在付費記錄中包含時數、費用和收入後，您可以在標籤為已付費之前編輯現有記錄的一些資訊。

1. 前往付費記錄。
1. 在左側面板中選取&#x200B;**記帳記錄詳細資料**&#x200B;後，編輯任何可用欄位中的資訊

   或

   按一下右上角的&#x200B;**編輯圖示** ![](assets/edit-icon.png)，然後編輯任何可用欄位中的資訊。

   更新下列專案：

   * **說明**
   * **記帳狀態**

     >[!TIP]
     >
     >如果您選取&#x200B;**Billed**&#x200B;作為Billing Status，則在您儲存變更後，將無法編輯付費記錄。

   * **記帳日期**
   * **採購單編號**
   * **發票識別碼**
   * **額外金額**

   下列欄位無法編輯：

   * **可記帳小時：**&#x200B;記帳記錄中包含之小時實際收入的總和。 如需有關在付費記錄中包含時數的詳細資訊，請參閱本文中的[在付費記錄中包含可付費時數](#include-billable-hours-in-a-billing-record)一節。

   * **可記帳費用**：包含在記帳記錄中的可記帳費用實際金額總計。 如需將可記帳費用包含在記帳記錄中的詳細資訊，請參閱本文中的[將可記帳費用包含在記帳記錄中](#include-billable-expenses-in-a-billing-record)一節。

   * **可記帳收入**：記帳記錄中包含之任務的固定收入總計。 如需有關在付費記錄中包含固定收入的詳細資訊，請參閱本文中的[在付費記錄中包含固定收入](#include-fixed-revenues-in-a-billing-record)小節。

   * **記帳記錄總計**：所有可記帳金額的總計。 計算公式如下：

     ```
     Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
     ```

1. 按一下&#x200B;**儲存****變更**。
