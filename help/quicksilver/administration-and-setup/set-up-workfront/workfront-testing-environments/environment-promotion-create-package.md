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
recommendations: noDisplay, noCatalog
exl-id: 0ac8c7df-2d38-4291-861e-52fb5e748537
source-git-commit: d249751b78e9d40fe7a351db14cbf0f3b7c79889
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# 建立或編輯環境升級套件

您必須在要複製物件的環境中建立套件 **從**. 例如，如果您在您的「自訂重新整理沙箱」環境中設定專案並將其升級至您的生產環境，則必須在您的「自訂重新整理沙箱」環境中建立套件。

>[!IMPORTANT]
>
>如果您在設定環境升級的物件時重新整理自訂重新整理沙箱，則重新整理時將會遺失該設定。 我們建議您不要重新整理「自訂重新整理沙箱」，除非所有未完成的環境升級物件和套件都已成功升級。

## 存取需求

您必須具備下列條件：

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 計畫</strong>
   </td>
   <td> 貴組織必須採用新的定價模式，並擁有Prime或Ultimate計畫。
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 授權</strong>
   </td>
   <td> [！UICONTROL標準]
   </td>
  </tr>
   <tr>
   <td>存取層級設定
   </td>
   <td>您必須是 [!DNL Workfront] 管理員。
   </td>
  </tr>
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 建立套件

1. 前往您要在其中建立套件的環境。 這是您複製物件的環境 **從**.
1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **[!UICONTROL 設定]** ![「設定」圖示](/help/_includes/assets/gear-icon-setup.png).
1. 選取 **系統** 在左側導覽中，然後選取 **環境升級**.
1. 按一下 **建立封裝**.

   「新建促銷活動封裝」頁面隨即開啟。

1. 在 **封裝名稱** 欄位，輸入封裝的名稱。
1. 在 **說明** 欄位，輸入此封裝的說明。
1. 若要將物件加入封裝，請按一下 **新增物件** 在左側導覽中並選取您要新增的物件型別。
1. 從清單中選取一或多個物件，或在搜尋列中鍵入名稱，並在物件出現在清單中時選取物件。 您可以在清單中選取多個物件。
1. 按一下 **新增（X個物件）** 將選取的物件加入封裝。

   >[!INFO]
   >
   >**範例**
   >
   >如果您選取了三個專案以新增至專案，按鈕會顯示 **新增3個專案**.

   您新增的物件會顯示在頁面右側的「封裝內容」區域中。

1. 若要新增其他型別的物件，請重複步驟7-9。
1. （選擇性）若要從封裝中移除物件，請將游標暫留在「封裝內容」區域中的物件上，然後按一下物件旁邊的X。
1. 將所有想要的物件新增至封裝之後，請按一下 **儲存並關閉** 以儲存封裝而不進行組裝。

   或

   按一下 **儲存並組裝** 以儲存及組裝封裝。

   >[!NOTE]
   >
   >* 如果封裝的名稱中包含五個以上的字元以及至少新增了一個物件，則可使用「儲存並關閉」和「儲存並組裝」按鈕。
   >* 您無法組裝處於可安裝狀態（例如測試或作用中）的封裝。

## 編輯或組合現有套件

1. 前往您要在其中建立套件的環境。 這是您複製物件的環境 **從**.
1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **[!UICONTROL 設定]** ![「設定」圖示](/help/_includes/assets/gear-icon-setup.png).
1. 選取 **系統** 在左側導覽中，然後選取 **環境升級**.
1. 從顯示的清單中選取封裝。
1. （視條件而定）若要檢視停用的套件，請啟用 **顯示已淘汰的封裝** 選項。
1. （選擇性）若要檢視內容（包括所有物件及其子物件），請按一下 **內容** 區段。
1. （選擇性）若要檢視此套件的先前安裝與安裝嘗試，請按一下 **部署**.
1. （選擇性）若要編輯套件，請按一下 **編輯套裝** 在畫面的右上角。
1. 若要安裝套件，請按一下 **安裝** 在畫面的右上角。

   如需安裝套件的說明，請參閱 [安裝環境升級套件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md).
