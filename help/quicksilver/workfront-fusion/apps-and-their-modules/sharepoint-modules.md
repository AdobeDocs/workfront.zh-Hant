---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: SharePoint模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用SharePoint的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 16d49031-06d2-4c86-bac4-f58cd9b2f1f5
source-git-commit: 8283022f24913988248005da0c8e583b29f19652
workflow-type: tm+mt
source-wordcount: '2371'
ht-degree: 0%

---

# [!DNL SharePoint] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL SharePoint]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!DNL SharePoint] 模組，您必須 [!DNL SharePoint] 帳戶。

## Connect [!DNL SharePoint] to [!DNL Workfront Fusion] {#connect-sharepoint-to-workfront-fusion}

* [Connect [!DNL SharePoint] to [!DNL Workfront Fusion] 使用 [!DNL Microsoft] 帳戶](#connect-sharepoint-to-workfront-fusion-using-a-microsoft-account)
* [Connect [!DNL SharePoint] to [!DNL Workfront Fusion] 使用進階設定](#connect-sharepoint-to-workfront-fusion-using-advanced-settings)

### Connect [!DNL SharePoint] to [!DNL Workfront Fusion] 使用 [!DNL Microsoft] 帳戶

您可以使用 [!DNL Microsoft] 帳戶來建立連線至 [!DNL SharePoint]. 有關連接 [!DNL Sharepoint] 帳戶 [!DNL Workfront Fusion]，請參閱 [建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

### Connect [!DNL SharePoint] to [!DNL Workfront Fusion] 使用進階設定

連接 [!DNL SharePoint] to [!DNL Workfront Fusion] 沒有 [!DNL Microsoft] 帳戶，您需要用戶端ID、用戶端密碼和租用戶ID。

1. 按一下 **[!UICONTROL 新增]** 在 **[!DNL SharePoint]** 方塊以開啟 **[!UICONTROL 建立連線]** 框。

1. （選用）變更預設值 **[!UICONTROL 連線名稱]**.
1. 按一下 **[!UICONTROL 顯示高級設定]**.
1. 輸入 [!DNL SharePoint] **[!UICONTROL 用戶端ID]** 和 **[!UICONTROL 用戶端密碼]**.

1. 按一下 **[!UICONTROL 繼續]**.
1. 在顯示的登入視窗中，輸入您的憑證以登入應用程式（如果尚未登入）。
1. （條件性）若 **[!UICONTROL 允許]** 按鈕隨即顯示，按一下按鈕以將應用程式連線至 [!DNL Workfront Fusion].

## [!DNL SharePoint] 模組及其欄位

設定時 [!DNL SharePoint] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL SharePoint] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [驅動器項](#drive-item)
* [項目](#item)
* [清單](#list)
* [頁面（測試版）](#page-beta)
* [網站](#site)
* [其他](#other)

### 驅動器項

* [建立檔案](#create-a-file)
* [建立資料夾](#create-a-folder)
* [取得檔案](#get-a-file)
* [監看資料夾項目](#watch-folder-items)

#### 建立檔案

此動作模組會在SharePoint中建立新檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入站點、驅動器和資料夾ID]</td> 
   <td> <p>選取如何識別要建立的檔案位置。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong>, <strong>[!UICONTROL清單ID]</strong>，和 <strong>[!UICONTROL資料夾ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL從您關注的清單中選擇]</strong> </p> <p>選取要建立檔案的位置。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</td> 
  </tr>  </tbody> 
</table>

#### 建立資料夾

此動作模組會在SharePoint中建立新資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入站點、驅動器和資料夾ID]</td> 
   <td> <p>選擇要如何標識要建立的資料夾的位置。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong>, <strong>[!UICONTROL清單ID]</strong>，和 <strong>[!UICONTROL資料夾ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL從您關注的清單中選擇]</strong> </p> <p>選取要建立資料夾的位置。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾名稱]</td> 
   <td>輸入或映射新資料夾的名稱。</td> 
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
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入站點、驅動器和資料夾ID]</td> 
   <td> <p>選擇要如何標識要獲取的檔案的位置。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong>, <strong>[!UICONTROL清單ID]</strong>，和 <strong>[!UICONTROL檔案ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL從您關注的清單中選擇]</strong> </p> <p>選取檔案的位置。 </p> </li> 
    </ul> </td> 
  </tr> 
</tbody> 
</table>

#### 監看資料夾項目

當您選取的資料夾中更新項目時，此觸發程式模組就會啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入站點、驅動器和資料夾ID]</td> 
   <td> <p>選擇要如何標識要獲取的檔案的位置。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong>, <strong>[!UICONTROL清單ID]</strong>，和 <strong>[!UICONTROL資料夾ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL從您關注的清單中選擇]</strong> </p> <p>選擇要監視的資料夾的位置。 </p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>輸入項目數上限 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。</td> 
  <tr>
  </tr>
</tbody> 
</table>

### 項目

* [[!UICONTROL 監看項目]](#watch-items)
* [[!UICONTROL 清單項目]](#list-items)
* [[!UICONTROL 取得項目]](#get-an-item)
* [[!UICONTROL 建立項目]](#create-an-item)
* [[!UICONTROL 更新項目]](#update-an-item)
* [[!UICONTROL 刪除項目]](#delete-an-item)

#### [!UICONTROL 監看項目]

此觸發模組會在建立或修改項目時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL監視清單]</td> 
   <td>選擇要按建立時間（新項目）或修改時間（更新項目）監視清單。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入站點和清單ID]</td> 
   <td> <p>選擇要如何標識要監視的網站和清單。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong> 和 <strong>[!UICONTROL清單ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL從您關注的清單中選擇]</strong> </p> <p>選擇要監視的網站，然後選擇清單。 這些下拉式清單只會擷取後續的網站。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期期間返回的項目數上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清單項目]

此動作模組會擷取指定清單中所有項目的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL清單項]</td> 
   <td> <p>選取要如何識別要從中擷取項目的清單。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong> 和 <strong>[!UICONTROL清單ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇包含要從中檢索項的清單的網站，然後選擇該清單。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期期間返回的項目數上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得項目]

此動作模組會傳回指定項目的資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL獲取項]</td> 
   <td> <p>選擇要如何標識包含要獲取項目的站點和清單。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong>, <strong>[!UICONTROL清單ID]</strong>，和 <strong>[!UICONTROL項目ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇包含要從中檢索項的清單的網站，然後選擇該清單，然後選擇該項。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立項目]

此動作模組會在SharePoint清單中建立新項目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL建立項目]</td> 
   <td> <p>選取您要如何識別網站，並列出您要建立項目的位置。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong> 和 <strong>[!UICONTROL清單ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇包含要建立項的清單的站點，然後選擇該清單。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL欄位]</td> 
   <td>對於要為新項目設定的每個欄位，輸入欄位的鍵（標識欄位），以及您希望新項目在該欄位中具有的值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新項目]

此動作模組會更新SharePoint清單中的現有項目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL更新項]</td> 
   <td> <p>選擇要如何標識包含要更新項的站點和清單。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong>, <strong>[!UICONTROL清單ID]</strong>，和 <strong>[!UICONTROL項目ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇包含要更新項的站點，然後選擇清單，然後選擇項。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL欄位]</td> 
   <td>對於要為新項目更新的每個欄位，輸入欄位的鍵（標識欄位），以及您希望該項目在該欄位中具有的新值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除項目]

此動作模組會刪除SharePoint清單中的現有項目。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL更新項]</td> 
   <td> <p>選擇要如何標識包含要刪除項的站點和清單。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong>, <strong>[!UICONTROL清單ID]</strong>，和 <strong>[!UICONTROL項目ID]</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇包含要刪除的項的站點，然後選擇清單，然後選擇項。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 清單

* [[!UICONTROL 監視清單]](#watch-lists)
* [[!UICONTROL 清單清單]](#list-lists)
* [[!UICONTROL 取得清單]](#get-a-list)
* [[!UICONTROL 建立清單]](#create-a-list)

#### [!UICONTROL 監視清單]

建立或修改清單時，此觸發器模組就會啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL監視清單]</td> 
   <td>選擇要按建立時間（新項目）或修改時間（更新項目）監視清單。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入站點和清單ID]</td> 
   <td> <p>選擇要如何標識要監視的網站和清單。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong> 您要監視的清單位於何處。</p> </li> 
     <li> <p><strong>[!UICONTROL從您關注的清單中選擇]</strong> </p> <p>選擇要監視的網站。 下拉式清單只會擷取您追蹤的網站。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大清單數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清單清單]

此動作模組會擷取指定清單中所有項目的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL清單]</td> 
   <td> <p>選擇要如何識別要從中檢索清單的站點。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇包含要檢索的清單的網站。 下拉式清單只會擷取您追蹤的網站。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大清單數。</p> </td> 
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
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL獲取清單]</td> 
   <td> <p>選擇要如何標識包含要獲取項目的站點和清單。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong> 和 <strong>清單ID</strong> 中。</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇包含要檢索的清單的站點，然後選擇該清單。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立清單]

此動作模組會在SharePoint中建立新清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入站點ID]</td> 
   <td> <p>選取您要如何識別網站，並列出您要建立清單的位置。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong> 建立清單的位置。</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇要建立清單的網站。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示名稱]</td> 
   <td>輸入或映射新清單的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL描述]</td> 
   <td>輸入或映射新清單的說明。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL添加列]</td> 
   <td>對於要為新清單設定的每列，輸入 <strong>[!UICONTROL名稱]</strong> ，然後選取 <strong>[!UICONTROL類型]</strong> 的值。</td> 
  </tr> 
 </tbody> 
