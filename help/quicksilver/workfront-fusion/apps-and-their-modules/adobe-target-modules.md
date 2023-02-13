---
filename: adobe-target-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Target模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Adobe Target], as well as connect it to multiple third-party applications and services. [!DNL Adobe Target] 模組可讓您建立、讀取、更新或刪除記錄、列出指定類型的所有記錄、根據您指定的條件搜尋記錄，或對自訂API呼叫執行 [!DNL Adobe Target] API。
author: Becky
exl-id: 9597806b-d4bf-4627-b27d-30e24a1e6776
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2598'
ht-degree: 0%

---

# [!DNL Adobe Target] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Adobe Target]，並將其連接至多個協力廠商應用程式和服務。 [!DNL Adobe Target] 模組可讓您建立、建立、讀取、更新或刪除記錄、列出指定類型的所有記錄、根據您指定的條件搜尋記錄，或對自訂API呼叫執行 [!DNL Adobe Target] API。


如果您需要建立案例的相關指示，請參閱 [建立藍本](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
      <td>
        <p>[!UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
      <td>
        <p>[!UICONTROL計畫]、[!UICONTROL工作]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合）</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">產品</td>
      <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td>
    </tr>
    </tr>
  </tbody>
</table>


若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

您可以使用 [!DNL Adobe Target] 連接器，您必須確保符合下列必要條件：

* 您必須具有活動 [!DNL Adobe Target] 帳戶。

## 建立連線至 [!DNL Adobe Target]

為 [!DNL Adobe Target] 模組：

1. 按一下 **[!UICONTROL 新增]** 的下界。

1. 填寫下列欄位：

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL連接名]</td>
        <td>
          <p>輸入此連接的名稱。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL客戶端ID]</td>
        <td>輸入 [!DNL Adobe] 用戶端ID。 您可在 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL客戶端密碼]</td>
        <td>輸入 [!DNL Adobe] 用戶端密碼。 您可在 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL組織ID]</td>
        <td>輸入 [!DNL Adobe] 組織ID。 您可在 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL技術帳戶ID]</td>
        <td>輸入 [!DNL Adobe] 技術帳戶ID。 您可在 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL租戶]</td>
        <td>
          <p> 若要找到您的租用戶，請登入 [!DNL Adobe Experience Cloud]，開啟 [!DNL Target]，然後按一下 [!DNL Target] 卡片。 使用「租用戶ID」值，如URL子網域中所述。</p>
          <p>例如，若您的URL登入時 [!DNL Adobe Target] is <code>&lt;https://mycompany.experiencecloud.adobe.com/...></code> 您的租用戶ID為「mycompany」。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL元作用域]</td>
        <td>輸入 <code>ent_marketing_sdk</code>       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL私鑰]</td>
        <td>
          <p>在 [!DNL Adobe Developer Console]. </p>
          <p>若要擷取私密金鑰或憑證：</p>
          <ol>
            <li value="1">
              <p>按一下 <b>[!UICONTROL提取]</b>.</p>
            </li>
            <li value="2">
              <p>選取要擷取的檔案類型。</p>
            </li>
            <li value="3">
              <p>選取包含私密金鑰或憑證的檔案。</p>
            </li>
            <li value="4">
              <p>輸入檔案的密碼。</p>
            </li>
            <li value="5">
              <p>按一下 <b>[!UICONTROL保存]</b> 以解壓縮檔案並返回連接設定。</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. 按一下 **[!UICONTROL 繼續]** 以儲存連線並返回模組。

## [!DNL Adobe Target] 模組及其欄位

設定時 [!DNL Adobe Target] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Adobe Target] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
    <td role="rowheader">[!UICONTROL連接]</td>
    <td>有關建立連接的說明 [!DNL Adobe Target]，請參閱 <a href="#Create" class="MCXref xref" >建立連線至 [!DNL Adobe Target]</a> 這篇文章。</td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL記錄類型]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>選擇要建立的記錄類型。</p>
      <ul>
        <li>
          <p>[!UICONTROL AB活動]</p>
          <p>繼續 <a href="#AB%C2%A0Activ" class="MCXref xref" >AB活動欄位</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL XT活動]</p>
          <p>繼續 <a href="#XT" class="MCXref xref" >XT活動欄位</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL選件]</p>
          <p>繼續 <a href="#Offer" class="MCXref xref" >優惠方案欄位</a>.</p>
        </li>
        <li>
          <p>[!UICONTROL對象]</p>
          <p>繼續 <a href="#Audience" class="MCXref xref" >對象欄位</a>.</p>
        </li>
      </ul>
    </td>
  </tr>
