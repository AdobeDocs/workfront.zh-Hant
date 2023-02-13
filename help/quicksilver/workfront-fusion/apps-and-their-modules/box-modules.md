---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: 盒模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Box的工作流程，並將其連接至多個協力廠商應用程式和服務。 監視指定的資料夾以檢查檔案更改、修改和刪除現有檔案，或將新檔案上載到資料夾。
author: Becky
feature: Workfront Fusion
exl-id: 965ce570-40bf-474d-b318-0d2de8be6b9d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# 盒模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Box]，並將其連接至多個協力廠商應用程式和服務。 監視指定的資料夾以檢查檔案更改、修改和刪除現有檔案，或將新檔案上載到資料夾。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Box] 模組，您必須 [!DNL Box] 帳戶。

## [!DNL Box] 模組及其欄位

設定時 [!DNL Box] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Box] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 觸發器

* [[!UICONTROL 新事件]](#new-event)
* [[!UICONTROL 監看檔案]](#watch-files)

#### [!UICONTROL 新事件]

此即時觸發模組會在檔案新增、移動、複製、刪除、鎖定或解除鎖定時啟動案例。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>選取您要用來監視傳出訊息的網頁連結。 若要新增網頁連結，請按一下 <strong>[!UICONTROL添加]</strong> 並輸入webhook的名稱和連接。</p> <p> 有關將您的[!UICONTROL Box]帳戶連接到[!UICONTROL Workfront Fusion]的說明，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">將模組的應用程式或Web服務連接到[!UICONTROL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!UICONTROL Adobe Workfront Fusion]中建立案例</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL返回事件的最大數]</p> </td> 
   <td> <p>輸入在每個方案執行週期中，希望模組返回的事件數最多。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監看檔案]

若新增新檔案或在觀看的資料夾中更新現有檔案，此觸發程式模組就會啟動案例。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>有關連接 [!DNL Box] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  <tr> 
   <td role="rowheader">Watch</td> 
   <td> <p>選擇要監視的檔案類型。</p> 
    <ul> 
     <li> <p><strong>僅新檔案</strong> </p> <p>新增新檔案時，就會開始情境。</p> </li> 
     <li> <p><strong>新檔案和所有更改</strong> </p> <p>當新增檔案，或修改檔案內容或檔案屬性（如其名稱）時，就會開始情境。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>下載檔案的最大數量</p> </td> 
   <td> <p>輸入在每個方案執行週期中要模組返回的最大檔案數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 上傳] 檔案](#upload-a-file)
* [[!UICONTROL 更新檔案]](#update-a-file)
* [[!UICONTROL 刪除檔案]](#delete-a-file)
* [[!UICONTROL 取得檔案]](#get-a-file)

#### [!UICONTROL 上傳檔案]

此動作模組會上傳檔案。

您可指定檔案。 您也可以為檔案提供新的檔案名稱。

模組會傳回檔案的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Box] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>如果此模組未成功，請考慮下列事項：
>
>* 檔案大小可能超過 [!DNL Box] 計畫，或者你用了 [!DNL Box] 帳戶的儲存配額。 若要獲得更多儲存空間，請從 [!DNL Box] 或升級您的 [!DNL Box] 帳戶。
>* [!DNL Box] 不會將多個同名檔案上傳至單一資料夾。 如果目標資料夾包含的檔案名稱與要上傳的檔案相同，則方案執行會終止，並產生錯誤。 若要避免此情況，請重新命名檔案。 如果您想更新檔案，請使用 **[!UICONTROL 更新檔案]** 模組。


#### [!UICONTROL 更新檔案]

此動作模組會更新檔案。

您可指定檔案的ID。

模組會傳回檔案的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Box] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案ID]</td> 
   <td>輸入或映射要更新模組的檔案的唯一ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案]

此動作模組會刪除檔案。

您可指定檔案的ID。

模組會傳回檔案的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Box] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案ID]</td> 
   <td>輸入或映射要更新模組的檔案的唯一ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

此動作模組會下載檔案。

您可指定檔案的ID。

模組會傳回檔案的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

>[!NOTE]
>
>此模組對於將檔案提供給後續模組非常有用。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Box] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案ID]</td> 
   <td>輸入或映射要更新模組的檔案的唯一ID。</td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Possible problems</h2>
-->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is drafted out because we don't have a download module for Box yet</p>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Watch files trigger module doesn't download a file contained in the folder.</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">There are several situations when downloading a file fails:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The current file lock setting does not allow the file to be downloaded or the downloading of the file is disabled. In this case, the file is ignored.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the scenario started, the file was being uploaded to the server and was not ready to be downloaded. The scenario run gets stopped and Workfront Fusion tries downloading the file again during the next execution of the scenario.</li>
  -->
