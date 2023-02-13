---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用OneDrive的工作流，並將其連接到多個第三方應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3934'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL OneDrive]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!DNL OneDrive] 模組，您必須 [!DNL Microsoft OneDrive] 帳戶。

## 連接 [!DNL OneDrive] 服務 [!DNL Workfront Fusion]

有關連接 [!DNL OneDrive] 帳戶 [!UICONTROL Workfront融合]，請參閱 [建立連線至 [!UICONTROL Adobe Workfront融合]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive] 模組及其欄位

設定時 [!DNL OneDrive] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL OneDrive] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [檔案/資料夾](#filefolder)
* [其他](#other)

### 檔案/資料夾

* [[!UICONTROL 監視檔案/資料夾]](#watch-filesfolders)
* [[!UICONTROL 搜索檔案/資料夾]](#search-filesfolders)
* [[!UICONTROL 取得檔案]](#get-a-file)
* [[!UICONTROL 下載檔案]](#download-a-file)
* [[!UICONTROL 上傳檔案]](#upload-a-file)
* [[!UICONTROL 建立資料夾]](#create-a-folder)
* [[!UICONTROL 取得共用連結]](#get-a-share-link)
* [[!UICONTROL 移動檔案/資料夾]](#move-a-filefolder)
* [[!UICONTROL 複製檔案]](#copy-a-file)
* [[!UICONTROL 刪除檔案/資料夾]](#delete-a-filefolder)

#### [!UICONTROL 監視檔案/資料夾]

此觸發器模組會在建立或更新檔案或資料夾時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL OneDrive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL監視檔案/資料夾]</td> 
   <td> <p>選擇要如何監視檔案或資料夾：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL按建立時間]</b> </p> <p>監視新檔案或資料夾。</p> </li> 
     <li> <p><b>[!UICONTROL按更新時間]</b> </p> <p>請留意更新的現有檔案或資料夾。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選擇要監視的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>輸入要模組監視的驅動器ID。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> <p>導覽至您要模組監看的資料夾。 您也可以輸入查詢以篩選傳回的結果。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL與我共用]</b> </p> <p>模組會監視已與驅動器所有者共用的檔案。</p> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取您要模組監看的SharePoint網站。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇要模組監視其驅動器的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇項目類型]</td> 
   <td> <p>選擇要監視檔案、資料夾還是兩者。</p> <p>注意：您無法監視[!UICONTROL與我共用]驅動器中的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>



#### [!UICONTROL 搜索檔案/資料夾]

此搜索模組根據您設定的條件返回檔案和資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL OneDrive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選擇要搜索的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>輸入要模組搜索的驅動器ID。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> <p>導覽至您要模組搜尋的資料夾。 您也可以輸入查詢以篩選傳回的結果。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL與我共用]</b> </p> <p>模組搜索已與驅動器所有者共用的檔案。</p> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取 [!DNL SharePoint] 您希望模組搜尋的網站。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇要模組搜索其驅動器的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇項目類型]</td> 
   <td> <p>選擇要搜索檔案、資料夾還是兩者。</p> <p>注意：您無法在[!UICONTROL與我共用]驅動器中搜索資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

此動作模組會取得指定檔案的中繼資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL OneDrive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（檔案ID和檔案路徑）]</td> 
   <td>選擇要按檔案ID還是按檔案路徑標識檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入檔案ID] / [!UICONTROL檔案路徑]</td> 
   <td> <p>選擇要如何輸入檔案ID或檔案路徑：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手動輸入]</b> </p> <p>如果要直接輸入ID或路徑，或從上一個模組映射，請選擇此選項。</p> </li> 
     <li> <p><b>[!UICONTROL從清單中選擇]</b> </p> <p>如果要從可用檔案或路徑清單中選擇此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選擇要搜索的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>輸入包含要獲取的檔案的驅動器的ID。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取包含您要取得之檔案的SharePoint網站。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇驅動器包含要獲取的檔案的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇或映射包含要獲取的檔案的驅動器。 如果您在[!UICONTROL啟用以輸入驅動器ID]欄位中選擇[!UICONTROL否]，則此欄位不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案] / [!UICONTROL檔案ID] / [!UICONTROL檔案路徑]</td> 
   <td> <p>如果您選擇了[!UICONTROL手動輸入]，請輸入或映射要獲取的檔案的檔案ID或路徑。</p> <p>如果選擇了[!UICONTROL從清單中選擇]，請選擇要獲取的檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載檔案]

此動作模組會下載指定的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL OneDrive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（檔案ID和檔案路徑）]</td> 
   <td>選擇要按檔案ID還是按檔案路徑標識檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">輸入檔案ID /檔案路徑</td> 
   <td> <p>選擇要如何輸入檔案ID或檔案路徑：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手動輸入]</b> </p> <p>如果要直接輸入ID或路徑，或從上一個模組映射，請選擇此選項。</p> </li> 
     <li> <p><b>[!UICONTROL從清單中選擇]</b> </p> <p>如果要從可用檔案或路徑清單中選擇此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取要包含您要下載之檔案的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>輸入包含要下載的檔案的驅動器ID。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取包含您要下載之檔案的SharePoint網站。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇其驅動器包含要下載的檔案的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇或映射包含要下載的檔案的驅動器。 如果您在[!UICONTROL啟用以輸入驅動器ID]欄位中選擇[!UICONTROL否]，則此欄位不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案] / [!UICONTROL檔案ID] / [!UICONTROL檔案路徑]</td>
   <td> <p>如果您選擇[!UICONTROL手動輸入]，請輸入或映射要下載的檔案的檔案ID或路徑。</p> <p>如果選擇了[!UICONTROL從清單中選擇]，請選擇要下載的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL轉換為PDF]</td> 
   <td> <p>啟用此選項可將檔案轉換為PDF檔案。 可以從下列檔案類型中轉換：</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>檔案</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>鍋</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>POTX</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XLSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳檔案]

