---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 使用cURL新增HTTP模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 5eac3e87-0dd3-4bad-ae3e-77264329b717
source-git-commit: 3983d811a849c01b3c34b1cd6ee895e5552225a6
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# 使用cURL新增HTTP模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [使用cURL新增HTTP模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/use-curl-create-http.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

您可以將cURL請求貼入情境中，然後Fusion會建立根據cURL請求設定的HTTP模組。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront計畫</td>  
      <td>任何</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront授權</td>  
      <td>
        新增： Standard<br>
        或<br>
        目前：工作或以上
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion授權</td>  
      <td> 
        目前：無Workfront Fusion授權需求。<br>
        或<br>
        舊版：任何
      </td>  
    </tr>  
    <tr>  
      <td>產品</td>  
      <td> 
        新增：選取或Prime Workfront計畫：您的組織必須購買Adobe Workfront Fusion。<br>
        Ultimate Workfront計畫：包含Workfront Fusion。<br>
        或<br>
        目前：您的組織必須購買Adobe Workfront Fusion。
      </td>  
    </tr> 
  </tbody>  
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

+++

## 從cURL請求建立HTTP模組


若要使用cURL建立HTTP模組：

1. 在Fusion外部建立cURL要求的文字，例如在文字編輯器中。
1. 將cURL請求複製到剪貼簿。
1. 按一下左側面板中的&#x200B;**[!UICONTROL 案例]**&#x200B;索引標籤。
1. 選取您要建立模組的情境。
1. 按一下情境上的任何位置，以輸入情境編輯器。
1. 在案例編輯器中的任何空白處按一下滑鼠右鍵，然後選取&#x200B;**貼上**。

   或

   按下Ctrl + V (Windows)或Cmd + V (Mac)。


   HTML模組隨即建立。
1. 拖曳模組以將其連線至您的案例。

## 疑難排解

如果您的cURL未貼上情境中，請檢查瀏覽器設定，以確保已啟用從剪貼簿貼上的功能。


