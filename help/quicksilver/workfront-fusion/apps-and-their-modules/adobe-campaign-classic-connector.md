---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Campaign v7/v8模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1490'
ht-degree: 1%

---

# [!DNL Adobe Campaign]模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [Adobe Campaign模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/adobe-campaign-classic-connector.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

透過[!DNL Adobe Campaign]模組，您可以根據[!DNL Adobe Campaign v7/v8]帳戶中的事件啟動[!DNL Adobe Workfront Fusion]案例、建立、讀取或更新記錄、使用您設定的條件搜尋記錄，以及執行自訂API呼叫。

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

您必須將Fusion IP位址新增到[!DNL Adobe Campaign]。

* 如需將IP位址新增至您的Campaign允許清單的指示，請參閱Adobe Campaign檔案中的[將IP位址新增至允許清單](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list)。
* 如需新增至允許清單的IP位址清單，請參閱[用於存取Adobe Workfront Fusion的IP位址](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md)。

## Adobe Campaign API資訊

Adobe Campaign聯結器會使用以下專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v1.7.22</td> 
  </tr>
 </tbody> 
 </table>

## 將[!DNL Adobe Campaign]連線至[!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>我們強烈建議您建立伺服器對伺服器連線。 Adobe Campaign已更新其API，僅接受伺服器對伺服器連線。 如果您要連線至Campaign 8或更新版本，則&#x200B;**必須**&#x200B;建立伺服器對伺服器連線。
>
>如需有關Campaign新連線需求的詳細資訊，請參閱Campaign檔案中的[將Campaign技術運運算元移轉至Adobe Developer Console](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html)。

1. 在任何[!DNL Adobe Campaign]模組中，按一下[!UICONTROL 連線]欄位旁的&#x200B;**[!UICONTROL 新增]**。
1. 填寫下列欄位：
   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[！UICONTROL連線型別]</td>
          <td>
            <p>選擇您要建立基本連線還是伺服器對伺服器連線。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL連線名稱]</td>
          <td>
            <p>輸入此連線的名稱。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL基底URL]</td>
          <td>輸入您用來連線至[!DNL Adobe Campaign]執行個體的基底URL。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL使用者名稱]</td>
          <td>如果您要建立基本連線，請輸入您的Adobe Campaign使用者名稱。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL密碼]</td>
          <td>如果您要建立基本連線，請輸入您的Adobe Campaign密碼。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL使用者端ID]</td>
          <td>如果您正在建立伺服器對伺服器連線，請輸入您的[!DNL Adobe] [！UICONTROL使用者端ID]。 這可以在[!DNL Adobe Developer Console]的[！UICONTROL認證詳細資料]區段中找到。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL使用者端密碼]</td>
          <td>如果您正在建立伺服器對伺服器連線，請輸入您的[!DNL Adobe] [！UICONTROL使用者端密碼]。 這可以在[!DNL Adobe Developer Console]的[！UICONTROL認證詳細資料]區段中找到。
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL環境]</td>
          <td>選取您是連線至生產或非生產環境。
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL型別]</td>
          <td>選取您要連線到服務帳戶還是個人帳戶。
        </tr>
   </tbody>
    </table>
1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以建立連線並返回模組。

## [!DNL Adobe Campaign]模組及其欄位

當您設定[!DNL Adobe Campaign]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Adobe Campaign]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [觸發程序](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發程序

#### [!UICONTROL 觀看記錄]

此排程觸發模組會在記錄變更時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >建立與[!DNL Adobe Campaign]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td>選取您要監視新記錄、更新記錄或兩者。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資源]</td> 
   <td>選取您要監視的資源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">要包含在輸出中的[！UICONTROL欄位]</td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要包含在輸出中的自訂欄位]</td> 
   <td>對於要包含在輸出中的每個自訂欄位，按一下<b>[！UICONTROL新增]</b>並輸入自訂欄位的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL傳回結果的最大數目]</td> 
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>


### 動作

