---
product-area: documents
navigation-topic: proofing-overview
title: 在網路校訂檢視器擴充功能中檢閱互動式內容
description: Adobe Workfront檢閱工具是瀏覽器擴充功能，可讓您校訂ZIP檔案或具有URL的互動式內容。
author: Courtney
feature: Digital Content and Documents
source-git-commit: 5650ebfbf115908cbf2b89ffeab0551a4ecacc2d
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---


# 使用Adobe Workfront稽核工具稽核互動式內容

<span class="preview">Adobe Workfront檢閱工具將於2024年11月7日推出。 此擴充功能目前是測試版。</span>

Adobe Workfront檢閱工具是網頁型瀏覽器擴充功能，可讓您校訂ZIP檔案或具有URL的互動式內容。 Adobe Workfront檢閱工具提供下列瀏覽器：

* Firefox
* Chrome
* Edge

對於無法在iFrame中開啟網站的網站（例如Figma），建議使用「案頭校訂檢視器」。


## 將Adobe Workfront檢閱工具設為URL和ZIP校樣的預設檢視器

若要使用網頁檢閱工具進行URL和ZIP校訂，Workfront管理員必須調整互動式校訂的預設設定。

1. 在Workfront的主要功能表中，按一下&#x200B;**校樣**。
1. 按一下「**帳戶設定**」，然後按一下「**設定**」標籤。
1. 在&#x200B;**校訂預設值**&#x200B;區段中，找到&#x200B;**互動式校訂的案頭校訂檢視器**，然後按一下&#x200B;**設定**。
1. 在下拉式功能表中，選擇&#x200B;**已停用**。 從URL或ZIP檔案建立的互動式校訂現在會自動在Adobe Workfront檢閱工具（網頁瀏覽器）中開啟。
1. 按一下「**儲存**」。

>[!NOTE]
>
>此變更適用於預覽和生產環境中的所有互動式校樣。 我們建議先在預覽環境中測試新體驗，然後再在生產環境中啟用。 您可以將所有互動式校訂的帳戶設定變更回&#x200B;**已啟用**，以輕鬆切換回案頭檢視器。

## 將Adobe Workfront檢閱工具設為僅適用於ZIP校樣的預設檢視器

若只要將Web檢閱工具用於ZIP校訂，Workfront管理員必須調整互動校訂的預設設定。

1. 在Workfront的主要功能表中，按一下&#x200B;**校樣**。
1. 按一下「**帳戶設定**」，然後按一下「**設定**」標籤。
1. 在&#x200B;**校訂預設值**&#x200B;區段中，找到&#x200B;**互動式校訂的案頭校訂檢視器**，然後按一下&#x200B;**設定**。
1. 在下拉式功能表中，選擇&#x200B;**僅針對從URL**&#x200B;建立的互動式校訂啟用。 從ZIP檔案建立的互動式校樣現在會自動在Adobe Workfront檢閱工具（網頁瀏覽器）中開啟。 從URL建立的互動式校訂仍然會在案頭校訂檢視器中開啟。
1. 按一下「**儲存**」。

>[!NOTE]
>
>此變更適用於預覽和生產環境中的所有互動式校樣。 我們建議先在預覽環境中測試新體驗，然後再在生產環境中啟用。 您可以將所有互動式校訂的帳戶設定變更回&#x200B;**已啟用**，以輕鬆切換回案頭檢視器。

## 安裝擴充功能

稽核者和核准者必須安裝Adobe Workfront稽核工具。 在下列其中一個瀏覽器中：

* [Firefox擴充功能](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome擴充功能](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

安裝擴充功能後，互動式校樣會自動在Adobe Workfront檢閱工具中開啟。

>[!IMPORTANT]
>
>您必須移除舊版Web Viewer擴充功能，才能使用Adobe Workfront檢閱工具。



