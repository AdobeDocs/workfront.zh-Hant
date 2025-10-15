---
title: 在Portfolio Optimizer中排定專案的優先順序
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: 您可以在Portfolio Optimizer中排定專案的優先順序，以建立專案的完成順序。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# 優先處理[!UICONTROL Portfolio Optimizer]中的專案

您可以在[!UICONTROL Portfolio Optimizer]中排定專案的優先順序，以建立專案的完成順序。

使用[!UICONTROL Portfolio Optimizer]時，請考量下列事項：

* 在[!UICONTROL Portfolio Optimizer]頂端的專案會被視為比底部列出的專案更重要。 您必須依照專案在[!UICONTROL Portfolio Optimizer]中的優先順序完成專案，Portfolio才能最佳化。
* [!UICONTROL Portfolio Optimizer]中專案的優先順序與位於專案[!UICONTROL 專案詳細資料]索引標籤上的[!UICONTROL 優先順序]欄位無關。

  [!UICONTROL 專案詳細資料]索引標籤上的[!UICONTROL 優先順序]欄位是視覺化旗標，您可以手動指定，以瞭解專案的重要性。

* 如果在Portfolio Optimizer中啟用了專案優先順序，[!DNL Resource Planner]中會顯示該優先順序。 在[!DNL Resource Planner]中，專案接收資源的順序為其[!UICONTROL 資源規劃工具]優先順序，而不是[!UICONTROL Portfolio優先順序]。

  如需有關在[!UICONTROL 資源規劃工具]中排定專案優先順序的資訊，請參閱文章[在[!UICONTROL 資源規劃工具]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)中排定專案的優先順序。

* **[!UICONTROL Portfolio最佳化工具]**&#x200B;的[!UICONTROL 專案優先順序]區域依預設會以[!UICONTROL 計劃開始日期]和[!UICONTROL 淨值]的順序顯示專案。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 封裝</td> 
   <td> <p>Workfront Prime或更高版本</p>
      <p>工作流程Prime或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>[!UICONTROL 標準]</p>
   <p>[!UICONTROL 計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>[!UICONTROL Edit]對[!UICONTROL Portfolios]和[!UICONTROL Projects]的存取權</p>  </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>投資組合的[!UICONTROL Manage]許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>Contribute or higher permissions to the projects</p> 
   <p>You must have Manage permissions to all the projects in the list to be able to use <b>Set project priority</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## 變更[!UICONTROL Portfolio Optimizer]中專案的優先順序

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)。

1. 按一下&#x200B;**[!UICONTROL 投資組合]**。
1. （選擇性）在&#x200B;**[!UICONTROL 篩選器]**&#x200B;下拉式選單中選取正確的篩選器，以檢視正確的投資組合清單。
1. 按一下投資組合的名稱以開啟。
1. 按一下左側面板中的&#x200B;**[!UICONTROL Portfolio最佳化]**。
1. 在[!UICONTROL 專案最佳化]區域中，變更專案的優先順序，方法是依優先順序拖曳專案，然後拖曳至所需的顯示位置。

   ![Portfolio optimizer與專案](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   當您完成重新排列專案時，在專案最佳化區域中按一下&#x200B;**[!UICONTROL 設定優先順序]**。 專案將會根據新訂單接收新編號。

1. 按一下&#x200B;**[!UICONTROL 儲存]**，將新專案優先順序儲存在[!UICONTROL Portfolio最佳化工具]。 優先順序會以數字&#x200B;**#**&#x200B;欄中的數字列出。

   >[!TIP]
   >
   >這並不一定會變更[!UICONTROL Portfolio Optimizer]中專案的順序，因為專案清單可能會依&#x200B;**#**&#x200B;欄以外的欄排序。 按一下&#x200B;**#**&#x200B;資料行標題，依專案優先順序排序清單。

   您可以透過在資源規劃工具中啟用[!UICONTROL 顯示Portfolio優先順序]設定，檢視專案在&#x200B;**[!UICONTROL Portfolio最佳化工具]**&#x200B;中的優先順序。

   如需有關在[!UICONTROL 資源規劃工具]中排定專案優先順序的資訊，請參閱文章[在[!UICONTROL 資源規劃工具]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)中排定專案的優先順序。
