---
content-type: reference
navigation-topic: announcements
title: 將自訂SMTP移除為傳出電子郵件選項
description: 在20.3版本（預計於2020年8月發行）中，Adobe Workfront正改用新的電子郵件系統，大幅提升您傳送電子郵件以取得Workfront更新和通知的可靠性。 因此，客戶將無法再使用自己的SMTP電子郵件伺服器，將其電子郵件從Workfront平台轉送給目標收件者。 所有電子郵件都會直接從Workfront Mail Server傳送。
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
source-git-commit: 9bc394c718becbac2848c2d91ba3202483699b6f
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# 將自訂SMTP移除為傳出電子郵件選項

在20.3版本（預計於2020年8月發行）中，Adobe Workfront正改用新的電子郵件系統，大幅提升您傳送電子郵件以取得Workfront更新和通知的可靠性。 因此，客戶將無法再使用自己的SMTP電子郵件伺服器，將其電子郵件從Workfront平台轉送給目標收件者。 所有電子郵件都會直接從Workfront Mail Server傳送。

您可以以系統管理員身分登入，並導覽至「設定」 > 「電子郵件」 > 「設定」 ，即可存取此功能。 以下是螢幕擷圖，醒目提示功能：

![](assets/email-server-settings-350x226.png)

此螢幕擷取畫面中強調顯示的設定會自動轉換，以搭配20.3版使用Workfront Mail Server選項。

如果已配置自定義SMTP郵件伺服器，則 **我們強烈建議您與IT團隊聯絡** 以確保不會因傳入電子郵件而封鎖來自notifications@my.workfront.com的電子郵件至您的系統。 您也可以參考設定防火牆，以取得流量和電子郵件來源IP位址的詳細資訊。

若您有任何其他問題或疑慮，請聯絡 [Workfront支援團隊](https://one.workfront.com/s/support?language=en_US).
