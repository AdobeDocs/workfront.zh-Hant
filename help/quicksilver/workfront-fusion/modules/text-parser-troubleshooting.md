---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion]中的文字剖析器疑難排解'
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的文字剖析器疑難排解

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [文字剖析器](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/text-parser.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

如果您無法取得文字剖析器以產生任何輸出，請使用此資訊。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 疑難排解

案例的範例，您想要剖析檔案檔案「filename.docx」的檔案型別，且檔案名稱的副檔名在DOCX、PDF和CSV之間一律不同。

您可以在此情況下選擇使用的運算式是[!DNL \..+]

如果您要在regex101.com上的regex運算式上使用此運算式，則會取得完全相符專案。

![](assets/regex-expression-350x130.png)

在上圖中，副檔名正確相符。 如果您接受這個要求，並嘗試在文字剖析器中實作：

![](assets/text-parser-350x602.png)

您將不會得到相符項：

![](assets/text-parser-you-dont-get-a-match-350x365.png)

原因在於「i」僅顯示每個相符項的相符數，因此在此例中，我們有2個相符項，因此「i」後面有一個數值1和2。 此情況下的使用案例是，如果您只需要比對或傳遞資料至篩選器，就可以指定由數值表示的值（第二個相符值）。

![](assets/text-parser-matches-350x355.png)

為了能夠取得您在要剖析的零件中新增方括弧所需的相符值（例如，從「filename.docx」 — 「docx」中擷取），然後根據我們用於此案例的規則運算式情境，方括弧應套用在\上。(.+)

這會擷取DOCX、將其置於群組中，並保留「」。 盡情享受吧。

![](assets/text-parser-get-matches-350x592.png)

在下圖所示的輸出中，擷取群組將符合任何字元（行終止元除外）。

![](assets/text-parser-output-350x389.png)

另一個同時納入regex的因應措施是使用取代函式

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

然後將`abcdefghijklmno pqr stuvw xyz.docx`取代為您的實際檔案名稱變數。
