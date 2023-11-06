---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target模組
description: 在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] 模組可讓您建立、讀取、更新或刪除記錄、列出特定型別的所有記錄、根據您指定的條件搜尋記錄，或執行自訂API呼叫至 [!DNL Adobe Target] API。
author: Becky
feature: Workfront Fusion
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 51db439995430dad86e41190520824743216df69
workflow-type: tm+mt
source-wordcount: '2646'
ht-degree: 0%

---

# [!DNL Adobe Target] 模組

在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL Adobe Target]，並連結至多個協力廠商應用程式和服務。 [!DNL Adobe Target] 模組可讓您建立、讀取、更新或刪除記錄、列出特定型別的所有記錄、根據您指定的條件搜尋記錄，或執行自訂API呼叫至 [!DNL Adobe Target] API。


如果您需要有關建立情境的指示，請參閱 [建立情境](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
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
    </tr>
  </tbody>
</table>


若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

開始使用 [!DNL Adobe Target] 聯結器時，您必須確定符合下列先決條件：

* 您必須擁有使用中 [!DNL Adobe Target] 帳戶。

## 建立與的連線 [!DNL Adobe Target]

若要為建立連線，請執行下列步驟： [!DNL Adobe Target] 模組：

1. 按一下 **[!UICONTROL 新增]** ，位於「連線」方塊旁。

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
        <td role="rowheader">[！UICONTROL使用者端ID]</td>
        <td>輸入您的 [!DNL Adobe] 使用者端ID。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL使用者端密碼]</td>
        <td>輸入您的 [!DNL Adobe] 使用者端密碼。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL組織ID]</td>
        <td>輸入您的 [!DNL Adobe] 組織ID。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL技術帳戶ID]</td>
        <td>輸入您的 [!DNL Adobe] 技術帳戶ID。 您可在的[！UICONTROL憑證詳細資料]區段中找到 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL租使用者]</td>
        <td>
          <p> 若要尋找您的租使用者，請登入 [!DNL Adobe Experience Cloud]，開啟 [!DNL Target]，然後按一下 [!DNL Target] 卡片。 使用URL子網域中所述的租使用者ID值。</p>
          <p>例如，如果您在登入時的URL [!DNL Adobe Target] 是 <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> 則您的租使用者ID為「mycompany」。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL中繼範圍]</td>
        <td>輸入 <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL私密金鑰]</td>
        <td>
          <p>輸入在中建立您的認證時產生的私密金鑰 [!DNL Adobe Developer Console]. </p>
          <p>若要擷取您的私密金鑰或憑證：</p>
          <ol>
            <li value="1">
              <p>按一下 <b>[！UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>選取要解壓縮的檔案型別。</p>
            </li>
            <li value="3">
              <p>選取包含私密金鑰或憑證的檔案。</p>
            </li>
            <li value="4">
              <p>輸入檔案的密碼。</p>
            </li>
            <li value="5">
              <p>按一下 <b>[！UICONTROL儲存]</b> 以擷取檔案並返回連線設定。</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. 按一下 **[!UICONTROL 繼續]** 以儲存連線並返回模組。

## [!DNL Adobe Target] 模組及其欄位

當您設定 [!DNL Adobe Target] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Adobe Target] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [動作](#actions)

* [搜尋](#searches)


### 動作

* [[!UICONTROL 建立記錄]](#create-a-record)

* [[!UICONTROL 進行自訂API呼叫]](#make-a-custom-api-call)

* [[!UICONTROL 刪除記錄]](#delete-a-record)

* [[!UICONTROL 讀取記錄]](#read-a-record)

* [[!UICONTROL 更新記錄]](#update-a-record)


#### [!UICONTROL 建立記錄]

此動作模組會建立AB或XT活動、選件或對象。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[！UICONTROL Connection]</td>
    <td>有關建立與的連線的指示 [!DNL Adobe Target]，請參閱 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >建立與的連線 [!DNL Adobe Target]</a> 本文章內容。</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[！UICONTROL記錄型別]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>選取您要建立的記錄型別。</p>
      <ul>
        <li>
          <p>[！UICONTROL AB活動]</p>
          <p>繼續至 <a href="#ab-activity-fields" class="MCXref xref" >ab活動欄位</a>.</p>
        </li>
        <li>
          <p>[！UICONTROL XT活動]</p>
          <p>繼續至 <a href="#xt-activity-fields" class="MCXref xref" >XT活動欄位</a>.</p>
        </li>
        <li>
          <p>[！UICONTROL選件]</p>
          <p>繼續至 <a href="#offer-fields" class="MCXref xref" >選件欄位</a>.</p>
        </li>
        <li>
          <p>[！UICONTROL對象]</p>
          <p>繼續至 <a href="#audience-fields" class="MCXref xref" >對象欄位</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### ab活動欄位

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
      <td>輸入或對應此活動的名稱。 名稱不能超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Options]</td>
      <td>
        <p>針對您想要新增至活動的每個選項，按一下 <b>[！UICONTROL新增專案]</b> 並填入下列欄位：</p>
        <ul>
          <li>
            <p><b>[！UICONTROL選項本機ID]</b>
            </p>
            <p>輸入或對應要用於跨API請求追蹤選項的字串。</p>
          </li>
          <li>
            <p><b>[！UICONTROL名稱]</b>
            </p>
            <p>輸入或對映選項的名稱。 名稱不得超過250個字元。</p>
          </li>
          <li>
            <p><b>[！UICONTROL選件ID]</b>
            </p>
          </li>
          <li>
            <p>選取或對應與選項相關聯的優惠。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL位置]</td>
      <td>
        <p>針對您要新增至活動的每個Mbox，按一下 <b>[！UICONTROL新增專案]</b> 並填入下列欄位：</p>
        <ul>
          <li>
            <p>[！UICONTROL對象ID]</p>
            <p>針對您想要新增至Mbox的每個對象，按一下 <b>[！UICONTROL新增專案]</b> 並選取對象ID。</p>
          </li>
          <li>
            <p><b>[！UICONTROL位置本機ID]</b>
            </p>
            <p>輸入或對應要用來跨API請求追蹤位置的字串。</p>
          </li>
          <li>
            <p><b>[！UICONTROL名稱]</b>
            </p>
            <p>輸入或對應「位置」的名稱。 名稱不得超過250個字元。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL體驗]</td>
      <td>
        <p>頁面上提供內容選件的位置清單。 位置包含以下內容：
</p>
        <ul>
          <li>
            <p><b>[！UICONTROL體驗本機ID]</b>
            </p>
            <p>輸入或對映體驗的ID</p>
          </li>
          <li>
            <p><b>[！UICONTROL名稱]</b>
            </p>
            <p>輸入或對映體驗的名稱

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>針對您想檢視體驗的每個對象，按一下 <b>[！UICONTROL新增專案]</b> 並輸入對象ID。

</p>
          </li>
          <li>
            <p><b>[！UICONTROL訪客百分比]</b>
            </p>
            <p>輸入或對映分配至體驗的訪客百分比</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL第三方ID]</td>
      <td>輸入或對應ID以識別此活動。 您可以選擇此ID。 此ID不得與其他活動相同，且不得超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL開始於]</td>
      <td>以格式輸入或對應開始活動的日期和時間 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL結尾為]</td>
      <td>輸入或對應日期和時間，以使用格式結束活動 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL狀態]</td>
      <td>
        <p>輸入或對映活動的狀態。</p>
        <ul>
          <li>
            <p>[！UICONTROL已核准]</p>
          </li>
          <li>
            <p>[！UICONTROL已停用]</p>
          </li>
          <li>
            <p>[！UICONTROL已暫停]</p>
          </li>
          <li>
            <p>[！UICONTROL已儲存] </p>
          </li>
          <li>
            <p>[！UICONTROL已刪除]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL優先順序]</td>
      <td>輸入定義活動優先順序的數字。 數字越大，優先順序越高。 此值必須介於0到999之間。 預設值為5。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL自動分配流量]</td>
      <td>
        <p>啟用此選項以自動分配流量。 自動分配會將更多流量傳送到更成功的體驗。</p>
        <p>選取或對應評估標準，以判斷哪個體驗更成功。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Workspace]</td>
      <td>輸入或對應與活動相關聯的工作區</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL屬性ID] </td>
      <td>針對您想要新增至活動的每個屬性，按一下 <b>[！UICONTROL新增專案]</b> 並選取或對應屬性的ID。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[！UICONTROL報表受眾]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>針對您想要新增至活動的每個報表對象，按一下[！UICONTROL新增專案]並輸入下列資訊：</p>
        <ul>
          <li>
            <p><b>[！UICONTROL報表對象本機ID]</b>
            </p>
            <p>輸入或對應字串，用於跨API請求追蹤報表對象。</p>
          </li>
          <li>
            <p><b>[！UICONTROL對象ID]</b>
            </p>
            <p>輸入或對應要在報告中使用的區段</p>
          </li>
          <li>
            <p><b>[！UICONTROL量度本機ID]</b>
            </p>
            <p>輸入或對應字串，用於跨API請求追蹤量度。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### XT活動欄位

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
      <td>輸入或對應此活動的名稱。 名稱不能超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Options]</td>
      <td>
        <p>針對您想要新增至活動的每個選項，按一下 <b>[！UICONTROL新增專案]</b> 並填入下列欄位：</p>
        <ul>
          <li>
            <p><b>[！UICONTROL選項本機ID]</b>
            </p>
            <p>輸入或對應要用於跨API請求追蹤選項的字串。</p>
          </li>
          <li>
            <p><b>[！UICONTROL名稱]</b>
            </p>
            <p>輸入或對映選項的名稱。 名稱不得超過250個字元。</p>
          </li>
          <li>
            <p><b>[！UICONTROL選件ID]</b>
            </p>
          </li>
          <li>
            <p>選取或對應與選項相關聯的優惠。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL位置]</td>
      <td>
        <p>針對您要新增至活動的每個Mbox，按一下 <b>[！UICONTROL新增專案]</b> 並填入下列欄位：</p>
        <ul>
          <li>
            <p>[！UICONTROL對象ID]</p>
            <p>針對您想要新增至Mbox的每個對象，按一下 <b>[！UICONTROL新增專案]</b> 並選取對象ID。</p>
          </li>
          <li>
            <p><b>[！UICONTROL位置本機ID]</b>
            </p>
            <p>輸入或對應要用來跨API請求追蹤位置的字串。</p>
          </li>
          <li>
            <p><b>[！UICONTROL名稱]</b>
            </p>
            <p>輸入或對應「位置」的名稱。 名稱不得超過250個字元。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL體驗]</td>
      <td>
        <p>頁面上提供內容選件的位置清單。 位置包含以下內容：
