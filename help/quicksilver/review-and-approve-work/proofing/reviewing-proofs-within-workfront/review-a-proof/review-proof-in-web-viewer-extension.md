---
product-area: documents
navigation-topic: proofing-overview
title: 在網路校訂檢視器擴充功能中檢閱互動式內容
description: Adobe Workfront檢閱工具是瀏覽器擴充功能，可讓您校訂ZIP檔案或具有URL的互動式內容。
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 5a8bfdeae7f5d23ecf835e652cf0ff5efd5aa410
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 1%

---

# 使用Adobe Workfront稽核工具稽核互動式內容

<span class="preview">Adobe Workfront檢閱工具已於2024年11月7日推出。 此擴充功能目前是測試版。</span>

Adobe Workfront檢閱工具是網頁型瀏覽器擴充功能，可讓您校訂ZIP檔案或具有URL的互動式內容。 Adobe Workfront檢閱工具提供下列瀏覽器：

* Firefox
* Chrome
* Edge
* Safari

>[!IMPORTANT]
>
>檢閱GenStudio for Performance Marketing和Creative Cloud Express中的內容需要此擴充功能。 Assets會自動在網頁檢視器中開啟。 您不需要更新任何帳戶設定。


## 安裝擴充功能

### 先決條件

* 您必須移除舊版Web Viewer擴充功能，才能使用Adobe Workfront檢閱工具。

### 安裝擴充功能

稽核者和核准者必須安裝Adobe Workfront稽核工具。 在下列其中一個瀏覽器中：

* [Firefox擴充功能](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Chrome擴充功能](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)


為了讓互動式校訂在Adobe Workfront檢閱工具中自動開啟，Workfront管理員必須更新workfront中的校訂設定，如下節所述。

## 更新Workfront校訂預設值

若要使用Workfront檢閱工具做為互動式內容的預設檢視器，您必須更新Workfront中的校訂預設值。

>[!NOTE]
>
>如果您需要檢閱的內容位於以下網站，我們建議您使用案頭校訂檢視器
>
>* 需要SSO驗證
>* 防止在iFrame中開啟其網站，例如Figma

### 將Adobe Workfront檢閱工具設為URL和ZIP校樣的預設檢視器

若要使用網頁檢閱工具進行URL和ZIP校訂，Workfront管理員必須調整互動式校訂的預設設定。

1. 在Workfront的主要功能表中，按一下&#x200B;**校樣**。
1. 按一下「**帳戶設定**」，然後按一下「**設定**」標籤。
1. 在&#x200B;**校訂預設值**&#x200B;區段中，找到&#x200B;**互動式校訂的案頭校訂檢視器**，然後按一下&#x200B;**設定**。
1. 在下拉式功能表中，選擇&#x200B;**已停用**。 從URL或ZIP檔案建立的互動式校訂現在會自動在Adobe Workfront檢閱工具（網頁瀏覽器）中開啟。
1. 按一下「**儲存**」。

>[!NOTE]
>
>此變更會套用至Workfront執行個體中的所有互動式校樣。 我們建議先在預覽環境中測試新體驗，然後再在生產環境中啟用。 您可以將&#x200B;**互動式校訂的案頭校訂檢視器**&#x200B;帳戶設定變更回&#x200B;**為所有互動式校訂啟用**，以輕鬆切換回案頭檢視器。

### 將Adobe Workfront檢閱工具設為僅適用於ZIP校樣的預設檢視器

若只要將Web檢閱工具用於ZIP校訂，Workfront管理員必須調整互動校訂的預設設定。

1. 在Workfront的主要功能表中，按一下&#x200B;**校樣**。
1. 按一下「**帳戶設定**」，然後按一下「**設定**」標籤。
1. 在&#x200B;**校訂預設值**&#x200B;區段中，找到&#x200B;**互動式校訂的案頭校訂檢視器**，然後按一下&#x200B;**設定**。
1. 在下拉式功能表中，選擇&#x200B;**僅針對從URL**&#x200B;建立的互動式校訂啟用。 從ZIP檔案建立的互動式校樣現在會自動在Adobe Workfront檢閱工具（網頁瀏覽器）中開啟。 從URL建立的互動式校訂仍然會在案頭校訂檢視器中開啟。
1. 按一下「**儲存**」。

>[!NOTE]
>
>此變更會套用至Workfront執行個體中的所有ZIP校樣。 我們建議先在預覽環境中測試新體驗，然後再在生產環境中啟用。 您可以將&#x200B;**互動式校訂的案頭校訂檢視器**&#x200B;帳戶設定變更回&#x200B;**為所有互動式校訂啟用**，以輕鬆切換回案頭檢視器。

