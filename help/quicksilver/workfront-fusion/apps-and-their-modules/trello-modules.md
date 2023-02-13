---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: 特雷洛模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Trello的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '5039'
ht-degree: 0%

---

# [!UICONTROL 特雷洛] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!UICONTROL 特雷洛]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!DNL Trello] 模組，您必須 [!UICONTROL 特雷洛] 帳戶。

## Connect [!UICONTROL 特雷洛] to [!DNL Workfront Fusion]

有關連接 [!UICONTROL 特雷洛] 帳戶 [!DNL Workfront Fusion]，請參閱 [建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!UICONTROL 特雷洛] 模組及其欄位

設定時 [!UICONTROL 特雷洛] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!UICONTROL 特雷洛] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [面板](#boards)
* [清單](#lists)
* [卡片](#cards)
* [成員](#members)
* [核取清單](#checklists)
* [標籤](#labels)
* [註解](#comments)

### 面板

+++ **[!UICONTROL 監視板]**

新增展示板時，此觸發模組就會開始案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>展示板的最大數量 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 建立展示板]**

此動作模組會使用選取的設定建立新展示板。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名稱] </td> 
   <td> <p>輸入或映射新展示板的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL描述]</td> 
   <td> <p>視需要輸入或對應展示板說明。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL組織ID]</p> </td> 
   <td> <p>輸入或對應組織的ID。 組織ID可使用其他模組（如監看活動模組）來擷取。</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL權限級別]</p> </td> 
   <td> <p>每個權限層級的董事會有不同的投票和留言規則。 例如：如果您的董事會是[!UICONTROL專用]，而您將投票和注釋規則設定為[!UICONTROL全部]，您將會收到錯誤。 </p> <p>每個權限層級的投票和評論僅限於下列群組：</p> 
    <ul> 
     <li><strong>[!UICONTROL專用]</strong>:—&gt;成員、成員和觀察員</li> 
     <li><strong>[!UICONTROL（適用於組織）]</strong>:—&gt;成員、成員和觀察員、組織成員</li> 
     <li><strong>[!UICONTROL公用]</strong>:—&gt;成員、成員和觀察員、組織成員、全部</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL投票]</p> </td> 
   <td> <p>選擇一個選項，以指定誰可以在此板上投票。 請參閱[!UICONTROL權限層級]欄位，了解權限層級的投票限制。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL注釋]</p> </td> 
   <td> <p>選取選項，以指定誰可以對此展示板的資訊卡加上註解。 請參閱[!UICONTROL權限級別]欄位，以了解對權限級別的注釋限制。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL邀請]</p> </td> 
   <td> <p>選取可以邀請其他人加入此展示板的人員。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL自聯接]</p> </td> 
   <td> <p>選擇團隊成員是可以自己加入董事會還是必須受邀。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL預設標籤]</p> </td> 
   <td> <p>選擇是否使用新展示板的預設標籤集。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL預設清單]</p> </td> 
   <td> <p>選擇是否將預設清單集添加到展示板([!UICONTROL To Do]、[!UICONTROL Doing]、[!UICONTROL Done])。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL主板源ID]</p> </td> 
   <td> <p>選取或對應您要複製到新展示板的展示板ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL卡蓋]</p> </td> 
   <td> <p>選擇 <strong>[!UICONTROL是]</strong> 如果要為展示板啟用資訊卡封面。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL背景]</p> </td> 
   <td> <p>選取背景或自訂背景的顏色。</p> <p>注意：自訂背景僅適用於[!UICONTROL Trello Gold and Business Class]訂閱者。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL卡老化]</p> </td> 
   <td> <p>在兩種卡老化模式之間進行選擇。 </p> 
    <ul> 
     <li><strong>[!UICONTROL常規]</strong>:卡片隨著年齡增長而逐漸變得透明。 </li> 
     <li><strong>[!UICONTROL海盜]</strong>:卡片會像老海盜地圖一樣撕破，變黃，變老。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 編輯展示板]**

