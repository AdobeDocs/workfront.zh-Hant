---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: SharePoint模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用SharePoint的工作流程，並將其連結至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '2850'
ht-degree: 0%

---

# [!DNL SharePoint] 模組

在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL SharePoint]，以及將其連線到多個協力廠商應用程式和服務。

如果您需要建立案例的說明，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!DNL SharePoint] 模組，您必須擁有 [!DNL SharePoint] 帳戶。

## Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion] 使用 [!DNL Microsoft] 帳戶](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion] 使用進階設定](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion] 使用 [!DNL Microsoft] 帳戶

您可以使用 [!DNL Microsoft] 要建立連線的帳戶 [!DNL SharePoint]. 如需有關連線您的電腦的指示， [!DNL Sharepoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 [建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion] 使用進階設定

若要連線 [!DNL SharePoint] 至 [!DNL Workfront Fusion] 不含 [!DNL Microsoft] 帳戶，您需要使用者端ID、使用者端密碼和租使用者ID。

1. 按一下 **[!UICONTROL 新增]** 靠近 **[!DNL SharePoint]** 方塊以開啟 **[!UICONTROL 建立連線]** 方塊。

1. （選用）變更預設值 **[!UICONTROL 連線名稱]**.
1. 按一下 **[!UICONTROL 顯示進階設定]**.
1. 輸入 [!DNL SharePoint] **[!UICONTROL 使用者端ID]** 和 **[!UICONTROL 使用者端密碼]**.

1. 按一下 **[!UICONTROL 繼續]**.
1. 在顯示的登入視窗中，輸入您的認證以登入應用程式（如果尚未這麼做）。
1. （有條件）若為 **[!UICONTROL 允許]** 按鈕顯示，按一下按鈕以連線應用程式 [!DNL Workfront Fusion].

## [!DNL SharePoint] 模組及其欄位

當您設定 [!DNL SharePoint] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL SharePoint] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [磁碟機專案](#drive-item)
* [項目](#item)
* [清單](#list)
* [頁面（測試版）](#page-beta)
* [網站](#site)
* [其他](#other)

### 磁碟機專案

* [建立檔案](#create-a-file)
* [建立資料夾](#create-a-folder)
* [取得檔案](#get-a-file)
* [監視資料夾專案](#watch-folder-items)

#### 取得變更

此模組會傳回SharePoint中所做的變更。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入網站、磁碟機和資料夾ID]</td> 
   <td> <p>選取您要如何識別要擷取變更的資料夾位置。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>， <strong>[！UICONTROL清單ID]</strong>、和 <strong>[！UICONTROL資料夾ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從您追蹤的清單中選取]</strong> </p> <p>選取您要擷取變更的位置。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL權杖]</td> 
   <td> </td> 
  </tr>  </tbody> 
</table>

#### 建立資料夾

此動作模組會在SharePoint中建立新資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入網站、磁碟機和資料夾ID]</td> 
   <td> <p>選取要如何識別要建立的資料夾位置。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>， <strong>[！UICONTROL清單ID]</strong>、和 <strong>[！UICONTROL資料夾ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從您追蹤的清單中選取]</strong> </p> <p>選取您要建立資料夾的位置。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾名稱]</td> 
   <td>輸入或對應新資料夾的名稱。</td> 
  </tr>
  </tbody> 
</table>

#### 取得檔案

此動作模組會擷取指定的SharePoint檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入網站、磁碟機和資料夾ID]</td> 
   <td> <p>選取要如何識別要取得之檔案的位置。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>， <strong>[！UICONTROL清單ID]</strong>、和 <strong>[！UICONTROL檔案ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從您追蹤的清單中選取]</strong> </p> <p>選取檔案的位置。 </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### 監視資料夾專案

當您選取的資料夾中更新了專案時，此觸發模組就會啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入網站、磁碟機和資料夾ID]</td> 
   <td> <p>選取要如何識別要取得之檔案的位置。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>， <strong>[！UICONTROL清單ID]</strong>、和 <strong>[！UICONTROL資料夾識別碼]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從您追蹤的清單中選取]</strong> </p> <p>選取您要觀看的資料夾位置。 </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入專案的最大數量 [!DNL Workfront Fusion] 應該會在一個案例執行週期中傳回。</td> 
  <tr>
  </tr>
</tbody> 
</table>

### 項目

* [[!UICONTROL 複製專案]](#copy-an-item)
* [[!UICONTROL 建立專案]](#create-an-item)
* [[!UICONTROL 刪除專案]](#delete-an-item)
* [[!UICONTROL 取得專案]](#get-an-item)
* [[!UICONTROL 清單專案]](#list-items)
* [[!UICONTROL 移動專案]](#move-an-item)
* [[!UICONTROL 更新專案]](#update-an-item)
* [[!UICONTROL 觀看專案] （已排程）](#watch-items-scheduled)


#### [!UICONTROL 複製專案]

此動作模組會複製SharePoint清單中的現有專案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">輸入網站、磁碟機和資料夾ID</td> 
   <td> <p>選取您要如何識別包含您要複製之專案的場地和清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>， <strong>[！UICONTROL清單ID]</strong>、和 <strong>[！UICONTROL專案ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從您遵循的清單中選取]</strong> </p> <p>在「專案型別」欄位中，選取您要移動欄位或資料夾。  選取包含您要複製之專案的網站，然後選取清單，再選取專案。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目的地ID]</td> 
   <td> 輸入或對應您要複製專案的資料夾識別碼。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新名稱]</td> 
   <td>輸入或對應專案新復本的名稱。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立專案]

此動作模組會在SharePoint清單中建立新專案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL建立專案]</td> 
   <td> <p>選取您要如何識別網站以及要建立專案的清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong> 和 <strong>[！UICONTROL清單ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要建立專案之清單的網站，然後選取清單。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄位]</td> 
   <td>針對您想要為新專案設定的每個欄位，輸入欄位的索引鍵（識別欄位），以及您希望新專案在該欄位中擁有的值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除專案]

此動作模組會刪除SharePoint清單中的現有專案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL更新專案]</td> 
   <td> <p>選取您要如何識別包含您要刪除之專案的場地和清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>， <strong>[！UICONTROL清單ID]</strong>、和 <strong>[！UICONTROL專案ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要刪除之專案的網站，然後選取清單，再選取專案。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得專案]

此動作模組會傳回指定專案的資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL取得專案]</td> 
   <td> <p>選取您要如何識別網站以及包含您要取得之專案的清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>， <strong>[！UICONTROL清單ID]</strong>、和 <strong>[！UICONTROL專案ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要從中擷取專案的清單的網站，然後選取清單，再選取專案。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清單專案]

此動作模組會擷取指定清單中所有專案的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL清單專案]</td> 
   <td> <p>選取您要如何識別要從中擷取專案的清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong> 和 <strong>[！UICONTROL清單ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要從中擷取專案的清單的網站，然後選取清單。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大專案數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動專案]

此動作模組會複製SharePoint清單中的現有專案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">輸入網站、磁碟機和資料夾ID</td> 
   <td> <p>選取您要如何識別包含您要移動之專案的場地和清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>， <strong>[！UICONTROL清單ID]</strong>、和 <strong>[！UICONTROL專案ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從您遵循的清單中選取]</strong> </p> <p>在「專案型別」欄位中，選取您要移動欄位或資料夾。 選取包含您要複製之專案的網站，然後選取清單，再選取專案。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目的地ID]</td> 
   <td> 輸入或對應您要移動專案的資料夾識別碼。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新名稱]</td> 
   <td>輸入或對映已移動專案的名稱。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新專案]

