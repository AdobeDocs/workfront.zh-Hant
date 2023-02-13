---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets模組
description: 使用 [!DNL Adobe Experience Manager Assets] 連接器 [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] 帳戶、建立、上傳和更新資產，以及複製或移動資料夾和資產。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] 模組

使用 [!DNL Adobe Experience Manager Assets] 連接器 [!DNL Adobe Workfront Fusion]，您可以根據 [!DNL Adobe Experience Manager Assets] 帳戶、建立、上傳和更新資產，以及複製或移動資料夾和資產。

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

* 您必須有 [!DNL Adobe Experience Manager Assets] 帳戶來使用這些模組。
* 您必須設定 [!UICONTROL 伺服器對伺服器] 流量 [!DNL Adobe Developer console].

   有關設定的說明 [!UICONTROL 伺服器對伺服器] 流量 [!DNL Adobe Developer console]，請參閱 [產生伺服器端API的存取權杖](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

為 [!DNL Adobe Experience Manager Assets] 模組：

1. 按一下 [!UICONTROL 新增] 旁邊 [!UICONTROL 連線] 框。

2. 選取您要建立的連線類型：

   * **[!DNL AEM Assets as a Cloud Service]**

      此設定需要來自 [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]**

      此配置需要用戶名和密碼。

3. 填寫要建立的連接類型的欄位。

   針對 [!DNL AEM Assets as a Cloud Service]，請參閱 [為配置連接 [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   針對 [!UICONTROL AEM Assets基本]，請參閱 [為配置連接 [!UICONTROL AEM Assets基本]](#configure-the-connection-for-aem-assets-basic).

4. 按一下 **[!UICONTROL 繼續]** 以儲存連線並返回模組。


### 為配置連接 [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>這些欄位的資訊會在設定時產生 [!UICONTROL 伺服器對伺服器] 流量 [!DNL Adobe Developer Console]. 您可以在該設定期間產生的服務憑證JSON檔案中找到這些值。
>
>有關設定的說明 [!UICONTROL 伺服器對伺服器] 流量 [!UICONTROL Adobe Developer Console]，請參閱 [產生伺服器端API的存取權杖](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL連接名]</td>
                  <td>
                      <p>輸入此連接的名稱</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL實例URL（不帶尾斜線）]</td>
                  <td>輸入 [!DNL Adobe Experience Manager] 例項。 不包含斜線 <code>/</code> 填入。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL客戶端ID]</td>
                  <td>輸入在[!UICONTROL伺服器對伺服器]設定中生成的客戶端ID。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL客戶端密碼]</td>
                  <td>輸入在[!UICONTROL伺服器對伺服器]設定中生成的客戶端密碼。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL技術帳戶ID]</td>
                  <td>輸入技術帳戶的ID。 這是用戶端憑證JSON檔案中的「[!UICONTROL ID]」欄位。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL組織ID]</td>
                  <td class="">輸入組織ID。 這是用戶端認證JSON檔案中的「[!UICONTROL org]」欄位。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL元作用域]</td>
                  <td>輸入[!UICONTROL伺服器對伺服器]設定中生成的元作用域。</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL私鑰]</td>
                  <td>輸入在[!UICONTROL伺服器對伺服器]設定中生成的私鑰。 若要提取私密金鑰，請按一下[!UICONTROL提取]，然後輸入要提取的檔案以及該檔案的密碼。</td>
              </tr>
          </tbody>
      </table>


### 為配置連接 [!DNL AEM Assets Basic]

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL連接名]</td>
                <td>
                    <p>輸入此連接的名稱</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL實例URL（不帶尾斜線）]</td>
                <td>輸入 [!DNL Adobe Experience Manager] 例項。 不包含斜線 <code>/</code> 填入。</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL用戶名]</td>
                <td>輸入 [!DNL AEM Assets] 帳戶。</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL密碼]</td>
                <td>輸入 [!DNL AEM Assets] 帳戶。</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] 模組及其欄位

設定時 [!DNL Adobe Experience Manager Essentials] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Adobe Experience Manager Essentials] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL 複製資料夾或資產]

