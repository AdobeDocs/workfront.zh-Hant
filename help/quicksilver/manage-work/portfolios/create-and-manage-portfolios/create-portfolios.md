---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: 建立專案組合
description: Portfolio是競爭相同資源、預算和排程的專案集合。 Portfolio中的專案相當類似，因此會使用相同的資源集區，並針對相同的計分卡測量。
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 1%

---

# 建立專案組合

<!--Audited: 7/2024-->

Portfolio是競爭相同資源、預算和排程的專案集合。 Portfolio中的專案相當類似，因此會使用相同的資源集區，並針對相同的計分卡測量。

您可以使用投資組合將屬於相同產品線、部門、部門、公司或其他業務單位的專案分組。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>新增：[！UICONTROL Standard]</p>
   <p>目前：[！UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>[！UICONTROL Edit]對投資組合的存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>建立專案組合後，您預設擁有專案組合的管理許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立產品組合的方式

您可以使用下列其中一種方法，在Workfront中建立產品組合：

* 從主功能表的「投資組合」區域開始從頭開始建立投資組合。 本文會介紹如何從頭開始建立產品組合。

* 使用kick-start匯入投資組合。

  作為Workfront管理員，您可以使用kick-start匯入產品組合。

  如需有關在Workfront中使用Kick-Start匯入資料的資訊，請參閱[使用Kick-Start範本將資料匯入Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。

* 當您從Workfront Planning中的記錄型別連結投資組合時新增投資組合。

  您必須擁有新的Workfront授權和適用於Workfront的額外Workfront規劃授權。

  如需有關存取Workfront Planning的資訊，請參閱[存取總覽](/help/quicksilver/planning/access/access-overview.md)。

  如需透過將專案組合新增至記錄來建立專案組合的資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)一文中的「連線時建立記錄」一節。


## 建立專案組合

{{step1-click-main-menu}}

1. 按一下&#x200B;**[!UICONTROL 投資組合]**。
1. 按一下&#x200B;**[!UICONTROL 新增Portfolio]**。
1. 將&#x200B;**[!UICONTROL 未命名的Portfolio]**&#x200B;取代為您想要用於投資組合的名稱。

   名稱最多可包含255個字元。

1. （選擇性）按一下頁面頂端標題中&#x200B;**[!UICONTROL Portfolio Manager]**&#x200B;底下的名稱，指派投資組合的其他經理。

   ![Portfolio管理員名稱](assets/portfolio-manager-name-350x51.jpg)

   投資組合的建立者預設會指派您為投資組合經理。

1. 按一下左側面板中的&#x200B;**[!UICONTROL Portfolio詳細資料]**。
1. 在&#x200B;**[!UICONTROL 概觀]**&#x200B;區域中，變更下列任何資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL說明]</td> 
      <td> <p>輸入Portfolio的說明以指出其獨特性。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL Portfolio Manager]</td> 
      <td> <p>開始輸入您要指定做為投資組合經理的使用者名稱，然後當它出現在清單中時選取它。 這與[！UICONTROL Portfolio Owner]相同。 此人員可監督投資組合中專案所定義的工作，並可核准業務案例。</p> <p>重要：當您指定某人為[！UICONTROL Portfolio Manager]時，他們會自動取得專案組合、方案及專案組合中的[！UICONTROL管理]許可權。 </p> <p>提示：您也可以更新頁面頂端標題中的[！UICONTROL Portfolio Manager]。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">群組 </td> 
      <td> <p>如果群組擁有投資組合或負責完成投資組合，請新增單一群組的名稱。 </p> <p>您可以暫留在群組上，並按一下旁邊顯示的[！UICONTROL資訊]圖示<img src="assets/info-icon.png">，確定您選取的群組正確。 這會顯示工具提示，列出群組的相關資訊，例如群組及其管理員上方的群組階層。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）在[!UICONTROL Portfolio詳細資料]頁面右上角的&#x200B;**[!UICONTROL 新增自訂表單]**&#x200B;方塊內按一下，以選取產品組合的自訂表單並更新自訂欄位。

   >[!TIP]
   >
   >您必須先建立投資組合自訂表單，才能將其附加至投資組合。

1. 按一下「**[!UICONTROL 儲存變更]**」。
1. （選擇性）按一下左側面板中的&#x200B;**[!UICONTROL 程式]**，然後按一下&#x200B;**[!UICONTROL 新增程式]**，將程式新增至投資組合。

   如需建立程式的詳細資訊，請參閱[建立程式](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)。

1. （選擇性）按一下左側面板中的「**[!UICONTROL 專案]**」，然後按一下「**[!UICONTROL 新增專案]**」以將專案新增至投資組合。

   如需將專案新增至Portfolio的詳細資訊，請參閱[將專案新增至投資組合](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Deactivate a portfolio</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this and moved it to their own article: delete-deactivate-portfolios)</p>
<p>When you deactivate a portfolio, you can still access it from the Portfolios area, but it no longer displays in the list of portfolios when users try to add it to a project.</p>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2">Click <strong>Portfolios</strong> .</li>
<li value="3"> <p>Click the name of the portfolio.</p> </li>
<li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon.png"> to the right of the portfolio name, then click <strong>Deactivate Portfolio</strong>.</li>
</ol>
<h2>Delete a portfolio</h2>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> <p>Click <strong>Portfolios</strong> .</p> </li>
<li value="3"> <p>Select the portfolio, then click the Delete icon <img src="assets/delete.png">.</p> </li>
<li value="4"> <p>In the box that appears, click <strong>Yes, Delete It</strong> to confirm.</p> </li>
</ol>
</div>
-->
