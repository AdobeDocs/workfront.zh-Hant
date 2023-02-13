---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: 建立產品組合
description: Portfolio是爭奪相同資源、預算和排程的專案集合。 Portfolio中的專案類似程度，足以使用相同的資源池，並以相同的計分卡進行測量。
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: cf3466759a7263c446525b97dd2748ad17d0f7a6
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# 建立產品組合

Portfolio是爭奪相同資源、預算和排程的專案集合。 Portfolio中的專案類似程度，足以使用相同的資源池，並以相同的計分卡進行測量。

您可以使用Portfolio將屬於相同產品行、部門、部門、公司或其他業務單位的項目分組。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>[!UICONTROL編輯]對Portfolio的訪問</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>建立產品組合後，依預設，您會擁有其「管理」權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 建立產品組合

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **[!UICONTROL Portfolio]**.
1. 按一下 **[!UICONTROL 新Portfolio]**.
1. 取代 **[!UICONTROL 無標題Portfolio]** 以您想要的作品集名稱。

   名稱最多可包含255個字元。

1. （選用）按一下 **[!UICONTROL Portfolio管理員]** 在頁面頂端的標題中，為產品組合指派不同的管理員。

   ![](assets/portfolio-manager-name-350x51.jpg)

   作為產品組合的建立者，預設會將您指派為產品組合管理員。

1. 按一下 **[!UICONTROL Portfolio詳細資料]** 中。
1. 在 **[!UICONTROL 概述]** 區域中，更改以下任何資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td> <p>輸入Portfolio的說明，以指出其獨特之處。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROLPortfolio管理器]</td> 
      <td> <p>開始鍵入要指明為產品組合經理的用戶名稱，然後在清單中顯示時選擇該名稱。 這與[!UICONTROLPortfolio所有者]相同。 這是可以監督產品組合項目中定義的工作並批准業務案例的人員。</p> <p>重要：當您指定某人為[!UICONTROLPortfolio管理器]時，他們會自動獲得產品組合、方案和產品組合中專案的[!UICONTROL管理]權限。 </p> <p>提示：您也可以更新頁面頂端標題中的[!UICONTROLPortfolio管理器]。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">群組 </td> 
      <td> <p>如果群組擁有組合或有責任完成組合，請新增單一群組的名稱。 </p> <p>您可以將游標移至群組上並按一下[!UICONTROL資訊]圖示，以確定您選取的是正確的群組 <img src="assets/info-icon.png"> 顯示於其旁。 此工具提示會列出群組的相關資訊，例如上方的群組階層及其管理員。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選用）按一下內部 **[!UICONTROL 新增自訂表單]** 框 [!UICONTROL Portfolio詳細資料] 頁面，為產品組合選取自訂表單並更新自訂欄位。

   >[!TIP]
   >
   >您必須先建立產品組合自訂表單，才能將其附加至產品組合。

1. 按一下 **[!UICONTROL 儲存變更]**.
1. （選用）按一下 **[!UICONTROL 方案]** 在左側面板中，然後 **[!UICONTROL 新增方案]** 將程式添加到產品組合中。

   如需建立方案的詳細資訊，請參閱 [建立方案](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

1. （選用）按一下 **[!UICONTROL 專案]** 在左側面板中，然後 **[!UICONTROL 新增專案]** 將專案新增至產品組合。

   如需新增專案至Portfolio的詳細資訊，請參閱 [將專案新增至產品組合](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).

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