</p>
        <ul>
          <li>
            <p><b>[！UICONTROL體驗本機ID]</b>
            </p>
            <p>輸入或對映體驗的ID</p>
          </li>
          <li>
            <p><b>[！UICONTROL名稱]</b>
            </p>
            <p>輸入或對映體驗的名稱

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>針對您想檢視體驗的每個對象，按一下 <b>[！UICONTROL新增專案]</b> 並輸入對象ID。

</p>
          </li>
          <li>
            <p><b>[！UICONTROL訪客百分比]</b>
            </p>
            <p>輸入或對映分配至體驗的訪客百分比</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Metrics]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL第三方ID]</td>
      <td>輸入或對應ID以識別此活動。 您可以選擇此ID。 此ID不得與其他活動相同，且不得超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL開始於]</td>
      <td>以格式輸入或對應開始活動的日期和時間 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL結尾為]</td>
      <td>輸入或對應日期和時間，以使用格式結束活動 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL狀態]</td>
      <td>
        <p>輸入或對映活動的狀態。</p>
        <ul>
          <li>
            <p>[！UICONTROL已核准]</p>
          </li>
          <li>
            <p>[！UICONTROL已停用]</p>
          </li>
          <li>
            <p>[！UICONTROL已暫停]</p>
          </li>
          <li>
            <p>[！UICONTROL已儲存] </p>
          </li>
          <li>
            <p>[！UICONTROL已刪除]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL優先順序]</td>
      <td>輸入定義活動優先順序的數字。 數字越大，優先順序越高。 此值必須介於0到999之間。 預設值為5。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL自動分配流量]</td>
      <td>
        <p>啟用此選項以自動分配流量。 自動分配會將更多流量傳送到更成功的體驗。</p>
        <p>選取或對應評估標準，以判斷哪個體驗更成功。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Workspace]</td>
      <td>輸入或對應與活動相關聯的工作區</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL屬性ID] </td>
      <td>針對您想要新增至活動的每個屬性，按一下 <b>[！UICONTROL新增專案]</b> 並選取或對應屬性的ID。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[！UICONTROL報表受眾]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>針對您想要新增至活動的每個報表對象，按一下[！UICONTROL新增專案]並輸入下列資訊：</p>
        <ul>
          <li>
            <p><b>[！UICONTROL報表對象本機ID]</b>
            </p>
            <p>輸入或對應字串，用於跨API請求追蹤報表對象。</p>
          </li>
          <li>
            <p><b>[！UICONTROL對象ID]</b>
            </p>
            <p>輸入或對應要在報告中使用的區段</p>
          </li>
          <li>
            <p><b>[！UICONTROL量度本機ID]</b>
            </p>
            <p>輸入或對應字串，用於跨API請求追蹤量度。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### 選件欄位

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
      <td>輸入或對應此活動的名稱。 名稱不能超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL內容]</td>
      <td>
        <p>輸入或對應要向使用者顯示的優惠方案內容。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Workspace]</td>
      <td>
        <p>輸入或對應與選件相關聯之工作區的ID。 如果保留為空白，選件會與帳戶的預設工作區相關聯。 此功能僅適用於 [!DNL Target] Premium帳戶。</p>
      </td>
    </tr>
  </tbody>
