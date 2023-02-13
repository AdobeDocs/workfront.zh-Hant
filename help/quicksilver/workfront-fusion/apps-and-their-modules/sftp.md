---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: SFTP模組
description: 此 [!DNL Adobe Workfront Fusion SFTP] 模組可讓您監視所選資料夾/子資料夾中的檔案更改、將新檔案上載到所需資料夾、修改或刪除資料夾中已存在的現有檔案，或更改檔案權限。
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 0%

---

# SFTP模組

此 [!DNL Adobe Workfront Fusion] SFTP模組允許您監視選定資料夾/子資料夾中的檔案更改、將新檔案上載到所需資料夾、修改或刪除資料夾中已存在的現有檔案或更改檔案權限。

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

若要搭配使用SFTP [!DNL Workfront Fusion]，則必須有SFTP帳戶(例如 [!DNL GoDaddy] 網站托管)。

## 將SFTP連線至 [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

將您的SFTP帳戶連線至 [!DNL Workfront Fusion] 您需要輸入目標主機和SFTP憑證（使用者名稱和密碼，或使用者名稱和金鑰）至模組的 [!UICONTROL 建立連線] 對話框。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接名]</td> 
   <td> <p> 輸入SFTP連線的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL主機]</p> </td> 
   <td> <p>輸入您要連線的SFTP伺服器的主機名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL埠] </td> 
   <td> <p>輸入SFTP伺服器埠。 例如22。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL驗證類型]</p> </td> 
   <td> <p>選取您要用來連線至SFTP伺服器的授權方法。</p> 
    <ul> 
     <li><strong>[!UICONTROL用戶名和密碼]</strong>:輸入您的憑證。</li> 
     <li> <p><strong>[!UICONTROL用戶名和密鑰]</strong>:輸入您的使用者名稱和私密金鑰/憑證</p> <p>如果您想使用自簽名憑證使用TLS，請上傳私密金鑰以使用用戶端授權，或上傳憑證（P12或PFX檔案）。 如果您使用用戶端憑證授權，您可以在此處輸入您的CA憑證。</p> <p>[!DNL Workfront Fusion] 不會保留或儲存您在此處提供的任何資料（檔案、密碼）。 檔案和密碼僅用於擷取私密金鑰/憑證。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

輸入連接資訊後，按一下 **[!UICONTROL 繼續]** 建立連接。

## [!UICONTROL SFTP] 模組及其欄位

設定時 [!UICONTROL SFTP] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!UICONTROL SFTP] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 觸發器

#### [!UICONTROL 監視資料夾中的檔案]

在指定的資料夾中建立或更改檔案時返回具有詳細資訊的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td>
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>輸入或映射要監視的資料夾。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>緩衝大小[B]</td> 
   <td> <p> 輸入緩衝區大小（以位元組為單位）。 值定義從伺服器傳輸的塊的大小。 當值過高時，某些伺服器可能會造成問題或損壞檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回檔案的最大數]</td> 
   <td> <p> 設定檔案數上限 [!DNL Workfront Fusion] 將在一個週期內運作</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 資料夾中的監視子資料夾]

在指定的資料夾中建立或更改資料夾時，返回包含詳細資訊的資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>輸入或映射要監視的資料夾。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回檔案的最大數]</td> 
   <td> <p> 設定資料夾數量上限 [!DNL Workfront Fusion] 會在一個週期中傳回。</p> </td> 
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
   <td>[!UICONTROL連接] </td>
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL節目] </td> 
   <td> <p>選擇要檢索檔案、資料夾還是兩者。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>輸入或映射包含要列出的檔案或資料夾的資料夾。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索] </td> 
   <td> <p>輸入或映射搜索詞。 例如，如果要搜索副檔名為.txt的檔案，請輸入 <code>.txt</code>.您也可以輸入或映射要搜索的檔案的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排序依據]</td> 
   <td> <p> 選擇要按檔案名、大小、上次訪問日期還是上次修改日期對結果進行排序。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排序順序] </td> 
   <td> <p>選擇應以升序還是降序返回結果。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL即使模組未返回任何結果，仍繼續執行路由]</p> </td> 
   <td>啟用此選項，以確保此模組不會在未傳回任何結果時停止案例。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回結果的最大數]</td> 
   <td> <p> 設定 [!DNL Workfront Fusion] 會在一個週期中傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 獲取檔案]

