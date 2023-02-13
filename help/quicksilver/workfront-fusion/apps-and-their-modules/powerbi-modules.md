---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Power BI模組
description: Adobe Workfront Fusion除了需要Adobe Workfront授權外，還需要Adobe Workfront Fusion授權。
author: Becky
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 6d6aaa4e85690307f93dfc5179a489a09e9a2381
workflow-type: tm+mt
source-wordcount: '2352'
ht-degree: 0%

---

# [!DNL Power BI] 模組

[!DNL Power BI] 是一種應用程式，可讓您視覺化資料，並呈現給利害關係人。 它可以從多種來源取得資料。

>[!NOTE]
>
>[!DNL Workfront Fusion] 不是資料來源。 同時 [!DNL Workfront Fusion] 可以建立和使用資料來源，但不會儲存您的資料。


## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!DNL Plan], [!DNL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

&#42;&#42;如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI] 模組及其欄位

設定時 [!DNL Power BI], [!DNL Workfront Fusion] 顯示下列欄位。 除了這些欄位，還可能會根據應用程式或服務中的存取層級等因素顯示其他欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在Adobe Workfront Fusion中，將資訊從一個模組對應至另一個模組](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 儀表板

#### [!UICONTROL 列出控制面板]

此搜尋模組會擷取控制面板清單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>
        <p>選取或對應擁有您要列出之控制面板之群組的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]  </td>
      <td>
        <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 清單控制面板圖磚]

此搜尋模組會擷取控制面板圖磚清單。

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL輸入控制面板ID]</td>
    <td>
      <p>選取或對應選項，以選擇要列出其圖磚的控制面板。</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL儀表板ID]</td>
    <td>
      <p>輸入或對應包含您要列出的圖磚之控制面板的ID。</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL組ID]  </td>
    <td>選取或對應擁有控制面板（包含您要列出的圖磚）的群組的ID。</td>
  </tr>
  <tr>
    <td role="rowheader">[!UICONTROL限制]  </td>
    <td>
      <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL 取得控制面板]

此動作模組會擷取指定控制面板的中繼資料。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL輸入控制面板ID]</td>
      <td>
        <p>選取或對應選項，以選擇要擷取中繼資料的控制面板。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL儀表板ID]</td>
      <td>
        <p>輸入或對應您要擷取中繼資料的控制面板ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>選擇或映射擁有要檢索元資料的控制面板的組的ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 取得控制面板圖磚]

此動作模組會擷取指定控制面板方塊的中繼資料。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL輸入控制面板ID]</td>
      <td>
        <p>選取或對應選項，以選擇您要擷取的控制面板詳細資訊。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL儀表板ID]</td>
      <td>
        <p>輸入或映射要為其檢索詳細資訊的儀表板的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL磁貼ID]</td>
      <td>輸入或對應 [!DNL Power BI] 表徵圖，以檢索詳細資訊。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>選取或對應擁有您要擷取之圖磚的群組ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 建立控制面板]

此動作模組會建立新的控制面板。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL名稱]</td>
      <td>輸入或映射控制面板的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>選取或對應將擁有新控制面板之群組的ID。</td>
    </tr>
  </tbody>
</table>

### 報告

#### [!UICONTROL 清單報表]

此搜尋模組會擷取報表清單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>
        <p>選取或對應擁有您要清單之報表之群組的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]  </td>
      <td>
        <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p>
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
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL輸入報表ID]</td>
      <td>
        <p>選取或對應選項，以選擇您要擷取中繼資料的報表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL報表ID]</td>
      <td>
        <p>輸入或對應您要擷取中繼資料之報表的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>選取或對應擁有您要擷取中繼資料之報表之群組的ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 複製報表]

此動作模組會複製現有報表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL輸入報表ID]</td>
      <td>
        <p>選取或對應選項，以選擇您要複製的報表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL報表ID]</td>
      <td>
        <p>輸入或對應您要複製之報表的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>選取或對應擁有您要複製之報表之群組的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL新複製的報表名稱]</td>
      <td>輸入或映射新報表的名稱。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 刪除報表]

