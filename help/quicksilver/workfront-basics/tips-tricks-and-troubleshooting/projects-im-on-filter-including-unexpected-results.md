---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 我參與的專案篩選器包含未預期的結果
description: 請參閱本文以疑難排解我所在的專案篩選器，包括非預期的結果。
feature: Get Started with Workfront
author: Alina
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
TQID: https://experienceleague.adobe.com/xE5RW947MUFg5d2X6ikKhHSftQDUMxDJlC05un0oDH0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 13%

---

# 我參與的專案篩選器包含未預期的結果

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table>
  <tr>
   <td>Adobe Workfront 封裝
   </td>
   <td>任何</td>
  </tr>
  <tr>
   <td>Adobe Workfront 授權
   </td>
   <td><p>標準</p>
   <p>規劃</p>
   </td>
  </tr>
   <tr>
   <td>存取層級設定
   </td>
   <td>您必須是[!DNL Workfront]管理員。
   </td>
  </tr>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 問題

我所在的&#x200B;[!UICONTROL **專案**]&#x200B;篩選器包含我預料不到的結果，因為我沒有獲得這些專案的指派或關聯。

## 解決方案

我所在的&#x200B;[!UICONTROL **專案**]&#x200B;篩選器包含在其任何&#x200B;[!UICONTROL **專案詳細資料**]&#x200B;欄位中包含使用者的專案，包括容易遺漏或自動填寫的欄位，例如&#x200B;[!UICONTROL **輸入者**]&#x200B;或&#x200B;[!UICONTROL **贊助者ID**]。 若要移除不想要的結果，有兩種可能的解決方案：

1. 檢查篩選器所包含之每個非預期專案的&#x200B;[!UICONTROL **專案詳細資料**]，並從所有欄位中移除您的名稱。

   或

1. 請嘗試使用類似的篩選器，例如&#x200B;[!UICONTROL **我擁有的專案**]，其中僅包含特別指派給您的專案。

如需在[!DNL Workfront]中使用篩選器的詳細資訊，請參閱[篩選總覽](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)。
