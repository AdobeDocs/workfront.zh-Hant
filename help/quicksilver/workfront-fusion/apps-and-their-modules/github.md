---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: GitHub模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用GitHub的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 5e520aab-8307-4a52-96b6-13b284f9cb53
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 0%

---

# [!DNL GitHub] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!UICONTROL GitHub]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!DNL GitHub] 模組，必須有 [!DNL GitHub] 帳戶。

## Connect [!DNL GitHub] to [!DNL Workfront Fusion]

有關連接 [!DNL GitHub] 帳戶 [!UICONTROL Workfront融合]，請參閱 [建立連線至 [!UICONTROL Adobe Workfront融合]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL GitHub] 模組及其欄位。

設定時 [!DNL GitHub] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL GitHub] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)

### 觸發器

* [[!UICONTROL 監看問題]](#watch-issues)
* [[!UICONTROL 監視儲存庫]](#watch-repositories)
* [[!UICONTROL 沃奇福克斯]](#watch-forks)
* [[!UICONTROL 觀看留言]](#watch-comments)
* [[!UICONTROL 監看提取請求]](#watch-pull-requests)

#### [!UICONTROL 監看問題]

新增新問題或修改現有問題時，此模組就會觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL我想看]</td> 
   <td>選擇要監視所有儲存庫，還是僅監視一個儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>如果您選擇只監視一個儲存庫中的問題，請選擇要監視的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回問題的最大數量]</td> 
   <td>設定 [!DNL Workfront Fusion] 可在一個週期中運作。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>選取您只想關注新問題、新問題和所有變更。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL篩選器]</td> 
   <td> <p>您可以依關聯方式來篩選您要關注的問題。</p> 
    <ul> 
     <li>[!UICONTROL所有問題]</li> 
     <li>[!UICONTROL僅分配給我的問題]</li> 
     <li>[!UICONTROL僅由我建立的問題]</li> 
     <li>[!UICONTROL僅關於我的問題]</li> 
     <li>[!UICONTROL僅我已訂閱的更新]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL狀態]</td> 
   <td>選取您只要關注未結問題，或僅關注已結問題。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤]</td> 
   <td>新增標籤。 模組會監視此標籤的問題。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監視儲存庫]

建立或修改存放庫時，此模組就會觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回的儲存庫的最大數量]</td> 
   <td>設定 [!DNL Workfront Fusion] 可在一個週期中運作。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>選擇您要查看新儲存庫和所有更改，還是僅查看新儲存庫。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 沃奇福克斯]

建立新復本時，此模組就會觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇要監視福克斯的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回的分叉數上限]</td> 
   <td>設定 [!DNL Workfront Fusion] 可在一個週期中運作。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看留言]

新增新留言或修改現有留言時，此模組就會觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇要監視的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL問題編號]</td> 
   <td>如果要僅搜索對特定問題作出的新評論來限制搜索，請輸入問題編號。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回問題的最大數量]</td> 
   <td>設定 [!DNL Workfront Fusion] 可在一個週期中運作。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>選擇是否只監視新留言、留言和所有更改。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監看提取請求]

