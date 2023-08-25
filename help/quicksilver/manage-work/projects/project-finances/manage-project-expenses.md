---
product-area: projects
navigation-topic: financials
title: 管理專案費用
description: 專案與任務相關費用的建立與管理費用流程相同。 在業務案例中新增到專案的任何費用都會新增到費用標籤作為計畫費用。 如需業務案例的詳細資訊，請參閱為專案建立業務案例一文。
author: Alina
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: 647788221b4acff1cfd5e0ce14d5b99cf90ceee0
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 1%

---

# 管理專案費用

專案與任務相關費用的建立與管理費用流程相同。 在業務案例中新增到專案的任何費用都會新增到費用標籤作為計畫費用。 如需業務案例的詳細資訊，請參閱文章 [為專案建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

您所有任務和專案的費用總計會貢獻專案的總成本。 費用的「計畫金額」會貢獻專案的「計畫成本」，費用的「實際金額」會貢獻專案的「實際成本」。

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
   <td> <p>工作或更高 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案與財務資料的存取權</p> <p><b>附註</b> </p>
   <p> 如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>專案貢獻或更高許可權，並具有檢視或管理財務的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 新增費用

1. 移至您要輸入費用的專案。\
   如果您想要將費用新增至任務，請改為導覽至任務。 
1. 按一下 **顯示更多**，然後按一下 **費用**.
1. 按一下 **新增費用** .
此 **新增費用** 對話方塊隨即顯示。
1. 更新下列專案：

   * **說明：** 費用的說明。

   * **費用型別：** （必要）選取最能描述費用的類別。
   * **工作：** 開始輸入與此費用相關聯的工作名稱，然後當名稱出現在下拉式清單中時按一下它。
   * **計畫數量：** 費用的計畫預算金額。\
     這會影響專案的預算成本。

   * **實際數量：** 費用實際成本的金額。\
     這會影響專案的實際成本。

   * **計畫日期：** 費用的預期發生日期。 您可以使用在欄位中輸入日期 *mm/dd/yy* 格式，或按一下日曆圖示  ![](assets/calendar-icon.png) 並動態選取日期。

   * **支付日期：** 支付費用的日期。
   * **可記帳：** 若要對此費用開立帳單，請選取此選項。 建立付費記錄時，將費用分類為可付費很重要。
   * **可償還：** 如果需要償還費用，請選取此選項。 然後，您可以在費用已償還後，將費用標示為已償還。

1. 選取 **自訂表格** 並指定所需的任何其他資訊。 您必須先建立自訂表格，然後才能將其與費用建立關聯。 清單中只會顯示作用中的自訂表單。 如需建立自訂表單的相關資訊，請參閱文章 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 按一下 **儲存變更**.

## 刪除費用

1. 前往您要刪除費用的專案。
1. 按一下&#x200B;**顯示更多**，然後按一下 **費用**.
1. 選取您要刪除的費用，然後按一下 **刪除** ![刪除](assets/delete.png).

1. 按一下 **是的，刪除** 以確認刪除。
