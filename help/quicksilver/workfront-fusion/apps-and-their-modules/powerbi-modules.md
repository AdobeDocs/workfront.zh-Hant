---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Power BI模組
description: 除了Adobe Workfront授權，Adobe Workfront Fusion還需要Adobe Workfront Fusion授權。
author: Becky
feature: Workfront Fusion
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '2398'
ht-degree: 0%

---

# [!DNL Power BI]模組

[!DNL Power BI]是應用程式，可讓您以視覺效果呈現資料給利害關係人。 它可接收來自各種來源的資料。

>[!NOTE]
>
>[!DNL Workfront Fusion]不是資料來源。 雖然[!DNL Workfront Fusion]可以建立和使用資料來源，但不會儲存您的資料。


## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!DNL Plan]， [!DNL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

&#42;&#42;如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI]模組及其欄位

當您設定[!DNL Power BI]時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些以外，其他欄位可能會顯示，端視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在Adobe Workfront Fusion中將資訊從一個模組對應到另一個模組](../../workfront-fusion/mapping/map-information-between-modules.md)。

![](assets/map-toggle-350x74.png)

### 儀表板

#### [!UICONTROL 清單儀表板]

此搜尋模組會擷取控制面板清單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>
        <p>選取或對應擁有您要列出之控制面板的群組ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出儀表板圖磚]

此搜尋模組會擷取控制面板圖磚清單。

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL輸入儀表板ID]</td>
    <td>
      <p>選取或對應選項，以選擇要列出圖磚的控制面板。</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL儀表板ID]</td>
    <td>
      <p>輸入或對應包含您要列出之圖磚之控制面板的ID。</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL群組ID]  </td>
    <td>選取或對應擁有控制面板的群組ID，控制面板包含您要列出的圖磚。</td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL限制]  </td>
    <td>
      <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL 取得儀表板]

此動作模組會擷取指定控制面板的中繼資料。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入儀表板ID]</td>
      <td>
        <p>選取或對應選項，以選擇要擷取中繼資料的控制面板。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL儀表板ID]</td>
      <td>
        <p>輸入或對應您要擷取中繼資料之控制面板的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>選取或對應擁有您要擷取中繼資料之控制面板的群組ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 取得儀表板拼貼]

此動作模組會擷取指定控制面板圖磚的中繼資料。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入儀表板ID]</td>
      <td>
        <p>選取或對應選項，以選擇要擷取的控制面板詳細資訊。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL儀表板ID]</td>
      <td>
        <p>輸入或對應您要擷取其詳細資訊之控制面板的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL拼貼ID]</td>
      <td>輸入或對應您要擷取詳細資料的[!DNL Power BI]圖磚識別碼。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>選取或對應擁有您要擷取之圖磚之群組的ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 建立儀表板]

此動作模組會建立新的控制面板。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
      <td>輸入或對應控制面板的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>選取或對應將擁有新儀表板的群組ID。</td>
    </tr>
  </tbody>
</table>

### 報告

#### [!UICONTROL 清單報告]

此搜尋模組會擷取報表清單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>
        <p>選取或對應擁有您要列出之報告的群組ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 取得報表]

此動作模組會擷取指定報表的中繼資料。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入報表ID]</td>
      <td>
        <p>選取或對應選項，以選擇要擷取中繼資料的報表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL報表ID]</td>
      <td>
        <p>輸入或對應您要擷取中繼資料之報表的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>選取或對應擁有您要擷取中繼資料之報表的群組ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 複製報告]

此動作模組會複製現有報表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入報表ID]</td>
      <td>
        <p>選取或對應選項，以選擇要複製的報表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL報表ID]</td>
      <td>
        <p>輸入或對應您要複製之報表的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>選取或對應擁有您要複製之報表之群組的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL新複製的報表名稱]</td>
      <td>輸入或對應新報表的名稱。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 刪除報告]

此動作模組會刪除報表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入報表ID]</td>
      <td>
        <p>選取或對應選項，以選擇要刪除的報表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL報表ID]</td>
      <td>
        <p>輸入或對應您要刪除之報表的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>選取或對應擁有您要刪除之報表之群組的ID。</td>
    </tr>
  </tbody>
