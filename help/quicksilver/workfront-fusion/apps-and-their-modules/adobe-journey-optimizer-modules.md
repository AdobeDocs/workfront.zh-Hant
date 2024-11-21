---
filename: adobe-journey-optimizer-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Journey Optimizer模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用 [!DNL Adobe Journey Optimizer]的工作流程，並將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 2c1aea46-edbf-42a3-a6e9-f8aea042a48d
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '3692'
ht-degree: 0%

---

# [!DNL Adobe Journey Optimizer]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Adobe Journey Optimizer]的工作流程，並將其連線至多個協力廠商應用程式和服務。 [!DNL Adobe Journey Optimizer]模組可讓您建立、讀取、更新或刪除記錄，或執行對[!DNL Adobe Journey Optimizer] API的自訂API呼叫。


如果您需要有關建立案例的指示，請參閱[建立案例](../../workfront-fusion/scenarios/create-a-scenario.md)。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能使用本文中的功能：

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
      <td>
        <p>[！UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
      <td>
        <p>[！UICONTROL計畫]，[！UICONTROL工作]</p>
      </td>
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

+++

## 先決條件

使用[!DNL Adobe Journey Optimizer]聯結器之前，您必須確定符合下列先決條件：

* 您必須擁有使用中的[!DNL Adobe Journey Optimizer]帳戶。

## Adobe Journey Optimizer API資訊

Adobe Journey Optimizer聯結器會使用以下專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td>{{connection.url}}</td> 
  </tr>
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v1.7.11</td> 
  </tr>
 </tbody> 
 </table>

## 建立與Adobe Journey Optimizer的連線

您可以在任何Adobe Journey Optimizer模組中建立連線。

1. 按一下[連線]方塊旁的&#x200B;**[!UICONTROL 新增]**。

1. 填寫下列欄位：

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[！UICONTROL連線名稱]</td>
        <td>
          <p>輸入此連線的名稱。</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL環境]</td>
        <td>選取您要連線到生產或非生產環境。</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL型別]</td>
        <td>選取您要連線到服務帳戶還是個人帳戶。</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL使用者端ID]</td>
        <td>輸入您的[！UICONTROLAdobe] [！UICONTROL使用者端ID]。 您可在的[！UICONTROL Credentials]詳細資訊區段中找到 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL使用者端密碼]</td>
        <td>輸入您的[!DNL Adobe] [！UICONTROL使用者端密碼]。 您可在的[！UICONTROL Credentials]詳細資訊區段中找到 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL組織ID]</td>
        <td>輸入您的[!DNL Adobe] [！UICONTROL組織識別碼]。 您可在的[！UICONTROL Credentials]詳細資訊區段中找到 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL沙箱名稱]</td>
        <td>輸入此連線將使用的沙箱名稱。</td>
        </tr>
      </tbody>
    </table>


## [!DNL Adobe Journey Optimizer]模組及其欄位