此動作模組會編輯現有展示板的設定。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL主板ID]</p> </td> 
   <td> <p>輸入或映射您要模組建立的展示板的唯一[!UICONTROL Trello] ID。 您可以使用其他模組（如監看板模組）來擷取展示板ID</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL新名稱]</td> 
   <td> <p> 輸入或映射展示板的新名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL新說明]</td> 
   <td> <p> 視需要輸入或對應新展示板說明。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL組織ID]</p> </td> 
   <td> <p>輸入或映射您要模組編輯的展示板的唯一[!UICONTROL Trello] ID。 您可以使用其他模組來擷取展示板ID，例如 [!DNL Watch Activities] 模組。</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL訂閱] </td> 
   <td> <p>選取選項以指定代理使用者是否訂閱展示板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL權限級別]</p> </td> 
   <td> <p>每個權限層級的董事會有不同的投票和留言規則。 例如：如果您的董事會是[!UICONTROL專用]，而您將投票和注釋規則設定為[!UICONTROL全部]，您將會收到錯誤。 </p> <p>每個權限層級的投票和評論僅限於下列群組：</p> 
    <ul> 
     <li><strong>[!UICONTROL專用]</strong>:—&gt;成員、成員和觀察員</li> 
     <li><strong>[!UICONTROL（適用於組織）]</strong>:—&gt;成員、成員和觀察員、組織成員</li> 
     <li><strong>[!UICONTROL公用]</strong>:—&gt;成員、成員和觀察員、組織成員、全部</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL投票]</p> </td> 
   <td> <p>選擇一個選項，以指定誰可以在此板上投票。 請參閱[!UICONTROL權限層級]欄位，了解權限層級的投票限制。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL注釋]</p> </td> 
   <td> <p>選取選項，以指定誰可以對此展示板的資訊卡加上註解。 請參閱[!UICONTROL權限級別]欄位，以了解對權限級別的注釋限制。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL邀請] </td> 
   <td> <p>選取可以邀請人員加入此展示板的人員。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL自聯接]</td> 
   <td> <p> 選擇團隊成員是可以自己加入董事會還是必須受邀。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL卡蓋]</td> 
   <td> <p> 選取此展示板上是否應顯示資訊卡封面。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL背景] </td> 
   <td> <p>選取背景或自訂背景的顏色。</p> <p>注意：自訂背景僅適用於[!UICONTROL Trello Gold and Business Class]訂閱者。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL背景ID]</td> 
   <td> <p> 如果您已在[!UICONTROL背景]欄位中選擇使用自定義背景，請輸入或映射要使用的背景的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL卡老化]</p> </td> 
   <td> <p>在兩種卡老化模式之間進行選擇。 </p> 
    <ul> 
     <li><strong>[!UICONTROL常規]</strong>:卡片隨著年齡增長而逐漸變得透明。 </li> 
     <li><strong>[!UICONTROL海盜]</strong>:卡片會像老海盜地圖一樣撕破，變黃，變老。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！啟用UICONTROL日曆摘要]</td> 
   <td> <p> 選取是否啟用日曆摘要。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;color&gt; 標籤名稱]</td> 
   <td> <p> 將名稱指派給所需的顏色標籤。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存檔] </td> 
   <td> <p>選取選項，以指出您是否要封存（關閉）展示板。 </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 取得展示板]**

此動作模組會擷取展示板的詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL主板ID]</p> </td> 
   <td> <p>輸入或對應您要擷取相關資訊之展示板的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

此搜尋模組會擷取您所指定展示板的相關資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢] </td> 
   <td> <p>輸入或映射您要取得相關資訊的展示板名稱（或部分名稱）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回的展示板的最大數量]</td> 
   <td> <p> 輸入展示板的最大數量 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。 此值必須小於或等於1000。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL部分] </p> </td> 
   <td> <p>預設情況下，此模組將搜索成員內容，以查找查詢中每個單詞的完全匹配項。 啟用[!UICONTROL Partial]時，模組會尋找以查詢中任何字詞開頭的內容。</p> <p> 例如，如果您使用「開發」一詞來尋找標題為「我的開發狀態報表」的展示板，依預設，您需要搜尋整個字詞。 如果您已啟用[!UICONTROL Partial]，便可搜尋「dev」而非「development」。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL展示板] </td> 
   <td> <p>輸入"mine"或映射以逗號分隔的展示板ID清單。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 封存或取消封存展示板]**