</table>

### 資料集

#### [!UICONTROL 列出資料集]

此搜尋模組會擷取資料集清單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>選取或對應擁有您要擷取中繼資料之報表的群組ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]</td>
      <td>
        <p>在每個案例執行週期中，輸入或對應您要模組至[action]的最大記錄數量。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 取得資料集]

此動作模組會擷取指定資料集的中繼資料。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入報表ID]</td>
      <td>
        <p>選取或對應選項，以選擇要擷取中繼資料的報表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL報表ID]</td>
      <td>
        <p>輸入或對應您要擷取中繼資料之資料集的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>選取或對應擁有您要擷取中繼資料之資料集的群組ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 建立資料集]

此動作模組會建立新資料集。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
      <td>輸入或對應資料集的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>選取或對應將擁有新資料集的群組ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL預設模式]</td>
      <td>
        <p>選取或對應資料集的預設模式：</p>
        <ul>
          <li>
            <p><b>[！UICONTROL As Azure]</b>：與有即時連線的資料集 [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[！UICONTROL As on Prem]</b>：與[!DNL On-premise Analysis]服務有即時連線的資料集</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>：允許以程式設計方式存取資料，以推送資料至的資料集 [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>：支援資料串流的資料集，可程式化地存取以推送資料至 [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>：支援資料串流的資料集</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL表格]</td>
      <td>新增表格至資料集。 如需欄位，請參閱<a href="#Table" class="MCXref_0">表格欄位</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>新增資料來源。 如需欄位，請參閱<a href="#Data" class="MCXref_0">資料來源欄位</a>。</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>選取或對應資料集的刻意原則：</p>
        <ul>
          <li>
            <p>[！UICONTROL無]</p>
          </li>
          <li>
            <p>[！UICONTROL基本FIFO]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### 表格欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
      <td>
        <p>  輸入或對映表格的名稱。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL欄]</td>
      <td>
        <p>新增欄：</p>
        <ul>
          <li>
            <p><b>[！UICONTROL名稱]</b>
            </p>
            <p>輸入（對應）欄名稱。</p>
          </li>
          <li>
            <p><b>[！UICONTROL資料型別]</b>
            </p>
            <p>選取或對應資料型別：</p>
            <ul>
              <li>
                <p>[！UICONTROL字串]</p>
              </li>
              <li>
                <p>[！UICONTROL整數]</p>
              </li>
              <li>
                <p>[！UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[！UICONTROL日期時間]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[！UICONTROL格式字串]</b>
            </p>
            <p>輸入（對應）格式字串。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL列]</td>
      <td>輸入或對應列詳細資料。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Measures]</td>
      <td>新增表格的測量。</td>
    </tr>
  </tbody>
</table>

##### 資料來源欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL資料庫]  </td>
      <td>
        <p>輸入或對應您要使用的資料庫。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Server]  </td>
      <td>
        <p>輸入或對應您要使用的伺服器名稱。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL]  </td>
      <td>
        <p>輸入或對應您要使用的URL。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資料來源ID]</td>
      <td>
        <p>  輸入或對應資料來源的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資料來源型別]  </td>
      <td>
        <p>選取或對應資料來源型別。 範例： SQL。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL閘道ID]  </td>
      <td>輸入或對應您要使用的閘道識別碼。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 新增或刪除資料集資料表中的資料列]

