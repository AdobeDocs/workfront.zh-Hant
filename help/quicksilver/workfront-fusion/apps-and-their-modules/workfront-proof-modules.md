---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Workfront校訂模組
description: 在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL Workfront Proof]，並連結至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: 614fd206ea2c5fe103beb5be8f5ff99c8a45a502
workflow-type: tm+mt
source-wordcount: '3099'
ht-degree: 0%

---

# [!DNL Workfront Proof] 模組

在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL Workfront Proof]，並連結至多個協力廠商應用程式和服務。

如果您需要執行校訂中目前不支援的任務，這將很有用 [!DNL Workfront] 或 [!DNL Workfront Proof]，例如根據特定事件更新校訂及搜尋校訂的收件者。

此 [!DNL Workfront Proof] 聯結器不會計入貴組織可用的作用中應用程式數量。 所有情境，即使只使用 [!DNL Workfront Proof] 應用程式，確實會針對貴組織的案例總數計算。

如果您需要有關建立情境的指示，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 工作自動化與整合]，請參閱[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
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

## 連線 [!DNL Workfront Proof] 至 [!DNL Workfront Fusion]

您可以建立與您的電腦的連線， [!DNL Workfront Proof] 直接從a內的帳戶 [!DNL Workfront Fusion] 模組。

1. 在任何 [!DNL Workfront Fusion] 模組，按一下 [!UICONTROL **新增**] 在 [!UICONTROL 連線] 欄位

2. 填寫下列欄位：

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[！UICONTROL連線名稱]</p>
                </td>
                <td>輸入連線的名稱</td>
            </tr>
            <tr>
                <td  role="rowheader">[！UICONTROL connections.environmentType]</td>
                <td>選取這是生產環境或非生產環境，例如預覽或沙箱。</td>
            </tr>
            <tr>
                <td role="rowheader">[！UICONTROL connections.authenticationType]</td>
                <td>選取這是服務帳戶還是個人帳戶。</td>
            </tr>
            <tr>
                <td  role="rowheader">[！UICONTROL電子郵件/使用者名稱]</td>
                <td>輸入您的使用者名稱 [!DNL Workfront Proof] 帳戶。</td>
            </tr>
            <tr>
                <td  role="rowheader">[！UICONTROL密碼]</td>
                <td>輸入您的密碼 [!DNL Workfront Proof] 帳戶。</td>
            </tr>
            <tr>
                <td  role="rowheader">[！UICONTROL租使用者ID]</td>
                <td><strong>注意</strong>：不使用BYOK的客戶必須將此欄位留空。 <p>輸入此帳戶的租使用者ID。 如果您需要協助尋找租使用者ID，請聯絡Workfront客戶支援。</p></td>
            </tr>
            <tr>
                <td role="rowheader">[！UICONTROL網域延伸模組]</td>
                <td>輸入您用來存取帳戶之URL的副檔名。 <p>範例： <code>com</code> 或 <code>eu</code></p></td>
            </tr>
            <tr>
                <td  role="rowheader">[！UICONTROL生產、預覽或自訂環境]</td>
                <td>選取與生產、預覽或自訂環境的連線。</td>
            </tr>
        </tbody>
    </table>


3. 按一下 [!UICONTROL **繼續**] 以儲存連線並返回模組

## [!DNL Workfront Proof] 模組及其欄位

當您設定 [!DNL Workfront Proof] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Workfront Proof] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

