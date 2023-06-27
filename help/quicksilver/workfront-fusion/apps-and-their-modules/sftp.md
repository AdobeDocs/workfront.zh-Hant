---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: sftp模組
description: 此 [!DNL Adobe Workfront Fusion SFTP] 模組可讓您監視所選資料夾/子資料夾中的檔案變更、將新檔案上傳到所需的資料夾、修改或刪除資料夾中已有的現有檔案，或變更檔案許可權。
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1931'
ht-degree: 0%

---

# sftp模組

此 [!DNL Adobe Workfront Fusion] SFTP模組可讓您監視選取的資料夾/子資料夾中的檔案變更、將新檔案上傳到所需的資料夾、修改或刪除資料夾中已有的現有檔案，或變更檔案許可權。

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

若要搭配使用SFTP [!DNL Workfront Fusion]，則必須擁有SFTP帳戶(例如 [!DNL GoDaddy] 網站託管)。

## 將SFTP連線至 [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

若要將您的SFTP帳戶連線至 [!DNL Workfront Fusion] 您必須輸入目標主機和模組的SFTP認證（使用者名稱和密碼或使用者名稱和金鑰） [!UICONTROL 建立連線] 對話方塊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線名稱]</td> 
   <td> <p> 輸入SFTP連線的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL主機]</p> </td> 
   <td> <p>輸入您要連線之SFTP伺服器的主機名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線埠] </td> 
   <td> <p>輸入SFTP伺服器連線埠。 例如， 22。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL驗證型別]</p> </td> 
   <td> <p>選取您要用來連線至SFTP伺服器的授權方法。</p> 
    <ul> 
     <li><strong>[！UICONTROL使用者名稱和密碼]</strong>：輸入您的認證。</li> 
     <li> <p><strong>[！UICONTROL使用者名稱和金鑰]</strong>：輸入您的使用者名稱和私密金鑰/憑證</p> <p>如果您想要使用自行簽署憑證的TLS，請上傳私密金鑰以使用使用者端授權，或上傳您的憑證（P12或PFX檔案）。 如果您使用使用者端憑證授權，可以在這裡輸入您的CA憑證。</p> <p>[!DNL Workfront Fusion] 不會保留或儲存您在這裡提供的任何資料（檔案、密碼）。 檔案和密碼僅用於擷取私密金鑰/憑證。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

輸入連線資訊後，按一下 **[!UICONTROL 繼續]** 以建立連線。

## [!UICONTROL SFTP] 模組及其欄位

當您設定 [!UICONTROL SFTP] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!UICONTROL SFTP] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 觸發器

#### [!UICONTROL 監看資料夾中的檔案]

在指定的資料夾中建立或變更檔案時，傳回包含詳細資訊的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td>
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>輸入或對應您要觀看的資料夾。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>緩衝區大小[B]</td> 
   <td> <p> 輸入緩衝區大小（位元組）。 值會定義從伺服器傳輸之區塊的大小。 當值太高時，某些伺服器可能會導致問題或檔案損毀。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳回檔案的最大數目]</td> 
   <td> <p> 設定檔案的最大數量 [!DNL Workfront Fusion] 將在一個週期內使用</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監視資料夾中的子資料夾]

在指定的資料夾中建立或變更資料夾時，傳回包含詳細資訊的資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td> 
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>輸入或對應您要觀看的資料夾。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳回檔案的最大數目]</td> 
   <td> <p> 設定符合以下條件的資料夾數目上限： [!DNL Workfront Fusion] 會在一個週期內傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

#### [!UICONTROL 列出資料夾的內容]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td>
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Show] </td> 
   <td> <p>選取您要擷取檔案、資料夾或兩者。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>輸入或對應包含您要列出之檔案或資料夾的資料夾。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋] </td> 
   <td> <p>輸入或對映搜尋字詞。 例如，如果您要搜尋副檔名為.txt的檔案，請輸入 <code>.txt</code>您也可以輸入或對應您要搜尋的檔案名稱。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排序依據]</td> 
   <td> <p> 選取您要依檔案名稱、大小、上次存取日期或上次修改日期來排序結果。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排序順序] </td> 
   <td> <p>選取結果應依遞增或遞減順序傳回。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL即使模組未傳回任何結果，仍繼續執行路由]</p> </td> 
   <td>啟用此選項，以確保此模組不會在未傳回任何結果時停止案例。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳回結果的最大數目]</td> 
   <td> <p> 設定符合以下條件的最大結果數量： [!DNL Workfront Fusion] 會在一個週期內傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