此模組會列出指定資料夾中的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td>
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL緩衝區大小[B]]</td> 
   <td> <p> 輸入緩衝區大小（以位元組為單位）。 值定義從伺服器傳輸的塊的大小。 當值過高時，某些伺服器可能會造成問題或損壞檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>輸入或映射包含要列出的檔案或資料夾的資料夾。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索] </td> 
   <td> <p>輸入或映射搜索詞。 例如，如果要搜索副檔名為.txt的檔案，請輸入 <code>.txt</code>.您也可以輸入或映射要搜索的檔案的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排序依據]</td> 
   <td> <p> 選擇要按檔案名、大小、上次訪問日期還是上次修改日期對結果進行排序。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排序順序]</td> 
   <td> <p> 選擇應以升序還是降序返回結果。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL即使模組未返回任何結果，仍繼續執行路由]</p> </td> 
   <td>啟用此選項，以確保此模組不會在未傳回任何結果時停止案例。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回結果的最大數]</td> 
   <td> <p> 設定檔案數上限 [!DNL Workfront Fusion] 會在一個週期中傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得檔案]

此模組會擷取檔案詳細資訊，包括檔案的資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td>
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL緩衝區大小[B]]</td> 
   <td> <p> 輸入緩衝區大小（以位元組為單位）。 值定義從伺服器傳輸的塊的大小。 當值過高時，某些伺服器可能會造成問題或損壞檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案路徑] </td> 
   <td> <p>輸入檔案的路徑。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./file.txt</code>.</p> </td> 
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
   <td>[!UICONTROL連接] </td>
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>指定現有資料夾作為檔案的儲存位置。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源檔案]</td> 
   <td> <p> 映射來自前一個模組的源檔案，如[!UICONTROLDropbox] &gt; [!UICONTROL獲取檔案]。 您也可以輸入或映射檔案名和檔案資料。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL權限]</p> </td> 
   <td> <p>為檔案或資料夾設定所需的權限。 使用chmod參數。 例如： <code>777 </code>或 <code>-rwxrwxrwx</code>.</p> <p>有關chmod的詳細資訊，請參閱 <a href="https://ss64.com/bash/chmod.html">chmod檔案</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重新命名檔案]

更名檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td>
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案路徑]</td> 
   <td> <p> 輸入要更名的檔案的路徑。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL新檔案名]</td> 
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
   <td>[!UICONTROL連接] </td>
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案路徑]</td> 
   <td> <p> 輸入要移動的檔案的路徑。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL新資料夾]</td> 
   <td> <p> 輸入檔案新位置的路徑。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除檔案]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td>
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案路徑]</td> 
   <td> <p> 輸入要刪除的檔案的路徑。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新檔案權限]

可讓您變更檔案的權限。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td>
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案路徑]</td> 
   <td> <p> 輸入要移動的檔案的路徑。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL權限]</p> </td> 
   <td> <p>設定所需的檔案權限。 使用chmod參數。 例如， <code>777 </code>或 <code>-rwxrwxrwx</code>.</p> <p>必須符合模式 <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>有關chmod的詳細資訊，請參閱 <a href="https://ss64.com/bash/chmod.html">chmod檔案</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立資料夾]

在指定位置中建立新資料夾。

>[!NOTE]
>
>如果資料夾已存在，模組將擲回錯誤。 為了繼續不間斷的流，請將錯誤處理程式路由附加到模組以捕獲錯誤並使用 [!UICONTROL 繼續] 指示繼續流。 有關附加錯誤處理程式路由的資訊，請參見 [錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). 有關錯誤處理程式路由的資訊，請參見 [錯誤處理指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td>
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>指定現有資料夾作為新資料夾的儲存位置。 您可以指定絕對路徑，例如 <code>/home/user/file.txt</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾名稱]</td> 
   <td> <p> 輸入資料夾名稱。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL權限]</p> </td> 
   <td> <p>設定所需的資料夾權限。 使用chmod參數。 例如， <code>777 </code>或 <code>-rwxrwxrwx</code>.</p> <p>必須符合模式 <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>有關chmod的詳細資訊，請參閱 <a href="https://ss64.com/bash/chmod.html">chmod手冊頁</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除資料夾]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td>
   <td> <p>如需將SFTP帳戶連線至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">將SFTP連線至 [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> 指定要刪除的資料夾的路徑。 您可以指定絕對路徑，例如 <code>/home/user/</code>. 或者，您可以指定指向登錄用戶的特定資料夾的相對路徑，例如 <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
