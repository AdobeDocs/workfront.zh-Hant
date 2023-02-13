---
content-type: reference
navigation-topic: announcements
title: 叢集1、2和3的客戶必須更新任何允許清單IP區塊，以防止封鎖Adobe Workfront服務
description: 為了增強並改善我們的核心基礎架構，我們很快將叢集01、02和03上的Adobe Workfront客戶移轉至AWS公用雲。
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 4%

---

# 叢集1、2和3的客戶必須更新任何允許清單IP區塊，以防止封鎖Adobe Workfront服務

為了增強並改善我們的核心基礎架構，我們很快將叢集01、02和03上的Adobe Workfront客戶移轉至AWS公用雲。

在此變更中，您需要將下列IP新增至允許清單IP區塊，以防止封鎖Workfront服務：

對於SSO和POP:

* 34.215.145.168
* 54.69.155.48
* 35.160.44.226
* 34.213.96.218
* 3.16.210.22
* 3.16.229.153
* 18.224.117.99
* 3.18.123.153
* 3.211.159.196
* 3.85.255.45
* 3.210.78.197
* 3.211.23.183

對於電子郵件：

* 54.240.60.174
* 54.240.60.175

請務必在2019年5月13日前更新允許清單IP區塊。 如需詳細資訊，請參閱 [配置防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

感謝您持續支援Workfront，協助我們為客戶創造更可靠且健全的體驗。

如果您有任何其他問題，請造訪experience.workfront.com或致電844.306.4357（美國）或+44.1256.274200（歐洲、中東和非洲），與我們的支援團隊聯繫。

## 常見問題集

### Workfront為何做出這些改變？

為了持續為客戶提供最佳的服務，Workfront會不斷尋找改善使用者體驗的方法。 這一變化利用了新技術，使我們能夠提供盡可能好的體驗，並改進我們本已強健的安全模型。

### 身為Workfront管理員，我需要執行哪些動作？

請連絡您的內部IT或安全部門，以協助您檢閱允許清單IP區塊，以及新增上述IP。

### 如果我們不進行此變更，我的組織會期望什麼？

我們將服務移轉至新IP時，您將無法存取Workfront服務。