</table>

##### 對象欄位

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
      <td>輸入或對應此對象的名稱。 名稱不能超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL內容]</td>
      <td>
        <p>輸入或對應此對象的說明。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目標規則]</td>
      <td>
        <p>啟用切換即可讓規則變成必須套用所有規則的AND。</p>
        <p>針對您想要套用至對象的每個規則，按一下 <b>[！UICONTROL新增專案]</b> 並輸入您要套用之規則的JSON。 </p>
        <div class="example"><span class="autonumber"><span><b>範例: </b></span></span>
          <p>範例:</p>
          <p ><code>&lbrace;</code></p>
                    <p ><code>                "page": "url",</code>
                    </p>
                    <p><code>                "equals":&lbrack;</code>
                    </p>
                    <p ><code>                    "http://www.myhomepage.com/"</code>
                    </p>
                    <p><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;,</code>
                    </p>
                    <p ><code>            &lbrace;</code>
                    </p>
                    <p><code>                "geo": "region",</code>
                    </p>
                    <p><code>                "matches": &lbrack;</code>
                    </p>
                    <p ><code>                    "california"</code>
                    </p>
                    <p ><code>                &rbrack;</code>
                    </p>
                    <p ><code>            &rbrace;</code>
                    </p>
      </td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[！UICONTROL Workspace]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>輸入或對應與對象相關聯之工作區的ID。 如果保留為空白，選件會與帳戶的預設工作區相關聯。 此功能僅適用於 [!DNL Target Premium] 帳戶。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 進行自訂API呼叫]

