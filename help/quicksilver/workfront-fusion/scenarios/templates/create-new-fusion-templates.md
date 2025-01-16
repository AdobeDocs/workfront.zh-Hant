---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在 [!DNL Adobe Workfront Fusion]中建立新範本
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中建立新範本

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [建立新範本](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-and-manage-templates/create-new-fusion-templates.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

您可以在[!DNL Adobe] Workfront Fusion中建立新的情境範本。

>[!TIP]
>
>建立新範本之前，您可以檢查[!UICONTROL 公用範本]標籤，確認您要建立的範本尚未可用。

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
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
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

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 建立新範本

您可以使用與建立情境類似的程式來建立範本。 Fusion管理員也可以從現有的案例建立範本。

* [建立範本](#build-a-template)
* [從情境建立範本](#create-a-template-from-a-scenario)

### 建立範本

1. 按一下左側導覽面板中的&#x200B;**[!UICONTROL 範本]** ![](assets/fusion-template-icon.png)。
1. 按一下右上角的&#x200B;**[!UICONTROL 建立新範本]**。
1. （選擇性）取代左上角的預設&#x200B;**[!UICONTROL 新範本名稱]**&#x200B;以重新命名範本。
1. （選擇性）若要變更範本的語言，請按一下&#x200B;**[!UICONTROL 設定範本]** ![](assets/fusion-scenario-settings-icon.png)，然後從[語言]下拉式清單中選取語言。

   >[!IMPORTANT]
   >
   >「語言」選項對應於系統設定中可用的語言，並且只與公用範本的名稱及其說明有關。 一旦範本已儲存，您就無法變更範本語言。

1. （選擇性）若要輸入範本的說明，請按一下&#x200B;**[!UICONTROL 設定範本]** ![](assets/fusion-scenario-settings-icon.png)並輸入說明。
1. 以建立標準情境時的相同方式新增應用程式、模組和工具。

   若要新增內容說明至模組，請參閱本文中的[設定[!UICONTROL 精靈]功能](#set-up-wizard-functionality)。

   如需建立案例的詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。

   >[!NOTE]
   >
   >如果您的範本包含需要新增連線、憑證或其他隱私權敏感資訊的模組，則此資訊不會與範本使用者共用。

1. （選擇性）按一下&#x200B;**[!UICONTROL 執行一次]**&#x200B;以測試您的範本。
1. 按一下&#x200B;**[!UICONTROL 儲存]**&#x200B;圖示![](assets/save-icon.png)。

>[!NOTE]
>
>儲存您的範本後，您便可讓所有專案團隊成員看到該範本。 如果您希望範本可在團隊外部存取，您必須提交請求以核准並發佈。 請求會進入Adobe Workfront進行核准，並在獲得核准後，團隊以外的其他人即可存取範本。
>
>如需發佈範本的相關資訊，請參閱[Publish和共用 [!DNL Adobe Workfront Fusion] 範本](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md)。

### 從情境建立範本

>[!NOTE]
>
>您必須是Fusion管理員才能從案例建立範本。

1. 針對您要建立案例的案例，開啟案例詳細資訊頁面。
1. 按一下頁面右上角附近的&#x200B;**管理員**&#x200B;下拉式清單。
1. 選取&#x200B;**復製為範本**。

   情境會複製到新範本頁面中。
1. （選擇性）取代左上角的預設&#x200B;**[!UICONTROL 新範本名稱]**&#x200B;以重新命名範本。
1. （選擇性）若要變更範本的語言，請按一下&#x200B;**[!UICONTROL 設定範本]** ![](assets/fusion-scenario-settings-icon.png)，然後從[語言]下拉式清單中選取語言。

   >[!IMPORTANT]
   >
   >「語言」選項對應於系統設定中可用的語言，並且只與公用範本的名稱及其說明有關。 一旦範本已儲存，您就無法變更範本語言。

1. （選擇性）若要輸入範本的說明，請按一下&#x200B;**[!UICONTROL 設定範本]** ![](assets/fusion-scenario-settings-icon.png)並輸入說明。
1. 使用與編輯標準案例相同的方式來編輯應用程式、模組和工具。

   若要新增內容說明至模組，請參閱本文中的[設定[!UICONTROL 精靈]功能](#set-up-wizard-functionality)。

   >[!NOTE]
   >
   >如果您的範本包含需要新增連線、憑證或其他隱私權敏感資訊的模組，則此資訊不會與範本使用者共用。

1. （選擇性）按一下&#x200B;**[!UICONTROL 執行一次]**&#x200B;以測試您的範本。
1. 按一下&#x200B;**[!UICONTROL 儲存]**&#x200B;圖示![](assets/save-icon.png)。

## 設定[!UICONTROL 精靈]功能 {#set-up-wizard-functionality}

[!DNL Workfront Fusion template] [!UICONTROL 精靈]可讓您為範本的未來使用者提供模組中所使用特定欄位的相關指示或資訊。

1. 按一下新增至範本的模組，以檢視模組的欄位。
1. 找到您要新增[!UICONTROL 精靈]資訊的欄位，並為該欄位啟用&#x200B;**[!UICONTROL 在精靈中使用]**。
1. 在[!UICONTROL 說明]欄位中輸入您想要讓使用者看到的資訊。
1. （選擇性）若要讓使用者在使用範本時看到此文字，請啟用&#x200B;**[!UICONTROL 使用作為預設值]**。
1. 針對您想要提供資訊的每個欄位，重複步驟2至4。
1. 按一下&#x200B;**[!UICONTROL 確定]**&#x200B;以儲存變更並關閉模組。
