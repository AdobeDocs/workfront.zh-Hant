---
content-type: reference
navigation-topic: announcements
title: Adobe Workfront中需要TLS 1.2
description: 為提供最佳安全性，Adobe Workfront要求所有依賴TLS 1.0或更舊版本的瀏覽器連線和API整合均須升級為使用TLS 1.2。在預覽環境中，TLS 1.0已停用。
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Adobe Workfront中需要TLS 1.2

為提供最佳安全性，Adobe Workfront要求所有依賴TLS 1.0或更舊版本的瀏覽器連線和API整合均須升級為使用TLS 1.2。 在預覽環境中，TLS 1.0已停用。

Workfront已於2018年3月正式停止支援TLS 1.0。 自2019年1月9日起，所有採用TLS 1.0的整合功能將停止運作。  TLS 1.1將於2019年第4季停用。

以下小節提供這些重要里程碑的詳細資訊，以及貴組織如何為此升級做好準備：

## Workfront終止官方支援TLS 1.0（2018年3月5日）

Workfront已於2018年3月終止官方支援TLS 1.0。

採用TLS 1.0的瀏覽器連線和API整合仍可運作，但Workfront無法解決Workfront應用程式中與TLS 1.0相關的問題。

## Workfront整合使用TLS 1.0已停用（2019年1月9日）

自2019年1月9日起，所有採用TLS 1.0的Workfront瀏覽器連線和API整合都必須升級至使用TLS 1.1或更新版本。 持續運用TLS 1.0（傳入或傳出連線）的瀏覽器連線和API整合，在此時間之後將無法再與Workfront應用程式通訊。 

## 將於2019年第4季停用TLS 1.1

在生產環境中，TLS 1.1已於2019年10月21日停用。 此後，所有使用TLS 1.1的整合將無法繼續運作。

這項變更將於8月7日在「預覽」和「沙箱」環境中生效，以協助組織做好關閉的準備。

## 準備TLS升級

* [透過瀏覽器存取Workfront時](#when-accessing-workfront-via-the-browser)
* [透過API連線至Workfront時](#when-connecting-to-workfront-via-the-api)

### 透過瀏覽器存取Workfront時 {#when-accessing-workfront-via-the-browser}

確定您組織中的使用者透過支援的瀏覽器存取Workfront。 (如需支援瀏覽器的相關資訊，請參閱 [Adobe Workfront瀏覽器需求](../../../workfront-basics/workfront-browser-requirements.md).)

Workfront支援的所有瀏覽器都與TLS 1.2相容。

### 透過API連線至Workfront時 {#when-connecting-to-workfront-via-the-api}

如果您要透過API將協力廠商應用程式整合至Workfront（傳入或傳出），請確定您的整合已啟用TLS 1.2（和TLS 1.2加密通訊協定）。
