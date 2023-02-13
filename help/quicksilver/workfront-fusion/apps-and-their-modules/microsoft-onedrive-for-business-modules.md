---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive for Business模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Microsoft OneDrive for Business]，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Microsoft OneDrive for Business]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!DNL Microsoft OneDrive for Business] with [!DNL Adobe Workfront Fusion]，您需要 [!DNL Microsoft] 帳戶。

有關連接 [!DNL OneDrive for Business] 帳戶 [!DNL Workfront Fusion]，請參閱 [建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive for Business] 模組及其欄位

設定時 [!DNL Microsoft OneDrive for Business] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Microsoft OneDrive for Business] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)

### 觸發器

* [[!UICONTROL 監看檔案]](#watch-files)
* [[!UICONTROL 監看資料夾]](#watch-folders)

#### [!UICONTROL 監看檔案]

在觀看的資料夾中新增或更新新檔案時，此觸發器模組會啟用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL驅動器ID]</p> </td> 
   <td> <p>選擇要監視的驅動器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td> <p> 選擇要監視的資料夾。 在案例中，您只能監視一個資料夾。</p> <p>提示：若要追蹤多個資料夾，請為每個資料夾建立獨立的案例。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL我想看]</p> </td> 
   <td> <p>選擇您要監視新檔案和所有更改，還是僅監視新檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回行數上限]</td> 
   <td> <p> 設定 [!DNL Workfront Fusion] 可在一個週期中運作。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監看資料夾]

將新資料夾新增至正在觀看的資料夾時，此觸發器模組會啟用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL驅動器ID]</p> </td> 
   <td> <p>選擇要監視的驅動器。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td> <p> 選擇要監視的資料夾。 在案例中，您只能監視一個資料夾。</p> <p>提示：若要追蹤多個資料夾，請為每個資料夾建立獨立的案例。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL我想看]</p> </td> 
   <td> <p>選擇您是要查看新資料夾和所有更改，還是僅查看新資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回行數上限]</td> 
   <td> <p> 設定 [!DNL Workfront Fusion] 可在一個週期中運作。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 上傳檔案]](#upload-a-file)
* [[!UICONTROL 刪除檔案]](#delete-a-file)
* [[!UICONTROL 取得檔案]](#get-a-file)
* [[!UICONTROL 建立資料夾]](#create-a-folder)
* [[!UICONTROL 刪除資料夾]](#delete-a-folder)
* [[!UICONTROL 取得分享連結]](#get-a-sharing-link)

#### [!UICONTROL 上傳檔案]

此操作模組將二進位檔案或文本檔案上載到指定的資料夾

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇要將檔案上載到的驅動器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選擇驅動器內的資料夾。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL源檔案]</p> </td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL如果同名檔案存在]</td> 
   <td> <p> 如果與正在嘗試上載的檔案同名的檔案已存在，請選擇您要執行的操作。</p> 
    <ul> 
     <li>[!UICONTROL替換現有檔案]</li> 
     <li>[!UICONTROL更名新檔案]</li> 
     <li>[!UICONTROL結尾，出現錯誤]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案]

此操作模組將指定的檔案移動到資源回收筒。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇要從中刪除檔案的驅動器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td> <p>輸入要刪除的檔案ID。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

此動作模組會擷取具有指定ID的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇要從中檢索檔案的驅動器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案ID]</td> 
   <td> <p>輸入要檢索的檔案的ID。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立資料夾]

在指定的父資料夾內建立資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL連接]</strong> </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL驅動器ID]</strong> </td> 
   <td> <p>選擇要建立新資料夾的驅動器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL資料夾]</strong> </td> 
   <td> <p>選擇要在中建立新資料夾的資料夾。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL資料夾名稱]</strong> </td> 
   <td>輸入或映射新資料夾的名稱。</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除資料夾]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇要從中刪除檔案的驅動器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾ID]</td> 
   <td> <p>輸入或映射要刪除的資料夾ID。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得分享連結]

此模組會擷取您可共用的連結，以授予對指定檔案的存取權。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中建立案例 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL驅動器ID]</td> 
   <td> <p>選擇要將檔案上載到的驅動器。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enter]</td> 
   <td> <p>使用檔案ID或檔案路徑選擇檔案。 在顯示的欄位中輸入檔案ID或路徑。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL權限類型]</p> </td> 
   <td> <p>選擇是否希望接收連結的人員具有讀/寫權限或只讀權限。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL範圍]</td> 
   <td> <p> 選取您希望任何擁有連結的人都能存取該檔案，或僅供您組織的成員存取。</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