* [觀看校樣](#watch-proofs)
* [觀看PDF摘要](#watch-for-pdf-summary)
* [[!UICONTROL 觀看校訂活動]](#watch-proof-activity)

#### [!UICONTROL 觀看校樣]

當有人對校訂建立或做出決定時，此排程觸發模組會執行情境。

模組會傳回在指定期間找到的所有記錄清單，以及它們的型別。 它也會傳回您指定之欄位的值。 如果模組發現校訂上有決策，則會在個別欄位中同時包含先前和目前值。 您可以在情境中的後續模組中對應此資訊。

這會以您指定的定期排程間隔發生。

您必須有足夠的許可權可以存取中的校訂或校訂 [!DNL Workfront Proof] 以擷取此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">記錄類型</td> 
   <td>選擇型別 [!DNL Workfront Proof] 錄製您想要模組觀看的內容。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">輸出</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">限制</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看PDF摘要]

當有人為校訂建立PDF摘要時，此即時觸發模組會執行案例。

此模組需要webhook。

模組會傳回與校訂相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 它也會為PDF摘要建立新的事件訂閱，並輸出裝載中傳送之「pdf_url」屬性的內容。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Webhook]</td> 
   <td>您可以選取現有的webhook或建立新的webhook。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即時觸發器(webhook) [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看校訂活動]

此觸發模組會執行在校樣校樣上發生指定活動的情境。

模組會傳回與校訂相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 它也會為PDF摘要建立新的事件訂閱，並輸出以下來源的內容： `pdf_url` 在承載中傳送的屬性。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL活動型別]</td> 
   <td>選取您要觀看任何新決定（包括[！UICONTROL校訂]狀態變更），或僅整體校訂狀態變更。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 建立校訂]](#create-proof)
* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 下載校訂]](#download-proof)
* [[!UICONTROL 讀取記錄]](#read-a-record)
* [[!UICONTROL 請求PDF摘要]](#request-pdf-summary)
* [[!UICONTROL 更新校訂]](#update-proof)
* [[!UICONTROL 上傳檔案]](#upload-file)

#### [!UICONTROL 建立校訂]

此動作模組會在中建立新校訂或新版本的校訂 [!DNL Workfront Proof].

如果您要建立新版本，請指定新校訂和來源校訂的引數。

模組會傳回新校訂或校訂版本的ID。您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂型別]</td> 
   <td> <p>指定您希望建立的校訂具有基本工作流程還是[！UICONTROL自動化工作流程]。</p> <p>然後填寫針對您選擇的校樣型別顯示的欄位。 例如，如果您選擇[！UICONTROL自動化工作流程]，請填寫 <strong>[！UICONTROL工作流程階段]</strong> 欄位以設定階段。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL允許下載原始檔案]</td> 
   <td>選取您是否要允許下載建立校樣的原始檔案。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL Classic校訂檢視器]</td> 
   <td>選取您是否使用傳統校訂檢視器。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL將所有檔案合併為單一校訂]</td> 
   <td>啟用此選項可將所有檔案合併為單一多頁校訂。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL建立新校訂版本]</td> 
   <td>如果您希望模組建立現有校訂的新版本，請選取此選項。 然後，在 <strong>[！UICONTROL現有校訂ID]</strong> 顯示、對應或輸入校訂唯一ID的欄位。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自訂連結標籤]</td> 
   <td>輸入或對應自訂校樣連結的標籤。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自訂連結URL]</td> 
   <td>輸入或對應自訂連結的URL。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL訂閱者的預設電子郵件通知]</td> 
   <td>輸入下列其中一個數字，指出您要使用下列哪些預設電子郵件通知設定來建立校樣。
    <ul>
     <li><strong>1</strong>  — 所有新評論和回覆</li>
     <li><strong>2</strong>  — 回覆我的意見</li>
     <li><strong>3</strong>  — 每日摘要</li>
     <li><strong>4</strong>  — 每小時摘要</li>
     <li><strong>5</strong>  — 僅限決定</li>
     <li><strong>9</strong>  — 已停用</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL停用Excel摘要]</td> 
   <td>選取是否要停用將校訂評論下載到Excel檔案的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL停用PDF摘要]</td> 
   <td>選取是否要停用將校訂評論下載到PDF檔案的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL停用訂閱電子郵件]</td> 
   <td>選取是否要停用此校訂的訂閱電子郵件。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL啟用內嵌播放器]</td> 
   <td>選取是否要為此校訂啟用內嵌播放器。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL啟用訂閱]</td> 
   <td>選取是否允許非參與者人員訂閱校訂。<br>如果您選取此選項，也可以選取訂閱者的「預設角色」，如本表所述。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL啟用訂閱驗證]</td> 
   <td>選取是否要啟用訂閱電子郵件驗證。 如果已啟用，訂閱者必須按一下電子郵件中的連結來存取校訂。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL啟用團隊URL]</td> 
   <td>選取您要讓建立的校訂隱藏或顯示團隊URL。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL檔案雜湊] <span style="font-weight: normal;">或</span> [！UICONTROL檔案雜湊]</td> 
   <td>新增您要建立校樣的一個或多個檔案的ID。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL檔案名稱]</td> 
   <td>為建立的校訂新增檔案名稱或名稱。這是必填欄位。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL完成所有必要的決定時鎖定校訂]</td> 
   <td>指定您是否希望在做出所有必要的決定後鎖定建立的校訂。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL將此校訂通知收件者]</td> 
   <td>選取選項以指示您是否希望在建立校訂時通知收件者。&gt;</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂名稱]</td> 
   <td>輸入已建立校訂的名稱。這是必填欄位。 使用直立線符號(|)來分隔多個校訂的名稱。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂所有者ID]</td> 
   <td>輸入或對應校訂擁有者的ID。 如果此欄位留空，則校訂所有者將設定為目前使用者。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL參考ID]</td> 
   <td>輸入校訂的參考ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL需要電子簽章]</td> 
   <td>選擇您是否希望要求決定校訂的任何人提交電子簽章。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL需要登入]</td> 
   <td> <p>指定您是否希望建立的校訂需要登入。 </p> <p>此設定與中說明的[！UICONTROL需要登入]設定相同 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[！UICONTROL在中設定校訂設定] [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL解析度ID]</td> 
   <td>輸入您要用於校訂之解析度的ID。 如需解析度ID的清單，請參閱 [!DNL Workfront Proof] <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">API檔案</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROLSWF]</td> 
   <td>輸入SWF校訂的型別。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL Show] [item]</td> 
   <td>針對每個專案，選取是否要將其顯示在校樣中。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL工作區ID]</td> 
   <td>輸入您要在其中建立校訂的工作區ID。 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL收件者]</td> 
   <td>新增收件者的電子郵件地址，您已為建立的校訂提供所需的收件者。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL截止日期]</td> 
   <td> <p>指定您想對所建立校訂的截止日期。 使用以下日期格式：</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Workfront Proof] API。 如此一來，您就可以建立其他人無法完成的資料流程自動化 [!DNL Workfront Proof] 模組。

