---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: 從 [!DNL Adobe Workfront plugin] 到 [!DNL Creative Cloud]
description: 從 [!DNL Adobe Workfront plugin] 到 [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
source-git-commit: 67952bf88a782595e13e559bfbc14ce1c622d432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# 從 [!DNL Adobe Workfront plugin] 到 [!DNL Creative Cloud]

您可以將專案上傳為檔案，以供快速審核和核准，或僅儲存於 [!DNL Adobe Workfront].

>[!NOTE]
>
>Premiere Pro和After Effects目前不支援上傳檔案和校樣。


## 檔案限制

本節概述 [!DNL Workfront for Adobe Creative Cloud plugins].

### 新文檔版本僅接受一個檔案以便上載

因為 [!DNL Workfront] 檔案不能包含多個檔案，必須停用某些設定，才能將新檔案版本上傳至Workfront。

>[!NOTE]
>
>如果您必須產生多個檔案，則可改為建立校樣。 新校樣將不會與原始文檔關聯。



要將切換器更改回 [!DNL InDesign]:

1. 開啟 **設定導出檔案設定** 對話框。

   ![](assets/file-export-settings.png)

1. 找到您要匯出的資產類型，並依照下列說明調整設定：

   <table>
    <tr>
    <td><strong>PDF和PDF打印</strong>
    </td>
    <td>取消選擇 <strong>建立個別的PDF檔案</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>選擇 <strong>範圍</strong> 並輸入單頁號碼。 
    <p>
    <strong>附註</strong>:如果要上傳完整檔案，必須建立校樣。 
    </td>
    </tr>
    <tr>
    <td><strong>ePub和EPUB — 固定</strong>
    </td>
    <td>無需調整。
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>無需調整。
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td>選擇 <strong>範圍</strong> 並輸入單頁號碼。 
    <p>
    <strong>附註</strong>:如果要上傳完整檔案，必須建立校樣。 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>選擇 <strong>範圍</strong> 並輸入單頁號碼。 
    <p>
    <strong>附註</strong>:如果要上傳完整檔案，必須建立校樣。 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>無需調整。 
    </td>
    </tr>
    </table>