此動作模組會關閉或重新開啟您指定的展示板。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主板ID]</td> 
   <td> <p> 輸入或對應您要關閉或重新開啟之展示板的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存檔或取消存檔]</td> 
   <td> <p> 選取您要關閉（封存）或重新開啟（取消封存）展示板。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 將成員分配給展示板]**

此動作模組會將成員指派給您指定的展示板。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主板ID]</td> 
   <td> <p> 選擇要添加成員的展示板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL電子郵件地址]</td> 
   <td> <p> 輸入或映射要添加到展示板的成員的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL成員類型]</p> </td> 
   <td> <p>選擇要添加到展示板的成員類型。</p> 
    <ul> 
     <li><strong>[!UICONTROL管理員]</strong>:展示板管理員可以在展示板上執行任何展示板操作。</li> 
     <li><strong>[!UICONTROL標準]</strong>:一般成員只是董事會成員。</li> 
     <li><strong>[!UICONTROL觀察者]</strong>:觀察者是可唯讀存取展示板的成員。 <br>只有具有[!UICONTROL Trello Business Class]的團隊才能使用觀察員。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL全名]</td> 
   <td> <p> 輸入您要新增至展示板的使用者的完整名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 從展示板取消指派成員]**

此動作模組會從展示板中移除成員。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主板ID]</td> 
   <td> <p> 輸入（映射或選擇）您要移除使用者的展示板ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL成員] </td> 
   <td> <p>選擇要從展示板中刪除的成員。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 清單

+++ **[!UICONTROL 監看卡已移至清單]**

將資訊卡移至特定清單時，此觸發器模組會啟動。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主板]</td> 
   <td>選取包含您要監看資訊卡清單的展示板。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL清單]</td> 
   <td>選取您要監看卡片的清單。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>卡的最大數量 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 建立清單]**

此動作模組會在您指定的展示板上建立清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主板ID]</td> 
   <td> <p> 輸入或對應您要建立清單的展示板ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名稱] </td> 
   <td> <p>輸入或映射新清單的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL位置] </td> 
   <td> <p>選取您要將清單新增至頂端，還是將其附加至卡片底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL複製清單]</td> 
   <td> <p> 選擇要如何輸入要複製的清單的ID。</p> 
    <ul> 
     <li> <p><strong>手動輸入</strong> </p> <p>在 <strong>[!UICONTROL清單ID]</strong> 欄位中，輸入或映射要複製的清單的ID。<br></p> </li> 
     <li> <p><strong>選取</strong> </p> <p>選取包含您要複製之清單的展示板，然後選取清單。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 編輯清單]**

此動作模組會編輯現有清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL清單ID]</td> 
   <td> <p> 輸入或對應您要更新的清單ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名稱] </td> 
   <td> <p>輸入或映射清單的新名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主板ID]</td> 
   <td> <p> 對應或選取您要移動清單的展示板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL位置] </td> 
   <td> <p>選取您要將清單新增至頂端，還是將其附加至卡片底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL已訂閱]</td> 
   <td> <p>如果要將活動成員訂閱到清單中，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 取得清單]**

此動作模組會擷取特定清單的詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL清單ID]</p> </td> 
   <td> <p>輸入或映射要檢索相關資訊的清單的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 卡片

+++ **[!UICONTROL 手錶卡]**

新增卡片時，此觸發程式模組已啟動。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watched對象]</td> 
   <td> <p>選取您要監視卡片的位置。</p> 
    <ul> 
     <li><strong>[!UICONTROL所有卡]</strong> </li> 
     <li> <p><strong>特定主板上的卡</strong> </p> <p>選取您要監看資訊卡的展示板</p> </li> 
     <li> <p><strong>[！特定清單上的UICONTROL卡]</strong> </p> <p>選取包含您要監看卡片清單的展示板，然後選取清單。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>卡的最大數量 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 建立資訊卡]**