此模組會對 [!DNL Adobe Target] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Target]，請參閱 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >建立與的連線 [!DNL Adobe Target]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL [!DNL Target] 基礎URL]</td>
      <td>輸入或對應 [!DNL Target] 基礎URL。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL路徑]</p>
      </td>
      <td>
        <p>輸入相對於 {baseURL}/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標頭。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自動新增授權標頭和x-api-key標頭。</p>
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
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除單一AB活動、XT活動、選件或對象。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[！UICONTROL Connection]</td>
    <td>有關建立與的連線的指示 [!DNL Adobe Target]，請參閱 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >建立與的連線 [!DNL Adobe Target]</a> 本文章內容。</td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL記錄型別]</td>
    <td>選取您要刪除的記錄型別。</td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL記錄ID]</td>
    <td>輸入或對應您要刪除之記錄的ID。</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL 讀取記錄]

此動作模組會擷取單一活動、選件、對象、屬性或報表的資料。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[！UICONTROL Connection]</td>
    <td>有關建立與的連線的指示 [!DNL Adobe Target]，請參閱 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >建立與的連線 [!DNL Adobe Target]</a> 本文章內容。</td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL記錄型別]</td>
    <td>選取您要讀取的記錄型別。</td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL記錄ID]</td>
    <td>輸入或對應您要讀取之記錄的ID。</td>
  </tr>
</tbody>
</table>

