---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: FTP模組
description: FTP模組可讓您監視所選資料夾中的檔案變更、將新檔案上傳至所需資料夾，以及修改或刪除資料夾中已有的現有檔案。
author: Becky
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1295'
ht-degree: 0%

---

# FTP模組

FTP模組可讓您監視所選資料夾中的檔案變更、將新檔案上傳至所需資料夾，以及修改或刪除資料夾中已有的現有檔案。

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

為了使用 [Fusion App] with [!DNL Workfront Fusion]，您必須有FTP帳戶。

## 在FTP模組中建立連線 {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接名]</td> 
   <td> <p> 輸入FTP連線的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主機] </td> 
   <td> <p>輸入FTP伺服器主機名稱。 E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL埠] </td> 
   <td> <p>輸入FTP伺服器埠號。 E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用戶名] </td> 
   <td> <p>輸入您的FTP帳戶使用者名稱。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL密碼] </td> 
   <td> <p>輸入您的FTP帳戶密碼。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>使用安全連線(TLS)</p> </td> 
   <td> <p>選擇是否要使用安全連接。</p> <p style="font-weight: bold;">[!UICONTROL否]</p> <p>連接未被保護。</p> <p style="font-weight: bold;">[!UICONTROL顯式加密或隱式加密]</p> <p>使用SSL保護連線。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL拒絕未授權的證書]</p> </td> 
   <td> <p>啟用此選項可驗證FTP伺服器憑證。 如果驗證失敗，將不建立連接。 若要通過驗證，憑證必須符合下列其中一項標準：</p> 
    <ul> 
     <li>由根簽名 <a href="https://en.wikipedia.org/wiki/Certificate_authority">證書頒發機構</a></li> 
     <li>由中級憑證授權單位簽署(請參閱 <a href="https://knowledge.digicert.com/solution/SO16297.html">憑證鏈如何運作</a> 以取得進一步解釋)。 在此情況下，FTP伺服器上應安裝所有中繼憑證。</li> 
     <li>是在[!UICONTROL自簽名證書]欄位中提供的自簽名證書（請參閱下文）</li> </ul>

如果停用此選項，則不會驗證FTP伺服器憑證。 我們強烈建議不要禁用該選項，因為它會使連接不安全，並帶來嚴重的安全風險。</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL自簽名證書]</p> </td> 
   <td> <p>按一下 <b>[!UICONTROL提取]</b> 按鈕以開啟「上載」對話框。</p> <p>上傳憑證以搭配您的自行簽署憑證使用TLS。 [!DNL Workfront Fusion] 不會保留或儲存您提供的任何資料，例如檔案和密碼。 檔案和密碼僅用於解壓憑證。</p> </td> 
  </tr> 
 </tbody> 
</table>

## FTP模組及其欄位

