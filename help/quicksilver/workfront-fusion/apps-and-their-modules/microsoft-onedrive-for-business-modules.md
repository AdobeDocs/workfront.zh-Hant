---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: 商務用Microsoft OneDrive模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1257'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business]模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [商務用Microsoft OneDrive模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/microsoft-onedrive-for-business-modules.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Microsoft OneDrive for Business]的工作流程，並將其連線至多個協力廠商應用程式和服務。

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

若要搭配[!DNL Adobe Workfront Fusion]使用[!DNL Microsoft OneDrive for Business]，您需要[!DNL Microsoft]帳戶。

如需有關將您的[!DNL OneDrive for Business]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱[建立與Adobe的連線 [!DNL Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)



## 正在將[!DNL Microsoft OneDrive for Business]服務連線到[!DNL Workfront Fusion]

如需有關將您的[!DNL Microsoft OneDrive for Business]帳戶連線到[!UICONTROL Workfront Fusion]的指示，請參閱[建立與[!UICONTROL Adobe Workfront Fusion]的連線](../../workfront-fusion/connections/connect-to-fusion-general.md) — 基本指示

>[!NOTE]
>
>部分Microsoft應用程式使用相同的連線，而此連線會繫結至個別使用者許可權。 因此，在建立連線時，許可權同意畫面會顯示先前授與此使用者連線的所有許可權，以及目前應用程式所需的任何新許可權。
>
>例如，如果使用者擁有透過Excel聯結器授予的「讀取表格」許可權，然後在Outlook聯結器中建立連線以讀取電子郵件，則許可權同意畫面會顯示已授予的「讀取表格」許可權和新要求的「寫入電子郵件」許可權。

## [!DNL Microsoft OneDrive for Business]模組及其欄位

當您設定[!DNL Microsoft OneDrive for Business]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Microsoft OneDrive for Business]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [觸發程序](#triggers)
* [動作](#actions)

### 觸發程序

* [[!UICONTROL 觀看檔案]](#watch-files)
* [[!UICONTROL 監視資料夾]](#watch-folders)

#### [!UICONTROL 觀看檔案]

在被監視的資料夾中新增或更新新檔案時，此觸發模組會啟動。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL磁碟機ID]</p> </td> 
   <td> <p>選取您要觀看的磁碟機。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td> <p> 選取要監視的資料夾。 在案例中，您只能監視一個資料夾。</p> <p>提示：若要追蹤多個資料夾，請為每個資料夾建立獨立案例。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL我要觀看]</p> </td> 
   <td> <p>選取您是要監視新檔案與所有變更，還是隻監視新檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL傳回資料列數目上限]</td> 
   <td> <p> 設定[!DNL Workfront Fusion]在一個週期內可處理的最大結果數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監視資料夾]

將新資料夾新增到要監看的資料夾時，此觸發模組會啟動。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL磁碟機ID]</p> </td> 
   <td> <p>選取您要觀看的磁碟機。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td> <p> 選取要監視的資料夾。 在案例中，您只能監視一個資料夾。</p> <p>提示：若要追蹤多個資料夾，請為每個資料夾建立獨立案例。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL我要觀看]</p> </td> 
   <td> <p>選取您要監視新資料夾和所有變更，還是隻監視新資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL傳回資料列數目上限]</td> 
   <td> <p> 設定[!DNL Workfront Fusion]在一個週期內可處理的最大結果數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 上傳檔案]](#upload-a-file)
* [[!UICONTROL 刪除檔案]](#delete-a-file)
* [[!UICONTROL 取得檔案]](#get-a-file)
* [[!UICONTROL 建立資料夾]](#create-a-folder)
* [[!UICONTROL 刪除資料夾]](#delete-a-folder)
* [[!UICONTROL 取得共用連結]](#get-a-sharing-link)

#### [!UICONTROL 上傳檔案]

此動作模組會將二進位檔或文字檔上傳至指定的資料夾

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取您要上傳檔案的磁碟機。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取磁碟機中的資料夾。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Source檔案]</p> </td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL如果存在相同名稱的檔案]</td> 
   <td> <p> 選取當您嘗試上傳的檔案已存在時，您要執行的動作。</p> 
    <ul> 
     <li>[！UICONTROL取代現有的檔案]</li> 
     <li>[！UICONTROL重新命名新檔案]</li> 
     <li>[！UICONTROL結尾有錯誤]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案]

此動作模組會將指定的檔案移至資源回收筒。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取您要刪除檔案的磁碟機。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td> <p>輸入您要刪除之檔案的ID。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

此動作模組會擷取具有特定ID的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取您要擷取檔案的磁碟機。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td> <p>輸入您要擷取的檔案ID。 </p> </td> 
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
   <td><strong>[！UICONTROL連線]</strong> </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[！UICONTROL磁碟機識別碼]</strong> </td> 
   <td> <p>選取您要建立新資料夾的磁碟機。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[！UICONTROL資料夾]</strong> </td> 
   <td> <p>選取您要建立新資料夾的資料夾。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[！UICONTROL資料夾名稱]</strong> </td> 
   <td>輸入或對應新資料夾的名稱。</td> 
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
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取您要刪除檔案的磁碟機。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾ID]</td> 
   <td> <p>輸入或對應您要刪除的資料夾識別碼。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得共用連結]

此模組會擷取您可共用的連結，以授予指定檔案的存取權。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中建立案例一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連線到[!DNL Workfront Fusion]</a>。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL磁碟機ID]</td> 
   <td> <p>選取您要上傳檔案的磁碟機。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Enter]</td> 
   <td> <p>選取您要使用「檔案ID」或「檔案」路徑來選擇檔案。 在出現的欄位中輸入檔案ID或路徑。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL許可權型別]</p> </td> 
   <td> <p>選取您希望收到連結的人員具有讀取/寫入許可權還是唯讀。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL範圍]</td> 
   <td> <p> 選取您是否希望檔案僅供擁有連結的任何人存取或僅供組織成員存取。</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
