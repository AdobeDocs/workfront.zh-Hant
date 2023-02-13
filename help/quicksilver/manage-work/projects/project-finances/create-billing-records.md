---
navigation-topic: financials
title: 建立計費記錄
description: 除了設定收入和追蹤費用外，您還可以在項目上建立計費記錄，以了解需要計費的資訊。
author: Alina
feature: Work Management
exl-id: 6f17a892-7f64-4712-8ee2-7a1940b99be3
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 1%

---

# 建立計費記錄

除了設定收入和追蹤費用外，您還可以在項目上建立計費記錄，以了解需要計費的資訊。

您不能為任務建立計費記錄。 您只能為專案建立計費記錄。

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

## 帳單記錄概觀

系統會建立帳單記錄作為項目的附件，並包含來自項目的財務資料以及項目中任務的某些財務資訊。

在計畫使用計費記錄時，請考慮以下事項：

* 要將與項目相關的金額開單給外部供應商或合作夥伴時，可建立開單記錄。 除了向外部來源開單固定金額外，有時您還需要向外部承包商開單（從記錄時數），以及發生的費用或固定收入金額。 您可以將所有這些資訊納入相同的計費記錄中。
* 一旦帳單記錄設為「已計費」，便無法編輯該記錄。

   >[!IMPORTANT]
   >
   >當您的費率不同，而且您想要鎖定專案的收入和費用資訊時，這點很重要。 將其添加到計費記錄中並標籤為「已計費」，會在費率在您的系統中更新時阻止其更新。

* 無法刪除標籤為「已開單」的具有開單記錄的項目。

## 建立計費記錄

1. 導覽至專案。
1. 按一下 **帳單記錄** 中。

   此區段可能位於 **顯示更多**.

1. 使用 **帳單記錄詳細資訊** 在左側面板中選取，按一下 **新帳單記錄**.
1. 在 **新帳單記錄** 框中，指定以下資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>這是必填欄位. 指定帳單記錄的說明，以反映此記錄的用途或目的。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">記帳狀態</td> 
      <td> <p>選擇 <strong>未計費</strong>，如果此記錄尚未計費。</p> <p>選擇 <strong>已計費</strong> 開單記錄時。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">記帳日期</td> 
      <td>按一下日曆表徵圖，選擇此計費記錄的計費日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">訂單號</td> 
      <td>如果有與此開單記錄關聯的PO編號，請在此欄位中指定此資訊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">發票 ID</td> 
      <td>如果有與此開單記錄關聯的發票，請在此欄位中指定此資訊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">附加金額</td> 
      <td>輸入計費記錄的固定金額。 這是您打算為此項目向外部客戶、承包商或合作夥伴開單的金額。 在將開單記錄的狀態更改為「已開單」後，無法修改此金額。</td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）下方 **自訂Forms**，選擇要添加到計費記錄的自定義表單。

   您（或其他可存取自訂表單的使用者）必須先建立帳單記錄自訂表單，才能在此處選取。 清單中只會顯示使用中的自訂表單。 如需建立自訂表單的相關資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   您可以重複此步驟，以新增計費記錄所需的其他自訂表單。

1. 按一下 **儲存。**

   帳單記錄已建立。 要在計費記錄中包括「計費小時數」、「費用」和「固定收入」，請遵循以下子部分中概述的步驟。

## 在計費記錄中包括計費小時數、費用和固定收入