當您設定[!DNL Adobe Journey Optimizer]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Adobe Journey Optimizer]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [設定管理](#configuration-management)
* [封裝管理](#package-management)
* [記錄管理](#record-management)
* [訊息管理](#message-management)
* [狀態檢查](#status-checks)
* [搜尋](#searches)
* [其他](#other)




### 設定管理

* [建立設定](#create-a-configuration)
* [部署設定](#deploy-a-configuration)
* [更新設定](#update-a-configuration)
* [取消部署設定](#undeploy-a-configuration)
* [檢查配置是否可以部署](#check-if-configuration-can-be-deployed)
* [刪除設定](#delete-a-configuration)
* [取得設定](#get-a-configuration)

#### 建立設定

此動作模組會建立上限端點或節流設定。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取設定型別]</td> 
   <td>選取您要建立上限設定還是節流設定。<ul><li><p><b>頻率限定</b></p>繼續<a href="#capping-fields" class="MCXref xref" >限定欄位</a>。</li><li><p><b>節流</b></p>繼續<a href="#throttling-fields" class="MCXref xref" >節流欄位</a>。</li></ul></td> 
  </tr> 
   </tbody> 
</table>

##### 欄位上限

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>輸入或對應您要設定的端點URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL IMS組織ID]</td> 
   <td>輸入或對應組織的Adobe IMS ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Methods]</td> 
   <td>選取要在此設定中使用的方法。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL服務]</td> 
   <td>選取您要針對此設定使用動作或資料來源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL HTTP連線上限]</td> 
   <td>輸入或對應此端點的同時連線數目上限。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大呼叫數]</td> 
   <td>輸入或對應在「時段」欄位中指定的時段內要執行的最大呼叫數目。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL時段（毫秒）]</td> 
   <td>輸入或對應與「最大呼叫數」欄位相關的毫秒數。</td> 
  </tr> 
 </tbody> 
</table>

##### 節流欄位

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[！UICONTROL名稱]</td> 
   <td>輸入或對應此設定的名稱。</td> 
<tr> 
   <td role="rowheader">[！UICONTROL說明]</td> 
   <td>輸入或對應此設定的說明。</td> 
  </tr> 
<tr> 
   <td role="rowheader">[！UICONTROL URL模式]</td> 
   <td>輸入或對應您要節流之端點的URL。</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Methods]</td> 
   <td>選取要在此設定中使用的方法。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大輸送量]</td> 
   <td>選取您要針對此設定使用動作或資料來源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL HTTP連線上限]</td> 
   <td>輸入或對應此端點的同時連線數目上限。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大呼叫數]</td> 
   <td>輸入或對應您要為此端點設定的最大輸送量。 此值必須介於200到5000之間。</td> 
  </tr> 
 </tbody> 
</table>

#### 部署設定

此動作模組會部署指定的上限或節流設定。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取設定型別]</td> 
   <td>選取您要部署上限設定還是節流設定。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL組態ID]</td> 
   <td>輸入或對應您要部署的組態ID。</td> 
  </tr> 
 </tbody> 
</table>

#### 更新設定

此動作模組會更新指定的上限或節流設定。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取設定型別]</td> 
   <td>選取您要更新上限設定還是節流設定。<ul><li><p><b>頻率限定</b></p>如需欄位相關資訊，請參閱本文章建立設定一節中的<a href="#capping-fields" class="MCXref xref" >欄位上限</a>。</li><li><p><b>節流</b></p>如需欄位相關資訊，請參閱本文章建立設定一節中的<a href="#throttling-fields" class="MCXref xref" >節流欄位</a>。</li></ul></td> 
  </tr> 
  </tbody> 
</table>

#### 取消部署設定

此動作模組會取消部署上限或節流設定。 組態狀態已變回部署（`created`或`updated`）前的狀態。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取設定型別]</td> 
   <td>選取您要取消部署上限設定還是節流設定。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL組態ID]</td> 
   <td>輸入或對應您要取消部署的組態ID。</td> 
  </tr> 
 </tbody> 
</table>

#### 檢查配置是否可以部署

此動作模組會驗證是否可以部署上限或節流設定。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取設定型別]</td> 
   <td>選取您要檢查上限設定還是節流設定。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL組態ID]</td> 
   <td>輸入或對應您要檢查的組態ID。</td> 
  </tr> 
 </tbody> 
</table>

#### 刪除設定

此動作模組會刪除上限端點或節流設定。

如果已部署設定，則必須先解除部署該設定，然後才能將其刪除。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取設定型別]</td> 
   <td>選取您要刪除上限設定還是節流設定。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL組態ID]</td> 
   <td>輸入或對應您要刪除之設定的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### 取得設定

此動作模組會傳回由指定ID識別的上限或節流設定。 會傳回最新定義。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取設定型別]</td> 
   <td>選取您要擷取上限設定還是節流設定。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL組態ID]</td> 
   <td>輸入或對應您要擷取之設定的ID。</td> 
  </tr> 
 </tbody> 
</table>




### 封裝管理