</tbody>
</table>

##### AB活動欄位

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名稱]</td>
      <td>輸入或映射此活動的名稱。 名稱不得超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL選項]</td>
      <td>
        <p>針對您要新增至活動的每個選項，按一下 <b>[!UICONTROL添加項]</b> 並填寫下列欄位：</p>
        <ul>
          <li>
            <p><b>[!UICONTROL選項本地ID]</b>
            </p>
            <p>輸入或對應字串，以用於跨API請求追蹤選項。</p>
          </li>
          <li>
            <p><b>[!UICONTROL名稱]</b>
            </p>
            <p>輸入或對應選項的名稱。 名稱不得超過250個字元。</p>
          </li>
          <li>
            <p><b>[!UICONTROL選件ID]</b>
            </p>
          </li>
          <li>
            <p>選取或對應與選項相關聯的選件。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL位置]</td>
      <td>
        <p>針對您要新增至活動的每個Mbox，按一下 <b>[!UICONTROL添加項]</b> 並填寫下列欄位：</p>
        <ul>
          <li>
            <p>[!UICONTROL對象ID]</p>
            <p>針對您要新增至mbox的每個對象，按一下 <b>[!UICONTROL添加項]</b> 並選取「對象ID」 。</p>
          </li>
          <li>
            <p><b>[!UICONTROL位置本地ID]</b>
            </p>
            <p>輸入或對應字串，以用於追蹤各API請求的位置。</p>
          </li>
          <li>
            <p><b>[!UICONTROL名稱]</b>
            </p>
            <p>輸入或映射位置的名稱。 名稱不得超過250個字元。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL體驗]</td>
      <td>
        <p>頁面上提供內容選件的位置清單。 位置包含下列項目：
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL體驗本機ID]</b>
            </p>
            <p>輸入或對應體驗的ID</p>
          </li>
          <li>
            <p><b>[!UICONTROL名稱]</b>
            </p>
            <p>輸入或對應體驗的名稱

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>針對您想要查看體驗的每個對象，按一下 <b>[!UICONTROL添加項]</b> 並輸入對象ID。

