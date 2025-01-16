---
title: MariaDB模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# [!DNL MariaDB]模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [MariaDB模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/mariadb-modules.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL MariaDB]的工作流程，並將其連線至多個協力廠商應用程式和服務。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，貴組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

若要使用[!DNL MariaDB]模組，您必須有[!DNL MariaDB]帳戶。

## 將[!DNL MariaDB]連線至[!DNL Workfront Fusion]

您可以直接從[!DNL MariaDB]模組內建立與您的[!DNL MariaDB]帳戶的連線。

1. 在任何[!DNL MariaDB]模組中，按一下[!UICONTROL 連線]欄位旁的&#x200B;**[!UICONTROL 新增]**。
1. 設定下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL連線名稱]</p> </td> 
      <td> <p>輸入新連線的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL主機]</td> 
      <td> <p>輸入資料庫執行處理的IP位址或主機名稱。 此主機必須可從您的網路外部存取。</p> <p>範例： <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL連線埠]</td> 
      <td>預設連線埠為3306。 如果您使用非標準連線埠，請將此號碼設定為您的連線埠。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL資料庫名稱]</td> 
      <td>輸入您要與其互動的資料庫名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者名稱]</td> 
      <td>輸入您的使用者名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL密碼]</td> 
      <td>輸入您的密碼。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以建立連線並返回模組。

## [!DNL MariaDB]模組及其欄位

當您設定[!DNL MariaDB]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL MariaDB]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

### 執行查詢（進階）

此動作模組會根據您提供的查詢，從資料庫擷取資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關將您的[!DNL MariaDB]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">將[!DNL MariaDB]連線到[!DNL Workfront Fusion]</a>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Query]</td> 
   <td> <p>輸入您希望模組用來擷取資料的SQL查詢。</p> <p>重要：查詢中使用的變數不會經過淨化。 請務必正確清理變數，以防止SQL插入。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 從資料表選取資料列（進階）]

此模組會從您的資料庫讀取記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關將您的[!DNL MariaDB]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">將[!DNL MariaDB]連線到[!DNL Workfront Fusion]</a>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL表格]</td> 
   <td> <p>選取包含要讀取之記錄的表格。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td> <p>設定您要用來選取列的篩選器</p> 
    <ul> 
     <li> <p>選取您要搜尋的欄位</p> </li> 
     <li> <p>選取您要用於搜尋的運運算元</p> </li> 
     <li> <p>輸入或對應您要搜尋的值。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序] </td> 
   <td> <p>針對您想要排序結果的每個層級，按一下<strong>[！UICONTROL新增專案]</strong>，然後選取您想要排序結果的欄位，以及您想要以升序或降序排序</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>