</table>

### 頁面（測試版）

>[!NOTE]
>
>中的API `beta` 版本 [!DNL Microsoft Graph] 可能會有所變更。 不支援在生產應用程式中使用這些API。

#### [!UICONTROL 取得頁面]

此動作模組會傳回指定頁面的資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL獲取頁面]</td> 
   <td> <p>選取要如何識別要擷取的頁面。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong>和 <strong>[!UICONTROL頁面ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇包含要檢索的頁的站點，然後選擇該頁。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 網站

* [[!UICONTROL 搜尋網站]](#search-sites)
* [[!UICONTROL 取得網站]](#get-a-site)

#### [!UICONTROL 搜尋網站]

此動作模組會依您指定的參數來搜尋網站。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示名稱的關鍵字]</td> 
   <td> <p>輸入或映射要搜索網站的搜索詞。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的站點數上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得網站]

此動作模組會傳回指定網站的資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL獲取站點]</td> 
   <td> <p>選取要如何識別要擷取的頁面。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL站點ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選擇要檢索的網站。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### [!UICONTROL 進行API呼叫]

此模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL SharePoint] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sharepoint-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL SharePoint] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於的路徑 <code>https://graph.microsoft.com</code>. 範例:<code> /beta/sites</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 為您添加授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p> 以標準JSON物件的形式新增API呼叫的查詢。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL類型]</td> 
   <td>選取您要在API呼叫中傳送的資料類型。</td> 
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