</p>
          </li>
          <li>
            <p><b>[!UICONTROL訪客百分比]</b>
            </p>
            <p>輸入或對應分配給體驗的訪客百分比</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL度量]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL第三方ID]</td>
      <td>輸入或對應ID以識別此活動。 您可以選擇此ID。 此ID不得與其他活動相同，且不得超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL開始於]</td>
      <td>輸入或對應以格式啟動活動的日期和時間 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL結尾為]</td>
      <td>輸入或對應以格式結束活動的日期和時間 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL狀態]</td>
      <td>
        <p>輸入或對應活動的狀態。</p>
        <ul>
          <li>
            <p>[!UICONTROL已批准]</p>
          </li>
          <li>
            <p>[!UICONTROL已停用]</p>
          </li>
          <li>
            <p>[!UICONTROL已暫停]</p>
          </li>
          <li>
            <p>[!UICONTROL已保存] </p>
          </li>
          <li>
            <p>[！已刪除UICONTROL]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL優先順序]</td>
      <td>輸入定義活動優先順序的數字。 數字越高，優先順序越高。 此值必須介於0和999之間。 預設值為5。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL自動分配流量]</td>
      <td>
        <p>啟用此選項可自動分配流量。 自動分配會傳送更多流量給較成功的體驗。</p>
        <p>選取或對應評估標準，以判斷哪個體驗較成功。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>輸入或對應活動關聯的工作區</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL屬性ID] </td>
      <td>針對您要新增至活動的每個屬性，按一下 <b>[!UICONTROL添加項]</b> 並選取或對應屬性的ID。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL報表對象]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>對於您要新增至活動的每個報表對象，按一下[!UICONTROL新增項目]並輸入下列資訊：</p>
        <ul>
          <li>
            <p><b>[!UICONTROL報表對象本機ID]</b>
            </p>
            <p>輸入或對應字串，以用於跨API請求追蹤報表對象。</p>
          </li>
          <li>
            <p><b>[!UICONTROL對象ID]</b>
            </p>
            <p>輸入或對應要用於報表的區段</p>
          </li>
          <li>
            <p><b>[!UICONTROL量度本機ID]</b>
            </p>
            <p>輸入或對應字串，以用於跨API請求追蹤量度。</p>
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
      <td role="rowheader">[!UICONTROL名稱]</td>
      <td>輸入或映射此活動的名稱。 名稱不得超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL選項]</td>
      <td>
        <p>針對您要新增至活動的每個選項，按一下 <b>[!UICONTROL添加項]</b> 並填寫下列欄位：</p>
        <ul>
          <li>
            <p><b>[!UICONTROL選項本地ID]</b>
            </p>
            <p>輸入或對應字串，以用於跨API請求追蹤選項。</p>
          </li>
          <li>
            <p><b>[!UICONTROL名稱]</b>
            </p>
            <p>輸入或對應選項的名稱。 名稱不得超過250個字元。</p>
          </li>
          <li>
            <p><b>[!UICONTROL選件ID]</b>
            </p>
          </li>
          <li>
            <p>選取或對應與選項相關聯的選件。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL位置]</td>
      <td>
        <p>針對您要新增至活動的每個Mbox，按一下 <b>[!UICONTROL添加項]</b> 並填寫下列欄位：</p>
        <ul>
          <li>
            <p>[!UICONTROL對象ID]</p>
            <p>針對您要新增至mbox的每個對象，按一下 <b>[!UICONTROL添加項]</b> 並選取「對象ID」 。</p>
          </li>
          <li>
            <p><b>[!UICONTROL位置本地ID]</b>
            </p>
            <p>輸入或對應字串，以用於追蹤各API請求的位置。</p>
          </li>
          <li>
            <p><b>[!UICONTROL名稱]</b>
            </p>
            <p>輸入或映射位置的名稱。 名稱不得超過250個字元。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL體驗]</td>
      <td>
        <p>頁面上提供內容選件的位置清單。 位置包含下列項目：
</p>
        <ul>
          <li>
            <p><b>[!UICONTROL體驗本機ID]</b>
            </p>
            <p>輸入或對應體驗的ID</p>
          </li>
          <li>
            <p><b>[!UICONTROL名稱]</b>
            </p>
            <p>輸入或對應體驗的名稱

</p>
          </li>
          <li>
            <p><b>[!DNL Audience IDs]</b>
            </p>
            <p>針對您想要查看體驗的每個對象，按一下 <b>[!UICONTROL添加項]</b> 並輸入對象ID。