此動作模組會更新SharePoint清單中的現有專案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL更新專案]</td> 
   <td> <p>選取您要如何識別包含您要更新之專案的地點和清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>， <strong>[！UICONTROL清單ID]</strong>、和 <strong>[！UICONTROL專案ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要更新之專案的地點，然後選取清單，再選取專案。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄位]</td> 
   <td>對於要更新新專案的每個欄位，輸入欄位的索引鍵（識別欄位），以及您希望專案對該欄位具有的新值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看專案] （已排程）

此觸發模組會在建立或修改專案時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL監看清單]</td> 
   <td>選取您要依建立時間（新專案）或修改時間（更新專案）來監視清單。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入網站和清單ID]</td> 
   <td> <p>選取您要如何識別要觀看的網站和清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong> 和 <strong>[！UICONTROL清單ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從您追蹤的清單中選取]</strong> </p> <p>選取您要觀看的網站，然後選取清單。 這些下拉式清單只會擷取追蹤的網站。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大專案數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 清單

* [[!UICONTROL 建立清單]](#create-a-list)
* [[!UICONTROL 取得清單]](#get-a-list)
* [[!UICONTROL 清單清單]](#list-lists)
* [[!UICONTROL 觀看清單]](#watch-lists)

#### [!UICONTROL 建立清單]

此動作模組會在SharePoint中建立新清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入網站ID]</td> 
   <td> <p>選取您要如何識別網站和要建立清單的清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong> 建立清單的位置。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取您要建立清單的網站。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示名稱]</td> 
   <td>輸入或對應新清單的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL說明]</td> 
   <td>輸入或對應新清單的說明。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新增欄]</td> 
   <td>對於要為新清單設定的每個欄，輸入 <strong>[！UICONTROL名稱]</strong> 欄位中輸入，然後選取 <strong>[！UICONTROL型別]</strong> 您希望新欄擁有的值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得清單]

