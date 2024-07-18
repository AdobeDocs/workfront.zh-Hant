---
content-type: reference
navigation-topic: announcements
title: Adobe Workfront中需要TLS 1.2
description: 為了提供最佳安全性，Adobe Workfront要求所有依賴TLS 1.0或較舊版本的瀏覽器連線和API整合，升級為使用TLS 1.2。在預覽環境中，TLS 1.0已停用。
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Adobe Workfront中需要TLS 1.2

為了提供最佳安全性，Adobe Workfront要求所有依賴TLS 1.0或較舊版本的瀏覽器連線和API整合，升級為使用TLS 1.2。 在預覽環境中，TLS 1.0已停用。

Workfront已於2018年3月正式終止支援TLS 1.0。 所有運用TLS 1.0的整合功能自2019年1月9日起停止運作。  TLS 1.1將於2019年第4季停用。

以下章節提供關於這些重要里程碑的更多詳細資訊，以及您如何在組織中為此升級做好準備：

## Workfront終止對TLS 1.0的官方支援（2018年3月5日）

Workfront已於2018年3月終止對TLS 1.0的官方支援。

運用TLS 1.0的瀏覽器連線和API整合仍可運作，但Workfront將無法解決Workfront應用程式中與TLS 1.0相關的問題。

## 使用TLS 1.0的Workfront整合已停用（2019年1月9日）

在2019年1月9日，所有運用TLS 1.0的Workfront瀏覽器連線和API整合都必須升級為使用TLS 1.1或更新版本。 在此時間之後，繼續運用TLS 1.0 （傳入或傳出連線）的瀏覽器連線和API整合將無法再與Workfront應用程式通訊。 

## TLS 1.1將於2019年第4季停用

在生產環境中，TLS 1.1已於2019年10月21日停用。 在這之後，所有使用TLS 1.1的整合將無法繼續運作。

這項變更將於8月7日在預覽和沙箱環境中生效，以協助組織準備關閉。

## 準備TLS升級

* [透過瀏覽器存取Workfront時](#when-accessing-workfront-via-the-browser)
* [透過API連線Workfront時](#when-connecting-to-workfront-via-the-api)

### 透過瀏覽器存取Workfront時 {#when-accessing-workfront-via-the-browser}

確保貴組織中的使用者透過支援的瀏覽器存取Workfront。 (如需支援瀏覽器的相關資訊，請參閱[Adobe Workfront瀏覽器需求](../../../workfront-basics/workfront-browser-requirements.md)。)

Workfront支援的所有瀏覽器都與TLS 1.2相容。

### 透過API連線Workfront時 {#when-connecting-to-workfront-via-the-api}

如果您透過API （傳入或傳出）將協力廠商應用程式整合至Workfront，請確保在整合中啟用TLS 1.2 （和TLS 1.2加密通訊協定）。
