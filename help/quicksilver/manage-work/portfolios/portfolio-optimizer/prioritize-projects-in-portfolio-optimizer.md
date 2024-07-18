---
title: 在Portfolio最佳化工具中排定專案的優先順序
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: 您可以在Portfolio最佳化工具中排定專案的優先順序，以建立專案的完成順序。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# 優先處理[!UICONTROL Portfolio最佳化工具]中的專案

您可以在[!UICONTROL Portfolio最佳化工具]中排定專案的優先順序，以建立專案應完成的順序。

使用[!UICONTROL Portfolio最佳化工具]時，請考量下列事項：

* 在[!UICONTROL Portfolio最佳化工具]頂端的專案會被視為比底部列出的專案更重要。 您必須依照專案在[!UICONTROL Portfolio最佳化工具]中的優先順序完成專案，Portfolio才能最佳化。
* [!UICONTROL Portfolio最佳化工具]中專案的優先順序與位於專案[!UICONTROL 專案詳細資料]索引標籤上的[!UICONTROL 優先順序]欄位無關。

  [!UICONTROL 專案詳細資料]索引標籤上的[!UICONTROL 優先順序]欄位是視覺化旗標，您可以手動指定，以瞭解專案的重要性。

* 在Portfolio最佳化工具中的專案優先順序會顯示在[!DNL Resource Planner]中（如果在其中啟用）。 在[!DNL Resource Planner]中，專案接收資源的順序是其[!UICONTROL 資源規劃工具]優先順序，而不是[!UICONTROL Portfolio優先順序]。

  如需有關在[!UICONTROL 資源規劃工具]中排定專案優先順序的資訊，請參閱文章[在[!UICONTROL 資源規劃工具]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)中排定專案的優先順序。

* 根據預設，[!UICONTROL Portfolio最佳化工具]的&#x200B;**[!UICONTROL 專案優先順序]**&#x200B;區域會以[!UICONTROL 計劃開始日期]和[!UICONTROL 淨值]的順序顯示專案。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>[！UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>[！UICONTROL Edit]專案和Portfolio的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>投資組合的[！UICONTROL Manage]許可權</p> <p>Contribute或更高的專案許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 變更[!UICONTROL Portfolio最佳化工具]中專案的優先順序

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**[!UICONTROL Portfolio]**。
1. （選擇性）在&#x200B;**[!UICONTROL 篩選器]**&#x200B;下拉式選單中選取正確的篩選器，以檢視正確的投資組合清單。
1. 按一下投資組合的名稱以開啟。
1. 按一下左側面板中的&#x200B;**[!UICONTROL Portfolio最佳化]**。
1. 在[!UICONTROL 專案最佳化]區域中，變更專案的優先順序，方法是依優先順序拖曳專案，然後拖曳至所需的顯示位置。

   ![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   當您完成重新排列專案時，在專案最佳化區域中按一下&#x200B;**[!UICONTROL 設定優先順序]**。 專案將會根據新訂單接收新編號。

1. 按一下&#x200B;**[!UICONTROL 儲存]**，將新專案優先順序儲存在[!UICONTROL Portfolio最佳化工具]。 優先順序會以數字&#x200B;**#**&#x200B;欄中的數字列出。

   >[!TIP]
   >
   >這不一定會變更[!UICONTROL Portfolio最佳化工具]中專案的順序，因為專案清單可能會依&#x200B;**#**&#x200B;欄以外的欄排序。 按一下&#x200B;**#**&#x200B;資料行標題，依專案優先順序排序清單。

   您可以透過在資源規劃工具中啟用&#x200B;**[!UICONTROL 顯示Portfolio優先順序]**&#x200B;設定，檢視專案在[!UICONTROL Portfolio最佳化工具]中的優先順序。

   如需有關在[!UICONTROL 資源規劃工具]中排定專案優先順序的資訊，請參閱文章[在[!UICONTROL 資源規劃工具]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)中排定專案的優先順序。
