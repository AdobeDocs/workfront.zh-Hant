---
title: MariaDB模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL MariaDB]，並將其連接至多個協力廠商應用程式和服務。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# [!DNL MariaDB] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL MariaDB]，並將其連接至多個協力廠商應用程式和服務。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!DNL MariaDB] 模組，您必須 [!DNL MariaDB] 帳戶。

## Connect [!DNL MariaDB] to [!DNL Workfront Fusion]

您可以建立與 [!DNL MariaDB] 直接從內部 [!DNL MariaDB] 模組。

1. 在任何 [!DNL MariaDB] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 設定下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL連接名]</p> </td> 
      <td> <p>輸入新連接的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL主機]</td> 
      <td> <p>輸入資料庫實例的IP地址或主機名。 此主機必須可從網路外部訪問。</p> <p>範例: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL埠]</td> 
      <td>預設埠為3306。 如果使用非標準埠，請將此編號設定為埠。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL資料庫名稱]</td> 
      <td>輸入要與之交互的資料庫的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL用戶名]</td> 
      <td>輸入您的使用者名稱.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL密碼]</td> 
      <td>輸入密碼。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## [!DNL MariaDB] 模組及其欄位

設定時 [!DNL MariaDB] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL MariaDB] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 執行查詢（進階）

此動作模組會根據您提供的查詢，從您的資料庫中擷取資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL MariaDB] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connect [!DNL MariaDB] to [!DNL Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢]</td> 
   <td> <p>輸入要模組用於檢索資料的SQL查詢。</p> <p>重要：查詢中使用的變數不會經過處理。 請務必正確處理變數，以防止SQL插入。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 從表格中選取列（進階）]

此模組從資料庫讀取記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL MariaDB] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connect [!DNL MariaDB] to [!DNL Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL表]</td> 
   <td> <p>選擇包含要讀取的記錄的表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL篩選器]</td> 
   <td> <p>設定要依據其選取列的篩選器</p> 
    <ul> 
     <li> <p>選擇要搜索的欄位</p> </li> 
     <li> <p>選擇要用於搜索的運算子</p> </li> 
     <li> <p>輸入或映射要搜索的值。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序] </td> 
   <td> <p>對於要按結果排序的每個級別，按一下 <strong>[!UICONTROL添加項]</strong>，然後選取要依排序結果的欄位，以及要遞增排序還是遞減排序</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>