#### [!UICONTROL 更新記錄]

此動作模組會更新活動、選件或對象。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Target]，請參閱 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >建立與的連線 [!DNL Adobe Target]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL記錄型別]</td>
      <td>
        <p>選取您要更新的記錄型別。</p>
        <ul>
          <li>
            <p><b>[！UICONTROL AB活動]</b>
            </p>
            <p>請參閱中的欄位說明 <a href="#ab-activity-fields" class="MCXref xref" >ab活動欄位</a> 在 <a href="#create-a-record" class="MCXref xref" >建立記錄</a>.</p>
          </li>
          <li>
            <p><b>[！UICONTROL XT活動]</b>
            </p>
            <p>請參閱中的欄位說明 <a href="#xt-activity-fields" class="MCXref xref" >XT活動欄位</a> 在 <a href="#create-a-record" class="MCXref xref" >建立記錄</a>.</p>
          </li>
          <li>
            <p><b>[！UICONTROL其他活動]</b>
            </p>
            <p>選取您要更新值的欄位，然後輸入欄位的新值。</p>
          </li>
          <li>
            <p><b>[！UICONTROL選件]</b>
            </p>
            <p>請參閱中的欄位說明 <a href="#offer-fields" class="MCXref xref" >選件欄位</a> 在 <a href="#create-a-record" class="MCXref xref" >建立記錄</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>請參閱中的欄位說明 <a href="#audience-fields" class="MCXref xref" >對象欄位</a> 在 <a href="#create-a-record" class="MCXref xref" >建立記錄</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL記錄ID]</td>
      <td>輸入或對應您要更新的記錄ID。</td>
    </tr>
  </tbody>
</table>

### 搜尋

* [[!UICONTROL 取得記錄]](#get-records)

* [[!UICONTROL 搜尋]](#search)


#### [!UICONTROL 取得記錄]

此搜尋模組會擷取所選型別的記錄清單。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Target]，請參閱 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >建立與的連線 [!DNL Adobe Target]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL記錄型別]</td>
      <td>選取您要更新的記錄型別。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL排序依據]</td>
      <td>針對您要排序的每個欄位，按一下 <b>[！UICONTROL新增專案]</b> 並選取欄位，以及傳回的結果應為遞增還是遞減。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL開始於]</td>
      <td>
        <p>輸入您要擷取記錄的最早日期。 </p>
        <p>如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">輸入強制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL結尾為]</td>
      <td>
        <p>輸入您要擷取記錄的最晚日期。 </p>
        <p>如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">輸入強制 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 搜尋]

此搜尋模組會根據您指定的條件搜尋活動、選件或對象。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[！UICONTROL Connection]</td>
    <td>有關建立與的連線的指示 [!DNL Adobe Target]，請參閱 <a href="#create-a-connection-to-adobe-target" class="MCXref xref" >建立與的連線 [!DNL Adobe Target]</a> 本文章內容。</td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL記錄型別]</td>
    <td>選取您要更新的記錄型別。</td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL排序依據]</td>
    <td>針對您要排序的每個欄位，按一下 <b>[！UICONTROL新增專案]</b> 並選取欄位，以及傳回的結果應為遞增還是遞減。</td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL搜尋條件]</td>
    <td>針對您要設定的每個規則，選取欄位、運運算元和值。 按一下 <b>[！UICONTROL新增和規則]</b> 以建立其他規則。</td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL位移]</td>
    <td>
      <p>輸入您希望模組傳回的第一個回應編號。 第一個傳回回回回回應的位移為 <code>0</code>. 將此欄位與[！UICONTROL Maximum number of returned results]欄位搭配使用，可將回應分頁。</p>
      <p>例如，若要檢視回應的第三個頁面，當每個頁面有10個回應時，請將[！UICONTROL Offset]設為20，並將[！UICONTROL Maximum number of returned]設為10。</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[！UICONTROL傳回結果的最大數目]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。 將此欄位與[！UICONTROL Offset]欄位搭配使用，可將回應分頁。</p>
      <p>例如，若要檢視回應的第三個頁面，當每個頁面有10個回應時，請將[！UICONTROL Offset]設為20，並將[！UICONTROL Maximum number of returned]設為10。</p>
    </td>
  </tr>
</tbody>
</table>