此動作模組會新增或刪除指定推送資料集表格的列。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入表格]</td>
      <td>選取或對應選項以選取包含您要調整之表格的資料集。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資料集ID]</td>
      <td>輸入或對應包含您要新增或刪除之列的資料集ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資料表名稱]  </td>
      <td>
        <p>輸入或對應包含您要新增或刪除之資料列的表格名稱。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>輸入或對應擁有資料集之群組的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL選取動作]</td>
      <td>
        <p>選取或對應您要執行的動作。</p>
        <ul>
          <li>
            <p>[！UICONTROL新增列]</p>
          </li>
          <li>
            <p>[！UICONTROL Delete All Rows]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL列]</td>
      <td>
        <p>新增列欄位。</p>
        <ul>
          <li>
            <p><b>[！UICONTROL索引鍵]</b>
            </p>
            <p>輸入或對應金鑰名稱。</p>
          </li>
          <li>
            <p><b>[！UICONTROL欄位型別]</b>
            </p>
            <p>選取或對應欄位型別：</p>
            <ul>
              <li>
                <p>布林值</p>
              </li>
              <li>
                <p>日期</p>
              </li>
              <li>
                <p>文字</p>
              </li>
              <li>
                <p>數字</p>
              </li>
            </ul>
          </li>
          <li>
            <p>[！UICONTROL值]</p>
            <p>輸入或對應索引鍵值。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 重新整理資料集]

此動作模組會重新整理指定的資料集。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入資料集]</td>
      <td>選取或對應選項，以選取您要重新整理的資料集。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資料集ID]</td>
      <td>輸入或對應您要重新整理之資料集的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資料表名稱]  </td>
      <td>
        <p>輸入或對應包含您要新增或刪除之資料列的表格名稱。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>輸入或對應擁有資料集之群組的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL通知選項]  </td>
      <td>
        <p>選取或對應選項以通知：</p>
        <ul>
          <li>
            <p>[！UICONTROL Mail on Completion]</p>
          </li>
          <li>
            <p>[！UICONTROL郵件失敗]</p>
          </li>
          <li>
            <p>[！UICONTROL無通知]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 刪除資料集]

此動作模組會刪除資料集。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL輸入報表ID]</td>
      <td>
        <p>選取或對應選項，以選擇要刪除的資料集。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL報表ID]</td>
      <td>
        <p>輸入或對應您要刪除之資料集的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL群組ID]  </td>
      <td>選取或對應擁有您要刪除之資料集的群組ID。</td>
    </tr>
  </tbody>
</table>

### 應用程式

#### [!UICONTROL 觀看應用程式]

此觸發模組會在應用程式更新時啟動案例。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出應用程式]

此搜尋模組會擷取已安裝的所有應用程式清單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出應用程式的報表]

此搜尋模組會從指定的應用程式擷取所有報表的清單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL應用程式ID]</td>
      <td>選取或對應您要從中列出報表之應用程式的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出應用程式的儀表板]

此搜尋模組會從指定的應用程式擷取控制面板清單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL應用程式ID]</td>
      <td>選取或對應您要列出控制面板之應用程式的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 取得應用程式]

此動作模組會擷取指定應用程式的中繼資料。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL應用程式ID]  </td>
      <td>
        <p>選取或對應您要擷取的應用程式ID。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 取得應用程式的報表]

此動作模組會擷取指定應用程式報表的中繼資料。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL應用程式ID]  </td>
      <td>
        <p>選取或對應包含您要擷取之報表的應用程式ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL報表ID]</td>
      <td>
        <p>  選取或對應您要擷取之報表的ID。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 取得應用程式的儀表板]

此動作模組會擷取指定應用程式控制面板的中繼資料。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL應用程式ID]  </td>
      <td>
        <p>選取或對應包含您要擷取之控制面板的應用程式ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL報表ID]</td>
      <td>
        <p>  選取或對應您要擷取之控制面板的ID。</p>
      </td>
    </tr>
  </tbody>
</table>

### 其他

#### [!UICONTROL 進行API呼叫]

此動作模組會執行[!DNL Power BI] API的API呼叫。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>如需有關將您的[!DNL Power BI]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL路徑]</p>
      </td>
      <td>
        <p>輸入相對於<code>https://api.powerbi.com</code>的路徑。 範例： <code>/v1.0/myorg/datasets</code>。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
      <td>
        <p>選取設定API呼叫所需的[！UICONTROL HTTP]要求方法。 如需詳細資訊，請參閱[！UICONTROL HTTP]要求方法。</p>
      </td>
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
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