此動作模組會傳回指定清單的資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL取得清單]</td> 
   <td> <p>選取您要如何識別網站以及包含您要取得之專案的清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong> 和 <strong>清單ID</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要擷取之清單的網站，然後選取清單。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清單清單]

此動作模組會擷取指定清單中所有專案的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL清單清單]</td> 
   <td> <p>選取您要如何識別要從中擷取清單的網站。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>.</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要擷取之清單的網站。 下拉式清單只會擷取您關注的網站。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大清單數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看清單]

建立或修改清單時，此觸發模組就會啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL監看清單]</td> 
   <td>選取您要依建立時間（新專案）或修改時間（更新專案）來監視清單。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入網站和清單ID]</td> 
   <td> <p>選取您要如何識別要觀看的網站和清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong> 您要觀看的清單所在的位置。</p> </li> 
     <li> <p><strong>[！UICONTROL從您追蹤的清單中選取]</strong> </p> <p>選取您要觀看的網站。 下拉式清單只會擷取您關注的網站。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大清單數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 頁面（測試版）

>[!NOTE]
>
>中的API `beta` 中的版本 [!DNL Microsoft Graph] 隨時可能變更。 不支援在生產應用程式中使用這些API。

#### [!UICONTROL 取得頁面]

此動作模組會傳回指定頁面的資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL取得頁面]</td> 
   <td> <p>選取您要如何識別要擷取的頁面。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>和 <strong>[！UICONTROL頁面ID]</strong>.</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要擷取之頁面的網站，然後選取頁面。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 網站

* [[!UICONTROL 取得網站]](#get-a-site)
* [[!UICONTROL 搜尋網站]](#search-sites)

#### [!UICONTROL 取得網站]

此動作模組會傳回指定網站的資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL取得網站]</td> 
   <td> <p>選取您要如何識別要擷取的頁面。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>.</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取您要擷取的網站。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋網站]

此動作模組會依您指定的引數搜尋網站。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">顯示名稱的[！UICONTROL關鍵字]</td> 
   <td> <p>輸入或對應您要搜尋網站的搜尋字詞。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大網站數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### 取得變更

此模組會擷取在SharePoint資料夾中所做的增加、更新及刪除。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入網站、磁碟機和資料夾ID]</td> 
   <td> <p>選取您要如何識別包含您要更新之專案的地點和清單。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[！UICONTROL網站ID]</strong>， <strong>[！UICONTROL磁碟機ID]</strong>、和 <strong>[！UICONTROL資料夾ID]</strong> 在出現的欄位中。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含您要更新之專案的網站，然後選取磁碟機，再選取資料夾。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL權杖]</td> 
   <td> 代號會識別模組應該從何時開始擷取變更。  </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 進行API呼叫]

此模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL SharePoint] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於 <code>https://graph.microsoft.com</code>. 範例:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p> 以標準JSON物件的形式新增API呼叫的查詢。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL型別]</td> 
   <td>選取您要在API呼叫中傳送的資料型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### 觀看活動

此即時觸發模組會在SharePoint中新增、更新或刪除專案時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <!--
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL SharePoint] account to [!DNL Workfront Fusion], see <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  -->
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook]</td> 
   <td> <p>選取現有的webhook，或按一下「新增」以建立新的webhook。</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

