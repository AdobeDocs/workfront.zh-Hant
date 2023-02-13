---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Workfront校樣模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Workfront Proof]，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: a79c6b2fb2b651987f973bc0d74e0eeea312c5bc
workflow-type: tm+mt
source-wordcount: '2886'
ht-degree: 0%

---

# [!DNL Workfront Proof] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Workfront Proof]，並將其連接至多個協力廠商應用程式和服務。

如果您需要執行內校對中目前不支援的任務，這個功能會很有幫助 [!DNL Workfront] 或 [!DNL Workfront Proof]，例如根據特定事件更新校樣並搜尋校樣的收件者。

此 [!DNL Workfront Proof] 連接器不會計入貴組織可用的作用中應用程式數量。 所有情況，即使它們僅使用 [!DNL Workfront Proof] 應用程式時，請確實計入貴組織的案例總數。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Workfront Proof] 模組及其欄位

設定時 [!DNL Workfront Proof] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Workfront Proof] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

* [監看校樣](#watch-proofs)
* [觀看PDF摘要](#watch-for-pdf-summary)
* [[!UICONTROL 監看校樣活動]](#watch-proof-activity)

#### [!UICONTROL 監看校樣]

此排程的觸發程式模組會在使用者建立或決定校樣時執行案例。

模組會傳回在您指定期間內找到的所有記錄清單及其類型。 它也會傳回您指定欄位的值。 如果模組發現對校樣做出的決定，則會在個別欄位中同時包含先前和目前的值。 您可以在案例的後續模組中對應此資訊。

這會以您指定的定期排程間隔進行。

您必須有足夠的權限才能存取中的校樣或校樣 [!DNL Workfront Proof] 以便檢索此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">記錄類型</td> 
   <td>選取 [!DNL Workfront Proof] 記錄您要讓模組觀看的項目。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">輸出</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">限制</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看PDF摘要]

此即時觸發模組會在有人建立校樣的PDF摘要時執行案例。

此模組中需要Webhook。

模組會傳回與校樣相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 它也會為PDF摘要建立新事件訂閱，並從裝載中傳送的「pdf_url」屬性輸出內容。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>您可以選取現有的網頁連結或建立新的網頁連結。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即時觸發器(Webhook) [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監看校樣活動]

此觸發器模組會在校樣校樣上發生指定的活動時執行案例。

模組會傳回與校樣相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 它也會為PDF摘要建立新事件訂閱，並輸出 `pdf_url` 屬性。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL活動類型]</td> 
   <td>選取您是要觀看任何新決策（包括[!UICONTROL校樣]狀態變更），還是只看整體校樣狀態變更。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 建立校訂]](#create-proof)
* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 下載校樣]](#download-proof)
* [[!UICONTROL 閱讀記錄]](#read-a-record)
* [[!UICONTROL 請求PDF摘要]](#request-pdf-summary)
* [[!UICONTROL 更新校樣]](#update-proof)
* [[!UICONTROL 上傳檔案]](#upload-file)

#### [!UICONTROL 建立校訂]

此動作模組會在中建立新校樣或新版本的校樣 [!DNL Workfront Proof].

如果要建立新版本，請指定新校樣的參數和源校樣。

該模組返回新校樣或校樣版本的ID。您可以在場景中的後續模組中映射此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣類型]</td> 
   <td> <p>指定您要建立的校樣具有基本工作流程還是[!UICONTROL自動化工作流程]。</p> <p>然後填寫您所選校樣類型所顯示的欄位。 例如，如果您選擇[!UICONTROL自動化工作流]，請填寫 <strong>[!UICONTROL工作流階段]</strong> 欄位來設定階段。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL允許下載原始檔案]</td> 
   <td>選擇是否允許下載建立校樣的原始檔案。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic校樣查看器]</td> 
   <td>選取您是否使用傳統校樣檢視器。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL將所有檔案合併為單一校樣]</td> 
   <td>啟用此選項可將所有檔案合併成單一多頁校樣。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL建立新校樣版本]</td> 
   <td>如果要讓模組建立現有校樣的新版本，請選取此選項。 然後，在 <strong>[!UICONTROL現有校樣ID]</strong> 欄位，可顯示、映射或輸入校樣的唯一ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自訂連結標籤]</td> 
   <td>輸入或對應自訂校樣連結的標籤。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自訂連結URL]</td> 
   <td>輸入或對應自訂連結的URL。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL訂閱者的預設電子郵件通知]</td> 
   <td>輸入下列數字之一，以指出您要用於所建立校樣的下列預設電子郵件通知設定。
    <ul>
     <li><strong>1</strong>  — 所有新評論和答復</li>
     <li><strong>2</strong>  — 對我評論的答復</li>
     <li><strong>3</strong>  — 每日摘要</li>
     <li><strong>4</strong>  — 每小時摘要</li>
     <li><strong>5</strong>  — 僅決策</li>
     <li><strong>9</strong>  — 已禁用</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL禁用Excel摘要]</td> 
   <td>選擇是否要禁用將校樣注釋下載到Excel檔案的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL禁用PDF摘要]</td> 
   <td>選擇是否要禁用將校樣注釋下載到PDF檔案的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL禁用訂閱電子郵件]</td> 
   <td>選取您是否要停用此校樣的訂閱電子郵件。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL啟用內嵌播放器]</td> 
   <td>選擇是否要為此校樣啟用嵌入式播放器。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL啟用訂閱]</td> 
   <td>選擇是否允許非參與者的人訂閱校樣。<br>如果選擇此選項，您也可以選擇訂閱者的預設角色，如此表所述。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL啟用訂閱驗證]</td> 
   <td>選擇是否要啟用訂閱電子郵件驗證。 如果已啟用此功能，訂閱者必須按一下電子郵件中的連結才能存取校樣。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL啟用團隊URL]</td> 
   <td>選擇是否要建立的校樣來隱藏或顯示團隊URL。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL檔案哈希] <span style="font-weight: normal;">或</span> [!UICONTROL檔案哈希]</td> 
   <td>新增您要建立校樣或校樣之檔案的ID。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL檔案名]</td> 
   <td>為已建立的校樣添加檔案名或名稱。這是必填欄位。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL在做出所有必要決策時鎖定校樣]</td> 
   <td>指定是否希望建立的校樣在做出所有必要決策後鎖定。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL通知收件者此校樣]</td> 
   <td>選取選項，以指出您是否要在建立校樣時通知收件者。&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣名稱]</td> 
   <td>輸入已建立校樣的名稱這是必填欄位。 使用垂直號(|)為多個校樣分隔名稱。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣所有者ID]</td> 
   <td>輸入或映射校樣擁有者的ID。 如果此欄位留空，則校樣擁有者會設為目前使用者。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL參考ID]</td> 
   <td>輸入校樣的參考ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL需要電子簽名]</td> 
   <td>選擇是否要求對證明做出決策的任何人提交電子簽名。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL需要登錄]</td> 
   <td> <p>指定您是否希望建立的校樣需要登入。 </p> <p>這與以下主題中說明的[!UICONTROL需要登入]設定相同： <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在 [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL解析度ID]</td> 
   <td>輸入要用於校樣的解析度ID。 如需解析度ID的清單，請參閱 [!DNL Workfront Proof] <a href="http://api.proofhq.com/home/objects/soapworkflowproofobject">API檔案</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROLSWF]</td> 
   <td>輸入SWF校樣類型。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Show] [item]</td> 
   <td>針對每個項目，選取是否要在校樣中顯示。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>輸入要在中建立校樣的工作區ID。 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL收件者]</td> 
   <td>新增您要收件者的電子郵件地址，以取得建立的校樣。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL截止日期]</td> 
   <td> <p>指定要建立校樣的截止時間。 使用下列日期格式：</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Workfront Proof] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Workfront Proof] 模組。