* [建立套件](#create-a-package)
* [更新套件](#update-a-package)
* [刪除套裝](#delete-a-package)
* [查詢封裝](#look-up-a-package)
* [匯入套件](#import-a-package)
* [Publish a套件](#publish-a-package)
* [提交匯入](#submit-an-import)



#### 建立套件

此動作模組會建立多成品套件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名稱]</td> 
   <td>輸入或對應封裝的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL說明]</td> 
   <td>輸入或對應封裝的說明。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL到期日]</td> 
   <td>輸入或對應定義封裝到期日的時間戳記。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL封裝型別]</td> 
   <td>選取您要建立的封裝型別。<ul><li><p><b>完全</b></p>此套件將包含所有成品</p></li><li><p><b>部分</b></p><p>此套件將僅包含您新增的成品。 </p></li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL成品]</td> 
   <td>如果您正在建立部分封裝，請針對您想要新增的每個成品，按一下<b>新增成品</b>，並指定成品的識別碼、型別和標題。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source Sandbox]</td> 
   <td>輸入或對應沙箱的名稱和IMS組織ID，該沙箱包含您要套件包含的專案。</td> 
  </tr> 
 </tbody> 
</table>

#### 更新套件

此動作模組會從封裝新增或刪除成品，或更新封裝中繼資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取動作]</td> 
   <td>選取您要採取的動作。<ul><li><p><b>新增成品</b></p><p>針對您要新增的每個成品，按一下<b>新增成品</b>並指定成品的識別碼、型別和標題，然後輸入或對應封裝的到期日。 </p></li><li><p><b>刪除成品</b></p><p>針對您要刪除的每個成品，按一下<b>新增成品</b>，並指定成品的識別碼、型別和標題。 </p></li><li><p><b>更新中繼資料</b></p><p>輸入名稱、說明或來源沙箱名稱或IMS組織ID的新值。</p></li></ul></td> 
  </tr> 
 </tbody> 
</table>

#### 刪除套裝

此動作模組會刪除多成品封裝。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL封裝ID]</td> 
   <td>輸入或對應您要刪除之封裝的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### 查詢封裝

此動作模組會擷取指定封裝的詳細資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL封裝ID]</td> 
   <td>輸入或對應您要傳回詳細資訊之套件的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### 匯入套件

此動作模組會擷取指定目標沙箱中的衝突物件。 衝突的物件代表類似物件，這些物件已經存在於目標沙箱中。

您必須先發佈套件，才能匯入它。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL封裝ID]</td> 
   <td>輸入或對應您要匯入之套件的ID。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL Target sandbox]</td> 
   <td>輸入或對應您要匯入封裝的沙箱名稱。</td> 
  </tr> 
 </tbody> 
</table>

#### Publish a套件

您必須先發佈套件，才能匯入它。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL封裝ID]</td> 
   <td>輸入或對應您要發佈的套件ID。</td> 
  </tr> 
 </tbody> 
</table>

#### 提交匯入

在您檢閱衝突並提供替代之後，此動作模組會提交套件的匯入。 結果會以承載的形式提供，這會開始針對在承載中指定的目的地沙箱匯入作業。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL封裝ID]</td> 
   <td>輸入或對應您要發佈的套件ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名稱]</td> 
   <td>輸入或對應匯入工作的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL說明]</td> 
   <td>輸入或對應匯入工作的說明</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL （目的地沙箱）名稱]</td> 
   <td>輸入或對映您要為其提交匯入之沙箱的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL （目的地沙箱） IMS組織ID]</td> 
   <td>輸入或對應您要提交匯入之目標沙箱的Adobe IMS組織ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL (Source sandbox) ID]</td> 
   <td>輸入或對應包含您要發佈之套件的沙箱的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL (Source sandbox)型別]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL (Source sandbox)連結]</td> 
   <td>輸入或對應您要發佈的套件連結。</td> 
  </tr> 
 </tbody> 
</table>


<!--

### Artifact management