模組會傳回狀態代碼、標題和內文。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL方法]</td> 
   <td>設定API呼叫的動作。 如需瞭解可用的動作，請參閱 <a href="https://api.proofhq.com/">校訂API檔案</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL內文(XML)]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL 下載校訂]

此動作模組會下載您使用其ID識別的特定校訂的來源檔案。

您指定校訂的ID。

模組會傳回用於建立校訂之來源檔案的內容。您可以在情境中的後續模組中對應此資訊。

您必須有足夠的許可權才能存取中的記錄 [!DNL Workfront Proof] 以擷取此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂ID]</td> 
   <td> <p>輸入可在[！UICONTROL校訂詳細資訊]頁面上找到的校訂唯一ID。 如需詳細資訊，請參閱 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">在中管理校訂詳細資訊 [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組從中的單一校訂讀取資料 [!DNL Workfront Proof].

您可以指定校訂的ID以及您想要從校訂中取得的資訊。

模組會傳回您為校樣選擇的欄位值及其型別。 您可以在情境中的後續模組中對應此資訊。

您必須有足夠的許可權才能存取中的記錄 [!DNL Workfront Proof] 以擷取此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td>選取您要讀取校訂、校訂評論或校訂稽核者。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL輸出]</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td>輸入或對映唯一的 [!DNL Workfront Proof] 您希望模組讀取的記錄ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 請求PDF摘要]

此動作模組請求中特定校訂的PDF摘要 [!DNL Workfront Proof].

您指定校訂的ID。

模組會傳回PDF摘要資訊。 您可以在情境中的後續模組中對應此資訊。

您必須有足夠的許可權才能存取中的記錄 [!DNL Workfront Proof] 以擷取此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂ID]</td> 
   <td> <p>輸入唯一的 [!DNL Workfront Proof] 您要要求PDF摘要的校訂ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL回呼URL]</td> 
   <td>輸入或對應您想要傳送PDF摘要的URL。</td> 
  </tr> 
 </tbody> 
</table>

##### 可能的錯誤

* **錯誤**： &quot;[!UICONTROL 您沒有執行此要求的許可權。 此階段必須至少包含一個收件者。]&quot;
* **解決方案**：請確定您不是唯一一個指派給工作流程階段的人。 必須有另一個使用者被指派至工作流程的階段。

#### [!UICONTROL 更新校訂]

