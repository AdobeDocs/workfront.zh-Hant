---
content-type: overview
product-area: portfolios
navigation-topic: portfolios-overview
title: 瞭解Portfolio方法
description: Portfolio是具有統一特性的專案集合。 這些專案通常會爭奪相同的資源、預算或時段。 您可以將投資組合分割成計畫，並在將專案新增到Portfolio之前建立專案與計畫的關聯。
author: Alina
feature: Work Management, Strategic Planning
exl-id: b340501e-1190-415e-aa96-5aad177c4b7b
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# 瞭解產品組合方法

<!-- Audited: 1/2024 -->

Portfolio或專案Portfolio管理(PPM)是排定專案清單優先順序及加以管理的程式，以達成特定的業務目標。

如需PPM的一般資訊，請參閱[Portfolio管理概觀](/help/quicksilver/manage-work/portfolios/portfolios-overview/portfolio-managament-overview.md)。

在Adobe Workfront中，專案組合是具有統一特性的專案集合。 這些專案通常會爭奪相同的資源、預算或時段。 您可以將投資組合分割成計畫，並在將專案新增到Portfolio之前建立專案與計畫的關聯。

您可以使用「專案組合與計畫」來組織專案。 透過組織專案，您可以比較類似的專案，並決定資源的最佳使用時機。

如需有關使用程式的資訊，請參閱[建立程式](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)。

本文包含有關Workfront投資組合的一般資訊。

## 建立投資組合所需的存取權

<!--leave the table uncollapsed as this article is about access-->

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 套件</td> 
   <td> <p>Workfront Prime或更高版本</p>
   <p>工作流程Prime或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>[！UICONTROL標準]</p>
   <p>[！UICONTROL計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>[！UICONTROL Edit]對投資組合的存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>建立專案組合後，您預設擁有專案組合的管理許可權</p> 
   <p>管理編輯投資組合或新增專案的許可權</p>
   <p>檢視投資組合的許可權，以在Workfront中檢視它</p>
    </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>New: Any</p>
   <p>Current:[!UICONTROL Business] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard]</p>
   <p>Current:[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>After you create a portfolio, you have Manage permissions to it, by default</p> 
   <p>Manage permissions to edit a portfolio or add projects to it</p>
   <p>View permissions to a portfolio to view it in Workfront</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## 瞭解[!DNL Adobe Workfront]投資組合方法

在[!DNL Workfront]中，您可以將專案新增至投資組合以建立及組織您的投資組合。

建議您遵循下列步驟，有效率地組織您的產品組合：

1. 為專案建立業務案例，並將專案與Portfolio建立關聯。

   若要建立可為貴組織帶來價值的有效產品組合，您必須從專案請求開始，在此為您定義稍後新增至產品組合的每個專案的業務案例。

   [!UICONTROL 業務案例]包含下列資訊：

   * 專案的一般資訊(說明、Portfolio和方案指派、專案所有者和贊助者)
   * 專案目的或目的
   * 預估費用成本
   * 勞力成本的資源預算
   * 一致性分數
   * 風險評估

   如需[!UICONTROL 商業案例]的詳細資訊，請參閱[為專案建立商業案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

   在建立其業務案例時，您可以將專案與投資組合建立關聯。 您必須先建立投資組合，才能將其與專案建立關聯。 如需詳細資訊，請參閱[建立投資組合](/help/quicksilver/manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)

   您在建立業務案例期間收集的詳細資料會用於[!UICONTROL 投資組合最佳化工具]和[!UICONTROL 資源規劃工具]，以協助管理選取專案。
1. 建立專案的業務案例時，建立資源集區與專案的關聯。

   產品組合通常設定為與資源集區對應。 Portfolio中的程式也與資源集區一致。 此相互關聯有助於確保所有資源規劃符合Portfolio的用途，因為同一Portfolio中的專案通常會爭奪相同的資源。

   如需詳細資訊，請參閱[建立資源集區](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)。

1. 取得您的Portfolio管理員核准的[!UICONTROL 業務案例]。

   如需詳細資訊，請參閱[核准業務案例](/help/quicksilver/manage-work/projects/define-a-business-case/approve-business-case.md)。
1. 在[!UICONTROL Portfolio Optimizer]中管理投資組合中專案的效能。

   Portfolio經理可以使用Portfolio儀表板追蹤投資組合內的財務績效。 此儀表板會顯示在Portfolio的標題中。

   如需Portfolio的財務欄位相關資訊，請參閱[Portfolio Optimizer概觀](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md#financial-fieds-subsection)中的[瞭解Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)區段。
