---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classic模組
description: 使用 [!DNL Adobe Campaign Classic] 模組，您可以啟動 [!DNL Adobe Workfront Fusion] 根據您設定之事件的案例 [!DNL Adobe Campaign Classic] 科目、建立、讀取或更新協定與其他記錄、使用您設定的條件搜尋記錄，以及上傳檔案。
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 455d439ec2a9034043cac2570851ab2f9fecc276
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 0%

---

# [!DNL Adobe Campaign Classic] 模組

使用 [!DNL Adobe Campaign Classic] 模組，您可以啟動 [!DNL Adobe Workfront Fusion] 根據您設定之事件的案例 [!DNL Adobe Campaign Classic] 帳戶、建立、讀取或更新記錄、使用您設定的條件搜尋記錄，以及執行自訂API呼叫。

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
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 連線 [!DNL Adobe Campaign Classic] 至 [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>我們強烈建議您建立伺服器對伺服器連線。 Adobe Campaign已更新其API，僅接受伺服器對伺服器連線。 如果您要連線至Campaign版本8或更新版本，請 **必須** 建立伺服器對伺服器連線。
>
>如需Campaign新連線需求的詳細資訊，請參閱 [Campaign技術運運算元移轉至Adobe Developer主控台](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) （在Campaign檔案中）。

1. 在任何 [!DNL Adobe Campaign Classic] 模組，按一下 **[!UICONTROL 新增]** 在 [!UICONTROL 連線] 欄位。
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
          <td>輸入您用來連線至您的裝置的基底URL [!DNL Adobe Campaign Classic] 執行個體。</td>
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
          <td>如果您要建立伺服器對伺服器連線，請輸入 [!DNL Adobe] [！UICONTROL使用者端識別碼]。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL使用者端密碼]</td>
          <td>如果您要建立伺服器對伺服器連線，請輸入 [!DNL Adobe] [！UICONTROL使用者端密碼]。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
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
1. 按一下 **[!UICONTROL 繼續]** 以建立連線並返回模組。

## [!DNL Adobe Campaign Classic] 模組及其欄位

當您設定 [!DNL Adobe Campaign Classic] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Adobe Campaign Classic] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

#### [!UICONTROL 觀看記錄]

此排程觸發模組會在記錄變更時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>有關建立與的連線的指示 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >建立與的連線 [!DNL Adobe Campaign Classic]</a> 本文章內容。</td> 
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
   <td>對於要包含在輸出中的每個自訂欄位，按一下 <b>[！UICONTROL新增]</b> 並輸入自訂欄位的名稱。</td> 
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

此動作模組會在中建立新記錄 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有關建立與的連線的指示 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >建立與的連線 [!DNL Adobe Campaign Classic]</a> 本文章內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資源]</td> 
   <td>選擇型別 [!DNL Adobe Campaign Classic] 您要建立的記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄位] </td> 
   <td>選取建立記錄時您想要設定值的欄位，然後填寫這些欄位的值。 欄位會依您選取的記錄型別而有所不同。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自訂欄位]</td> 
   <td> 對於您想要新增到新記錄的每個自訂欄位，按一下 <b>[！UICONTROL新增專案]</b> 並輸入或對應欄位的名稱和值。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 進行自訂API呼叫]

此模組會對 [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有關建立與的連線的指示 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >建立與的連線 [!DNL Adobe Campaign Classic]</a> 本文章內容。</td> 
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

此動作模組會從中刪除單一記錄 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有關建立與的連線的指示 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >建立與的連線 [!DNL Adobe Campaign Classic]</a> 本文章內容。</td> 
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

此動作模組會針對中的物件執行選取的動作 [!DNL Adobe Campaign Classic] API。

如需特定動作和欄位的詳細資訊，請參閱 [[!DNL Adobe Campaign] - API檔案](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有關建立與的連線的指示 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >建立與的連線 [!DNL Adobe Campaign Classic]</a> 本文章內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL動作]</td> 
   <td><p>選取要在物件上執行的動作。</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> 如需可用欄位，請參閱 <a href="#search" class="MCXref xref" >[！UICONTROL搜尋]</a> 本文章內容。 </p></li>
     <li><p><b>[！UICONTROL Get]</b></p><p> 如需可用欄位，請參閱 <a href="#search" class="MCXref xref" >[！UICONTROL搜尋]</a> 本文章內容。 </p></li> 
   <li><p><b>[！UICONTROL建立]</b></p><p> 如需可用欄位，請參閱 <a href="#create-a-record" class="MCXref xref" >[！UICONTROL建立記錄]</a> 本文章內容。 </p></li>
   <li><p><b>[！UICONTROL更新]</b></p><p> 如需可用欄位，請參閱 <a href="#update-record" class="MCXref xref" >[！UICONTROL更新記錄]</a> 本文章內容。 </p></li>
   <li><p><b>[！UICONTROL Delete]</b></p><p> 如需可用欄位，請參閱 <a href="#delete-record" class="MCXref xref" >[！UICONTROL刪除記錄]</a> 本文章內容。 </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組會從讀取記錄 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有關建立與的連線的指示 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >建立與的連線 [!DNL Adobe Campaign Classic]</a> 本文章內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資源]</td> 
   <td>選擇型別 [!DNL Adobe Campaign Classic] 您要讀取的記錄。</td> 
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
   <td>對於要包含在輸出中的每個自訂欄位，按一下 <b>[！UICONTROL新增]</b> 並輸入自訂欄位的名稱。</td> 
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
   <td>有關建立與的連線的指示 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >建立與的連線 [!DNL Adobe Campaign Classic]</a> 本文章內容。</td> 
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

此動作模組會更新中的單一記錄 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有關建立與的連線的指示 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >建立與的連線 [!DNL Adobe Campaign Classic]</a> 本文章內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資源]</td> 
   <td>選擇型別 [!DNL Adobe Campaign Classic] 您要建立的記錄。</td> 
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
   <td> 對於每個要更新的自訂欄位，按一下 <b>[！UICONTROL新增專案]</b> 並輸入或對應欄位的名稱和值。 </td> 
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
   <td>有關建立與的連線的指示 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >建立與的連線 [!DNL Adobe Campaign Classic]</a> 本文章內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資源]</td> 
   <td>選擇型別 [!DNL Adobe Campaign Classic] 您要建立的記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>
