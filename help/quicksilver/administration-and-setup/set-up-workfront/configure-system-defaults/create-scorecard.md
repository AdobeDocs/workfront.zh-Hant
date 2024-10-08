---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 建立計分卡
description: 計分卡可測量專案與專案組合先前建立之條件的符合程度。 計分卡通常會反映組織的使命、價值和策略目標。Portfolio管理員通常會定義計分卡問題和答案，以確保它們在專案優先順序和選擇期間是有意義和價值的。  [!DNL Adobe Workfront] 管理員會根據投資組合經理的建議來建置計分卡。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 1%

---

# 建立計分卡

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

計分卡可測量專案與專案組合先前建立之條件的符合程度。 計分卡通常可反映組織的使命、價值和策略目標。

Portfolio管理員通常會定義計分卡問題和答案，以確保它們在專案優先順序設定和選擇期間具有意義和價值。 [!DNL Adobe Workfront]管理員會根據投資組合經理的建議來建置計分卡。

為計分卡選擇的問題和答案必須可量化，以便提供可比較不同專案的對齊值。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>目前： [！UICONTROL Business]或更高版本</p> 
   或
   <p>新增：[！UICONTROL Prime]或以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>目前： [！UICONTROL計畫]</p>
   或
   <p>新增：[！UICONTROL Standard]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立計分卡

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 計分卡]**，然後按一下&#x200B;**[!UICONTROL 新增計分卡]**&#x200B;以啟動計分卡產生器並建立計分卡。

1. 指定&#x200B;**[!UICONTROL 計分卡名稱]**&#x200B;和&#x200B;**[!UICONTROL 描述]**。

   將計分卡與專案建立關聯時，會顯示名稱。 說明會顯示在計分卡清單中的計分卡名稱旁。

1. 按一下&#x200B;**[!UICONTROL 新增問題]**&#x200B;下拉式功能表，開啟[!UICONTROL 計分卡問題]區段，然後指定您問題的下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL Question]</td> 
      <td>輸入您要納入計分卡中的問題。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL點]</td> 
      <td>輸入此問題的最大可能分數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL負點]</td> 
      <td>選取此選項以指出[!DNL Workfront]應該從總可能點數中減去。 負分無法新增到計分卡的最大可能點數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL顯示型別]</td> 
      <td>如果您想要在計分卡中顯示數值欄位，讓使用者可指定介於0到100之間的任何值，請選取<strong>[！UICONTROL Value(0-100)]</strong>。<p>或者，選取<strong>[！UICONTROL下拉式清單]</strong>或<strong>[！UICONTROL選項按鈕]</strong>，以建立使用者可使用該控制項指定的答案。 按一下<strong>[！UICONTROL新增答案]</strong>，然後輸入此答案的<strong>[！UICONTROL值]</strong> （以百分點為單位），以備回應完成。 如果您選擇100%，則會完全達到分配給此問題的點數。 如果您要指出此答案只包含分配給此問題的總點數的一部分，請選取較低的百分比值。 例如，如果您的問題值是10點，而您想要此答案攜帶其中5點，請為您的值選擇50%。</p>
      <p>如果您要指出此答案為預設答案，請選取<strong>[！UICONTROL預設值]</strong>。</strong></p>
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 新增問題]**，依照相同步驟將更多問題和答案新增至您的計分卡。

   >[!NOTE]
   >
   >您可以依照正確順序拖放問題，重新排序計分卡中的問題。

1. 當您完成輸入所有資訊時，請按一下[儲存]。****

   這樣會建立計分卡，專案經理現在可以將其附加至其專案業務案例中。

## 將計分卡套用至專案

具有[!UICONTROL 管理]專案許可權的使用者可以在[!DNL Workfront]管理員建立計分卡後，將計分卡套用至專案。

計分卡會新增至專案，作為建立專案業務案例的一部分。 如需將計分卡新增至專案的詳細資訊，請參閱[將計分卡套用至專案並產生一致性分數](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)。

如需有關專案許可權的詳細資訊，請參閱[在 [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)中共用專案。
