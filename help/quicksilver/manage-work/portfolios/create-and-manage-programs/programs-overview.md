---
content-type: overview
product-area: portfolios
navigation-topic: create and manage programs
title: 計畫總覽
description: 計畫是具有統一特性的專案集合。 這些專案通常會爭奪相同的資源、預算或時段。 計畫是投資組合的子群組。 在將專案新增到投資組合之前，您可以將其與方案建立關聯。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1c64fe00-12e3-49f6-b864-b8f89ed9140d
source-git-commit: 8cd6c47acf8de313bab5fe7298125eb63cc10faf
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 1%

---

# 計畫總覽

<!-- Audited: 08/2025 -->

在Adobe Workfront中，計畫是具有統一特性的專案集合。 例如，他們可能會為相同的預算、資源或時間範圍而競爭。 計畫是投資組合的子群組。

本文包含Workfront中程式的一般資訊。


## 建立計畫所需的存取權

<!--leave the table uncollapsed as this article is about access-->

若要建立和管理產品組合，您必須具備下列存取權：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 封裝</td> 
   <td> <p>任何</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>[!UICONTROL 標準]</p>
   <p>[!UICONTROL 計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>[!UICONTROL Edit]對[!UICONTROL Portfolios]和[!UICONTROL Programs]的存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理編輯計畫或新增專案的許可權</p>
   <p>管理計畫所屬投資組合的許可權 </p>
   <p>檢視計畫的許可權以檢視它</p>
   <p>建立方案後，預設擁有其管理許可權</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>New: Any</p>
   <p>Current: [!UICONTROL Business] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard]</p>
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to edit a program or add projects to it</p>
   <p>Manage permissions to the portfolio that the program belongs to </p>
   <p>View permissions to a program to view it</p>
   <p>After you create a program, you have Manage permissions to it, by default</p> 
    </td> 
  </tr> 
 </tbody> 
</table>-->


## 有關使用方案的注意事項

* 您可以使用投資組合和計畫來組織專案。 透過組織專案，您可以比較類似的專案，並決定資源的最佳使用時機。

* 計畫是投資組合的子群組。 如果投資組合包含太多專案，您可以將它分割成多個方案，並先依方案組織專案，再依投資組合組織專案。

  例如，您可以有行銷2024產品組合，分為四個季度計畫。

* 屬於相同計畫的專案通常會爭奪相同的資源、預算或時段。

* 您必須先建立投資組合，然後才可以在同一個投資組合中建立多個計畫。

  如需有關使用程式的資訊，請參閱[建立程式](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)。

* 您必須先建立投資組合，然後是方案，然後才能將專案關聯到方案和投資組合。

* 建立專案、計畫與投資組合時，請考量下列事項：

   * 專案可以是獨立的，不必與方案或投資組合相關聯。
   * 專案可以與投資組合相關聯，但它不需要也與計畫相關聯。
   * 方案必須一律與投資組合相關聯。 它永遠不可能存在於投資組合之外。
   * 與方案相關聯的專案總是與方案的投資組合相關聯。
   * 一個計畫只能與一個投資組合相關聯。
   * 一個專案一次只能與一個方案和方案的投資組合相關聯。
   * 一個投資組合可以有多個計畫和專案。
   * 一個計畫可以有多個專案。

  如需建立專案與投資組合的相關資訊，請參閱下列文章：
   * [建立專案](/help/quicksilver/manage-work/projects/create-projects/create-project.md)
   * [建立專案組合](/help/quicksilver/manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)


* 您可以使用專案組合最佳化工具來分析專案組合內所有專案的效能。 您無法單獨比較相同方案中多個專案的效能。 您必須在投資組合層級分析專案績效。

  如需詳細資訊，請參閱[在Portfolio最佳化工具中最佳化專案](/help/quicksilver/manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md)。
