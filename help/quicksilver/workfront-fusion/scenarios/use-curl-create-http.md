---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 使用cURL新增HTTP模組
description: 您可以將cURL請求貼入情境中，然後Fusion會建立根據cURL請求設定的HTTP模組。
author: Becky
feature: Workfront Fusion
source-git-commit: 4cc881f4f5a28bd105e6898ad7ffb57c1dafb563
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# 使用cURL新增HTTP模組

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

   >[!IMPORTANT]
   >
   >如果您在Windows電腦上使用Fusion，您的cURL請求不得包含分行符號。
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

如果您的cURL未貼入情境中，請檢查下列專案：

* 檢查您的瀏覽器設定，以確保已啟用從剪貼簿貼上。
* 如果您正在執行Windows，請檢查cURL要求，確保其中不包含分行符號。