此動作模組會在選取的清單中建立資訊卡。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入清單ID]</td> 
   <td> <p> 選取您要如何輸入要新增資訊卡之清單的ID。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在 <strong>[!UICONTROL清單ID]</strong> 欄位中，輸入或映射您要新增資訊卡的清單ID。<br></p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選取包含您要複製之清單的展示板，然後選取清單。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤] </td> 
   <td> <p>對於您要新增至卡片的每個標籤，輸入標籤的ID。 例如，可使用[!UICONTROL擷取標籤]模組來擷取ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL成員]</td> 
   <td>對於要添加到卡的每個成員，輸入該成員的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名稱] </td> 
   <td> <p>輸入新卡的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL描述]</p> </td> 
   <td> <p>輸入資訊卡的說明。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL位置] </td> 
   <td> <p>選取要將卡片新增至頂端，還是將卡片附加至清單底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL到期日]</td> 
   <td> <p> 輸入卡的到期日。 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL到期完成]</td> 
   <td> <p> 啟用此選項可將卡片標示為到期日已完成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案URL]</td> 
   <td> <p>輸入或對應您要新增為資訊卡附件之檔案的URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL源檔案]</p> </td> 
   <td> <p>輸入或映射要作為附件添加到卡的檔案的資訊。</p> 
    <ul> 
     <li>[!UICONTROL檔案名]:輸入或映射檔案名，包括副檔名。</li> 
     <li> 
     <p>從上一個模組中選擇檔案，或映射檔案的名稱和資料</p> 
     <p>注意：每個附件有10 MB的檔案上傳限制。 但是，[!UICONTROL業務類]和[!UICONTROL Trello Gold]成員的每個附件有250 MB的檔案上載限制。</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL複製卡]</td> 
   <td> <p> 選取您要如何輸入要複製之資訊卡的ID。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在 <strong>[!UICONTROL卡ID]</strong> 欄位中，輸入或對應您要複製之資訊卡的ID。<br></p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選取包含您要複製之卡片的展示板，然後選取包含卡片的清單，然後選取卡片。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 編輯資訊卡]**

此動作模組會編輯現有的資訊卡。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入卡ID]</td> 
   <td> <p> 選取要如何輸入要編輯之資訊卡的ID。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在 <strong>[!UICONTROL卡ID]</strong> 欄位中，輸入或對應您要編輯的資訊卡ID。<br></p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選取包含您要編輯之卡片的展示板，然後選取包含卡片的清單，然後選取卡片。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL新名稱]</td> 
   <td> <p>輸入或映射卡片的新名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL新說明]</p> </td> 
   <td> <p>輸入或映射卡的新說明。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL移動卡]</p> </td> 
   <td> <p>選取展示板或展示板，並列出您要移動資訊卡的位置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤] </td> 
   <td> <p>新增您要新增至卡片之任何標籤的ID。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL位置] </td> 
   <td> <p>選取要將卡片新增至頂端，還是將卡片附加至清單底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL到期日]</td> 
   <td> <p> 輸入卡的到期日。 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL到期完成]</td> 
   <td> <p> 如果啟用此選項，卡片會在到期日標示為完成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL成員] </td> 
   <td> <p>添加或映射要添加到卡的任何成員的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件封面ID]</p> </td> 
   <td> <p>輸入或映射您希望卡片用作封面的影像附件ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL訂閱] </td> 
   <td> <p>選擇是否應該訂閱成員卡。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存檔] </td> 
   <td> <p>選取選項以指出您是否要封存（關閉）資訊卡。 </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 取得資訊卡]**

此動作模組會擷取選取卡片的詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主板ID]</td> 
   <td> <p>輸入展示板的ID，該展示板包含您要擷取其詳細資訊的資訊卡。 這可讓您查看展示板的自訂欄位名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入卡ID]</td> 
   <td> <p> 選取您要如何輸入要擷取其詳細資訊之資訊卡的ID。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在 <strong>[!UICONTROL卡ID]</strong> 欄位中，輸入或映射要檢索詳細資訊的卡的ID。<br></p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選取包含您要擷取其詳細資訊之資訊卡的展示板，然後選取包含該資訊卡的清單，然後選取資訊卡。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 搜尋卡片]**