* [[!UICONTROL 建立記錄]](#create-a-record)
* [[!UICONTROL 進行自訂API呼叫]](#make-a-custom-api-call)
* [[!UICONTROL 刪除記錄]](#delete-record)
* [[!UICONTROL 執行動作]](#perform-an-action)
* [[!UICONTROL 讀取記錄]](#-read-a-record)
* [[!UICONTROL 訂閱或取消訂閱]](#subscribe-or-unsubscribe)
* [[!UICONTROL 更新記錄]](#update-record)

#### [!UICONTROL 建立記錄]

此動作模組會在[!DNL Adobe Campaign]中建立新記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >建立與[!DNL Adobe Campaign]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資源]</td> 
   <td>選取您要建立的[!DNL Adobe Campaign]記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄位] </td> 
   <td>選取建立記錄時您想要設定值的欄位，然後填寫這些欄位的值。 欄位會依您選取的記錄型別而有所不同。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自訂欄位]</td> 
   <td> 針對您想要新增至新記錄的每個自訂欄位，按一下<b>[！UICONTROL新增專案]</b>，然後輸入或對應欄位的名稱和值。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 進行自訂API呼叫]

此模組會對[!DNL Adobe Campaign] API發出自訂API呼叫

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >建立與[!DNL Adobe Campaign]</a>的連線。</td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL動作]</td>
      <td><p>選取您希望API呼叫執行的動作。</p>
      <p>[！UICONTROL執行查詢]</p>
      <p>[！UICONTROL寫入]</p>
      <p>[！UICONTROL Get entity if more recent]</p>
      <p>[！UICONTROL全選]</p>
      <p>[！UICONTROL推送事件]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標頭。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自動新增[！UICONTROL x-security]權杖標頭。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL XML Body]</td>
   <td> <p>以XML新增API呼叫的內文內容，而不使用工作階段元素。 </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會從[!DNL Adobe Campaign]刪除單一記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >建立與[!DNL Adobe Campaign]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資源]</td> 
   <td>選取您要刪除的資源型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入或對應您要刪除之資源的ID。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 執行動作]

此動作模組會對[!DNL Adobe Campaign] API中的物件執行選取的動作。

如需特定動作和欄位的詳細資訊，請參閱[[!DNL Adobe Campaign] - API檔案](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >建立與[!DNL Adobe Campaign]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL動作]</td> 
   <td><p>選取要在物件上執行的動作。</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> 如需可用欄位，請參閱本文中的<a href="#search" class="MCXref xref" >[！UICONTROL搜尋]</a>。 </p></li>
     <li><p><b>[！UICONTROL Get]</b></p><p> 如需可用欄位，請參閱本文中的<a href="#search" class="MCXref xref" >[！UICONTROL搜尋]</a>。 </p></li> 
   <li><p><b>[！UICONTROL建立]</b></p><p> 如需可用欄位，請參閱本文中的<a href="#create-a-record" class="MCXref xref" >[！UICONTROL建立記錄]</a>。 </p></li>
   <li><p><b>[！UICONTROL更新]</b></p><p> 如需可用欄位，請參閱本文中的<a href="#update-record" class="MCXref xref" >[！UICONTROL更新記錄]</a>。 </p></li>
   <li><p><b>[！UICONTROL Delete]</b></p><p> 如需可用欄位，請參閱本文中的<a href="#delete-record" class="MCXref xref" >[！UICONTROL刪除記錄]</a>。 </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組從[!DNL Adobe Campaign]讀取記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >建立與[!DNL Adobe Campaign]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資源]</td> 
   <td>選取您要讀取的[!DNL Adobe Campaign]記錄型別。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL ID] </td> 
   <td>輸入對應您要讀取之記錄的ID。</td> 
  </tr> 
 <tr> 
   <td role="rowheader">要包含在輸出中的[！UICONTROL欄位] </td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要包含在輸出中的自訂欄位]</td> 
   <td>對於要包含在輸出中的每個自訂欄位，按一下<b>[！UICONTROL新增]</b>並輸入自訂欄位的名稱。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 訂閱或取消訂閱]

此動作模組會訂閱資訊服務的使用者或取消訂閱資訊服務的使用者。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >建立與[!DNL Adobe Campaign]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL訂閱或取消訂閱]</td> 
   <td>選取您要訂閱或取消訂閱資訊服務。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL服務名稱]</td> 
   <td>選取您要訂閱或取消訂閱的服務。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL收件者電子郵件地址] </td> 
   <td>輸入或對應您要訂閱或取消訂閱資訊服務之使用者的電子郵件地址。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新記錄]

此動作模組更新[!DNL Adobe Campaign]中的單一記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >建立與[!DNL Adobe Campaign]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資源]</td> 
   <td>選取您要建立的[!DNL Adobe Campaign]記錄型別。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL ID] </td> 
   <td>輸入對應您要更新之記錄的ID。</td> 
  </tr> 
<tr> 
   <td role="rowheader">[！UICONTROL欄位] </td> 
   <td>選取您要更新值的欄位，然後填寫這些欄位的值。 欄位會依您選取的記錄型別而有所不同。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自訂欄位]</td> 
   <td> 針對您要更新的每個自訂欄位，按一下<b>[！UICONTROL新增專案]</b>，然後輸入或對應欄位的名稱和值。 </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

#### [!UICONTROL 搜尋]

此搜尋模組會根據指定的條件傳回記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >建立與[!DNL Adobe Campaign]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資源]</td> 
   <td>選取您要建立的[!DNL Adobe Campaign]記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>
