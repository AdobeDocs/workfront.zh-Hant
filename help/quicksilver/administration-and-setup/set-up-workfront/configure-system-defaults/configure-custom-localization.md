---
user-type: administrator
product-area: system-administration;setup
title: 設定自訂本地化
description: 自訂本地化可讓您定義不同語言的自訂辭彙和片語。 Workfront接著會以瀏覽器設定中所設定的語言顯示這些詞語。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: b077c95d8bb795fcd7c0983c78b7533cb8167270
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 4%
---
# 設定自訂本地化

{{highlighted-preview}}

自訂本地化可讓您<span class="preview">使用AI</span>定義不同語言的自訂辭彙和片語。 Workfront接著會以使用者的Adobe Identity Management (IMS)設定中所設定的語言顯示這些詞語。

例如，「目標對象」標籤可本地化為德文「Zielgruppe」。 任何以德文選取為主要瀏覽器語言的使用者，都會看到「Zielgruppe」一詞，當作任何以英文標示「目標對象」欄位的標籤。

您可以設定多種語言的翻譯。 目前可用的語言包括：

* 中文 (繁體)
* 中文 (簡體)
* 法文
* 德文
* 義大利文
* 日文
* 韓文
* 葡萄牙文 (巴西)
* 西班牙文

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>工作流程Prime或更高版本 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員才能設定翻譯。</p>  </td> 
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定本地化時的注意事項

設定本地化時，請考量下列事項：

* 您可以將辭彙設定為翻譯成多種語言。
* 本地化會套用至自訂欄位標籤（包括當做欄標題使用時）和工具提示。
* 自訂本地化可套用至從Business Rules產生的訊息，但必須在Business Rule中啟用。

  如需指示，請參閱建立及編輯商業規則一文中的[在商業規則中啟用本地化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules)。

## 設定翻譯

翻譯可在「設定」區域中設定。

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![設定圖示](/help/_includes/assets/gear-icon-setup.png)。
1. 在設定區域中，按一下左側導覽面板中的&#x200B;**本地化**。
1. 若要新增翻譯，請按一下&#x200B;**新增列**。
1. 在&#x200B;**英文**&#x200B;欄中，輸入應翻譯的英文辭彙。
1. 在您想要翻譯字詞的語言欄中，輸入目標語言中的字詞。
1. （選擇性）若要將字詞翻譯成其他語言，請將翻譯新增至適當的語言欄。
1. （選擇性）若要重新排序語言欄，請按一下要移動的欄標題，並將其拖曳至所需位置。
1. （選擇性）若要刪除字詞的翻譯，請按一下字詞旁的核取方塊，然後按一下頁面底部藍色列中的&#x200B;**刪除**。

<div class="preview">

## 使用AI翻譯將未翻譯的自訂文字當地語系化

您可以使用AI來本地化自訂文字。 您可以選取字詞和語言，並可在套用翻譯前核准翻譯。

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![設定圖示](/help/_includes/assets/gear-icon-setup.png)。
1. 在設定區域中，按一下左側導覽面板中的&#x200B;**本地化**。
1. 在[本地化]區域中，選取&#x200B;**未翻譯的自訂文字**&#x200B;索引標籤。

   未翻譯的自訂文字清單隨即顯示。 這包括欄位標籤和自訂規則訊息等文字。

1. 選取一或多個要本地化的詞語。
1. 在熒幕底部的藍色列中，選取&#x200B;**使用AI翻譯**。

   「產生翻譯」視窗隨即開啟。

1. 按一下您要翻譯成這些辭彙的語言。 若要快速選取所有語言，請按一下&#x200B;**全選**。
1. （選用）若要提供更明確的翻譯指引，請在「AI指示」欄位中輸入指示。
1. 按一下&#x200B;**產生**。

   AI開始產生翻譯。

   「檢閱翻譯」視窗隨即開啟。

1. （可選）若要調整翻譯或新增您自己的翻譯，請按一下表格中適當的方塊，然後輸入所要的翻譯。
1. 按一下「**儲存**」。

## 將當地語系化辭彙翻譯成其他語言

您可以使用AI將先前本地化的辭彙翻譯成新的語言，或提供您自己的翻譯。

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![設定圖示](/help/_includes/assets/gear-icon-setup.png)。
1. 在設定區域中，按一下左側導覽面板中的&#x200B;**本地化**。
1. 在本地化區域中，選取&#x200B;**翻譯**&#x200B;索引標籤。

   先前翻譯的辭彙及其翻譯的清單隨即顯示。

1. （選擇性）若要編輯或直接輸入翻譯，請按一下表格中適當的方塊，然後輸入所要的翻譯。
1. 按一下這些辭彙旁邊的核取方塊，選取您要為其產生其他翻譯的辭彙。
1. 在頁面底部的藍色列中，按一下&#x200B;**以AI填入**。


   「產生翻譯」視窗隨即開啟。

1. 按一下您要翻譯成這些辭彙的語言。 若要快速選取所有語言，請按一下&#x200B;**全選**。
1. （選用）若要提供更明確的翻譯指引，請在「AI指示」欄位中輸入指示。
1. 按一下&#x200B;**產生**。

   AI開始產生翻譯。

   「檢閱翻譯」視窗隨即開啟。

1. （可選）若要調整翻譯或新增您自己的翻譯，請按一下表格中適當的方塊，然後輸入所要的翻譯。
1. 按一下「**儲存**」。
1. （選擇性）若要刪除字詞的所有翻譯，請按一下字詞旁的核取方塊，然後按一下頁面底部藍色列中的&#x200B;**刪除**。


</div>
