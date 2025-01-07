---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 比較不同環境之間的物件
description: 您可以跨環境比較物件，以確保您的環境推進套件包含您需要的物件。
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: f476b1f84fcb905537bde0c10d0a322773f6af0f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 比較不同環境之間的物件

您可以比較環境之間的物件，以確保您的環境推進套件包含您需要的物件。

您可以選取要比較的環境和物件型別。 Workfront會比較兩個環境中所選型別的所有物件，並顯示物件差異的相關資料。

## 存取需求

您必須具備下列條件：

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront]計畫</strong>
   </td>
   <td> Prime或Ultimate （僅限新計畫）
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront]個授權</strong>
   </td>
   <td> [！UICONTROL標準]
   </td>
  </tr>
   <tr>
   <td>存取層級設定
   </td>
   <td>您必須是[!DNL Workfront]管理員。
   </td>
  </tr>
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先決條件

您的組織必須位於Adobe Business Platform上，才能比較環境之間的物件。

## 產生物件比較

1. 移至您要比較物件的環境。
1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![設定圖示](/help/_includes/assets/gear-icon-setup.png)。
1. 在左側導覽中選取&#x200B;**系統**，然後選取&#x200B;**環境升級**。
1. 按一下熒幕右上角附近的&#x200B;**比較環境**。
1. 在&#x200B;**Source環境**&#x200B;欄位中，選取您想在其中建立套件的環境。 這是您從&#x200B;**複製物件**&#x200B;的環境。
1. 在&#x200B;**目標環境**&#x200B;欄位中，選取您要安裝套件的環境。 這是您正在將物件&#x200B;**複製到**&#x200B;的環境。
1. 在&#x200B;**要比較的物件**&#x200B;區域中，選取您要在環境之間比較的物件型別。
1. 按一下熒幕右上角附近的&#x200B;**產生比較**。

   視比較物件的數目和大小而定，比較可能需要一些時間才能產生。

## 檢視物件比較

比較產生完成後，比較隨即顯示。

清單包括存在於來源環境中的所選型別的物件、目標環境中是否缺少這些物件，以及兩者之間是否有欄位差異。

>[!BEGINSHADEBOX]

![比較範例](assets/environment-promotion-comparison.png)

在此範例中：

* 第一行顯示存在於目標環境中，但與來源環境不同的物件。
* 第二行顯示存在於目標環境中的物件，與來源環境中的物件相同。
* 第三行顯示目標環境中不存在的物件。

>[!ENDSHADEBOX]

## 從物件比較建立套件

您可以直接從物件比較建立封裝。

如需相關指示，請參閱「建立或編輯環境推進封裝」一文中的[從物件比較建立封裝](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-a-package-from-an-object-comparison)。
