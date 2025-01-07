---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 建立或編輯環境升級套件
description: 環境推進功能旨在提供與組態相關的物件從一個環境移動到另一個環境的功能。 瞭解如何建立環境升級套件，以便安裝在其他環境中。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: 839b53afb9233ef0e36e981b243c8b2593b45f0f
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# 建立或編輯環境升級套件

您必須在要從&#x200B;**複製物件**&#x200B;的環境中建立封裝。 例如，如果您在您的「自訂重新整理沙箱」環境中設定專案並將其升級至您的生產環境，則必須在您的「自訂重新整理沙箱」環境中建立套件。

>[!IMPORTANT]
>
>如果您在設定環境升級的物件時重新整理自訂重新整理沙箱，則重新整理時將會遺失該設定。 我們建議您不要重新整理「自訂重新整理沙箱」，除非所有未完成的環境升級物件和套件都已成功升級。

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

## 建立套件

1. 前往您要在其中建立套件的環境。 這是您從&#x200B;**複製物件**&#x200B;的環境。
1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![設定圖示](/help/_includes/assets/gear-icon-setup.png)。
1. 在左側導覽中選取&#x200B;**系統**，然後選取&#x200B;**環境升級**。
1. 按一下&#x200B;**建立封裝**。

   「新建促銷活動封裝」頁面隨即開啟。

1. 在&#x200B;**封裝名稱**&#x200B;欄位中，輸入封裝的名稱。
1. 在&#x200B;**描述**&#x200B;欄位中，輸入此封裝的描述。
1. 若要將物件加入封裝，請在左側導覽中選取您要加入的物件型別。
1. 從出現的清單中選取一或多個物件，或在搜尋列中鍵入名稱，並在物件出現在清單中時選取物件。 您可以在清單中選取多個物件。

   此清單包括最多500個所選物件型別的物件。 若要找出不在清單上的物件，請使用搜尋列。
1. 按一下&#x200B;**新增（X物件）**，將選取的物件新增至封裝。

   >[!INFO]
   >
   >**範例**
   >
   >如果您已選取三個要新增至專案的專案，按鈕會顯示&#x200B;**新增3個專案**。

   您新增的物件會顯示在頁面右側的「封裝內容」區域中。

1. 若要新增其他型別的物件，請重複步驟7-9。
1. （選擇性）若要從封裝中移除物件，請將游標暫留在「封裝內容」區域中的物件上，然後按一下物件旁邊的X。
1. 將所有想要的物件加入封裝之後，按一下[儲存並關閉] ****&#x200B;儲存封裝而不進行組裝。

   或

   按一下&#x200B;**儲存並組裝**&#x200B;以儲存並組裝封裝。

   >[!NOTE]
   >
   >* 如果封裝的名稱中包含五個以上的字元以及至少新增了一個物件，則可使用「儲存並關閉」和「儲存並組裝」按鈕。
   >* 您無法組裝處於可安裝狀態（例如測試或作用中）的封裝。

## 編輯或組合現有套件

套件必須處於`DRAFT`狀態才能進行編輯。

1. 移至您想要在其中編輯套件的環境。 這是最初建立套件的環境。
1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![設定圖示](/help/_includes/assets/gear-icon-setup.png)。
1. 在左側導覽中選取&#x200B;**系統**，然後選取&#x200B;**環境升級**。
1. 從顯示的清單中選取封裝。
1. （視條件而定）若要檢視停用的封裝，請啟用&#x200B;**顯示已淘汰的封裝**&#x200B;選項。
1. （選擇性）若要檢視內容（包括所有物件及其子物件），請在&#x200B;**內容**&#x200B;區段中按一下物件型別旁的下拉箭頭。
1. （選擇性）若要檢視此套裝程式的先前安裝與安裝嘗試，請按一下&#x200B;**部署**。
1. （選擇性）若要編輯封裝，請按一下畫面右上角的&#x200B;**編輯封裝**。
套件必須處於`DRAFT`狀態才能進行編輯。 若要將封裝移動到`DRAFT`狀態，請在&#x200B;**狀態**&#x200B;欄位中選取`Draft`。 然後，您可以繼續編輯封裝。
1. 若要安裝套件，請按一下畫面右上角的&#x200B;**安裝**。

   如需安裝套件的說明，請參閱[安裝環境升級套件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)。

## 從物件比較建立套件

您可以直接從物件比較建立封裝。

1. 建立物件比較，如[比較環境間的物件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md)中所述。
1. 在產生的比較中，選取要包含在封裝中的物件。
1. 按一下熒幕右上角的&#x200B;**建立封裝**。
1. 輸入封裝的名稱和描述。
1. 在[建立封裝]視窗中，按一下[建立封裝]。****

   套件隨即產生。
