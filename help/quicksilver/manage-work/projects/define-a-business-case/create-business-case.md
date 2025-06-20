---
navigation-topic: business-case-and-scorecards
title: 為專案建立業務案例
description: 您可以使用業務案例來請求專案，並定義專案的目的、預算和潛在利益。 Portfolio經理或專案贊助者會使用業務案例的資訊來分析專案，並在核准專案之前先設定其優先順序。
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---

# 為專案建立業務案例

<!--Audited: 6/2025-->

您可以使用業務案例來請求專案，並定義專案的目的、預算和潛在利益。 Portfolio經理或專案贊助者會使用業務案例的資訊來分析專案，並在核准專案之前先設定其優先順序。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> 
   <p>目前：Prime或更新版本</p> 
   <p>舊版：Pro或更高版本</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td> 
   <p>目前：標準 </p> 
   <p>舊版：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>編輯專案、財務資料及資源管理的存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p>管理專案或更高的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

透過業務案例請求專案時，請考慮以下事項：

* 您的Adobe Workfront管理員或群組管理員必須啟用業務案例的區段，這些區段才會出現在您的專案中。\
  如需有關在系統層級啟用業務案例中章節的資訊，請參閱文章[設定系統範圍的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

  如需業務案例領域的相關資訊，請參閱文章[業務案例領域概觀](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)。

* 如果您希望專案在Portfolio Optimizer中收到分數，您必須完成業務案例的所有區域，但「目標」區域除外。 完成目標區域為選用。 專案會在Portfolio Optimizer中收到分數，即使此區域未完成。

  如需有關使用計分卡和Portfolio Optimizer的資訊，請參閱文章[將計分卡套用至專案並產生一致性分數](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)。

## 建立業務案例

{{step1-to-projects}}

1. 按一下&#x200B;**新增專案**，然後從出現的下拉式清單中選取&#x200B;**要求專案**。 專案已建立，且預設會指派&#x200B;**Idea**&#x200B;狀態。

   >[!CAUTION]
   >
   >如果您的Workfront例項中已刪除「構想」狀態，則專案會根據「專案偏好設定」區域中的定義，置於新專案的預設狀態。 如需有關設定專案偏好設定的資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

1. 在專案標題欄位中輸入名稱。
1. （選擇性）按一下&#x200B;**更多**&#x200B;圖示![更多圖示](assets/qs-more-icon-on-an-object.png)，然後&#x200B;**附加範本**&#x200B;以建立專案的工作劃分結構。

   或

   開始手動將任務新增至專案。

1. （視條件而定）如果您已選取附加範本，請繼續將範本附加到專案。
1. 在左側面板中，按一下&#x200B;**業務案例**。
1. （選擇性）若要編輯&#x200B;**專案資訊**&#x200B;區段，請按一下&#x200B;**編輯專案資訊**。 

   如需有關編輯&#x200B;**專案資訊**&#x200B;區段欄位的詳細資訊，請參閱文章[業務案例區域概觀](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)中的[專案資訊](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info)區段。

1. （選擇性）若要編輯&#x200B;**目標**&#x200B;區段，請按一下&#x200B;**編輯目標**。

   如需有關編輯業務案例的&#x200B;**目標**&#x200B;區段的詳細資訊，請參閱文章[業務案例領域總覽](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)中的[目標](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals)區段。

1. （選擇性）若要編輯&#x200B;**費用**&#x200B;區段，請按一下&#x200B;**編輯費用**。

   如需有關編輯業務案例的&#x200B;**費用**&#x200B;區段的詳細資訊，請參閱文章[業務案例領域總覽](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)中的[費用](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses)區段。

1. （選擇性）按一下&#x200B;**編輯資源預算**&#x200B;以預算您的資源，並取得與專案上工作角色相關的預算勞力成本。 如需詳細資訊，請參閱業務案例中的[預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

   >[!TIP]
   >
   >此處顯示的資訊與系統層級資源預算工具中顯示的資訊相同。

1. （選擇性）按一下&#x200B;**編輯風險**&#x200B;以新增此專案的潛在風險。 如需有關將風險新增至業務案例的資訊，請參閱文章[業務案例領域概觀](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)中的[風險](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks)區段。
1. （選擇性）在&#x200B;**將計分卡新增至此專案**&#x200B;下拉式功能表中選取&#x200B;**計分卡**。

   必須先建立計分卡，才能將其附加至專案。

   如需計分卡的詳細資訊，請參閱文章[將計分卡套用至專案並產生一致性分數](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)。

1. （選擇性）在&#x200B;**自訂Forms**&#x200B;下拉式功能表中選取&#x200B;**自訂表單**。

   必須先建立自訂Forms，才能將其附加到專案。

   如需有關自訂Forms的詳細資訊，請參閱文章[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 按一下&#x200B;**提交**。 專案狀態已變更為&#x200B;**已要求**，並已提交以核准業務案例。

   如需核准業務案例的詳細資訊，請參閱文章[核准業務案例](../../../manage-work/projects/define-a-business-case/approve-business-case.md)。


>[!TIP]
>
> 完成業務案例後，您可以將副本匯出至.pdf檔案。 如需將業務案例匯出為.pdf檔案的詳細資訊，請參閱[匯出專案的業務案例](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md)。


