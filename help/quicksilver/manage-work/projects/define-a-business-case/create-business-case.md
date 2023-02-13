---
navigation-topic: business-case-and-scorecards
title: 為項目建立業務案例
description: 您可以使用業務案例來請求項目並定義項目的用途、預算和潛在收益。 Portfolio經理或項目贊助商使用業務案例中的資訊，在批准項目之前分析項目並確定其優先順序。
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 0%

---

# 為項目建立業務案例

您可以使用業務案例來請求項目並定義項目的用途、預算和潛在收益。 Portfolio經理或項目贊助商使用業務案例中的資訊，在批准項目之前分析項目並確定其優先順序。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計畫或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對項目、財務資料和資源管理的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案的或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

透過業務案例要求專案時，請考量下列事項：

* 您的Adobe Workfront管理員或群組管理員必須先啟用「業務案例」的區段，才能顯示在您的專案中。\
   有關在系統級別啟用「業務案例」中各節的資訊，請參閱文章 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   有關「業務案例」區域的資訊，請參閱文章 [業務案例領域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* 如果希望項目在Portfolio優化程式中獲得分數，則必須完成除目標區域之外的業務案例的所有區域。 完成「目標」區域是選填的。 即使此區域尚未完成，專案仍會在Portfolio最佳化程式中收到分數。

   如需使用計分卡和使用Portfolio最佳化程式的相關資訊，請參閱文章 [將計分卡套用至專案並產生對齊分數](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## 建立業務案例

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)，然後按一下 **專案**.
1. 按一下 **新增專案** 選取 **要求專案**.\
   依預設，專案會放置在 **構想** 狀態。

   >[!CAUTION]
   >
   >如果已在您的Workfront執行個體中刪除構想狀態，則會將專案置於新專案的預設狀態，如「專案偏好設定」區域中所定義。 有關設定項目首選項的資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. 指定專案的名稱，然後按Enter鍵。
1. （選用）按一下 **更多** 圖示 ![](assets/qs-more-icon-on-an-object.png)，然後 **附加模板**，以建立專案的工作劃分結構。

   或

   開始手動將任務添加到項目。

1. （條件性）如果您選取附加範本，請繼續將範本附加至專案
1. 按一下 **業務案例** 中。
1. （選用）按一下 **編輯專案資訊**. 

   有關編輯「業務案例」的「項目資訊」部分中欄位的詳細資訊，請參閱 [專案資訊](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) 在文章中 [業務案例領域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. （選用）按一下 **編輯目標**.

   有關編輯業務案例的「目標」部分的詳細資訊，請參閱 [目標](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) 在文章中 [業務案例領域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. （選用）按一下&#x200B;**編輯費用**.

   有關編輯「業務案例」的「費用」部分的詳細資訊，請參閱 [費用](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) 在文章中 [業務案例領域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. （可選）使用「資源預算」區域來預算資源，並獲取與項目上的任務職責關聯的預算人工成本。 如需詳細資訊，請參閱 [業務案例中的預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >此處顯示的資訊與系統級資源預算工具中顯示的資訊相同。

1. （選用）按一下 **編輯風險** 為項目增加潛在風險。 有關向業務案例添加風險的資訊，請參閱 [風險](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks) 文章一節 [業務案例領域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
1. （選用）選取&#x200B;**計分卡** 在 **新增計分卡****至此專案** 下拉式功能表。

   必須先建立計分卡，才能將其附加至專案。

   如需計分卡的詳細資訊，請參閱文章 [將計分卡套用至專案並產生對齊分數](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. （選用）選取 **自訂表單** 在 **自訂Forms** 下拉式功能表。

   必須先建立自訂Forms，才能將其附加至專案。

   如需自訂Forms的詳細資訊，請參閱文章 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 按一下 **提交**.

   專案狀態已變更為 **已請求** 並提交以批准《業務案例》。

   有關批准業務案例的詳細資訊，請參閱文章 [批准業務案例](../../../manage-work/projects/define-a-business-case/approve-business-case.md).

1. （選用）完成商業案例後，您可以將其復本匯出為.pdf檔案。 有關將業務案例導出為.pdf檔案的詳細資訊，請參閱文章中的「導出業務案例」部分 [業務案例領域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
