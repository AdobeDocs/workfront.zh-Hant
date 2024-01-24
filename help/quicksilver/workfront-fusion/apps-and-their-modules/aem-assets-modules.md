---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets模組
description: 使用 [!DNL Adobe Experience Manager Assets] 的聯結器 [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] 帳戶、建立、上傳和更新資產，以及複製或行動資料夾和資產。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1543'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] 模組

使用 [!DNL Adobe Experience Manager Assets] 的聯結器 [!DNL Adobe Workfront Fusion]，您可以根據中的事件開始案例 [!DNL Adobe Experience Manager Assets] 帳戶、建立、上傳和更新資產，以及複製或行動資料夾和資產。

如需Adobe Experience Manager Assets聯結器的簡介，請參閱：

* [Adobe Experience Manager Assets](https://video.tv.adobe.com/v/3427034/){target=_blank}

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

## 先決條件

* 您必須擁有 [!DNL Adobe Experience Manager Assets] 帳戶以使用這些模組。
* 您必須設定 [!UICONTROL 伺服器對伺服器] 中的流量 [!DNL Adobe Developer console].

  如需設定的指示 [!UICONTROL 伺服器對伺服器] 中的流量 [!DNL Adobe Developer console]，請參閱 [為伺服器端API產生存取權杖](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## 連線 [!DNL Adobe Experience Manager Assets] 至 [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

若要為建立連線，請執行下列步驟： [!DNL Adobe Experience Manager Assets] 模組：

1. 按一下 [!UICONTROL 新增] 在 [!UICONTROL 連線] 方塊。

2. 選取要建立的連線型別：

   * **[!DNL AEM Assets as a Cloud Service]**

     此設定需要來自的資訊 [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]([!DNL Adobe Managed Services])**

     此設定需要使用者名稱和密碼。

3. 填寫您要建立之連線型別的欄位。

   的 [!DNL AEM Assets as a Cloud Service]，請參閱 [設定連線 [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   的 [!UICONTROL AEM Assets Basic] ([!DNL Adobe Managed Services])，請參閱 [設定連線 [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. 按一下 **[!UICONTROL 繼續]** 以儲存連線並返回模組。


### 設定連線 [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>這些欄位的資訊會在設定過程中產生 [!UICONTROL 伺服器對伺服器] 流量位於 [!DNL Adobe Developer Console]. 您可以在設定過程中產生的服務認證JSON檔案中找到這些值。
>
>如需設定的指示 [!UICONTROL 伺服器對伺服器] 流量位於 [!UICONTROL Adobe Developer Console]，請參閱 [為伺服器端API產生存取權杖](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[！UICONTROL連線名稱]</td>
                  <td>
                      <p>輸入此連線的名稱</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL執行個體URL，不含尾隨斜線]</td>
                  <td>輸入您的URL [!DNL Adobe Experience Manager] 執行個體。 請勿包含斜線 <code>/</code> 於URL結尾。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL使用者端ID]</td>
                  <td>輸入在[！UICONTROL伺服器對伺服器]安裝程式中產生的使用者端ID。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL使用者端密碼]</td>
                  <td>輸入在[！UICONTROL伺服器對伺服器]安裝程式中產生的使用者端密碼。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL技術帳戶ID]</td>
                  <td>輸入技術帳戶的ID。 這是使用者端憑證JSON檔案中的「[！UICONTROL id]」欄位。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL組織ID]</td>
                  <td class="">輸入組織的ID。 這是使用者端憑證JSON檔案中的「[！UICONTROL org]」欄位。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL中繼範圍]</td>
                  <td>輸入在[！UICONTROL伺服器對伺服器]安裝程式中產生的中繼範圍。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL私密金鑰]</td>
                  <td>輸入在[！UICONTROL伺服器對伺服器]安裝程式中產生的私密金鑰。 若要擷取私密金鑰，請按一下[！UICONTROL擷取]，然後輸入要擷取的檔案和檔案密碼。</td>
              </tr>
          </tbody>
      </table>


### 設定連線 [!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[！UICONTROL連線名稱]</td>
                <td>
                    <p>輸入此連線的名稱</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[！UICONTROL執行個體URL，不含尾隨斜線]</td>
                <td>輸入您的URL [!DNL Adobe Experience Manager] 執行個體。 請勿包含斜線 <code>/</code> 於URL結尾。</td>
            </tr>
            <tr>
                <td role="rowheader">[！UICONTROL使用者名稱]</td>
                <td>輸入的使用者名稱 [!DNL AEM Assets] 此連線使用的帳戶。</td>
            </tr>
            <tr>
                <td role="rowheader">[！UICONTROL密碼]</td>
                <td>輸入密碼 [!DNL AEM Assets] 此連線使用的帳戶。</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] 模組及其欄位

當您設定 [!DNL Adobe Experience Manager Essentials] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Adobe Experience Manager Essentials] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL 複製資料夾或資產]

