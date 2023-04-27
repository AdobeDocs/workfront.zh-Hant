---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 正在篩選包含意外結果的項目
description: 閱讀本文，疑難排解「我正在使用」篩選器中包含未預期結果的問題。
feature: Get Started with Workfront
author: Nolan
source-git-commit: ba261e5121b4a28f71c58f883c784f4e8d2ada81
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 1%

---

# 「我所在的項目」篩選器包含意外的結果

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 授權</strong></td> 
   <td> <p>[!UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置</strong></td> 
   <td> <p>[!UICONTROL系統管理員]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

此 [!UICONTROL **正在執行的項目**] 篩選器包含我不會預期的結果，因為我沒有被指派或與這些專案關聯。

## 解決方案

此 [!UICONTROL **正在執行的項目**] 篩選器包含的專案包含任何 [!UICONTROL **專案詳細資料**] 欄位，包括容易遺漏或自動填入的欄位，例如 [!UICONTROL **輸入者**] 或 [!UICONTROL **發起人ID**]. 若要移除不想要的結果，有兩種可能的解決方案：

1. 檢查 [!UICONTROL **專案詳細資料**] 為篩選器包含的每個非預期專案，並從所有欄位中移除您的名稱。

   或

1. 嘗試使用類似的篩選器，例如 [!UICONTROL **我擁有的專案**]，僅包含專門指派給您的專案。

如需在 [!DNL Workfront]，請參閱 [篩選器概觀(於 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)