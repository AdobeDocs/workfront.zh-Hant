---
product-area: projects
navigation-topic: financials
title: 管理項目費用
description: 項目和任務相關費用的建立和管理費用的流程相同。 在「業務案例」中添加到項目的任何費用都將作為計畫費用添加到「費用」標籤中。 有關「業務案例」的詳細資訊，請參閱建立專案的業務案例一文。
author: Alina
feature: Work Management
exl-id: 80c41b08-3618-4d6e-8d07-1736b2f824ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 1%

---

# 管理項目費用

項目和任務相關費用的建立和管理費用的流程相同。 在「業務案例」中添加到項目的任何費用都將作為計畫費用添加到「費用」標籤中。 有關「業務案例」的詳細資訊，請參閱文章 [為項目建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

來自所有任務和項目的總費用將計入項目的總成本。 費用的「計畫金額」將計入項目的「計畫成本」，而費用的「實際金額」將計入項目的「實際成本」。

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

## 新增費用

1. 轉到要輸入費用的項目。\
   如果要向任務添加費用，請改為定位至任務。 
1. 按一下 **顯示****更多**，然後按一下 **費用。**
1. 按一下 **添加費用。**
此 
**添加費用** 對話框。
1. 更新下列項目：

   * **說明：** 費用的說明。

   * **費用類型：** （必要）選擇最能說明費用的類別。
   * **任務：** 開始鍵入與此費用關聯的任務的名稱，然後在下拉清單中出現時按一下它。
   * **計畫金額：** 費用的計畫預算金額。\
      這會影響項目的預算成本。

   * **實際金額：** 費用的實際成本金額。\
      這會影響項目的實際成本。

   * **計畫日期：** 支出的預期日期。 您可以使用 *mm/dd/yy* 格式，或者按一下日曆圖示  ![](assets/calendar-icon.png) 並動態選取日期。

   * **付款日期：** 支付費用的日期。
   * **計費：** 如果要開單此費用，請選擇此選項。 建立計費記錄時，將費用分類為計費非常重要。
   * **可償還：** 如果需要報銷費用，請選擇此選項。 然後，您可以在報銷費用後將費用標籤為已報銷。

1. 選取 **自訂表單** 並指定任何需要的其他資訊。 您必須先建立自訂表單，才能將其與費用建立關聯。 清單中只會顯示使用中的自訂表單。 如需建立自訂表單的相關資訊，請參閱文章 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 按一下 **儲存變更。**

## 刪除費用

1. 轉到要刪除費用的項目。
1. 按一下&#x200B;**顯示****更多**，然後按一下 **費用。**
1. 選擇要刪除的費用，然後按一下 **刪除** ![刪除](assets/delete.png).

1. 按一下 **是，刪除它** 確認刪除。 