* [Copy artifacts synchronously](#copy-artifacts-synchronously)
* [Export artifacts asynchronously](#export-artifacts-asynchronously)
* [Import artifacts asynchronously](#import-artifacts-asynchronously)

#### Copy artifacts synchronously

This action module copies artifacts from a source sandbox into a destination sandbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for the new file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for the new file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination sandbox]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>For each artifact you want to copy, click <b>Add artifact</b> and continue to <a href="#artifact-fields" class="MCXref xref" >Artifact fields</a>.</td> 
  </tr> 
 </tbody> 
</table>

##### Artifact fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the artifact.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Enter or map the artifact type, such as <code>REGISTRY_SCHEMA<code> or <code>JOURNEY</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version]</td> 
   <td>Enter or map the visibility of the artifact. This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Enter or map the visibility (tenant or global). This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Found]</td> 
   <td>Select <b>Yes</b> if this item was found using a GET operation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tasks]</td> 
   <td>For each task you want to add, click <b>Add task</b> and fill in the following:
   <ul>
   <li><p><b>Method</b></p></li>
   <li><p><b>Action</b></p></li>
   <li><p><b>Using</b></p></li>
   <li><p><b>With</b></p></li>
   </ul>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>For each task you want to add, click <b>Add message</b> and fill in the following:
   <ul>
   <li><p><b>Status</b></p><p>Enter or map the status that this message represents, such as <code>ERROR</code>.</li>
   <li><p><b>Attempt</b></p><p>Enter or map the attempt number related to this message. This may be useful if different attempts produce different messages.</p></li>
   <li><p><b>Message</b></p><p>Enter or map the text of the message.</li>
   <li><p><b>Object</b></p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

#### Export Artifacts asynchronously

This action module exports artifacts from the specified sandbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td>Enter or map a name for the export file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Enter or map a description for the export file</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Artifacts]</td> 
   <td>For each artifact you want to export, click <b>Add artifact</b> and continue to <a href="#artifact-fields" class="MCXref xref" >Artifact fields</a>.</td> 
  </tr> 
 </tbody> 
</table>

##### Artifact fields

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the artifact.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Enter or map the artifact type, such as <code>REGISTRY_SCHEMA<code> or <code>JOURNEY</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Version]</td> 
   <td>Enter or map the visibility of the artifact. This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Visibility]</td> 
   <td>Enter or map the visibility (tenant or global). This applies only to Registry objects.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Found]</td> 
   <td>Select <b>Yes</b> if this item was found using a GET operation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tasks]</td> 
   <td>For each task you want to add, click <b>Add task</b> and fill in the following:
   <ul>
   <li><p><b>Method</b></p></li>
   <li><p><b>Action</b></p></li>
   <li><p><b>Using</b></p></li>
   <li><p><b>With</b></p></li>
   </ul>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>For each task you want to add, click <b>Add message</b> and fill in the following:
   <ul>
   <li><p><b>Status</b></p><p>Enter or map the status that this message represents, such as <code>ERROR</code>.</li>
   <li><p><b>Attempt</b></p><p>Enter or map the attempt number related to this message. This may be useful if different attempts produce different messages.</p></li>
   <li><p><b>Message</b></p><p>Enter or map the text of the message.</li>
   <li><p><b>Object</b></p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>



#### Import Artifacts asynchronously

This action module imports a snapshot containing artifacts.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Snapshot ID]</td> 
   <td>Enter or map the ID of the snapshot you want to import.</td> 
  </tr> 
 </tbody> 
</table>

-->

### 記錄管理

* [建立記錄](#create-a-record)
* [更新記錄](#update-a-record)
* [刪除記錄](#delete-a-record)
* [修補記錄](#patch-a-record)
* [取得記錄](#get-a-record)

#### 建立記錄

此動作模組會建立新的內容範本或內容片段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取內容型別]</td> 
   <td>選取您要建立內容範本還是內容片段。<ul><li><p><b>內容範本</b></p>繼續<a href="#template-fields" class="MCXref xref" >範本欄位</a>。</li><li><p><b>內容片段</b></p>繼續<a href="#fragment-fields" class="MCXref xref" >片段欄位</a>。</li></ul></td> 
  </tr> 
  </tbody> 
</table>

##### 範本欄位

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[！UICONTROL名稱]</td> 
   <td>輸入或對應此內容範本的名稱。</td> 
<tr> 
   <td role="rowheader">[！UICONTROL說明]</td> 
   <td>輸入或對應此內容範本的說明。</td> 
  </tr> 
<tr> 
   <td role="rowheader">[！UICONTROL型別]</td> 
   <td>選取您要建立的範本型別。</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL頻道]</td> 
   <td>選取此範本中包含的管道。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內容範本來源]</td> 
   <td>選取此範本的來源。</td>  
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL中繼資料]</td> 
   <td>若要在新範本中加入自訂屬性，請選取「新增中繼資料」，然後輸入或對應中繼資料的索引鍵和值。 對您要包含的每個自訂欄位重複此動作。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL電子郵件HTML]</td> 
   <td>輸入或對應此範本中包含之電子郵件的HTML。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL編輯器內容]</td> 
   <td>若要在電子郵件中包含自訂屬性，請選取「新增編輯器內容」，然後輸入或對應內容的索引鍵和值。 對您要包含的每個自訂欄位重複此動作。</td> 
  </tr> 
 </tbody> 