模組會傳回狀態代碼、標題和內文。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL方法]</td> 
   <td>設定API呼叫的動作。 如需可用動作，請參閱 <a href="http://api.proofhq.com/">證明API檔案</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL主體(XML)]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例:**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL 下載校樣]

此動作模組會下載您使用其ID識別之特定校樣的來源檔案。

您需指定校樣的ID。

該模組返回用於建立校樣的源檔案的內容。您可以在場景中的後續模組中映射此資訊。

您必須擁有足夠的權限才能存取 [!DNL Workfront Proof] 以便檢索此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣ID]</td> 
   <td> <p>輸入校樣的唯一ID，可在[!UICONTROL Proof Details]頁面上找到。 如需詳細資訊，請參閱 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">在中管理校樣詳細資料 [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 閱讀記錄]

此動作模組會從中的單一校樣讀取資料 [!DNL Workfront Proof].

您可以指定校樣的ID以及您要從校樣取得的資訊。

模組會傳回您為校樣選擇的欄位值及其類型。 您可以在案例的後續模組中對應此資訊。

您必須擁有足夠的權限才能存取 [!DNL Workfront Proof] 以便檢索此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄類型]</td> 
   <td>選擇您要閱讀校樣、校樣評論或校樣審核者。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL輸出]</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>輸入或對應唯一 [!DNL Workfront Proof] 您要模組讀取的記錄ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 請求PDF摘要]

此動作模組會要求中特定校樣的PDF摘要 [!DNL Workfront Proof].

您需指定校樣的ID。

模組返回PDF摘要資訊。 您可以在案例的後續模組中對應此資訊。