此動作模組會傳回與搜尋查詢相符的卡片。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主板] </td> 
   <td> <p>選取您要搜尋的展示板。 如果未選取任何展示板，則會搜尋所有展示板。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL查詢]</p> </td> 
   <td> <p>輸入搜索查詢。 您可以使用下列搜尋運算子來調整搜尋範圍：</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>您可以新增「 — 」至任何運算子，以執行否定搜尋，例如 <code>[!UICONTROL -has:members]</code> 搜索未分配任何成員的卡。</p> </li> 
     <li><code><strong>@name</strong></code> <p>返回分配給成員的卡。 您也可以使用 <code>member:</code>. 使用 <code>@me</code> 僅包含卡片。</p> </li> 
     <li><code><strong>#label</strong></code> <p>傳回標示為的卡片。 您也可以使用 <code>label:</code>. 例如， <code>label:"FIX IT"</code> 會傳回標籤為「FIX IT」的卡片。</p> </li> 
     <li><code><strong>board:id</strong></code> <p>傳回特定展示板內的資訊卡。 例如， <code>board:Trello</code> 會傳回展示板名稱中具有[!UICONTROL Trello]的展示板上的資訊卡。</p> </li> 
     <li><code><strong>list:name</strong></code> <p>傳回名為「name」的清單中的卡片。</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>傳回附件的卡片。 此 <code>has</code>:運算子也可搭配其他屬性使用，例如 <code>has:description</code>, <code>has:cover</code>, <code>has:members</code>，或 <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>傳回24小時內到期的卡。 此 <code>due:</code> 運算子也可搭配其他時間範圍使用，例如 <code>due:week</code>, <code>due:month</code>，或 <code>due:overdue</code>. 您也可以搜尋特定的日期範圍。 例如，新增 <code>due:14</code> 要搜索的資訊卡包括未來14天到期的資訊卡。</p> </li> 
     <li><code><strong>created:day</strong></code> <p>傳回過去24小時內建立的資訊卡。 此<code> created:</code> 運算子也可搭配其他時間範圍使用，例如 <code>created:week</code> 或 <code>created:month</code>. 您也可以搜尋特定的日期範圍。 例如，新增 <code>created:14</code> 搜尋包含過去14天內建立的資訊卡。</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>傳回過去24小時內編輯的資訊卡。 此 <code>edited:</code> 運算子也可搭配其他時間範圍使用，例如 <code>edited:week</code> 或 <code>edited:month</code>. 您也可以搜尋特定的日期範圍。 例如，新增 <code>edited:21</code> 搜尋包含在過去21天內編輯的資訊卡。</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>傳回與卡片說明、核取清單、留言或名稱文字相符的卡片。 例如，註解："FIX IT"會傳回備注中含有"FIX IT"的資訊卡。</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>傳回已開啟或封存的資訊卡。 如果兩者都未指定，則[!UICONTROL Trello]將返回這兩種類型。</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>只包括有星號的牌。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回卡的最大數量]</td> 
   <td> <p> 卡的最大數量 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。 此值必須小於或等於1000。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL部分] </td> 
   <td> <p>預設情況下，此模組將搜索成員內容，以查找查詢中每個單詞的完全匹配項。 啟用[!UICONTROL Partial]時，模組會尋找以查詢中任何字詞開頭的內容。</p> <p> 例如，如果您使用「開發」一詞來尋找標題為「我的開發狀態報表」的展示板，依預設，您需要搜尋整個字詞。 如果您已啟用[!UICONTROL Partial]，便可搜尋「dev」而非「development」。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL卡] </td> 
   <td> <p>新增您要特別搜尋的任何卡片。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 封存或取消封存資訊卡]**

此動作模組會封存或將資訊卡傳回展示板。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL卡ID]</td> 
   <td> <p> 輸入或對應您要封存或傳回展示板的資訊卡ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL存檔或取消存檔]</td> 
   <td> <p> 選取您要關閉資訊卡（封存）或將資訊卡傳回展示板（取消封存）。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 新增附件]**

