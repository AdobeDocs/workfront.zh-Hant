---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選器：比較兩個欄位來排除清單中的專案」
description: 您可以比較清單中兩個欄位，藉此篩選清單中的專案。 例如，您只能顯示任務的實際完成日期晚於計畫完成日期的任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 4532e08bddf993426e9d4eed6f7f8bd638663188
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# 篩選器：比較兩個欄位來排除清單中的專案

<!--Audited: 10/2024-->

您可以比較清單中兩個欄位，藉此篩選清單中的專案。 例如，您只能顯示任務的實際完成日期晚於計畫完成日期的任務。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改篩選器的貢獻者 </p></li>
   <li><p>用於修改報告的標準</p></li> </ul>

<p>目前：</p>
   <ul><li><p>請求修改篩選器 </p></li>
   <li><p>計畫修改報表</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 比較兩個欄位以篩選專案

1. 前往工作清單。
1. 從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取&#x200B;**新增篩選器**。

1. 為&#x200B;**任務：實際完成日期** > **大於** > **選取日期**&#x200B;新增篩選器。

   >[!TIP]
   >
   >選擇您要用於所選欄位的過濾條件修正因子（若有）。

1. 按一下&#x200B;**文字模式**。
1. 在顯示的區域中，新增下列程式碼：

   `actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt`

1. 按一下&#x200B;**套用** > **另存新檔**。