</table>

##### 片段欄位

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> <tr> 
   <td role="rowheader">[！UICONTROL名稱]</td> 
   <td>輸入或對應此內容片段的名稱。</td> 
<tr> 
   <td role="rowheader">[！UICONTROL說明]</td> 
   <td>輸入或對應此內容片段的說明。</td> 
  </tr> 
<tr> 
   <td role="rowheader">[！UICONTROL型別]</td> 
   <td>選取您要建立的範本型別。</td> 
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL頻道]</td> 
   <td>選取此範本中包含的管道。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內容片段來源]</td> 
   <td>選取此片段的來源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL中繼資料]</td> 
   <td>若要在新範本中加入自訂屬性，請選取「新增中繼資料」，然後輸入或對應中繼資料的索引鍵和值。 對您要包含的每個自訂欄位重複此動作。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內容]</td> 
   <td>輸入或對應片段的內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL編輯器內容]</td> 
   <td>若要在電子郵件中包含自訂屬性，請選取「新增編輯器內容」，然後輸入或對應內容的索引鍵和值。 對您要包含的每個自訂欄位重複此動作。</td> 
  </tr> 
 </tbody> 
</table>

#### 更新記錄

此動作模組會更新內容範本或片段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取內容型別]</td> 
   <td>選取您要更新上限設定還是節流設定。<ul><li><p><b>範本</b></p>如需欄位，請參閱本文章建立記錄一節中的<a href="#template-fields" class="MCXref xref" >範本欄位</a>。</li><li><p><b>片段</b></p>如需欄位，請參閱本文章建立記錄一節中的<a href="#fragment-fields" class="MCXref xref" >片段欄位</a>。</li></ul></td> 
  </tr> 
  </tbody> 
  </table>

#### 刪除記錄

此動作模組會刪除內容範本或內容片段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取內容型別]</td> 
   <td>選取您要刪除內容範本或內容片段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL範本/片段ID]</td> 
   <td>輸入或對應您要刪除之範本或片段的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### 修補記錄

此動作模組使用JSON指標格式的PATCH更新記錄

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取內容型別]</td> 
   <td>選取您是修補內容範本還是內容片段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL範本/片段ID]</td> 
   <td>輸入或對應您要修補之範本或片段的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL裝載資料]</td> 
   <td>若要將記錄新增至此修補程式的裝載： <ol><li>按一下<b>新增記錄</b>。</li><li>選取操作：新增、移除或取代。</li><li>在「路徑」欄位中，選取您要修正名稱或說明。</li><li> 在「從」欄位中，輸入或對應包含JSON指標值的字串。</li><li>在「值」欄位中，輸入要用於作業的值。</li></ol></td> 
  </tr> 
 </tbody> 
</table>

#### 取得記錄

此動作模組會傳回指定ID所識別的內容範本或內容片段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取內容型別]</td> 
   <td>選取您要擷取內容範本或內容片段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL範本/片段ID]</td> 
   <td>輸入或對應您要擷取之範本或片段的ID。</td> 
  </tr> 
 </tbody> 
</table>


### 訊息管理

