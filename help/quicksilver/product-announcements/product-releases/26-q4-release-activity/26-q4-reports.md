---
title: 2026年第四季報表增強功能
description: 2026年第四季報表增強功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: 3599b27bb1b838ebe7d0a2648e6c67333da83dc8
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 2%
---
# 2026年第四季報表增強功能

本頁說明2026年第四季版本針對預覽環境所進行的報告增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2026年第四季版本週期目前可用的所有變更清單，請參閱[2026年第四季版本概觀](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)。

## Google Cloud Platform和Microsoft Azure現在提供畫布控制面板

>[!NOTE]
>
>預覽：不適用
>生產快速發行： 2026年10月14日
>適用於所有人的生產： 2026年10月15日

Google Cloud Platform (GCP)和Azure上的Workfront執行個體現在可以選擇加入「畫布控制面板」開放Beta版。 如需詳細資訊，請參閱[使用畫布儀表板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md)。

## 註冊Workfront Data Connect的Snowflake私人清單

>[!NOTE]
>
>預覽：不適用
>生產快速發行： 2026年10月14日
>適用於所有人的生產： 2026年10月15日

您現在可以透過註冊私人清單，直接與組織的Snowflake帳戶共用您的Workfront Data Connect資料。 此連線方法使用Snowflake的私人清單功能，在不公開資料的情況下在組織之間安全地共用資料，並且跨地區和託管平台運作。

當您想要將Workfront資料與企業資料倉儲中的其他資料結合時，私人清單會很有用。 由於資料位於您自己的Snowflake帳戶中，因此您可以連同其他資料一起查詢。

如需詳細資訊，請參閱[註冊Workfront資料連線的私人清單](/help/quicksilver/reports-and-dashboards/data-lake/register-a-private-listing.md)。

## 報告MCP工具現在可用於畫布儀表板

>[!NOTE]
>
>預覽： 2026年10月1日
>生產快速發行： 2026年10月14日
>適用於所有人的生產： 2026年10月15日

為了更方便使用畫布控制面板，我們在Workfront MCP中新增了工具。 現在，您可以透過聊天來建立和管理Canvas控制面板，而且控制面板和Widget都是使用您的Workfront資料為您建立的。 這適用於Claude和Cursor等MCP使用者端。

例如，您可以：

* 透過詢問建立報告。 以自然語言描述儀表板或圖表，而非手動建置。
* 就地編輯。 要求重新命名Widget、變更篩選器、交換圖表型別或調整大小，而變更會套用至即時儀表板。
* 重複使用您擁有的資源。 複製現有的儀表板或Widget作為起點，而非從頭重建。

### 支援的功能

**儀表板**

* 建立新儀表板
* 列出您的儀表板（您的、與您共用、全部或我的最愛），並按標題搜尋
* 開啟或檢視控制面板的結構
* 更新標題、說明、貨幣、篩選和提示
* 複製儀表板（無論是否包含其Widget、提示和篩選器）
* 刪除儀表板

**介面工具集**

* KPI — 單一彙總數字（總計、平均值、計數、最小值、最大值等）
* 圖表 — 長條圖、直條圖、折線圖和圓餅圖；支援簡單、多系列和棧疊圖表
* 表格 — 具有列群組的多欄表格
* 檢視Widget的設定，以及更新、複製、調整大小或重新定位，或刪除它

**報告選項**

* 使用條件和AND/OR群組篩選資料
* 依任何欄位分組和彙總
* 從重要績效指標或圖表向下追溯至基礎記錄
* 自訂欄標籤、數字、日期和貨幣格式，以及條件式儲存格樣式
* 儀表板層級提示和篩選器

如需詳細資訊，請參閱[使用畫布儀表板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md)。

## 在畫布儀表板之間複製或移動Widget

>[!NOTE]
>
>預覽： 2026年10月1日
>生產快速發行： 2026年10月14日
>適用於所有人的生產： 2026年10月15日

您現在可以將Widget複製到相同儀表板、您擁有編輯存取權的另一個儀表板或新儀表板。 您也可以將Widget移至您對其擁有編輯存取權的另一個儀表板，或移至新儀表板。

當您複製Widget時，將會開啟一個對話方塊，您可在其中選取目標控制面板以及是否要複製或移動Widget。 過去，Report Builder會立即開啟。

## 在畫布儀表板中篩選集合關係

>[!NOTE]
>
>預覽： 2026年10月1日
>生產快速發行： 2026年10月14日
>適用於所有人的生產： 2026年10月15日