此動作模組會刪除報表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL輸入報表ID]</td>
      <td>
        <p>選取或對應選項，以選擇您要刪除的報表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL報表ID]</td>
      <td>
        <p>輸入或對應您要刪除之報表的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
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
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>選取或對應擁有您要擷取中繼資料之報表之群組的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>
        <p>輸入或映射在每個方案執行週期中希望模組執行[action]的記錄數上限。</p>
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
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL輸入報表ID]</td>
      <td>
        <p>選取或對應選項，以選擇您要擷取中繼資料的報表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL報表ID]</td>
      <td>
        <p>輸入或對應您要擷取中繼資料之資料集的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
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
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL名稱]</td>
      <td>輸入或對應資料集的名稱。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>選取或對應將擁有新資料集之群組的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL預設模式]</td>
      <td>
        <p>選取或對應資料集的預設模式：</p>
        <ul>
          <li>
            <p><b>[!UICONTROL As Azure]</b>:具有即時連線的資料集 [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[!UICONTROL在Prem上為]</b>:具有即時連線的資料集 [!DNL On-premise Analysis] 服務</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>:可程式化存取的資料集，可將資料推送至 [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>:支援資料串流且可程式化存取，將資料推送至 [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>:支援資料串流的資料集</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL表]</td>
      <td>將表格新增至資料集。 如需欄位，請參閱 <a href="#Table" class="MCXref_0">表格欄位</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>新增資料來源。 如需欄位，請參閱 <a href="#Data" class="MCXref_0">資料來源欄位</a>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>選擇或映射資料集的目標策略：</p>
        <ul>
          <li>
            <p>[!UICONTROL無]</p>
          </li>
          <li>
            <p>[!UICONTROL基本FIFO]</p>
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
      <td role="rowheader">[!UICONTROL名稱]</td>
      <td>
        <p>  輸入或映射表的名稱。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL列]</td>
      <td>
        <p>新增欄：</p>
        <ul>
          <li>
            <p><b>[!UICONTROL名稱]</b>
            </p>
            <p>輸入（映射）列名。</p>
          </li>
          <li>
            <p><b>[!UICONTROL資料類型]</b>
            </p>
            <p>選擇或映射資料類型：</p>
            <ul>
              <li>
                <p>[!UICONTROL字串]</p>
              </li>
              <li>
                <p>[!UICONTROL整數]</p>
              </li>
              <li>
                <p>[!UICONTROL布林值]</p>
              </li>
              <li>
                <p>[!UICONTROL日期時間]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[!UICONTROL格式字串]</b>
            </p>
            <p>輸入（對應）格式字串。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL行]</td>
      <td>輸入或映射行詳細資訊。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL度量]</td>
      <td>為表添加度量。</td>
    </tr>
  </tbody>
</table>

##### 資料來源欄位

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL資料庫]  </td>
      <td>
        <p>輸入或映射要使用的資料庫。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL伺服器]  </td>
      <td>
        <p>輸入或映射要使用的伺服器的名稱。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]  </td>
      <td>
        <p>輸入或對應您要使用的URL。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL資料源ID]</td>
      <td>
        <p>  輸入或映射資料源的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL資料源類型]  </td>
      <td>
        <p>選擇或映射資料源類型。 範例：SQL。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL網關ID]  </td>
      <td>輸入或映射要使用的網關的ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 新增或刪除資料集表格中的列]

