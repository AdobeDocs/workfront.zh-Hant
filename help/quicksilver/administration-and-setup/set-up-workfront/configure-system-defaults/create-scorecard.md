---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 建立計分卡
description: 計分卡可衡量專案與先前建立之產品組合標準的一致程度。 計分卡通常反映組織的使命、價值和戰略目標。Portfolio經理通常會定義計分卡問題和答案，以確保它們在項目優先順序和選擇期間具有意義和價值。 安 [!DNL Adobe Workfront] 管理員會根據產品組合管理員的建議來建立計分卡。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# 建立計分卡

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

計分卡可衡量專案與先前建立之產品組合標準的一致程度。 計分卡通常反映組織的使命、價值和戰略目標。

Portfolio經理通常會定義計分卡問題和答案，以確保在進行專案優先順序排列和選取時，這些問題和答案有意義且有價值。 安 [!DNL Adobe Workfront] 管理員會根據產品組合管理員的建議來建立計分卡。

為計分卡選擇的問題和答案必須可量化，才能提供比較不同專案的協調價值。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>[!UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
 </tbody> 
</table>

## 建立計分卡

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 計分卡]**，然後按一下 **[!UICONTROL 新增計分卡]** 建立新計分卡並啟動計分卡建立程式。

1. 指定 **[!UICONTROL 計分卡名稱]** 和 **[!UICONTROL 說明]**.

   將計分卡與專案關聯時，系統會顯示名稱。 說明會顯示在計分卡清單中計分卡名稱旁。

1. 按一下 **[!UICONTROL 添加問題]** 下拉式功能表來開啟 [!UICONTROL 計分卡問題] ，然後指定下列問題資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL問題]</td> 
      <td>輸入要納入計分卡的問題。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL點]</td> 
      <td>輸入此問題可能的最大點數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL負點]</td> 
      <td>選取此選項以指出 [!DNL Workfront] 應從可能的總點數中減去。 無法將負分數新增至計分卡的最大可能點數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL顯示類型]</td> 
      <td>選擇 <strong>[!UICONTROL值(0-100)]</strong> 如果您想在計分卡中顯示數值欄位，讓使用者可以在其中指定0到100之間的任何值。<p>或者，選取 <strong>[!UICONTROL下拉式清單]</strong> 或 <strong>[!UICONTROL單選按鈕]</strong> 若要建立答案，使用者可使用該控制項指定。 按一下 <strong>[!UICONTROL添加答案]</strong>，然後輸入 <strong>[!UICONTROL值]</strong> 以百分點表示，若已完成。 如果您選擇100%，則會完全達到為此問題分配的點數。 如果您想指出此答案僅包含分配給此問題的總點數的一部分，請選取較低百分比值。 例如，如果您的問題值為10分，而且您希望此答案包含其中的5分，請為您的值選擇50%。</p>
      <p>選擇 <strong>[!UICONTROL預設值]</strong> 如果您指出此答案為預設答案，則此為預設答案。</strong></p>
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 添加問題]** 請依照相同步驟，為計分卡新增更多問題和答案。

   >[!NOTE]
   >
   >您可以以正確的順序拖放問題，重新排序計分卡中的問題。

1. 按一下 **[!UICONTROL 儲存]** 完成輸入資料時。

## 將計分卡套用至專案

使用 [!UICONTROL 管理] 專案的權限可在由建立計分卡後，將計分卡套用至專案 [!DNL Workfront] 管理員。

專案會新增計分卡，作為建立專案商業案例的一部分。 如需將計分卡新增至專案的詳細資訊，請參閱 [將計分卡套用至專案並產生對齊分數](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

如需建立計分卡的詳細資訊，請參閱 [建立計分卡](#create-a-scorecard).

如需專案權限的詳細資訊，請參閱 [在中共用專案 [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