此動作模組會將附件新增至選取的卡片。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入卡ID]</td> 
   <td> <p> 選取您要如何輸入要擷取其詳細資訊之資訊卡的ID。</p> 
    <ul> 
     <li> <p><strong>手動輸入</strong> </p> <p>在 <strong>[!UICONTROL卡ID]</strong> 欄位中，輸入或映射要檢索詳細資訊的卡的ID。<br></p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選取包含您要擷取其詳細資訊之資訊卡的展示板，然後選取包含該資訊卡的清單，然後選取資訊卡。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件類型]</p> </td> 
   <td> <p>選取您要直接上傳檔案，還是提供檔案的URL。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL檔案]</strong> </p> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </li> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>輸入檔案的URL，並提供附件的名稱。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 成員

+++ **[!UICONTROL 將成員分配給展示板]**

請參閱「[!UICONTROL 將成員分配給展示板]「」 [展示板](#boards).

+++

+++ **[!UICONTROL 從展示板取消指派成員]**

請參閱「[!UICONTROL 從展示板取消指派成員]「」 [展示板](#boards).

+++

+++ **[!UICONTROL 向卡添加成員]**

此操作模組將指定的成員添加到指定的卡。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL輸入卡ID和成員ID]</p> </td> 
   <td> <p>選擇要如何輸入卡ID和成員ID。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或對應 <strong>[!UICONTROL卡ID]</strong> 和 <strong>[!UICONTROL成員ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選擇包含要添加成員的卡的板，然後選擇包含卡的清單、卡本身以及要添加到卡的成員。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 搜尋成員]**

此動作模組會擷取 [!UICONTROL 特雷洛] 成員。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢] </td> 
   <td> <p>輸入要查找的用戶的完整名稱或用戶名。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL部分] </td> 
   <td> <p>預設情況下，此模組將搜索成員內容，以查找查詢中每個單詞的完全匹配項。 啟用[!UICONTROL Partial]時，模組會尋找以查詢中任何字詞開頭的內容。</p> <p> 例如，如果您使用「開發」一詞來尋找標題為「我的開發狀態報表」的展示板，依預設，您需要搜尋整個字詞。 如果您已啟用[!UICONTROL Partial]，便可搜尋「dev」而非「development」。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回成員的最大數]</td> 
   <td> <p> 成員數上限 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 核取清單

+++ **[!UICONTROL 建立檢查清單]**

此動作模組會在選取的卡片上建立檢查清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入卡ID]</td> 
   <td> <p> 選取要如何輸入要新增檢查清單之資訊卡的ID。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在 <strong>[!UICONTROL卡ID]</strong> 欄位中，輸入或對應您要新增檢查清單的資訊卡ID。<br></p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選取包含卡片的展示板，您要新增檢查清單，然後選取包含卡片的清單，然後選取卡片。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名稱] </td> 
   <td> <p>輸入或映射檢查清單的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL位置] </td> 
   <td> <p>選擇要將檢查清單添加到頂部，還是將[!UICONTROL]檢查清單附加到卡的底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL輸入檢查清單ID]</p> </td> 
   <td> <p>輸入或映射要複製到新清單的源檢查清單的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 建立檢查清單項目]**

此動作模組會將項目新增至特定檢查清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入檢查清單ID]</td> 
   <td> <p> 選擇要如何輸入要添加項的檢查清單的ID。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在 <strong>[!UICONTROL檢查清單ID]</strong> 欄位中，輸入或對應您要新增檢查清單的資訊卡ID。<br></p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選取包含卡片的展示板，您要新增檢查清單，然後選取包含卡片的清單，然後選取卡片，再選取檢查清單。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL項目名稱]</p> </td> 
   <td> <p>輸入或映射新項的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL位置]</p> </td> 
   <td> <p>選擇要將項目添加到清單的頂部，還是將[!UICONTROL附加]添加到清單的底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！已檢查UICONTROL]</p> </td> 
   <td> <p>如果要按已勾選的項目新增項目，請啟用此選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 編輯檢查清單項目]**

