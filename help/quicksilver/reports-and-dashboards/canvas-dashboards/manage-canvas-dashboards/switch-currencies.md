---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在畫布儀表板中使用貨幣欄位
description: 您可以在畫布控制面板中使用貨幣欄位。
author: Courtney
feature: Reports and Dashboards
source-git-commit: 3e4ab2dfc66efd262c0c2ad30a9c62758084f8ce
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 4%

---


# 在畫布儀表板中使用貨幣欄位

>[!IMPORTANT]
>
>畫布儀表板功能目前僅適用於參與Beta階段的使用者。 在此階段中，部分功能可能無法完成或如預期般運作。 請依照「畫布控制面板」測試版概觀文章中[提供意見回饋](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)一節的指示，提交有關您體驗的任何意見回饋。<br>
>如果您對可能的錯誤或技術問題有回饋，請向Workfront支援提交票證。 如需詳細資訊，請參閱[聯絡客戶支援](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>請注意，以下雲端服務供應商未提供此測試版：
>
>* 自備Amazon Web Services金鑰
>* Azure
>* Google Cloud Platform

## 存取需求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<p>任何 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td> 
<p>標準</p> 
<p>規劃</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td><p>編輯報告、儀表板和行事曆的存取權</p>
   <p>檢視財務資料的存取權</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td><p>管理儀表板的許可權</p>
  </td> 
  </tr> 
</tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先決條件

1. 您必須在Workfront例項中設定多種貨幣型別，才能使用本文所述的功能。 如需詳細資訊，請參閱[設定匯率](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

   >[!IMPORTANT]
   >
   >本文所述的功能僅適用於原生貨幣欄位。 即將支援自訂貨幣欄位。


## 設定畫布控制面板的預設貨幣

建立畫布控制面板時，您可以設定控制面板的預設貨幣。 除非已在報表層級鎖定貨幣欄位，否則此貨幣將用於顯示控制面板上報表中的所有原生貨幣欄位。

1. 在左側面板中，按一下&#x200B;**畫布控制面板**。

1. 按一下右上角的&#x200B;**新儀表板**。

1. 在&#x200B;**建立儀表板**&#x200B;方塊中，

1. 指定下列專案：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名稱</strong></td>
      <td><p>輸入儀表板的名稱。 我們建議僅使用UTF-8字元以避免相容性問題。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>說明 (選擇性)</strong></td>
      <td>輸入控制面板的說明。</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>貨幣</strong></td>
      <td>選擇儀表板的預設貨幣型別。 <br>
      <br>使用者可在篩選儀表板時切換不同的貨幣型別。</td>
     </tr>
    </tbody>
   </table>


## 在畫布儀表板上的貨幣之間切換

您可以在控制面板層級切換不同的貨幣型別。 包含貨幣欄位的報表將更新以反映所選的貨幣型別。

貨幣欄位可在報表層級鎖定。 如果貨幣欄位已鎖定，當您變更儀表板的貨幣型別時，該報表的貨幣型別將不會變更。

若要變更儀表板的貨幣型別，

1. 按一下控制面板詳細資訊頁面右上角的貨幣下拉式功能表。
1. 從清單中選取所需的貨幣型別。

   ![變更貨幣下拉式清單](assets/filter-by-currency.png)


## 限制

下表概述在「設定」的「匯率」區域中定義貨幣時的限制。

<table> 
<tr>
<td></td>
<td>使用者可以</td>
<td>使用者無法</td>
</tr>
<tr> 
<td>已定義單一貨幣</td>
<td>
<ul>
<li>在畫布圖表、KPI和表格報表中使用原生貨幣欄位</li>
<li>在畫布圖表、KPI和圖表報表中使用自訂貨幣欄位</li>
</ul>
</td>
<td>
<ul>
<li>指派預設貨幣給控制面板（建立或編輯控制面板時）</li>
<li>檢視並使用控制面板層級的貨幣切換</li>
<li>鎖定特定貨幣，以在畫布圖表、KPI或表格報告中檢視</li>
<li>在畫布圖表、重要績效指標及表格報表中使用「計畫」幣別欄位</li>
</ul>
</td> 
</tr>
</td> 
</tr> 
<tr>
<td>已定義多種貨幣</td>
<td>
<ul>
  <li>在畫布圖表、KPI和表格報表中使用原生貨幣欄位</li>
  <li>設定儀表板的預設貨幣（在建立或編輯儀表板時）</li>
  <li>檢視並使用控制面板層級的貨幣切換</li>
  <li>鎖定畫布圖表、KPI或表格報表中檢視的特定貨幣，以忽略控制面板貨幣切換偏好設定</li>
</ul>
</td>
<td><ul>
  <li>在畫布圖表、KPI和表格報表中使用自訂資料貨幣欄位</li>
  <li>在畫布圖表、重要績效指標及表格報表中使用「計畫」幣別欄位</li>
</ul>
</td>
</tr></table>