此動作模組會將資料夾或資產複製到Adobe Experience Manager Assets帳戶中的其他位置。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Adobe Experience Manager Assets] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">連線 [!DNL Adobe Experience Manager Assets] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要複製資料夾還是資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾] / [！UICONTROL資產選擇]</td> 
   <td>選取或對應您要複製的資料夾或資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目的地路徑]</td> 
   <td>選取或將路徑對應到新資料夾或資產的位置。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL複製資料夾的名稱] / [！UICONTROL資產]</td> 
   <td>輸入新資料夾或資產的名稱。 在中顯示的資料夾名稱 [!DNL Adobe Experience Manager Assets] 與原始名稱相同。 此處輸入的名稱會出現在新資料夾或資產的URL中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL複製子項]</td> 
   <td>啟用此選項可複製資料夾中的任何子資料夾或資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL覆寫]</td> 
   <td>啟用此選項可覆寫目的地位置上與正在複製的資料夾或資產同名的任何資料夾或資產。</td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Adobe Experience Manager Assets] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">連線 [!DNL Adobe Experience Manager Assets] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL物件型別]</td> 
   <td> <p>選取您想要在資產上建立資料夾或註解。</p> 
    <ul> 
     <li> <p>[！UICONTROL資料夾]</p> <p>填寫下列欄位：</p> 
      <ul> 
       <li> <p>[！UICONTROL名稱]</p> <p>輸入資料夾的名稱。 此名稱會出現在檔案路徑中，因此不得包含空格或其他字元。 </p> </li> 
       <li> <p>[！UICONTROL標題]</p> <p>輸入資料夾的標題，該標題可顯示而非名稱。</p> </li> 
      </ul> </li> 
     <li> <p>[！UICONTROL資產註解]</p> <p>填寫下列欄位：</p> 
      <ul> 
       <li> <p>[！UICONTROL資產選擇]</p> <p>選取或對應您要新增註解的資產ID。</p> </li> 
       <li> <p>[！UICONTROL註解]</p> <p>輸入註解的文字。</p> </li> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Adobe Experience Manager Assets] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">連線 [!DNL Adobe Experience Manager Assets] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要刪除資料夾、資產或轉譯。</p> 
    <ul> 
     <li> <p>[！UICONTROL資料夾]</p> <p>選取資料夾路徑中的資料夾，以選取要刪除的資料夾。</p> </li> 
     <li> <p>[！UICONTROL資產] </p> <p>選取資產路徑中的資料夾，然後選取您要刪除的資產。</p> </li> 
     <li> <p>[！UICONTROL轉譯]</p> <p>選取轉譯路徑中的資料夾，以選取轉譯。</p> <p>輸入或對映轉譯的名稱。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 取得資料夾清單]

此動作模組會擷取現有資料夾及其子系實體（資料夾或資產）的表示法。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Adobe Experience Manager Assets] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">連線 [!DNL Adobe Experience Manager Assets] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td>選取或對應您要擷取的資料夾。 若要將子資料夾新增至路徑，請按一下加號圖示並選取子資料夾。</td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Adobe Experience Manager Assets] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">連線 [!DNL Adobe Experience Manager Assets] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於 [!DNL Adobe Experience Manager] 基礎URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串] </td> 
   <td> <p>輸入請求查詢字串。 對於每個索引鍵/值組，按一下 <b>[！UICONTROL新增專案]</b> 並輸入[！UICONTROL Key]和[！UICONTROL Value]。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 行動資料夾或資產]

此動作模組會將指定路徑的資產或資料夾移至新位置。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Adobe Experience Manager Assets] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">連線 [!DNL Adobe Experience Manager Assets] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要行動資料夾或資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾] / [！UICONTROL資產]</td> 
   <td>選取或對應您要移動的資料夾或資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目的地路徑]</td> 
   <td>選取或將路徑對應至您要行動資料夾或資產的位置。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL已行動資料夾的名稱] / [！UICONTROL資產]</td> 
   <td>為移動的資料夾或資產輸入新名稱。 在中顯示的資料夾名稱 [!DNL Adobe Experience Manager Assets] 與原始名稱相同。 此處輸入的名稱會顯示在行動資料夾或資產的URL中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL覆寫]</td> 
   <td>啟用此選項可覆寫目的地位置上與正在複製的資料夾或資產同名的任何資料夾或資產。</td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Adobe Experience Manager Assets] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">連線 [!DNL Adobe Experience Manager Assets] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要刪除資產中繼資料還是資產轉譯。</p> 
    <ul> 
     <li> <p>[！UICONTROL資產中繼資料]</p> 
      <ul> 
       <li> <p>選取您要更新中繼資料的資產。</p> </li> 
       <li> <p>輸入資產的新標題。</p> </li> 
      </ul> </li> 
     <li> <p>[！UICONTROL資產轉譯]</p> 
      <ul> 
       <li> <p>選取您要更新轉譯的資產。</p> </li> 
       <li> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 上傳資產]

此動作模組會將資產上傳至 [!DNL Adobe Experience Manager Assets] 帳戶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Adobe Experience Manager Assets] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">連線 [!DNL Adobe Experience Manager Assets] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目的地]</td> 
   <td> <p>選取您要上傳資產的檔案夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL來源檔案]</td> 
   <td>輸入或對應來源檔案的名稱和資料。</td> 
  </tr> 
 </tbody> 
</table>
