---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 我參與的專案篩選器包含未預期的結果
description: 請參閱本文以疑難排解我所在的專案篩選器，包括非預期的結果。
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 1%

---

# 我參與的專案篩選器包含未預期的結果

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>[！UICONTROL計畫] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>[！UICONTROL系統管理員]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

此 [!UICONTROL **我參與的專案**] 篩選器包含我預料不到的結果，因為我沒有獲得這些專案的指派或關聯。

## 解決方案

此 [!UICONTROL **我參與的專案**] 篩選器包含在其任何一項中包含使用者的專案 [!UICONTROL **專案詳細資訊**] 欄位，包括容易遺漏或自動填寫的欄位，例如 [!UICONTROL **輸入者**] 或 [!UICONTROL **贊助者ID**]. 若要移除不想要的結果，有兩種可能的解決方案：

1. 檢查 [!UICONTROL **專案詳細資訊**] 針對篩選條件中包含的每個非預期專案，從所有欄位中移除您的名稱。

   或

1. 請嘗試使用類似的篩選器，例如 [!UICONTROL **我擁有的專案**]，僅包括特別指派給您的專案。

如需在中使用篩選器的詳細資訊 [!DNL Workfront]，請參閱 [篩選器概觀](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