* [觸發器](#triggers)
* [動作](#actions)

### 觸發器

#### [!UICONTROL 監看檔案]

[!UICONTROL 監看檔案] 是FTP的唯一觸發模組。 它會監控所選資料夾的檔案內容。 將新檔案插入指定資料夾時，會執行觸發器。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>如需建立與FTP帳戶連線的指示，請參閱 <a href="#create-a-connection" class="MCXref xref">FTP模組中的[!UICONTROL建立連線]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL資料夾]</p> </td> 
   <td> <p>選擇要監視的資料夾。</p> <p><b>注意：</b> 每個案例僅允許一個資料夾。 會忽略子資料夾。</p> <p><b>提示：</b> 若要追蹤多個資料夾，請為每個資料夾建立獨立的案例。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回檔案的最大數] </td> 
   <td> <p>設定 [!DNL Workfront Fusion] 可在一個週期中運作。 如果值設定得太高，則指定的第三方服務（逾時）可能會中斷連線。 [!DNL Workfront Fusion] 對此沒有影響。 建議您設定較低的值，並為最大週期數定義較高的值，或更頻繁地執行藍本。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 變更權限]](#change-permissions)
* [[!UICONTROL 建立資料夾]](#create-a-folder)
* [[!UICONTROL 刪除檔案]](#delete-a-file)
* [[!UICONTROL 刪除資料夾]](#delete-a-folder)
* [[!UICONTROL 取得檔案]](#get-a-file)
* [[!UICONTROL 資料夾中的檔案清單]](#list-of-files-in-a-folder)
* [[!UICONTROL 移動檔案或資料夾]](#move-a-file-or-folder)
* [[!UICONTROL 上傳] 檔案](#upload-a-file)

#### [!UICONTROL 變更權限]

此動作模組會變更檔案或資料夾的權限設定。

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL連接]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">如需建立與FTP帳戶連線的指示，請參閱 <a href="#Create" class="MCXref xref" >FTP模組中的[!UICONTROL建立連線]</a> 這篇文章。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL更改權限設定]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>選擇是否要更改檔案或資料夾的設定。</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL檔案路徑]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">輸入或將檔案路徑映射到資料夾或檔案。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL權限]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>設定所需的檔案或資料夾權限。 使用chmod參數。 例如： <code>777 </code>或 <code>-rwxrwxrwx</code>.</p>
               <p>權限必須符合模式 <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code>.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL 建立資料夾]

此動作模組會建立新資料夾。

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL連接]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">如需建立與FTP帳戶連線的指示，請參閱 <a href="#Create" class="MCXref xref" >FTP模組中的[!UICONTROL建立連線]</a> 這篇文章。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL資料夾路徑]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">輸入檔案路徑或將其映射到新資料夾。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL新資料夾名稱]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>輸入或映射新資料夾的名稱。</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL 刪除檔案]

從指定的資料夾刪除檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">如需建立與FTP帳戶連線的指示，請參閱 <a href="#Create" class="MCXref xref" >FTP模組中的[!UICONTROL建立連線]</a> 這篇文章。</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選取您要從中刪除檔案的FTP資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案名]</td> 
   <td> <p> 輸入檔案名，包括副檔名。 範例: <code>[!DNL image].png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除資料夾]

此動作模組會永久刪除指定的資料夾。

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL連接]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">如需建立與FTP帳戶連線的指示，請參閱 <a href="#Create" class="MCXref xref" >FTP模組中的[!UICONTROL建立連線]</a> 這篇文章。</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL資料夾]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>選取您要從中刪除檔案的FTP資料夾。</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL 取得檔案]

從FTP伺服器擷取可進一步處理的檔案，例如上傳至 [!DNL Dropbox].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>如需建立與FTP帳戶連線的指示，請參閱 <a href="#creating-the-ftp-connection" class="MCXref xref">建立FTP連線</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL檔案路徑]</td> 
   <td> <p> 輸入要獲取的檔案的路徑。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 資料夾中的檔案清單]

擷取檔案和/或資料夾資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>如需建立與FTP帳戶連線的指示，請參閱 <a href="#creating-the-ftp-connection" class="MCXref xref">建立FTP連線</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選取您要搜尋的FTP資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL節目] </td> 
   <td> <p>選擇您要檢索有關檔案或資料夾的資訊，還是兩者。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索] </td> 
   <td> <p>輸入搜索詞。 如果未輸入搜索詞，則將檢索指定資料夾中的所有檔案和資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回檔案的最大數]</td> 
   <td> <p> 設定此模組檢索的檔案的最大數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動檔案或資料夾]

此動作模組會將檔案或資料夾移至不同位置。

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL連接]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">如需建立與FTP帳戶連線的指示，請參閱 <a href="#Create" class="MCXref xref" >FTP模組中的[!UICONTROL建立連線]</a> 這篇文章。</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL舊檔案路徑]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>輸入要移動檔案的路徑。 範例: <code>/folder1/document.txt</code>.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[!UICONTROL新檔案路徑]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>輸入要將檔案移至的路徑。 範例: <code>/folder2/document.txt</code>.</p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL 上傳檔案]

將檔案上傳至FTP伺服器。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td>如需建立與FTP帳戶連線的指示，請參閱 <a href="#creating-the-ftp-connection" class="MCXref xref">建立FTP連線</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選取要上傳檔案的FTP資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源檔案] </td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL附加到已存在的檔案]</td> 
   <td> <p>如果已啟用此選項，且FTP伺服器上已存在檔案，則檔案的內容會附加至現有檔案。 如果未啟用此選項，則會覆寫檔案的內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL如果不存在建立資料夾] </td> 
   <td> <p>如果已啟用此選項，且您在「資料夾」欄位中輸入的資料夾在FTP伺服器上不存在，則模組會建立資料夾</p> </td> 
  </tr> 
 </tbody> 
</table>

## 疑難排解 {#troubleshooting}

如果您在連線建立期間或模組作業期間遇到FTP應用程式問題，請嘗試使用其中一個常用的FTP用戶端，然後嘗試執行相同的動作（例如在資料夾中建立連線或清單檔案）。 與FTP用戶端。 如果您在FTP用戶端也遇到相同問題，可能是FTP伺服器的設定錯誤所致。
