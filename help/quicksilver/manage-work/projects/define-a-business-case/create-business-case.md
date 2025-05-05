---
navigation-topic: business-case-and-scorecards
title: 為專案建立業務案例
description: 您可以使用業務案例來請求專案，並定義專案的目的、預算和潛在利益。 Portfolio經理或專案贊助者會使用業務案例的資訊來分析專案，並在核准專案之前先設定其優先順序。
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: fedb0328450896d212081715df4cde7644b169bc
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 0%

---

# 為專案建立業務案例

您可以使用業務案例來請求專案，並定義專案的目的、預算和潛在利益。 Portfolio經理或項目贊助者使用企業案例中的資訊在批准專案之前對其進行分析和優先順序排序。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Systems Workfront 許可證</td> 
   <td> <p>計劃或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級組態</td> 
   <td> <p>編輯對專案、財務數據和資源管理的訪問</p> <p>注意：如果您仍然沒有訪問許可權，請詢問您的 Workfront 管理員是否在您的訪問許可權級別中設置了其他限制。 有關 Workfront 管理員如何修改存取權限等級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理項目的許可權或更高許可權</p> <p>有關請求其他存取權限的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對物件 </a>的存取權限 。</p> </td> 
  </tr> 
 </tbody> 
</table>

有關此表中資訊的更多詳細資訊，請參閱 [Workfront 文件中](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)的訪問要求。

+++

## 先決條件

通過企業案例請求專案時，請考慮以下事項：

* 您的Adobe Workfront管理員或群組管理員必須啟用業務案例的區段，這些區段才會出現在您的專案中。\
  如需有關在系統層級啟用業務案例中章節的資訊，請參閱文章[設定系統範圍的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

  如需業務案例領域的相關資訊，請參閱文章[業務案例領域概觀](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)。

* 如果您希望專案在Portfolio優化器中獲得分數，則必須完成除目標區域之外的企業案例的所有區域。 完成目標區域是可選的。 專案在Portfolio優化器中接收分數，平均如果此區域未完成。

  如需有關使用計分卡和Portfolio Optimizer的資訊，請參閱文章[將計分卡套用至專案並產生一致性分數](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)。

## 建立業務案例

{{step1-to-projects}}

1. 按一下&#x200B;**新增專案**，然後從出現的下拉式清單中選取&#x200B;**要求專案**。 專案已建立，且預設會指派&#x200B;**Idea**&#x200B;狀態。

   >[!CAUTION]
   >
   >如果您的Workfront例項中已刪除「構想」狀態，則專案會根據「專案偏好設定」區域中的定義，置於新專案的預設狀態。 如需有關設定專案偏好設定的資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

1. 在專案標題欄位中輸入名稱。
1. （選擇）按兩下「 **更多** 」圖示 ![「更多」圖示](assets/qs-more-icon-on-an-object.png)，然後按下 **「附加範本** 」以創建專案的工作分解結構。

   或

   開始手動向專案添加任務。

1. （有條件）如果選擇附加範本，請繼續將範本附加到專案。
1. 在左側面板中，按兩下企業 **案例**」。
1. （選擇）要編輯“項目信息”**部分，請按兩下**&#x200B;編輯項目資訊&#x200B;**。**

   有關編輯「**項目資訊**」部分字段的詳細資訊，請參閱文章[企業](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)案例區域概述中的項目資訊[&#128279;](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info)部分。

1. （選擇）要编辑目標&#x200B;**&#x200B;**&#x200B;部分，請按兩下&#x200B;**編輯目標**。

   有關編輯企業案例的“**目標**”部分的詳細資訊，請參閱企業案例[&#128279;](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)區域概述一文[中的目標](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals)部分。

1. （選擇）要編輯 **“費用”** 部分，請按兩下 **編輯費用**。

   有關編輯&#x200B;**企業案例的「費用**」部分的詳細資訊，請參閱企業案例[&#128279;](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)區域概述一文[中的“費用](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses)”部分。

1. （選擇性）按一下&#x200B;**編輯資源預算**&#x200B;以預算您的資源，並取得與專案上工作角色相關的預算勞力成本。 如需詳細資訊，請參閱業務案例中的[預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

   >[!TIP]
   >
   >此處顯示的資訊與系統層級資源預算工具中顯示的資訊相同。

1. （選擇性）按一下&#x200B;**編輯風險**&#x200B;以新增此專案的潛在風險。 有關向企業案例添加風險的資訊，請參閱[企業案例](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)區域概述一文[中的“風險](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks)”部分。
1. （選擇）**在將**&#x200B;計分卡新增至此專案&#x200B;**下拉功能表中選取計分卡**。

   必須先建立計分卡，才能將其附加至專案。

   有關計分卡的詳細資訊，請參閱將計分卡套用到專案並生成對齊方式分數[&#128279;](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)一文。

1. （選擇）**在自定義Forms**&#x200B;下拉功能表中選擇&#x200B;**自定義表單。**

   必須先建立自定義Forms，才能將其附加到專案。

   有關自定義Forms窗體的詳細資訊，請參閱建立自定義表單[&#128279;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)一文。

1. 按兩下&#x200B;**提交**。 項目狀態將更改為 **「已請求」** 並提交該專案以批准企業案例。

   有關批准企業案例的詳細信息，請參閱批准企業案例[&#128279;](../../../manage-work/projects/define-a-business-case/approve-business-case.md)一文。


>[!TIP]
>
> 完成企業案例后，可以將其副本導出到.pdf文件。有關將企業案例匯出到.pdf文件的詳細資訊，請參閱 [匯出專案的](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md)企業案例。