此動作模組會將檔案上傳至指定的資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL OneDrive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">輸入（資料夾位置ID和路徑）</td> 
   <td>選擇要按ID還是按路徑標識目標資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選取要上傳檔案的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>選擇包含要獲取的檔案的驅動器。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取 [!DNL SharePoint] 包含要上載檔案的資料夾的站點。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇驅動器包含要上載檔案的資料夾的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇包含要上載檔案的資料夾的驅動器。 如果您在[!UICONTROL啟用以輸入驅動器ID]欄位中選擇[!UICONTROL否]，則此欄位不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL如果存在同名檔案]</td> 
   <td>如果同名檔案已存在，請選擇如何繼續。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL描述]</td> 
   <td>將說明新增至上傳的檔案。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立資料夾]

此操作模組在指定的驅動器中建立新資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL OneDrive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選擇要建立資料夾的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>選擇要建立資料夾的驅動器。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取 [!DNL SharePoint] 要建立資料夾的網站。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇擁有要建立資料夾的驅動器的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇要建立資料夾的驅動器。 如果您在[!UICONTROL啟用以輸入驅動器ID]欄位中選擇[!UICONTROL否]，則此欄位不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td>如果希望新資料夾是子資料夾，請導航至希望其成為子資料夾的資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL新資料夾名稱]</td> 
   <td> <p>輸入或映射新資料夾的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL如果存在同名資料夾]</td> 
   <td>如果同名檔案已存在，請選擇如何繼續。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得共用連結]

此動作模組會傳回指定檔案的共用連結。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL OneDrive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（檔案ID和檔案路徑）]</td> 
   <td>選擇要按檔案ID還是按檔案路徑標識檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入檔案ID] / [!UICONTROL檔案路徑]</td> 
   <td> <p>選擇要如何輸入檔案ID或檔案路徑：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手動輸入]</b> </p> <p>如果要直接輸入ID或路徑，或從上一個模組映射，請選擇此選項。</p> </li> 
     <li> <p><b>[!UICONTROL從清單中選擇]</b> </p> <p>如果要從可用檔案或路徑清單中選擇此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選擇要檢索共用連結的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>輸入包含要檢索共用連結的檔案的驅動器的ID。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取包含您要擷取分享連結之檔案的SharePoint網站。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇其驅動器包含要檢索共用連結的檔案的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇或映射包含要檢索共用連結的檔案的驅動器。 如果您在[!UICONTROL啟用以輸入驅動器ID]欄位中選擇[!UICONTROL否]，則此欄位不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案] / [!UICONTROL檔案ID] / [!UICONTROL檔案路徑]</td> 
   <td> <p>如果選擇[!UICONTROL手動輸入]，請輸入或映射要檢索共用連結的檔案的檔案ID或路徑。</p> <p>如果從清單中選擇了[!UICONTROL選擇]，請選擇要檢索共用連結的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL權限類型]</td> 
   <td> <p>選擇是希望具有連結的人員能夠讀取和寫入檔案，還是只讀。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL範圍]</td> 
   <td>選取您要讓任何具有連結的人，或僅供具有連結之組織的成員使用檔案。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動檔案/資料夾]