</p>
          </li>
          <li>
            <p><b>[!UICONTROL訪客百分比]</b>
            </p>
            <p>輸入或對應分配給體驗的訪客百分比</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL度量]</td>
      <td> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL第三方ID]</td>
      <td>輸入或對應ID以識別此活動。 您可以選擇此ID。 此ID不得與其他活動相同，且不得超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL開始於]</td>
      <td>輸入或對應以格式啟動活動的日期和時間 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL結尾為]</td>
      <td>輸入或對應以格式結束活動的日期和時間 <code>YYYY-MM-DD hh:mm:ss.z</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL狀態]</td>
      <td>
        <p>輸入或對應活動的狀態。</p>
        <ul>
          <li>
            <p>[!UICONTROL已批准]</p>
          </li>
          <li>
            <p>[!UICONTROL已停用]</p>
          </li>
          <li>
            <p>[!UICONTROL已暫停]</p>
          </li>
          <li>
            <p>[!UICONTROL已保存] </p>
          </li>
          <li>
            <p>[！已刪除UICONTROL]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL優先順序]</td>
      <td>輸入定義活動優先順序的數字。 數字越高，優先順序越高。 此值必須介於0和999之間。 預設值為5。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL自動分配流量]</td>
      <td>
        <p>啟用此選項可自動分配流量。 自動分配會傳送更多流量給較成功的體驗。</p>
        <p>選取或對應評估標準，以判斷哪個體驗較成功。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>輸入或對應活動關聯的工作區</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL屬性ID] </td>
      <td>針對您要新增至活動的每個屬性，按一下 <b>[!UICONTROL添加項]</b> 並選取或對應屬性的ID。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL報表對象]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>對於您要新增至活動的每個報表對象，按一下[!UICONTROL新增項目]並輸入下列資訊：</p>
        <ul>
          <li>
            <p><b>[!UICONTROL報表對象本機ID]</b>
            </p>
            <p>輸入或對應字串，以用於跨API請求追蹤報表對象。</p>
          </li>
          <li>
            <p><b>[!UICONTROL對象ID]</b>
            </p>
            <p>輸入或對應要用於報表的區段</p>
          </li>
          <li>
            <p><b>[!UICONTROL量度本機ID]</b>
            </p>
            <p>輸入或對應字串，以用於跨API請求追蹤量度。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### 優惠方案欄位

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL名稱]</td>
      <td>輸入或映射此活動的名稱。 名稱不得超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL內容]</td>
      <td>
        <p>輸入或對應要向使用者顯示的選件內容。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>
        <p>輸入或對應與選件相關聯的工作區ID。 若保留為空白，則選件會與帳戶的預設工作區相關聯。 此功能僅適用於 [!DNL Target] 高級帳戶。</p>
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
      <td role="rowheader">[!UICONTROL名稱]</td>
      <td>輸入或對應此對象的名稱。 名稱不得超過250個字元。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL內容]</td>
      <td>
        <p>輸入或對應此對象的說明。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL目標規則]</td>
      <td>
        <p>啟用切換將規則設為「和」，即必須套用所有規則。</p>
        <p>針對您要套用至對象的每個規則，按一下 <b>[!UICONTROL添加項]</b> 並輸入要套用之規則的JSON。 </p>
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
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Workspace]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
        <p>輸入或對應與對象相關聯的工作區ID。 若保留為空白，則選件會與帳戶的預設工作區相關聯。 此功能僅適用於 [!DNL Target Premium] 帳戶。</p>
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
      <td role="rowheader">[!UICONTROL連接]</td>
      <td>有關建立連接的說明 [!DNL Adobe Target]，請參閱 <a href="#Create" class="MCXref xref" >建立連線至 [!DNL Adobe Target]</a> 這篇文章。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL [!DNL Target] 基礎URL]</td>
      <td>輸入或對應您的 [!DNL Target] 基礎URL。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL路徑]</p>
      </td>
      <td>
        <p>輸入相對於{baseURL}/的路徑</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL方法]</p>
      </td>
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL標題]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標題。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自動新增授權標題和x-api金鑰標題。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL查詢字串]  </td>
      <td>
        <p>輸入請求查詢字串。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL正文]</td>
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
    <td role="rowheader">[!UICONTROL連接]</td>
    <td>有關建立連接的說明 [!DNL Adobe Target]，請參閱 <a href="#Create" class="MCXref xref" >建立連線至 [!DNL Adobe Target]</a> 這篇文章。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL記錄類型]</td>
    <td>選擇要刪除的記錄類型。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL記錄ID]</td>
    <td>輸入或映射要刪除的記錄ID。</td>
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
    <td role="rowheader">[!UICONTROL連接]</td>
    <td>有關建立連接的說明 [!DNL Adobe Target]，請參閱 <a href="#Create" class="MCXref xref" >建立連線至 [!DNL Adobe Target]</a> 這篇文章。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL記錄類型]</td>
    <td>選擇要讀取的記錄類型。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL記錄ID]</td>
    <td>輸入或映射要讀取的記錄的ID。</td>
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
      <td role="rowheader">[!UICONTROL連接]</td>
      <td>有關建立連接的說明 [!DNL Adobe Target]，請參閱 <a href="#Create" class="MCXref xref" >建立連線至 [!DNL Adobe Target]</a> 這篇文章。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL記錄類型]</td>
      <td>
        <p>選擇要更新的記錄類型。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL AB活動]</b>
            </p>
            <p>請參閱 <a href="#AB%C2%A0Activ" class="MCXref xref" >AB活動欄位</a> 在 <a href="#Create2" class="MCXref xref" >建立記錄</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL XT活動]</b>
            </p>
            <p>請參閱 <a href="#XT" class="MCXref xref" >XT活動欄位</a> 在 <a href="#Create2" class="MCXref xref" >建立記錄</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL其他活動]</b>
            </p>
            <p>選擇要更新值的欄位，然後為欄位輸入新值。</p>
          </li>
          <li>
            <p><b>[!UICONTROL選件]</b>
            </p>
            <p>請參閱 <a href="#Offer" class="MCXref xref" >優惠方案欄位</a> 在 <a href="#Create2" class="MCXref xref" >建立記錄</a>.</p>
          </li>
          <li>
            <p><b>[!DNL Audience]</b>
            </p>
            <p>請參閱 <a href="#Audience" class="MCXref xref" >對象欄位</a> 在 <a href="#Create2" class="MCXref xref" >建立記錄</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL記錄ID]</td>
      <td>輸入或映射要更新的記錄ID。</td>
    </tr>
  </tbody>
