---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 中的文本解析器疑難解答 [!DNL Adobe Workfront Fusion]
description: 如果無法獲取文本解析器以生成任何輸出，請使用此資訊。
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 中的文本解析器疑難解答 [!DNL Adobe Workfront Fusion]

如果無法獲取文本解析器以生成任何輸出，請使用此資訊。

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 疑難排解

案例案例範例中，您想要剖析檔案檔案「filename.docx」的檔案類型，而檔案名稱的副檔名一律會因DOCX、PDF、CSV而異。

在此情況下，您可以選擇使用的運算式為 [!DNL \..+]

如果您要在regex101.com上使用此規則運算式，則會獲得完整符合。

![](assets/regex-expression-350x130.png)

在上圖中，檔案副檔名已正確相符。 如果您採取此動作，並嘗試在文字剖析器中實作：

![](assets/text-parser-350x602.png)

您不會得到相符項目：

![](assets/text-parser-you-dont-get-a-match-350x365.png)

原因在於「i」只顯示每次比對的符合數，因此在此例中，我們有2個符合，因為在「i」之後會有數值1和2。 其使用案例是，您若需要比對或傳遞資料，只需要第二個相符值，您就可以指定哪個值會以數值表示。

![](assets/text-parser-matches-350x355.png)

為了能夠取得將方括弧新增至要剖析之部件所需的相符值（例如，從&quot;filename.docx&quot; - &quot;docx&quot;中擷取），然後，根據我們用於此案例的regex運算式，應在\上套用方括弧。(.+)

這會擷取DOCX、將其放入群組，並保留「」。 從中解脫出來。

![](assets/text-parser-get-matches-350x592.png)

在下圖所示的輸出中，捕獲組將匹配任何字元（行終結器除外）。

![](assets/text-parser-output-350x389.png)

另一個也納入規則運算式的因應措施是使用取代函式

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

然後取代 `abcdefghijklmno pqr stuvw xyz.docx` 填入實際的檔案名稱變數。