此操作模組將檔案或資料夾移動到新資料夾位置

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL OneDrive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（檔案ID和檔案路徑）]</td> 
   <td>選擇要按檔案ID還是按檔案路徑標識檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入檔案ID /檔案路徑]</td> 
   <td> <p>選擇要如何輸入檔案ID或檔案路徑：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手動輸入]</b> </p> <p>如果要直接輸入ID或路徑，或從上一個模組映射，請選擇此選項。</p> </li> 
     <li> <p><b>[!UICONTROL從清單中選擇]</b> </p> <p>如果要從可用檔案或路徑清單中選擇此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選擇包含要移動的檔案或資料夾的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>輸入包含要移動的檔案或資料夾的驅動器ID。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取 [!DNL SharePoint] 包含要移動的檔案或資料夾的站點。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇要移動的檔案或資料夾的驅動器所在的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇或映射包含要移動的檔案或資料夾的驅動器。 如果您在[!UICONTROL啟用以輸入驅動器ID]欄位中選擇[!UICONTROL否]，則此欄位不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">選擇[!UICONTROL檔案/資料夾]</td> 
   <td>選擇要移動檔案還是資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL檔案] / [!UICONTROL檔案ID] / [!UICONTROL檔案路徑]</p> <p role="rowheader">[!UICONTROL資料夾] / [!UICONTROL資料夾ID] / [!UICONTROL資料夾路徑]</p> </td> 
   <td> <p>如果您選擇了[!UICONTROL手動輸入]，請輸入或映射要移動的檔案或資料夾的ID或路徑。</p> <p>如果從清單中選擇了[!UICONTROL選擇]，請選擇要移動的檔案或資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入新資料夾位置]</td> 
   <td> <p>選擇要如何輸入要將檔案或資料夾移動到的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手動輸入]</b> </p> <p>如果要直接輸入ID或路徑，或從上一個模組映射，請選擇此選項。</p> </li> 
     <li> <p><b>[!UICONTROL從清單中選擇]</b> </p> <p>如果要從可用檔案或路徑清單中選擇此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選擇要移動檔案或資料夾的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>輸入要移動檔案或資料夾的驅動器ID。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取 [!DNL SharePoint] 要移動檔案或資料夾的站點。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇要將檔案或資料夾移動到其驅動器的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇或映射包含要移動檔案或資料夾的資料夾的驅動器。 如果您在[!UICONTROL啟用以輸入驅動器ID]欄位中選擇[!UICONTROL否]，則此欄位不可用。</p> <p>如果將此欄位留空，則只能將檔案或資料夾移至相同的 [!DNL OneDrive].</p> <p>您可以將檔案和資料夾從[!UICONTROL我的驅動器]移動到[!UICONTROL站點的驅動器]或[!UICONTROL組的驅動器]。 </p> <p>您只能將檔案從[!UICONTROL站點的驅動器]移動到同一站點中的同一驅動器。</p> <p>您只能將檔案從[!UICONTROL組的驅動器]移動到同一組中的同一驅動器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td>輸入或映射要移動檔案或資料夾的資料夾。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製檔案]

此操作模組將檔案複製到新資料夾位置

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL OneDrive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（檔案ID和檔案路徑）]</td> 
   <td>選擇要按檔案ID還是按檔案路徑標識檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入檔案ID] / [!UICONTROL檔案路徑]</td> 
   <td> <p>選擇要如何輸入檔案ID或檔案路徑：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手動輸入]</b> </p> <p>如果要直接輸入ID或路徑，或從上一個模組映射，請選擇此選項。</p> </li> 
     <li> <p><b>[!UICONTROL從清單中選擇]</b> </p> <p>如果要從可用檔案或路徑清單中選擇此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選擇包含要複製的檔案的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>輸入包含要複製的檔案或資料夾的驅動器ID。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取包含您要移動之檔案的SharePoint網站。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇其驅動器包含要複製的檔案的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇或映射包含要複製的檔案的驅動器。 如果您在[!UICONTROL啟用以輸入驅動器ID]欄位中選擇[!UICONTROL否]，則此欄位不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL檔案] / [!UICONTROL檔案ID] / [!UICONTROL檔案路徑]</p> </td> 
   <td> <p>如果您選擇[!UICONTROL手動輸入]，請輸入或映射要複製的檔案的ID或路徑。</p> <p>如果從清單中選擇了[!UICONTROL選擇]，請選擇要複製的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入新資料夾位置]</td> 
   <td> <p>選擇要如何輸入要複製檔案或要複製到的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手動輸入]</b> </p> <p>如果要直接輸入ID或路徑，或從上一個模組映射，請選擇此選項。</p> </li> 
     <li> <p><b>[!UICONTROL從清單中選擇]</b> </p> <p>如果要從可用資料夾清單中選取，請選取此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL新OneDrive位置]</td> 
   <td> <p>選擇要複製檔案伺服器的位置。 如果您選擇從清單中選取新資料夾位置，則此選項可用。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>輸入要複製檔案的驅動器ID。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取 [!DNL SharePoint] 您要複製檔案的網站。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇要將檔案複製到其驅動器的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇或映射包含要將檔案複製到的資料夾的驅動器。 如果您在[!UICONTROL啟用以輸入驅動器ID]欄位中選擇[!UICONTROL否]，則此欄位不可用。</p> <p>如果將此保留為空，則只能在同一[!UICONTROL OneDrive]中複製檔案或資料夾。</p> <p>您可以將檔案和資料夾從[!UICONTROL我的驅動器]複製到[!UICONTROL站點的驅動器]或[!UICONTROL組的驅動器]。 </p> <p>您只能將檔案從[!UICONTROL站點的驅動器]複製到同一站點中的同一驅動器。</p> <p>您只能將檔案從[!UICONTROL組的驅動器]複製到同一組中的同一驅動器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td>輸入或映射要移動副本或資料夾的資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL新複製的檔案名]</td> 
   <td> <p>輸入或映射檔案新副本的名稱。 如果您不想變更原始檔案名稱，可將此項目保留空白。</p> <p>名稱必須包含副檔名。 範例:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案/資料夾]