此動作模組會將資料夾或資產複製到Adobe Experience Manager Assets帳戶中的其他位置。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Adobe Experience Manager Assets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選取您要複製資料夾或資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾] / [!UICONTROL資產選擇]</td> 
   <td>選取或對應您要複製的資料夾或資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL目標路徑]</td> 
   <td>選取或將路徑對應至新資料夾或資產的位置。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL複製資料夾的名稱] / [!UICONTROL資產]</td> 
   <td>輸入新資料夾或資產的名稱。 顯示於 [!DNL Adobe Experience Manager Assets] 與原始名稱相同。 此處輸入的名稱會顯示在新資料夾或資產的URL中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL複製子項]</td> 
   <td>啟用此選項可複製資料夾內的任何子資料夾或資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL覆蓋]</td> 
   <td>啟用此選項可覆寫目標位置中與要複製的資料夾或資產同名的任何資料夾或資產。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 建立記錄]

此動作模組會建立資料夾或資產註解。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Adobe Experience Manager Assets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL對象類型]</td> 
   <td> <p>選取您要建立資料夾或對資產加上註解。</p> 
    <ul> 
     <li> <p>[!UICONTROL資料夾]</p> <p>填寫下列欄位：</p> 
      <ul> 
       <li> <p>[!UICONTROL名稱]</p> <p>輸入資料夾的名稱。 此名稱會出現在檔案路徑中，因此不得包含空格或其他字元。 </p> </li> 
       <li> <p>[!UICONTROL標題]</p> <p>輸入資料夾的標題，該標題可顯示，而非名稱。</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL資產注釋]</p> <p>填寫下列欄位：</p> 
      <ul> 
       <li> <p>[!UICONTROL資產選擇]</p> <p>選取或對應您要新增註解的資產ID。</p> </li> 
       <li> <p>[!UICONTROL注釋]</p> <p>輸入注釋的文本。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除記錄]

此動作模組會刪除資料夾、資產或轉譯。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Adobe Experience Manager Assets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選取您要刪除資料夾、資產或轉譯。</p> 
    <ul> 
     <li> <p>[!UICONTROL資料夾]</p> <p>通過在其路徑中選擇資料夾，選擇要刪除的資料夾。</p> </li> 
     <li> <p>[!UICONTROL資產] </p> <p>在資產路徑中選取資料夾，然後選取您要刪除的資產，以選取資產。</p> </li> 
     <li> <p>[!UICONTROL轉譯]</p> <p>在其路徑中選取資料夾，以選取轉譯。</p> <p>輸入或映射格式副本的名稱。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 獲取資料夾清單]

此動作模組會擷取現有資料夾及其子實體（資料夾或資產）的表示法。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Adobe Experience Manager Assets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td>選擇或映射要檢索的資料夾。 若要將子資料夾新增至路徑，請按一下加號圖示並選取子資料夾。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 進行自訂API呼叫]

此動作模組會對 [!DNL Adobe Experience Manager Assets] API。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Adobe Experience Manager Assets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於您 [!DNL Adobe Experience Manager] 基礎URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動添加授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串] </td> 
   <td> <p>輸入請求查詢字串。 針對每個索引鍵/值組，按一下 <b>[!UICONTROL添加項]</b> 並輸入[!UICONTROL鍵]和[!UICONTROL值]。</p> </td> 
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

### [!UICONTROL 移動資料夾或資產]

此動作模組會將指定路徑的資產或資料夾移至新位置。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Adobe Experience Manager Assets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選取您要移動資料夾或資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾] / [!UICONTROL資產]</td> 
   <td>選取或對應您要移動的資料夾或資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL目標路徑]</td> 
   <td>選取或對應路徑至您要移動資料夾或資產的位置。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL已移動資料夾的名稱] / [!UICONTROL資產]</td> 
   <td>輸入已移動資料夾或資產的新名稱。 顯示於 [!DNL Adobe Experience Manager Assets] 與原始名稱相同。 此處輸入的名稱會顯示在已移動資料夾或資產的URL中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL覆蓋]</td> 
   <td>啟用此選項可覆寫目標位置中與要複製的資料夾或資產同名的任何資料夾或資產。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新記錄]

此動作模組會更新現有記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Adobe Experience Manager Assets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選取您要刪除資產中繼資料或資產轉譯。</p> 
    <ul> 
     <li> <p>[!UICONTROL資產中繼資料]</p> 
      <ul> 
       <li> <p>選取您要更新中繼資料的資產。</p> </li> 
       <li> <p>輸入資產的新標題。</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset轉譯]</p> 
      <ul> 
       <li> <p>選取您要更新轉譯的資產。</p> </li> 
       <li> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 上傳資產]

此動作模組會將資產上傳至您的 [!DNL Adobe Experience Manager Assets] 帳戶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Adobe Experience Manager Assets] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL目標]</td> 
   <td> <p>選取您要上傳資產的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td>輸入或映射源檔案的名稱和資料。</td> 
  </tr> 
 </tbody> 
</table>