* [觸發單一訊息執行](#trigger-a-unitary-message-execution)
* [觸發以對象為基礎的訊息](#trigger-an-audience-based-message)
* [檢查以對象為基礎的訊息的狀態](#check-the-status-for-audience-based-message)



#### 觸發單一訊息執行

此動作模組會向您指定的收件者觸發單一訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL請求ID]</td> 
   <td>輸入或對應與此訊息關聯之要求的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL促銷活動ID]</td> 
   <td>輸入或對應與此訊息相關聯之行銷活動的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL收件者]</td> 
   <td>針對您想要收到此郵件的每個收件者，按一下[新增收件者] <b></b>並輸入下列內容：
   <ul>
   <li><p><b>類型</b></p>選取<code>aep</code>。</li>
   <li><p><b>使用者 ID</b></p>輸入或對應收件者的Adobe Experience Platform設定檔識別碼。</li>
   <li><p><b>名稱空間</b></p>輸入或對應收件者的Adobe Experience Platform設定檔名稱空間。</li>
   <li><p><b>電子郵件地址</b></p></li>
   <li><p><b>行動電話號碼</b></p></li>
   <li><p><b>名字</b></p></li>
   <li><p><b>姓氏</b></p></li>
   <li><p><b>產品</b></p>輸入或對應與此訊息相關聯的產品。 這用於訊息內容中的動態變數替代。</li>
   </ul></td> 
  </tr> 
 </tbody> 
</table>

#### 觸發以對象為基礎的訊息

此動作模組會根據您指定的請求和促銷活動，觸發以對象為基礎的訊息的執行。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL請求ID]</td> 
   <td>輸入或對應與此訊息關聯之要求的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL促銷活動ID]</td> 
   <td>輸入或對應與此訊息相關聯之行銷活動的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL產品]</td> 
   <td>輸入或對應與此訊息相關聯的產品。 這用於訊息內容中的動態變數替代。</td> 
  </tr> 
 </tbody> 
</table>

#### 檢查以對象為基礎的訊息的狀態

此動作模組會檢查以對象為基礎的批次訊息的狀態。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL訊息執行ID]</td> 
   <td>輸入或對應您要檢查之訊息執行的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 狀態檢查

<!--* [Check service health](#check-service-health)-->
* [檢查匯入相依性](#check-the-import-dependencies)
* [檢查匯入工作的狀態](#check-the-status-of-an-import-job)

<!--

#### Check service health

This action module checks that the service represented by the connection is running.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions on creating a connection to [!DNL Adobe Journey Optimizer], see <a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >Create a connection to [!DNL Adobe Journey Optimizer]</a> in this article.</td> 
  </tr> 
 </tbody> 
</table>

-->

#### 檢查匯入相依性

此動作模組會檢查封裝成品的相關性。 這可讓您檢查您是否具有匯入套件成品的許可權。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL封裝ID]</td> 
   <td>輸入或對應您要檢查其許可權的套件ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Target sandbox]</td> 
   <td>輸入或對應您要匯入封裝的沙箱名稱。</td> 
  </tr> 
 </tbody> 
</table>

#### 檢查匯入工作的狀態

此動作模組會檢查匯入作業是成功還是失敗。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作ID]</td> 
   <td>輸入或對應您要擷取資料之作業的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [列出所有相依物件](#list-all-dependent-objects)
* [清單設定](#list-configurations)
* [列出匯出和匯入工作](#list-export-and-import-jobs)
* [列出封裝](#list-packages)
* [清單記錄](#list-records)

#### 列出所有相依物件

此搜尋模組會列出指定封裝中物件的所有相依物件

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL封裝物件]</td> 
   <td>對於封裝中要傳回相依物件的每個物件，按一下<b>新增物件</b>並輸入物件的名稱和型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL封裝ID]</td> 
   <td>輸入或對應您要列出其相依物件的封裝識別碼。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL Target sandbox]</td> 
   <td>輸入或對映沙箱的名稱，該沙箱包含您要列出其相依物件的套件。</td> 
  </tr> 
 </tbody> 
</table>

#### 清單設定

此動作模組會列出所有上限或節流設定。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取設定型別]</td> 
   <td>選取您要列出上限設定還是節流設定。</td> 
  </tr> 
 </tbody> 
</table>

#### 列出匯出和匯入工作

此搜尋模組會列出目前的匯出和匯入工作。 您可以使用查詢引數來篩選清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL傳回結果的最大數目]</td> 
      <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Order by]</td> 
      <td>選取要依建立日期或修改日期排序結果。</td>
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL查詢引數]</td> 
   <td>針對您要篩選依據的每個查詢引數，按一下<b>新增查詢引數</b>，然後選取欄位和運運算元，並輸入篩選的欄位值。</td> 
  </tr> 
 </tbody> 