此模組會列出指定資料夾中的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td>
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL緩衝區大小[B]]</td> 
   <td> <p> 輸入緩衝區大小（位元組）。 值會定義從伺服器傳輸之區塊的大小。 當值太高時，某些伺服器可能會導致問題或檔案損毀。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>輸入或對應包含您要列出之檔案或資料夾的資料夾。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋] </td> 
   <td> <p>輸入或對映搜尋字詞。 例如，如果您要搜尋副檔名為.txt的檔案，請輸入 <code>.txt</code>您也可以輸入或對應您要搜尋的檔案名稱。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排序依據]</td> 
   <td> <p> 選取是否要依檔案名稱、大小、上次存取日期或上次修改日期來排序結果。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排序順序]</td> 
   <td> <p> 選取結果應依遞增或遞減順序傳回。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL即使模組未傳回任何結果，仍繼續執行路由]</p> </td> 
   <td>啟用此選項，以確保此模組不會在未傳回任何結果時停止案例。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳回結果的最大數目]</td> 
   <td> <p> 設定檔案的最大數量 [!DNL Workfront Fusion] 會在一個週期內傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

此模組會擷取檔案詳細資料，包括檔案的資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td>
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL緩衝區大小[B]]</td> 
   <td> <p> 輸入緩衝區大小（位元組）。 值會定義從伺服器傳輸之區塊的大小。 當值太高時，某些伺服器可能會導致問題或檔案損毀。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案路徑] </td> 
   <td> <p>輸入檔案的路徑。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳檔案]

此模組可讓您將檔案上傳至SFTP伺服器。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td>
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>指定現有的資料夾作為檔案的儲存位置。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL來源檔案]</td> 
   <td> <p> 從先前的模組對應來源檔案，例如[！UICONTROLDropbox] &gt; [！UICONTROL取得檔案]。 您也可以輸入或對應檔案名稱和檔案資料。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Permissions]</p> </td> 
   <td> <p>為檔案或資料夾設定所需的許可權。 使用chmod引數。 例如： <code>777 </code>或 <code>-rwxrwxrwx</code>.</p> <p>如需chmod的詳細資訊，請參閱 <a href="https://ss64.com/bash/chmod.html">chmod檔案</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重新命名檔案]

重新命名檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td>
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案路徑]</td> 
   <td> <p> 輸入要重新命名的檔案路徑。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL新檔案名稱]</td> 
   <td> <p> 輸入檔案的新名稱，包括副檔名。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動檔案]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td>
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案路徑]</td> 
   <td> <p> 輸入要移動的檔案路徑。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL新資料夾]</td> 
   <td> <p> 輸入檔案新位置的路徑。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td>
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案路徑]</td> 
   <td> <p> 輸入您要刪除的檔案路徑。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新檔案許可權]

可讓您變更檔案的許可權。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td>
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案路徑]</td> 
   <td> <p> 輸入要移動的檔案路徑。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Permissions]</p> </td> 
   <td> <p>設定所需的檔案許可權。 使用chmod引數。 例如， <code>777 </code>或 <code>-rwxrwxrwx</code>.</p> <p>必須符合模式 <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>如需chmod的詳細資訊，請參閱 <a href="https://ss64.com/bash/chmod.html">chmod檔案</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立資料夾]

在指定位置建立新資料夾。

>[!NOTE]
>
>如果資料夾已存在，模組將擲回錯誤。 若要繼續流程而不中斷，請將錯誤處理常式路由附加至模組以擷取錯誤，並採用 [!UICONTROL 繼續] 指示繼續流程。 如需有關附加錯誤處理常式路由的資訊，請參閱 [中的錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). 如需有關錯誤處理常式路由的資訊，請參閱 [中用於錯誤處理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td>
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>指定現有資料夾作為新資料夾的儲存位置。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾名稱]</td> 
   <td> <p> 輸入資料夾名稱。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Permissions]</p> </td> 
   <td> <p>設定所需的檔案夾許可權。 使用chmod引數。 例如， <code>777 </code>或 <code>-rwxrwxrwx</code>.</p> <p>必須符合模式 <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>如需chmod的詳細資訊，請參閱 <a href="https://ss64.com/bash/chmod.html">chmod線上手冊</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除資料夾]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線] </td>
   <td> <p>如需有關將SFTP帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> 指定您要刪除的資料夾路徑。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登入使用者特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