此動作模組會新增或刪除指定推送資料集表格的列。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL輸入表]</td>
      <td>選取或對應選項，以選取包含您要調整之表格的資料集。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL資料集ID]</td>
      <td>輸入或對應包含您要新增或刪除之列的資料集ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL表名]  </td>
      <td>
        <p>輸入或映射包含要添加或刪除的行的表的名稱。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>輸入或對應擁有資料集之群組的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL選擇操作]</td>
      <td>
        <p>選取或對應您要執行的動作。</p>
        <ul>
          <li>
            <p>[!UICONTROL添加行]</p>
          </li>
          <li>
            <p>[!UICONTROL刪除所有行]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL行]</td>
      <td>
        <p>新增列欄位。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL密鑰]</b>
            </p>
            <p>輸入或映射鍵名。</p>
          </li>
          <li>
            <p><b>[!UICONTROL欄位類型]</b>
            </p>
            <p>選擇或映射欄位類型：</p>
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
                <p>數量</p>
              </li>
            </ul>
          </li>
          <li>
            <p>[!UICONTROL值]</p>
            <p>輸入或對應鍵值。</p>
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
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL輸入資料集]</td>
      <td>選取或對應選項，以選取您要重新整理的資料集。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL資料集ID]</td>
      <td>輸入或對應您要重新整理的資料集ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL表名]  </td>
      <td>
        <p>輸入或映射包含要添加或刪除的行的表的名稱。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>輸入或對應擁有資料集之群組的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL通知選項]  </td>
      <td>
        <p>選擇或映射要通知的選項：</p>
        <ul>
          <li>
            <p>[!UICONTROL完成時發送的郵件]</p>
          </li>
          <li>
            <p>[!UICONTROL失敗時發送郵件]</p>
          </li>
          <li>
            <p>[!UICONTROL無通知]</p>
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
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL輸入報表ID]</td>
      <td>
        <p>選取或對應選項，以選擇您要刪除的資料集。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL報表ID]</td>
      <td>
        <p>輸入或對應您要刪除之資料集的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL組ID]  </td>
      <td>選取或對應擁有您要刪除之資料集之群組的ID。</td>
    </tr>
  </tbody>
</table>

### 應用程式

#### [!UICONTROL Watch應用]

此觸發器模組會在應用程式更新時啟動案例。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]  </td>
      <td>
        <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出應用程式]

此搜尋模組會擷取所有已安裝應用程式的清單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]  </td>
      <td>
        <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出應用程式的報表]

此搜尋模組會從指定的應用程式中擷取所有報表的清單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL應用程式ID]</td>
      <td>選取或對應您要列出報表之應用程式的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]  </td>
      <td>
        <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出應用程式的控制面板]

此搜尋模組會從指定的應用程式擷取控制面板清單。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL應用程式ID]</td>
      <td>選取或對應您要列出控制面板之應用程式的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]  </td>
      <td>
        <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p>
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
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL應用程式ID]  </td>
      <td>
        <p>選取或對應您要擷取之應用程式的ID。</p>
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
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL應用程式ID]  </td>
      <td>
        <p>選取或對應包含您要擷取之報表之應用程式的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL報表ID]</td>
      <td>
        <p>  選取或對應您要擷取之報表的ID。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 取得應用程式的控制面板]

此動作模組會擷取指定應用程式控制面板的中繼資料。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL應用程式ID]  </td>
      <td>
        <p>選取或對應包含您要擷取之控制面板之應用程式的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL報表ID]</td>
      <td>
        <p>  選取或對應您要擷取之控制面板的ID。</p>
      </td>
    </tr>
  </tbody>
</table>

### 其他

#### [!UICONTROL 進行API呼叫]

此動作模組會執行對 [!DNL Power BI] API。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td> <p>有關連接 [!DNL Power BI] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL路徑]</p>
      </td>
      <td>
        <p>輸入相對於的路徑 <code>https://api.powerbi.com</code>. 範例: <code>/v1.0/myorg/datasets</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL方法]</p>
      </td>
      <td>
        <p>選取設定API呼叫所需的[!UICONTROL HTTP]要求方法。 如需詳細資訊，請參閱[!UICONTROL HTTP]要求方法。</p>
      </td>
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