您必須擁有足夠的權限才能存取 [!DNL Workfront Proof] 以便檢索此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣ID]</td> 
   <td> <p>輸入唯一 [!DNL Workfront Proof] 您要為其請求PDF摘要的校樣ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL回呼URL]</td> 
   <td>輸入或對應您要傳送PDF摘要的URL。</td> 
  </tr> 
 </tbody> 
</table>

##### 可能的錯誤

* **錯誤**:&quot;[!UICONTROL 您沒有執行此請求的權限。 階段必須至少包含一個收件者。]&quot;
* **解決方案**:請確定您並非唯一指派給工作流程階段的人。 必須為工作流的各個階段分配另一個用戶。

#### [!UICONTROL 更新校樣]

此動作模組會更新 [!DNL Workfront Proof].

您可以指定校樣的ID和記錄類型，以及要在輸出中包含的欄位。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

您必須擁有足夠的權限才能存取 [!DNL Workfront Proof] 以便檢索此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣ID]</td> 
   <td> <p>輸入校樣的唯一ID，可在[!UICONTROL Proof Details]頁面上找到。 如需詳細資訊，請參閱 <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">在中管理校樣詳細資料 [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL截止日期]</td> 
   <td> <p>指定要建立校樣的截止時間。 使用下列日期格式：</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL訂閱者的預設電子郵件通知]</td> 
   <td>選取您要用於所建立校樣的下列預設電子郵件通知設定。
    <ul>
     <li> [!UICONTROL所有新評論和答復]</li>
     <li>[!UICONTROL對我評論的答復]</li>
     <li>[!UICONTROL每日摘要]</li>
     <li> [!UICONTROL每小時摘要]</li>
     <li> [！僅UICONTROL決策]</li>
     <li> [!UICONTROL已禁用]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL預設角色]</td> 
   <td>選擇校樣的預設角色。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL禁用訂閱電子郵件]</td> 
   <td>選取您是否要停用此校樣的訂閱電子郵件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL啟用訂閱]</td> 
   <td>選擇是否允許非參與者的人訂閱校樣。<br>如果選擇此選項，您也可以為訂閱者選擇[!UICONTROL預設角色]，如此表所述。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL啟用訂閱驗證]</td> 
   <td>選擇是否要啟用訂閱電子郵件驗證。 如果已啟用此功能，訂閱者必須按一下電子郵件中的連結才能存取校樣。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL啟用團隊URL]</td> 
   <td>選擇是否要建立的校樣來隱藏或顯示團隊URL。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL在做出所有必要決策時鎖定校樣]</td> 
   <td>指定是否希望建立的校樣在做出所有必要決策後鎖定。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL消息]</td> 
   <td>輸入或映射要隨校樣一起顯示的訊息。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣ID] </td> 
   <td>輸入或對應您要更新校樣的ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣名稱]</td> 
   <td>輸入或映射要更新的校樣的名稱。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL需要登錄]</td> 
   <td> <p>指定您是否希望建立的校樣需要登入。 </p> <p>這與以下主題中說明的[!UICONTROL需要登入]設定相同： <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在 [!DNL Workfront Proof]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL按贊顯示版本]</td> 
   <td>選取是否要顯示此校樣其他版本的連結。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主題]</td> 
   <td>輸入或映射校樣的主題</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳檔案]

此動作模組上傳檔案以與 [!UICONTROL 建立校樣] 模組 [!DNL Workfront Proof].

模組會傳回上傳檔案的雜湊ID。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源檔案]</td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 搜尋]](#search)
* [[!UICONTROL 清單工作流模板]](#list-workflow-templates)

#### [!UICONTROL 搜尋]

此搜尋模組會在 [!DNL Workfront Proof] 符合您指定的搜尋查詢。

如果模組正在搜尋校樣，則會傳回校樣的ID。 或者，如果它正在搜索收件人，則它會返回收件人的用戶ID、電子郵件、名稱、位置和電子郵件別名。您可以在方案的後續模組中映射此資訊。

您必須擁有足夠的權限才能存取 [!DNL Workfront Proof] 以便檢索此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>搜尋</td> 
   <td> <p>請參閱[!UICONTROL ]選擇要模組搜索的記錄類型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL校樣]</strong> </p> <p>輸入要搜索校樣的校樣名稱。</p> </li> 
     <li> <p><strong>[!UICONTROL收件人]</strong> </p> <p>輸入要搜索的收件人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL結果集]</td> 
   <td>指示模組是否將搜索 <strong>[!UICONTROL所有匹配記錄]</strong> 或 <strong>[!UICONTROL第一個匹配記錄]</strong>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL排序依據]</td> 
   <td>選擇要按結果排序的欄位。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL排序方向]</td> 
   <td> <p>選擇要遞增排序還是降序排序結果。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清單工作流模板]

此搜索模組列出所有可用的工作流模板。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>有關連接 [!DNL Workfront Proof] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL輸出]</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大模板數。</p> </td> 
  </tr> 
 </tbody> 
</table>