此動作模組會刪除選取的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL OneDrive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter（檔案/資料夾ID和路徑）]</td> 
   <td>選擇要按檔案ID還是按檔案路徑標識檔案。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入檔案/資料夾ID /輸入檔案/資料夾路徑]</td> 
   <td> <p>選擇要如何輸入檔案ID或檔案路徑：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL手動輸入]</b> </p> <p>如果要直接輸入ID或路徑，或從上一個模組映射，請選擇此選項。</p> </li> 
     <li> <p><b>[!UICONTROL從清單中選擇]</b> </p> <p>如果要從可用檔案或路徑清單中選擇此選項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選擇您的 [!DNL OneDrive] 位置]</td> 
   <td> <p>選擇要搜索的位置：</p> 
    <ul> 
     <li> <p><b>[!UICONTROL我的驅動器]</b> </p> <p>選擇是否啟用模組以輸入驅動器ID。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL是]</b> </p> <p>輸入包含要刪除的檔案或資料夾的驅動器ID。</p> </li> 
       <li> <p><b>[!UICONTROL否]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL站點的驅動器]</b> </p> <p>選取 [!DNL SharePoint] 包含要刪除的檔案或資料夾的站點。 可用站點是Sites，隨後是登錄用戶。</p> </li> 
     <li> <p><b>[!UICONTROL組的驅動器]</b> </p> <p>選擇其驅動器包含要刪除的檔案或資料夾的組。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇或映射包含要刪除的檔案或資料夾的驅動器。 如果您在[!UICONTROL啟用以輸入驅動器ID]欄位中選擇[!UICONTROL否]，則此欄位不可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">選擇[!UICONTROL檔案/資料夾]</td> 
   <td>選擇要刪除檔案還是資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案] / [!UICONTROL檔案ID] / [!UICONTROL檔案路徑]</td>
   <td> <p>如果您選擇了[!UICONTROL手動輸入]，請輸入或映射要刪除的檔案的檔案ID或路徑。</p> <p>如果從清單中選擇了[!UICONTROL選擇]，請選擇要刪除的檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### [!UICONTROL 進行API呼叫]

此模組會執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關連接 [!DNL OneDrive] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>輸入相對於的路徑 <code>https://graph.microsoft.com</code>. 範例:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



## 如果您無法上傳或更新檔案

上傳或更新檔案失敗時，可能會發生幾個問題：

* 上傳的檔案太大，超過了 [!DNL OneDrive] 計畫，或者你用了 [!DNL OneDrive] 帳戶的儲存配額。 若要獲得更多儲存空間，請從 [!DNL OneDrive] 或升級您的 [!DNL OneDrive] 帳戶。
* OneDrive不允許將兩個同名檔案上載到一個資料夾。 如果目標資料夾包含的檔案名稱與要上傳的檔案相同，則方案執行會終止，並產生錯誤。 解決方案是直接重新命名要上傳的檔案。 如果您的目標是更新檔案，請使用 [!UICONTROL 更新檔案] 動作。
* 先前選取的資料夾（正要上傳檔案）已不存在。 情境停止，您將需要再次選取目標資料夾。
