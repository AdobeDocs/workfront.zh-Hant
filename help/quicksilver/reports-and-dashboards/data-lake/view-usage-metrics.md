---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 檢視Workfront Data Connect使用度量
description: 使用Workfront Data Connect Metrics索引標籤，您可以根據每月使用的計算小時數和執行的查詢數來檢視組織的使用量度。
author: Nolan
feature: Reports and Dashboards
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 1%

---

# 檢視[!DNL Workfront Data Connect]使用量度

使用[!DNL Workfront Data Connect] [!UICONTROL 量度]標籤，您可以根據使用的計算時數與執行的查詢數目，檢視組織的使用量度。 組織根據其授權型別和Data Connect附加元件購買提供的每月運算時數有限。 [!UICONTROL 量度]索引標籤會顯示與已使用專案相關的可用每月運算時數資訊。

## 存取需求

+++ 展開以檢視存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td><p>包含在下列計畫中：</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <p>可作為下列計畫的附加元件購買：</p> 
    <ul>
        <li>選取</li> 
        <li>Prime</li>
    </ul> 
    <p>Workfront Data Connect不適用於舊版Workfront計畫。</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 檢視使用量度和可用的運算時數

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;[!UICONTROL **設定**]。

1. 在左側面板中，按一下&#x200B;[!UICONTROL **系統**] > [!UICONTROL **資料存取**]。

1. 按一下「[!UICONTROL **量度**]」標籤。 您的使用量度會顯示在&#x200B;**計算使用量**&#x200B;圖表中，而執行的查詢數會顯示在&#x200B;**查詢計數**&#x200B;圖表中。

   ![資料連線使用量度](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. （選擇性）您可以使用&#x200B;[!UICONTROL **選取檢視**]&#x200B;下拉式功能表，變更兩個圖形所含資訊的時間範圍。

1. （選擇性）您可以使用&#x200B;**計算使用量**&#x200B;圖表上方的核取方塊來顯示或隱藏：
   * [!UICONTROL **每日運算時數**] — 您的組織每日使用的運算時數。
   * [!UICONTROL **每月累計計算時數**] — 貴組織在一個月內使用的計算時數總數。 每月重設為零。
   * [!UICONTROL **每月計算小時津貼**] — 貴組織根據授權和/或附加購買提供的計算小時數。
