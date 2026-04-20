---
user-type: administrator
product-area: system-administration;setup
title: 設定自訂本地化
description: 自訂本地化可讓您定義不同語言的自訂辭彙和片語。 Workfront接著會以瀏覽器設定中所設定的語言顯示這些詞語。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 7%

---

# 設定自訂本地化

自訂本地化可讓您定義不同語言的自訂辭彙和片語。 Workfront接著會以使用者的Adobe Identity Management (IMS)設定中所設定的語言顯示這些詞語。

例如，您可以設定標籤「目標對象」以翻譯成德文單詞「Zielgruppe」。 任何以德文選取為主要瀏覽器語言的使用者，都會看到「Zielgruppe」一詞，當作任何以英文標示「目標對象」欄位的標籤。

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
1. 若要將字詞翻譯成其他語言，請將翻譯新增至適當的語言欄。
1. 若要重新排序語言欄，請按一下要移動的欄標題，然後將其拖曳到所要的位置。