</table>

### 搜尋

* [[!UICONTROL 獲取記錄]](#get-records)

* [[!UICONTROL 搜尋]](#search)


#### [!UICONTROL 獲取記錄]

此搜索模組檢索選定類型的記錄清單。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
      <td>有關建立連接的說明 [!DNL Adobe Target]，請參閱 <a href="#Create" class="MCXref xref" >建立連線至 [!DNL Adobe Target]</a> 這篇文章。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL記錄類型]</td>
      <td>選擇要更新的記錄類型。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL排序依據]</td>
      <td>對於要排序的每個欄位，按一下 <b>[!UICONTROL添加項]</b> 並選取欄位，以及傳回的結果應遞增或遞減。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL開始於]</td>
      <td>
        <p>輸入要檢索記錄的最早日期。 </p>
        <p>如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL結尾為]</td>
      <td>
        <p>輸入要為其檢索記錄的最新日期。 </p>
        <p>如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 搜尋]

此搜尋模組會根據您指定的條件，搜尋「活動」、「選件」或「對象」。

<table style="table-layout:auto"> 
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL連接]</td>
    <td>有關建立連接的說明 [!DNL Adobe Target]，請參閱 <a href="#Create" class="MCXref xref" >建立連線至 [!DNL Adobe Target]</a> 這篇文章。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL記錄類型]</td>
    <td>選擇要更新的記錄類型。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL排序依據]</td>
    <td>對於要排序的每個欄位，按一下 <b>[!UICONTROL添加項]</b> 並選取欄位，以及傳回的結果應遞增或遞減。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL搜索條件]</td>
    <td>針對您要設定的每個規則，選取欄位、運算子和值。 按一下 <b>[!UICONTROL添加和規則]</b> 來建立其他規則。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL偏移]</td>
    <td>
      <p>輸入您要模組傳回的第一個回應數。 第一個傳回的回應的位移為 <code>0</code>. 將此欄位與[!UICONTROL返回結果的最大數]欄位組合使用，以分頁響應。</p>
      <p>例如，若要查看第三個回應頁面，當每個頁面有10個回應時，請將[!UICONTROL Offset]設為20，並將[!UICONTROL Maximum number of returned]結果設為10。</p>
    </td>
  </tr>
  <tr>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL返回結果的最大數]</td>
    <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
      <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。 將此欄位與[!UICONTROL Offset]欄位結合使用，以分頁回應。</p>
      <p>例如，若要查看第三個回應頁面，當每個頁面有10個回應時，請將[!UICONTROL Offset]設為20，並將[!UICONTROL Maximum number of returned]結果設為10。</p>
    </td>
  </tr>
</tbody>
</table>