此動作模組會更新中的現有校訂 [!DNL Workfront Proof].

您可以指定校樣ID和記錄型別，以及要包含在輸出中的欄位。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

您必須有足夠的許可權才能存取中的記錄 [!DNL Workfront Proof] 以擷取此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂ID]</td> 
   <td> <p>輸入可在[！UICONTROL校訂詳細資訊]頁面上找到的校訂唯一ID。 如需詳細資訊，請參閱 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">在中管理校訂詳細資訊 [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL截止日期]</td> 
   <td> <p>指定您想對所建立校訂的截止日期。 使用以下日期格式：</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL訂閱者的預設電子郵件通知]</td> 
   <td>選取您要用於已建立校訂的下列預設電子郵件通知設定之一。
    <ul>
     <li> [！UICONTROL所有新評論和回覆]</li>
     <li>[！UICONTROL回覆我的意見]</li>
     <li>[！UICONTROL每日摘要]</li>
     <li> [！UICONTROL每小時摘要]</li>
     <li> [！UICONTROL Decisions only]</li>
     <li> [！UICONTROL已停用]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL預設角色]</td> 
   <td>選取校訂的預設角色。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL停用訂閱電子郵件]</td> 
   <td>選取是否要停用此校訂的訂閱電子郵件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL啟用訂閱]</td> 
   <td>選取是否允許非參與者人員訂閱校訂。<br>如果您選取此選項，也可以為訂閱者選取[！UICONTROL預設角色]，如本表所述。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL啟用訂閱驗證]</td> 
   <td>選取是否要啟用訂閱電子郵件驗證。 如果已啟用，訂閱者必須按一下電子郵件中的連結來存取校訂。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL啟用團隊URL]</td> 
   <td>選取您要讓建立的校訂隱藏或顯示團隊URL。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL完成所有必要的決定時鎖定校訂]</td> 
   <td>指定您是否希望在做出所有必要的決定後鎖定建立的校訂。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL訊息]</td> 
   <td>輸入或對應您要伴隨校訂的訊息。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂ID] </td> 
   <td>輸入或對應您要更新之校訂的ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂名稱]</td> 
   <td>輸入或對應您要更新的校訂名稱。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL需要登入]</td> 
   <td> <p>指定您是否希望建立的校訂需要登入。 </p> <p>此設定與中說明的[！UICONTROL需要登入]設定相同 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[！UICONTROL在中設定校訂設定] [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL顯示類似版本]</td> 
   <td>選取您是否想要顯示此校訂其他版本的連結。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主旨]</td> 
   <td>輸入或對映證明的主題</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳檔案]

此動作模組會上傳檔案以用於 [!UICONTROL 建立校訂] 中的模組 [!DNL Workfront Proof].

模組會傳回已上傳檔案的雜湊ID。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL來源檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 搜尋]](#search)
* [[!UICONTROL 列出工作流程範本]](#list-workflow-templates)

#### [!UICONTROL 搜尋]

此搜尋模組會在中尋找物件中的記錄 [!DNL Workfront Proof] 符合您指定的搜尋查詢。

如果正在搜尋校訂，模組會傳回校訂ID。 或者，如果正在搜尋收件者，它會傳回收件者的使用者ID、電子郵件、名稱、位置及電子郵件別名。您可以將此資訊對應至案例中的後續模組。

您必須有足夠的許可權才能存取中的記錄 [!DNL Workfront Proof] 以擷取此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>搜尋</td> 
   <td> <p>Se[！UICONTROL ]選取您要模組搜尋的記錄型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL校訂]</strong> </p> <p>輸入您要搜尋之校訂的校訂名稱。</p> </li> 
     <li> <p><strong>[！UICONTROL收件者]</strong> </p> <p>輸入您要搜尋之收件者的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL結果集]</td> 
   <td>指出模組是否會搜尋 <strong>[！UICONTROL所有相符記錄]</strong> 或僅限 <strong>[！UICONTROL第一個比對記錄]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL排序依據]</td> 
   <td>選取您要排序結果的欄位。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL排序方向]</td> 
   <td> <p>選取您要以遞增或遞減方式排序結果。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出工作流程範本]

此搜尋模組會列出所有可用的工作流程範本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Workfront Proof] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL輸出]</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大範本數量。</p> </td> 
  </tr> 
 </tbody> 
</table>
