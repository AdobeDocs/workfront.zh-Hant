---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Power BI工具無法使用提供的密碼連線
description: 當您嘗試從Power BI工具登入Data Connect時，您會收到登入錯誤。
author: Courtney
feature: Reports and Dashboards
exl-id: c3f2b4a9-0831-48f0-871b-486d09ae5ea4
TQID: https://experienceleague.adobe.com/Z4RrMAPGd3CCti-cQFiJ7hlf-h8-suXeuoYfzk-9aKo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 229
ht-degree: 2%

---

# Power BI工具無法使用提供的密碼連線

## 問題

當您嘗試從Power BI工具登入Data Connect時，您會看到下列錯誤：

`Cannot connect from BI tool with provided password`

## 原因

建立JDBC連線時，Workfront會提供「資料連線」的暫時密碼。

在透過Power BI存取Data Connect之前，您必須先使用提供的連線詳細資料登入、更新臨時密碼，然後繼續登入。


## 解決方案

在Workfront中重設連線密碼，然後使用「編輯連線」對話方塊中提供的連結建立新密碼。

### 在Workfront中重設連線密碼

1. 前往「Workfront >設定>系統>資料連線」。
1. 從清單中尋找並開啟連線。
1. 在&#x200B;**重設連線密碼**&#x200B;下，核取方塊以確認您要重設密碼。
1. 按一下&#x200B;**重設連線密碼**。
   ![重設連線密碼](assets/reset-password.png)
1. 繼續前往下節。

### 建立連線的新密碼

1. 複製URL，並將其貼到新的瀏覽器標籤中。
1. 在Workfront中，複製連線使用者名稱和預設密碼，並貼到新的瀏覽器索引標籤中。
   ![複製url和預設密碼](assets/link-password.png)
1. 按一下&#x200B;**登入**。
1. 輸入新密碼，然後按一下&#x200B;**提交**。
1. 前往Power BI工具，使用新密碼登入。