</table>



#### 列出封裝

此搜尋模組會列出組織中的所有封裝。 您可以使用查詢引數來篩選清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始]</td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL傳回結果的最大數目]</td> 
      <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Order by]</td> 
      <td>選取要依建立日期或修改日期排序結果。</td>
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL查詢引數]</td> 
   <td>針對您要篩選依據的每個查詢引數，按一下<b>新增查詢引數</b>，然後選取欄位和運運算元，並輸入篩選的欄位值。</td> 
  </tr> 
 </tbody> 
</table>

#### 清單記錄

此搜尋模組會列出所有上限或節流設定。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選取內容型別]</td> 
   <td>選取您要擷取內容範本或內容片段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Order by]</td> 
   <td>輸入或對應您要以此清單排序的引數名稱。 新增<code>-</code>或<code>+</code>以遞減或遞增排序。 如果未指定符號，清單會遞減排序。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始]</td> 
   <td>此欄位用於分頁。 針對「排序依據」欄位中指定的屬性，輸入或對應下一頁的條件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Order by]</td> 
   <td>輸入或對應您要以此清單排序的引數名稱。 新增<code>-</code>或<code>+</code>以遞減或遞增排序。 如果未指定符號，清單會遞減排序。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL依屬性篩選]</td> 
   <td>針對您要新增的每個屬性篩選器，按一下<b>新增專案</b>並輸入屬性的索引鍵和值。 包含指定屬性值的記錄會包含在清單中。</td> 
  </tr> 
 </tbody> 
</table>


### 其他


#### 進行自訂API呼叫

此動作模組會對Adobe Journey Optimizer API發出自訂API呼叫。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td>如需建立[!DNL Adobe Journey Optimizer]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-journey-optimizer" class="MCXref xref" >建立與[!DNL Adobe Journey Optimizer]</a>的連線。</td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL]</td>
      <td>
        <p>輸入相對於基底URL的路徑。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標頭。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自動新增授權、<code>x-api-key</code>和<code>x-gw-ims-org-id</code>標頭。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL查詢字串]  </td>
      <td>
        <p>輸入請求查詢字串。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>







<!--

* [Check if configuration can be deployed](#check-if-configuration-can-be-deployed)
* [Check service health](#check-service-health)
* [Check the import dependencies](#check-the-import-dependencies)
* [Check the status for audience-based message](#status-for-audience-based-message)
* [Copy artifacts synchronously](#copy-artifacts-synchronously)
* [Create a configuration](#create-a-configuration)
* [Create a package](#create-a-package)
* [Create a record](#create-a-record)
* [Delete a configuration](#delete-a-configuration)
* [Delete a package](#delete-a-package)
* [Delete a record](#delete-a-record)
* [Deploy a configuration](#deploy-a-configuration)
* [Export artifacts asynchronously](#export-artifacts-asynchronously)
* [Get a configuration](#get-a-configuration)
* [Get a record](#get-a-record)
* [Import a package](#import-a-package)
* [Import artifacts asynchronously](#import-artifacts-asynchronously)
* [List all dependent objects](#list-all-dependent-objects)
* [List export and import jobs](#list-import-and-export-jobs)
* [Look up a package](#look-up-a-package)
* [Make a custom API call](#make-a-custom-api-call)
* [Patch a record](#patch-a-record)
* [Publish a package](#publish-a-package)
* [Submit an import](#submit-an-import)
* [Trigger a unitary message execution](#trigger-a-unitary-message-execution)
* [Trigger an audience-based message](#trigger-an-audience-based-message)
* [Undeploy a configuration](#undeploy-a-configuration)
* [Update a configuration](#update-a-configuration)
* [Update a package](#update-a-package)
* [Update a record](#update-a-record)
* [List configurations](#list-configurations)
* [List packages](#list-packages)
* [List records](#list-records)

-->
