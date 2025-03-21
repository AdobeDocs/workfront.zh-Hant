---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Power BI工具無法使用提供的密碼連線
description: 當您嘗試從Power BI工具登入Data Connect時，您會收到登入錯誤。
author: Courtney
feature: Reports and Dashboards
source-git-commit: 40050915153af6e1f70024461e193fb536d74e35
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

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

