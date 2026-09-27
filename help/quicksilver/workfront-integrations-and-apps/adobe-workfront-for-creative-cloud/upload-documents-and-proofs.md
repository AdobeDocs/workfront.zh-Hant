---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: 將檔案和校訂從[!DNL Adobe Workfront plugin]上傳到[!DNL Creative Cloud]
description: 將檔案和校訂從[!DNL Adobe Workfront plugin]上傳到[!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
TQID: 'https://experienceleague.adobe.com/bZsOnrrwZ7ksCaoM3jfIyeTO00XqG1hDTEmG5VmWOcA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%
---
# 將檔案和校訂從[!DNL Adobe Workfront plugin]上傳到[!DNL Creative Cloud]

您可以上傳專案作為檔案，以進行快速檢閱和核准，或僅儲存於[!DNL Adobe Workfront]。

>[!NOTE]
>
>Premiere Pro和After Effects目前不支援上傳檔案和校樣。


## 檔案限制

本節概述[!DNL Workfront for Adobe Creative Cloud plugins]中的已知檔案限制。

### 新檔案版本僅接受上傳一個檔案

由於[!DNL Workfront]檔案不能包含多個檔案，因此必須停用某些設定，才能將新檔案版本上傳到Workfront。

>[!NOTE]
>
>如果您必須產生多個檔案，您可以改為建立校訂。 新的校樣將不會與原始檔案相關聯。



若要在[!DNL InDesign]中將切換變更為單一檔案：

1. 開啟&#x200B;**設定匯出檔案設定**&#x200B;對話方塊。

   ![檔案匯出設定](assets/file-export-settings.png)

1. 找到您要匯出的資產型別，並依下列說明調整設定：

   <table>
    <tr>
    <td><strong>PDF和PDF-PRINT</strong>
    </td>
    <td>取消選取<strong>建立個別的PDF檔案</strong>。
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>選取<strong>範圍</strong>並輸入單一頁碼。 
    <p>
    <strong>附註</strong>：若要上傳完整檔案，您必須建立校訂。 
    </td>
    </tr>
    <tr>
    <td><strong>EPUB和EPUB — 已修正</strong>
    </td>
    <td>不需要調整。
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>不需要調整。
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td>選取<strong>範圍</strong>並輸入單一頁碼。 
    <p>
    <strong>附註</strong>：若要上傳完整檔案，您必須建立校訂。 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>選取<strong>範圍</strong>並輸入單一頁碼。 
    <p>
    <strong>附註</strong>：若要上傳完整檔案，您必須建立校訂。 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>不需要調整。 
    </td>
    </tr>
    </table>