* [在計費記錄中包括計費小時數](#include-billable-hours-in-a-billing-record)
* [在開單記錄中包括可開單費用](#include-billable-expenses-in-a-billing-record)
* [在計費記錄中包括固定收入](#include-fixed-revenues-in-a-billing-record)

### 在計費記錄中包括計費小時數 {#include-billable-hours-in-a-billing-record}

您可以在計費記錄中加入已登入工作、問題或專案的小時數。\
如果記錄小時數或其主要職務角色的使用者與每小時費率相關聯，則這些小時的收入會新增至計費記錄。

* [可以在計費記錄中添加幾小時](#what-hours-can-be-added-to-a-billing-record)
* [將小時數添加到計費記錄](#add-hours-to-a-billing-record)

#### 可以在計費記錄中添加幾小時 {#what-hours-can-be-added-to-a-billing-record}

您可以在符合下列條件時，將小時數新增至計費記錄：

* 任務、問題或項目記錄了數小時。
* 記錄小時數的「小時」類型會標示為「計為收入」。

   如需「小時類型」的詳細資訊，請參閱文章 [管理小時類型](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

* 如果記錄時間的使用者具有與其或其主要工作角色相關聯的每小時計費比率，則針對問題或專案記錄的所有小時數都可新增至計費記錄。
* 如果任務記錄了小時數，則任務必須具有以下收入類型：

   * 「收入類型」不能設定為「不可開單」。
   * 如果「收入類型」設為「每小時使用者」，則記錄該時間的使用者的設定檔中必須設定「每小時計費」比率。
   * 如果「收入類型」設定為「每小時」角色，則記錄該時間的用戶的「主要角色」必須具有「每小時計費」比率。

      >[!NOTE]
      >
      >您可以改寫項目層職務職責的開單費率。\
      >有關改寫職務開單費率的詳細資訊，請參閱文章中的「在項目層改寫職務開單費率」一節 [改寫任務職責開單費率和計算項目收入概覽](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

* 若 **需要為此項目批准的時間** 在「專案設定」下勾選，則專案擁有者必須核准記錄的小時數。\
   有關需要在項目時間進行審批的詳細資訊，請參閱文章 [需要為項目批准的時間](../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md).

#### 將小時數添加到計費記錄 {#add-hours-to-a-billing-record}

要將計費小時數添加到計費記錄，請執行以下操作：

1. 前往包含計費記錄的專案。
1. 按一下 **帳單記錄** 中。

   此區段可能位於 **顯示更多**.

1. 按一下 **說明** 開啟 **帳單記錄詳細資訊** 標籤。

1. 按一下 **計費小時數** 中。
1. 如果計費記錄中可能包含的小時數，請按一下 **添加小時**.\
   此 **添加計費小時數** 框。

   >[!NOTE]
   >
   >如果沒有記錄小時數，或者記錄的小時數不符合要添加到計費記錄中的條件，則 **添加小時** 按鈕未顯示。 如需可記錄哪些小時至計費記錄的詳細資訊，請參閱區段 [可以在計費記錄中添加幾小時](#what-hours-can-be-added-to-a-billing-record) 這篇文章。

1. 選擇要包括在計費記錄中的小時條目，然後按一下 **添加小時**.\
   小時數的實際成本會新增為 **計費小時數** 金額 **帳單記錄總計**.

1. （選用）按一下 **帳單記錄詳細資訊** 若要檢閱 **計費小時數** 和 **帳單記錄總計** 金額。 您也可以在計費記錄的標題中看到計費記錄合計。

### 在開單記錄中包括可開單費用 {#include-billable-expenses-in-a-billing-record}

如果要將「可開單費用」添加到開單記錄，請確保任務和項目上的費用標籤為「可開單」。 未標籤為「可開單」的費用不可用於在開單記錄中添加。 有關添加費用的詳細資訊，請參閱文章 [管理項目費用](../../../manage-work/projects/project-finances/manage-project-expenses.md).

要將可開單費用添加至開單記錄，請執行以下操作：

1. 前往包含計費記錄的專案。
1. 按一下 **帳單記錄** 中。

   您可能必須按一下 **顯示更多**，然後 **帳單記錄**.

1. 按一下 **說明** 開啟 **帳單記錄詳細資訊** 標籤。

1. 按一下 **計費費用** 中。
1. （條件性）如果已將費用添加到任務或項目中，並將其標籤為計費，請按一下 **添加費用**.

   >[!NOTE]
   >
   >如果您有費用，但未標籤為「計費」，則 **添加費用** 按鈕未顯示。 只有實際金額大於零的可開單費用才有資格納入開單記錄。

1. 選擇可添加到計費記錄的計費費用，然後按一下 **添加費用**.\
   費用的實際金額將作為 **計費費用** 金額 **帳單記錄總計**.

1. （選用）按一下 **帳單記錄詳細資訊** 若要檢閱 **計費費用** 和 **帳單記錄總計** 金額。 您也可以在計費記錄的標題中看到計費記錄合計。

### 在計費記錄中包括固定收入 {#include-fixed-revenues-in-a-billing-record}

如果您有具有「固定收入」可用的任務，則可以將「固定收入」添加到您的計費記錄中。 沒有其他類型的任務或項目收入可以添加到計費記錄中。 如需收入類型的詳細資訊，請參閱 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) 區段 [帳單和收入概觀](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

要將固定收入添加到計費記錄，請執行以下操作：

1. 前往包含計費記錄的專案。
1. 按一下 **帳單記錄** 中。

   您可能必須按一下 **顯示更多**，然後 **帳單記錄**.

1. 按一下 **說明** 開啟 **帳單記錄詳細資訊** 標籤。

1. 選取 **固定收入** 標籤。
1. 如果已將固定收入添加到任務中，請按一下 **添加固定收入**.

   >[!NOTE]
   >
   >如果任務上有收入額，但未標籤為「固定」，則 **新增固定收入** 按鈕未顯示。

1. 選擇要在計費記錄中包含其固定收入的任務，然後按一下 **添加任務**.\
   此 **固定收入** 任務數量會新增為 **計費收入** 金額 **帳單記錄總計**.

1. （選用）按一下 **帳單記錄詳細資訊** 若要檢閱 **計費收入** 和 **帳單記錄總計** 金額。 您也可以在計費記錄的標題中看到計費記錄合計。

## 編輯帳單記錄

在建立開單記錄並在開單記錄中包括小時數、費用和收入後，您可以在將現有記錄標籤為「已開單」之前，編輯現有記錄中的一些資訊。

1. 轉到計費記錄。
1. 使用 **帳單記錄詳細資訊** 在左側面板中選取，編輯任何可用欄位中的資訊

   或

   按一下 **編輯圖示** ![](assets/edit-icon.png) 在右上角，然後編輯任何可用欄位中的資訊。

   更新下列項目：

   * **說明**
   * **記帳狀態**

      >[!TIP]
      >
      >如果您選取 **已計費** 對於「帳單狀態」，在保存更改後，無法編輯帳單記錄。

   * **記帳日期**
   * **訂單號**
   * **發票 ID**
   * **附加金額**

   下列欄位無法編輯：

   * **計費小時數：** 計費記錄中包含的小時的實際收入總額。 有關將小時數納入計費記錄的詳細資訊，請參閱區段 [在計費記錄中包括計費小時數](#include-billable-hours-in-a-billing-record) 這篇文章。

   * **計費費用**:計費記錄中包括的可開單費用的實際金額合計。 有關在計費記錄中包括計費費用的詳細資訊，請參閱 [在開單記錄中包括可開單費用](#include-billable-expenses-in-a-billing-record) 這篇文章。

   * **計費收入**:計費記錄中包含之任務的固定收入總計。 有關在計費記錄中包括固定收入的詳細資訊，請參閱 [在計費記錄中包括固定收入](#include-fixed-revenues-in-a-billing-record) 這篇文章。

   * **帳單記錄總計**:所有可開單金額的合計。 此計算公式如下：

      ```
      Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)
      ```


1. 按一下 **儲存****變更**.