新增提取請求或修改現有提取請求時，此模組就會觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇要監視的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回提取請求的最大數]</td> 
   <td>設定 [!DNL Workfront Fusion] 可在一個週期中運作。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL狀態]</td> 
   <td>選取您要監看[!UICONTROL僅開啟提取]請求、[!UICONTROL僅關閉一個]請求，還是所有提取請求。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch]</td> 
   <td>選取您只想查看新提取請求，或新提取請求和所有變更。</td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 搜尋問題]](#search-for-an-issue)
* [[!UICONTROL 建立問題]](#create-an-issue)
* [[!UICONTROL 更新問題]](#update-an-issue)
* [[!UICONTROL 取得問題]](#get-an-issue)
* [[!UICONTROL 添加受分配者]](#add-assignees)
* [[!UICONTROL 刪除受分配者]](#remove-assignees)
* [[!UICONTROL 將標籤添加到問題]](#add-labels-to-an-issue)
* [[!UICONTROL 從問題中移除標籤]](#remove-a-label-from-an-issue)
* [[!UICONTROL 建立注釋]](#create-a-comment)
* [[!UICONTROL 列出注釋]](#list-comments)

#### [!UICONTROL 搜尋問題]

此模組會搜尋符合您搜尋條件的問題。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回問題的最大數量]</td> 
   <td>設定 [!DNL Workfront Fusion] 將在一個週期中運作（每個方案執行的重複次數）。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序依據]</td> 
   <td> <p>選擇要如何對搜索結果進行排序。</p> 
    <ul> 
     <li> <p>[!UICONTROL最匹配] </p> </li> 
     <li>[!UICONTROL建立日期]</li> 
     <li>[!UICONTROL更新日期]</li> 
     <li>[!UICONTROL注釋數]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序方向]</td> 
   <td> <p>選擇升序或降序。 </p> <p>日期，請選取 <strong>[!UICONTROL降序]</strong> 會先傳回最近的日期。 </p> <p>對於[!UICONTROL注釋數]，選擇 <strong>[!UICONTROL降序]</strong> 會先傳回評論數最多的問題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢]</td> 
   <td>輸入或映射您的搜索查詢。 有關搜索選項的詳細說明，請參閱 <a href="https://docs.github.com/en/github/searching-for-information-on-github/searching-issues-and-pull-requests">搜尋問題和提取請求</a> 在 [!DNL GitHub] 說明網站。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立問題]

此模組會在選取的存放庫中建立新問題。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇要在中建立問題的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL受託人]</td> 
   <td>選擇要指派給問題的人員。 可用的受分配者包括對儲存庫具有寫入權限的任何人，以及對儲存庫具有讀取權限的組織成員。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL里程碑]</td> 
   <td>選取您要與新問題建立關聯的里程碑。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤]</td> 
   <td>選擇要應用於新期的任何標籤。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td>輸入或映射新期的標題。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td>輸入或映射問題的正文，如說明或附加資訊</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新問題]

此模組會更新現有 [!DNL GitHub] 問題。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇要在中更新問題的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL受託人]</td> 
   <td>選擇要指派給問題的人員。 可用的受分配者包括對儲存庫具有寫入權限的任何人和對儲存庫具有讀取權限的組織成員。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL里程碑]</td> 
   <td>選取您要與問題關聯的里程碑。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤]</td> 
   <td>選擇要應用到問題的任何標籤。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL編號]</td> 
   <td>輸入或映射要更新的問題的問題編號。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL狀態]</td> 
   <td>選取您要將問題更新為的狀態。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td>輸入或映射問題的標題。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td>輸入或映射問題的正文，如說明或附加資訊</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得問題]

此模組會擷取指定問題的詳細資訊

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇包含要檢索詳細資訊的問題的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL編號]</td> 
   <td>輸入或映射要檢索詳細資訊的問題的問題編號。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加受分配者]

此模組將受分配者添加到指定問題

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇包含要向其添加受分配者的問題的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL受託人]</td> 
   <td>選擇要指派給問題的人員。 可用的受分配者包括對儲存庫具有寫入權限的任何人和對儲存庫具有讀取權限的組織成員。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL編號]</td> 
   <td>輸入或映射要添加受分配者的問題的問題編號。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除受分配者]

此模組會從指定的問題中刪除受分配者。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇包含要從中刪除受分配者的問題的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL受託人]</td> 
   <td>選擇要從問題中刪除的人員。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL編號]</td> 
   <td>輸入或映射要從中刪除受分配者的問題的問題編號。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將標籤添加到問題]

此模組會將標籤新增至問題。 標籤是在儲存庫級別定義的，只能由具有儲存庫寫入權限的人建立。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇包含要添加標籤的問題的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤]</td> 
   <td>選擇要添加到問題的標籤。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL編號]</td> 
   <td>輸入或映射要添加標籤的問題的問題編號。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從問題中移除標籤]

此模組會從問題中移除單一標籤。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇包含要從中刪除標籤的問題的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤]</td> 
   <td>選擇要從問題中刪除的標籤。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL編號]</td> 
   <td>輸入或映射要從中刪除標籤的問題的問題編號。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立注釋]

此模組會針對指定的問題建立註解。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇包含要建立評論的問題的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL編號]</td> 
   <td>輸入或映射要建立評論的問題的問題編號。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td>輸入或映射注釋的內容。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出注釋]

此模組會列出指定問題的所有評論。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL GitHub] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL儲存庫]</td> 
   <td>選擇要列出評論的問題的儲存庫。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL編號]</td> 
   <td>輸入或映射要列出評論的問題的問題編號。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sine]</td> 
   <td>模組將傳回在此日期之後建立的註解。 如需支援的日期格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回的注釋數上限]</td> 
   <td>設定 [!DNL Workfront Fusion] 可在一個週期中運作。 </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Troubleshooting</h2>
-->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Module does not receive any events</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a module does not receive any events, check the webhook settings in Github and make sure that:</p>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have set the correct type of event that the chosen module should receive</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have entered the correct Payload URL</p>
  -->