此動作模組會編輯現有的檢查清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入卡ID和檢查清單項ID]</td> 
   <td> <p> 選擇要如何輸入要編輯項目的卡片和檢查清單的ID。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在 <strong>[!UICONTROL檢查清單ID]</strong> 欄位中，輸入或對應您要新增檢查清單的資訊卡ID。</p> <p>在 <strong>[!UICONTROL檢查清單項ID]</strong> 欄位，輸入或映射檢查清單的ID。</p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選取包含卡片的展示板，您要新增檢查清單，然後選取包含卡片的清單，然後選取卡片，再選取檢查清單。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檢查清單ID]</td> 
   <td>選擇或映射要將檢查清單項目移動到的檢查清單。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL項目名稱]</p> </td> 
   <td> <p>輸入或映射新項的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL位置]</p> </td> 
   <td> <p>選擇要將項目添加到清單的頂部還是附加到清單的底部。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL狀態]</p> </td> 
   <td> <p>選擇檢查清單項目是完成還是不完整。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 標籤

+++ **[!UICONTROL 將標籤新增至卡片]**

此動作模組會將標籤新增至選取的卡片。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入卡ID]</td> 
   <td> <p> 選取要如何輸入要新增檢查清單之資訊卡的ID。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在 <strong>[!UICONTROL卡ID]</strong> 欄位中，輸入或對應您要新增檢查清單的資訊卡ID。 在<strong>[!UICONTROL標籤ID]</strong> 欄位中，輸入或映射要添加的標籤的ID。<br></p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選取包含卡片的展示板，您要新增檢查清單，然後選取包含卡片的清單，然後選取卡片。 </p> <p>選取您要新增至卡片的標籤。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### 註解

+++ **[!UICONTROL 觀看留言]**

在指定位置中有新注釋時檢索注釋詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watched對象]</td> 
   <td> <p>選擇要監視的注釋位置。</p> 
    <ul> 
     <li><strong>所有位置的[!UICONTROL所有卡]</strong> </li> 
     <li> <p><strong>[!UICONTROL主板]</strong> </p> <p>選取您要留意的展示板</p> </li> 
     <li> <p><strong>[!UICONTROL清單]</strong> </p> <p>選取包含您要留意之清單的展示板，然後選取清單。</p> </li> 
     <li><strong>[!UICONTROL卡]</strong> </li> 
     <li>選取包含您要留意留言之資訊卡的展示板，然後選取包含資訊卡的清單，再選取資訊卡。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>留言數上限 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 在資訊卡中建立註解]**

此動作模組會將註解新增至選取的卡片。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入卡ID]</td> 
   <td> <p> 選取要如何輸入要新增註解之卡片的ID。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在 <strong>[!UICONTROL卡ID]</strong> 欄位中，輸入或對應您要新增註解的資訊卡ID。<br></p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選取包含您要新增註解之卡片的展示板，然後選取包含卡片的清單，然後選取卡片。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注釋] </td> 
   <td> <p>輸入要添加到選定卡的注釋。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 列出資訊卡中的註解]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將[!UICONTROL Trello]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入卡ID]</td> 
   <td> <p> 選取要如何輸入要新增註解之卡片的ID。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>在 <strong>[!UICONTROL卡ID]</strong> 欄位中，輸入或對應您要新增註解的資訊卡ID。<br></p> </li> 
     <li> <p><strong>[!UICONTROL選擇]</strong> </p> <p>選取包含您要新增註解之卡片的展示板，然後選取包含卡片的清單，然後選取卡片。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回的注釋數上限]</td> 
   <td> <p> 輸入注釋的最大數量 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sine] </td> 
   <td> <p>設定建立評論的期間的開始日期。 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL之前] </td> 
   <td> <p>設定建立評論的期間的結束日期。 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL 特雷洛] 物件ID

* [如何在 [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [如何在 [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### 如何在 [!DNL Trello]

如果您想要編輯資訊卡或建立新留言，則需知道資訊卡的ID或其短連結。 您可以從的輸出取得此資訊 [!UICONTROL 新卡] 觸發。 通過開啟卡並按一下 [!UICONTROL 共用] 按鈕。 在 [!UICONTROL 連結到此卡] 框，在URL的結尾處 `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### 如何在 [!DNL Trello]

只能使用觸發器取得展示板、清單和留言ID。 此 [!DNL trello.com] 網站不會顯示這些ID。