當您在「畫布控制面板」中建立篩選器時，現在可以依集合關係進行篩選，這些欄位會連結至一組相關記錄，而非單一記錄。 例如，您可以篩選屬於專案之任務的狀態，以顯示具有「新」狀態任務的專案清單。

以前，篩選集合關係需要文字模式。

如需詳細資訊，請參閱[畫布控制面板的報告篩選器參考](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md)。

## 在畫布儀表板中複製儀表板

>[!NOTE]
>
>預覽： 2026年9月3日
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日

您現在可以使用新的&#x200B;**複製儀表板**&#x200B;動作來複製畫布儀表板。 任何使用者的存取層級授予控制面板的編輯或建立許可權時，都可以使用此動作，即使他們只有所複製之特定控制面板的檢視存取權。 沒有控制面板編輯或建立許可權的使用者看不到此動作。

當您複製儀表板時，可以重新命名儀表板、更新其說明和貨幣，以及選擇要延續到副本的Widget、儀表板篩選器和儀表板提示。

只有當您是指定的使用者或系統管理員時，才會保留Widget上的執行身分使用者設定。 共用偏好設定不會複製到新儀表板，並在複製完成後顯示一則確認訊息，其中包含新儀表板的連結。

過去，無法複製儀表板；使用者必須從頭開始重建儀表板，以建立對象特定變數。

## 畫布儀表板中的核准型別欄位

>[!NOTE]
>
>適用於所有人的生產： 2026年8月28日
>[!BADGE 不在排程]{type=Neutral}內

核准實體現在包含&#x200B;**核准型別**&#x200B;欄位，可讓使用者區分校訂核准、檔案版本核准、接收核准和其他核准型別。

## 畫布儀表板中的核准術語更新

>[!NOTE]
>
>適用於所有人的生產： 2026年8月28日
>[!BADGE 不在排程]{type=Neutral}內

為了清楚起見，已重新命名下列在畫布儀表板中用於檔案和工作核准的欄位名稱：

| 前一個名稱 | 新名稱 |
| --- | --- |
| 文件核准 | 核准 |
| 文件核准階段 | 核准階段 |
| 文件核准階段參與者 | 核准階段參與者 |
| 核准流程 | 工作核准流程 |
| 核准階段 | 工作核准階段 |
| 核准者狀態 | 工作核准者狀態 |
| 正在等待核准 | 正在等待工作核准 |

此變更不會影響目前報表的運作方式。

## 畫布儀表板中的樞紐分析表報表

>[!NOTE]
>
>預覽： 2026年8月27日
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日

「畫布控制面板」中的新樞紐分析表報表型別，會以準確、完整的統計來彙總資料。 您可以直接在儀表板上建立計數、總和和平均等量度，然後深入研究任何總計背後的基礎記錄。

如需詳細資訊，請參閱[在畫布儀表板中建立樞紐分析表](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md)。

## 強制排程報表的結束日期

>[!NOTE]
>
>預覽： 2026年8月13日
>生產快速發行： 2026年9月17日
>適用於所有人的生產： 2026年10月15日

排程報告現在需要結束日期，以防止無限期傳送。 超過其結束日期的排程會自動停用。

現有排程已更新為結束日期，以提高可靠性並減少不必要的系統使用。 Workfront也提供可見度和警告，協助您在報表排程生命週期接近結束日期時加以管理。

如需詳細資訊，請參閱[排程自動報告傳遞](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)。

## 清單和報告有原生參考欄位可用

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

您現在可以在Workfront中，將原生參考欄位新增至清單和報表。

原生參考欄位是自訂欄位。 當欄位位於附加到物件的自訂表單上時，會從物件資料填入欄位。 例如，如果欄位參考說明欄位，並且它位於附加到專案的自訂表單上，則會提取專案說明。 （如果沒有可用資料，欄位可能會顯示「N/A」。）

如需有關建立原生參考欄位的資訊，包括支援原生欄位的清單，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
如需有關新增欄位至報表的資訊，請參閱[建立自訂報表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 舊版清單和報告的多重選取欄位值順序一致

>[!NOTE]
>
>預覽： 2026年7月30日
>生產快速發行： 2026年8月13日
>適用於所有人的生產： 2026年10月15日

您現在可以在舊版清單和報告上，以一致且可預測的順序，檢視多選自訂欄位的所選選項。 欄位順序取決於欄位在自訂表單中的排列方式。

![自訂表單欄位順序符合清單或報告中選取值的順序](assets/new-field-order-multi-select.png)

以前，選取的選項會以您選取它們的順序顯示，或是以不一致的順序顯示，這會使列更難以掃描和比較。

備註：如果欄位使用文字模式，則不會套用新排序。
