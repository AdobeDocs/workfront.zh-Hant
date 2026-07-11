---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP伺服器工具
description: 透過Adobe Workfront MCP伺服器可用的工具參考清單，按Workfront區域分組。
author: Courtney
feature: Get Started with Workfront
source-git-commit: 5592c1b93b5e44c732f92d626ed878d2c4647ceb
workflow-type: tm+mt
source-wordcount: '1788'
ht-degree: 5%

---


# Adobe Workfront MCP伺服器工具

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它只能在「預覽Sandbox」環境中使用。</span>

本文列出[!DNL Adobe Workfront] MCP伺服器公開至已連線之AI代理平台的工具。 當您要求平台尋找、建立、更新或刪除Workfront專案時，平台會代表您呼叫這些工具。

如需有關如何透過AI代理平台使用這些工具的資訊，請參閱[使用Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)。 如需如何設定連線的詳細資訊，請參閱[設定Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。

>[!IMPORTANT]
>
>AI代理平台會使用您的Workfront帳戶、存取層級和物件許可權，在Workfront中運作。 只有當您在Workfront中擁有對應的存取權時，工具才能運作。 Adobe對使用AI代理平台變更Workfront資料概不負責。


## 讀取和寫入動作

下清單格中的每個工具都會在「動作」欄中分類為「讀取」或「寫入」動作：

* **讀取**：從Workfront擷取資訊，但不變更您的資料。 例如，尋找專案、列出檔案或取得記錄的詳細資訊。
* **寫入**：建立、更新或刪除Workfront資料。 例如，建立專案、更新記錄或刪除檢視。

您的Workfront管理員可控制AI代理平台可以使用的工具類別，方法是透過系統偏好設定中的兩個切換：

* **唯讀MCP工具** （預設為啟用）
* **寫入MCP工具** （預設為停用）

如果AI代理平台可以找到Workfront專案，但無法建立、更新或刪除它們，請要求Workfront管理員啟用寫入動作。 如需詳細資訊，請參閱&#x200B;*設定Adobe Workfront MCP伺服器*&#x200B;中的[管理員必要條件](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#admin-prerequisites)。

## 核准工具

### 文件

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 依名稱尋找檔案版本 | `approvals_find_document_version_by_name` | 依檔案名稱查詢檔案的目前版本ID。 支援部分比對。 | 讀取 |
| 依版本ID取得檔案 | `approvals_get_document_by_version_id` | 會擷取已知檔案版本ID的檔案詳細資訊（名稱、大小、上傳日期、上傳程式）。 | 讀取 |
| 依專案取得檔案 | `approvals_get_documents_by_project` | 列出Workfront專案內的檔案，每個檔案的目前版本ID。 | 讀取 |
| 解析檔案範圍 | `approvals_resolve_document_scope` | 將專案或資料夾展開至其包含的檔案版本ID清單中。 支援專案、資料夾和依名稱資料夾範圍。 | 讀取 |

<!--
| List AEM-linked folders* | `approvals_list_aem_linked_folders` | Lists Workfront document folders that are linked to Adobe Experience Manager. | Read |
| Send documents to AEM folder* | `approvals_send_documents_to_aem_folder` | Moves one or more Workfront documents to an AEM-linked folder. | Write |

*You must have a native [!DNL Adobe Experience Manager] integration configured in your Workfront instance to use these tools. For more information, see [Overview of Adobe Experience Manager Assets integrations](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/aem-asset-integrations.md).


*Sending documents to an AEM folder is not yet supported for projects on Adobe cloud storage. Support is expected in a future release.

-->

### 核准工作流程

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 取得核准工作流程資訊 | `approvals_get_approval_info` | 傳回檔案版本的目前核准工作流程（階段、參與者、狀態）。 | 讀取 |
| 建立或更新核准工作流程 | `approvals_create_or_update_approval_workflow` | 建立或更新檔案版本的核准工作流程階段。 支援線性和平行（圖形）階段相依性。 | 寫入 |
| 從範本建立核准 | `approvals_create_approval_from_template` | 使用現有範本在檔案上建立核准工作流程。 | 寫入 |
| 刪除核准階段 | `approvals_delete_approval_stage` | 依名稱或職位從核准工作流程中刪除單一階段。 只能刪除未啟動的階段。 | 寫入 |

<!--
| Add and remove participants for an approval in bulk | `approvals_bulk_update_approval_participants`<br>`approvals__submit_bulk_update_approval_participants` | Adds or removes participants to or from multiple approvals at the same time. Currently, bulk updates can be applied only across a single project. Bulk updates across multiple projects will be available in the near future. | Write |
-->

<!--
| Request document approval | `approvals_request_document_approval` | Opens a guided form for requesting approval on a document version (title, approvers/reviewers, optional due date and message). | Write |
-->

### 提醒

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 傳送提醒給參與者 | `approvals_send_reminder_to_participants` | 傳送提醒電子郵件給核准階段中的特定參與者。 僅適用於已開始、未完成、未鎖定的階段。 | 寫入 |
| 傳送提醒給未決定的參與者 | `approvals_send_reminder_to_undecided` | 傳送提醒電子郵件給核准階段中所有未決定的參與者（通知、開啟或評論）。 | 寫入 |

### 核准範本

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 清單核准範本 | `approvals_list_templates` | 列出此Workfront例項中可用的核准範本。 支援依建立者、參與者及使用排序進行篩選。 | 讀取 |
| 依名稱搜尋範本 | `approvals_search_template_by_name` | 依名稱尋找核准範本（不區分大小寫的部分相符）。 | 讀取 |
| 建立核准範本 | `approvals_create_template` | 建立具有線性或圖表式階段相依性的新核准範本。 | 寫入 |
| 更新核准範本 | `approvals_update_template` | 使用結構化修改（新增或移除參與者、重新命名階段、設定截止日期等）更新現有範本。 | 寫入 |
| 大量提醒利害關係人核准 | `approvals_send_approval_reminder` | 傳送核准提醒電子郵件給整個專案、資料夾、行銷活動或到期日視窗中的所有待核准者。 | 寫入 |
| 大量更新核准範本 | `approvals_update_template` | 對多個範本執行範本更新，例如將範本套用至資產、從頭開始或從現有核准流程建立新範本、編輯範本，以及跨範本和資產執行大量作業。 | 寫入 |
| 大量新增或移除核准參與者。 | `approvals_update_approval_participants`和`approvals__submit_update_approval_participants` | 在一個作業中新增、移除或取代整個投資組合、方案或專案範圍內的參與者。 | 寫入 |


### 查閱和使用者

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 取得目前使用者 | `approvals_get_current_user` | 傳回呼叫使用者的Workfront身分，包括名稱、使用者ID、主團隊名稱和主團隊ID。 | 讀取 |
| 依名稱尋找使用者 | `approvals_find_user_by_name` | 依名稱查詢Workfront使用者的ID （模糊或部分相符）。 傳回名稱、ID、電子郵件、標題和顯示圖片URL。 | 讀取 |
| 依名稱尋找團隊 | `approvals_find_team_by_name` | 依名稱查詢Workfront團隊的ID （模糊或部分相符）。 | 讀取 |
| 依名稱尋找專案 | `approvals_find_project_by_name` | 依整個系統的部分名稱相符專案來查詢Workfront專案。 | 讀取 |
| 依所有者取得專案 | `approvals_get_projects_by_owner` | 列出呼叫使用者是擁有者的Workfront專案。 | 讀取 |
| 取得Adobe地區 | `approvals_get_adobe_region` | 傳回雲端提供者地區的Adobe名稱。 | 讀取 |

<!--

## Insights tools

Insights tools retrieve information about Workfront objects.

| Title | Tool name | What it does | Action |
| --- | --- | --- | --- |
| Read documents | `insights_read_docs` | Load the Workfront playbook or domain documentation, such as conditions, status, dates, or field paths. This is the required first step before querying data. | Read |
| Get current user | `insights_get_current_user` | Retrieve your own Workfront identity, including name, ID, and URL. | Read |
| Search fields | `insights_search_fields` | Search for available fields (standard and custom) on projects, tasks, issues, users, portfolios, teams, and so on. | Read |
| Get field paths | `insights_get_field_paths` | Resolve dot-notation field paths for entities, required by the data query tool. | Read |
| Find ID by name | `insights_find_id_by_name` | Look up the ID of any Workfront object by name, such as projects, tasks, users, portfolios, and so on. | Read |
| Find Workfront data | `insights_find_workfront_data` | Find, filter, count, sort, and aggregate Workfront data. This is the main query and report tool. | Read |
| Summarize object | `insights_summarize_object` | Fetch and summarize a single Workfront object by ID. | Read |
| List entities | `insights_list_entities` | List all Workfront object types available to query. | Read |

-->

## 規劃工具

>[!IMPORTANT]
>
>* 若要搭配Workfront Planning使用MCP，您的組織必須位於包含Adobe Workfront Planning的Workfront套件上。

### 工作區

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 取得工作區 | `planning_get_workspace` | 依ID或別名擷取工作區的完整詳細資料。 | 讀取 |
| 取得工作區清單 | `planning_get_workspace_list` | 列出所有可用工作區以及以游標為基礎的分頁。 | 讀取 |
| 建立工作區 | `planning_create_workspace` | 建立新的空白工作區以組織記錄型別、欄位和資料。 | 寫入 |
| 透過範本建立工作區 | `planning_create_workspace_from_template` | 使用現有範本建立預先填入的新工作區。 | 寫入 |
| 更新工作區 | `planning_update_workspace` | 部分更新工作區 — 名稱、說明、圖示、區段或擁有者。 | 寫入 |
| 刪除工作區 | `planning_delete_workspace` | 永久刪除工作區及其所有資料。 | 寫入 |
| 將工作區轉換為範本 | `planning_convert_workspace_to_template` | 將現有工作區儲存為可重複使用的範本（需要管理員）。 | 寫入 |
| 取得工作區共用 | `planning_get_workspace_sharing` | 傳回工作區的目前共用和許可權設定。 | 讀取 |
| 修改工作區共用 | `planning_modify_workspace_sharing` | 更新誰擁有工作區的存取權及許可權層級。 | 寫入 |

### 記錄類型

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 取得記錄型別 | `planning_get_record_type` | 擷取記錄型別的完整詳細資料，包括其欄位和檢視。 | 讀取 |
| 建立記錄型別 | `planning_create_record_types` | 在工作區區段中建立一或多個記錄型別。 | 寫入 |
| 更新記錄類型 | `planning_update_record_type` | 部分更新記錄型別的名稱、說明、圖示或顏色。 | 寫入 |
| 刪除記錄類型 | `planning_delete_record_type` | 永久刪除記錄型別及其所有記錄、欄位和檢視。 | 寫入 |
| 列出全域記錄型別 | `planning_list_global_record_types` | 列出目前使用者可見的所有集中定義（全域）記錄型別。 | 讀取 |
| 列出可新增的全域記錄型別 | `planning_list_addable_global_record_types` | 列出可新增至特定工作區的全域記錄型別。 | 讀取 |
| 將全域記錄型別新增至工作區 | `planning_add_global_record_type_to_workspace` | 將全域記錄型別連結至指定的工作區。 | 寫入 |
| 從工作區移除全域記錄型別 | `planning_remove_global_record_type_from_workspace` | 從工作區取消連結全域記錄型別；刪除該工作區中的所有記錄。 | 寫入 |
| 取得外部記錄工作區 | `planning_get_external_record_workspaces` | 尋找哪些工作區和記錄型別已連線至特定外部記錄。 | 讀取 |
| 取得記錄型別共用 | `planning_get_record_type_sharing` | 傳回特定記錄型別的共用和許可權。 | 讀取 |
| 修改記錄型別共用 | `planning_modify_record_type_sharing` | 更新誰可以存取記錄型別以及什麼許可權層級。 | 寫入 |

### 記錄

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 取得記錄 | `planning_get_record` | 依ID擷取單一記錄的完整詳細資料。 | 讀取 |
| 搜尋記錄 | `planning_search_records` | 搜尋和篩選記錄型別中的記錄。 | 讀取 |
| 大量記錄動作 | `planning_bulk_record_actions` | 在單一請求中建立、更新、刪除或還原多個記錄。 | 寫入 |
| 建立連線記錄 | `planning_create_connection_record` | 在連線的外部系統（例如Workfront專案）中建立新記錄。 | 寫入 |
| 更新記錄順序 | `planning_update_records_order` | 變更記錄型態中記錄的顯示順序。 | 寫入 |
| 取得記錄變更記錄 | `planning_get_record_change_log` | 傳回記錄的欄位層級編輯歷史記錄。 | 讀取 |
| 取得記錄共用 | `planning_get_record_sharing` | 傳回特定記錄的共用設定。 | 讀取 |
| 修改記錄共用 | `planning_modify_records_sharing` | 更新誰可以存取一或多個記錄，以及以什麼許可權層級存取。 | 寫入 |

### 欄位

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 取得欄位 | `planning_get_field` | 依ID擷取欄位的完整詳細資料和值結構描述。 | 讀取 |
| 建立欄位 | `planning_create_fields` | 新增一或多個欄位（欄）至記錄型別。 | 寫入 |
| 更新欄位 | `planning_update_field` | 部分更新欄位的名稱、說明、選項或設定。 | 寫入 |
| 刪除欄位 | `planning_delete_field` | 從記錄型別中永久移除欄位及其所有資料。 | 寫入 |

### 檢視

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 取得檢視 | `planning_get_view` | 依ID傳回檢視的完整詳細資料。 | 讀取 |
| 建立檢視 | `planning_create_view` | 為記錄型別建立新的表格、時間表或行事曆檢視。 | 寫入 |
| 更新檢視 | `planning_update_view` | 部分更新現有檢視的設定、篩選器或排序。 | 寫入 |
| 刪除檢視 | `planning_delete_view` | 永久刪除檢視（記錄不受影響）。 | 寫入 |
| 取得檢視共用 | `planning_get_view_sharing` | 傳回特定檢視的共用設定。 | 讀取 |
| 修改檢視共用 | `planning_modify_view_sharing` | 更新誰可以存取檢視以及以什麼許可權層級。 | 寫入 |

### 範本

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 取得範本清單 | `planning_get_template_list` | 列出所有可用的工作區範本及摘要資訊。 | 讀取 |
| 取得範本 | `planning_get_template` | 依ID擷取特定範本的完整詳細資料。 | 讀取 |

### 搜尋與公用程式

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 搜尋資源 | `planning_search_resources` | 依名稱跨工作區、記錄型別和檢視進行搜尋。 | 讀取 |
| 搜尋共用資料 | `planning_search_sharing_data` | 依名稱尋找使用者、群組、團隊、角色和公司，以進行共用和許可權。 | 讀取 |
| 搜尋使用者 | `planning_search_users` | 搜尋具有分頁支援的使用者。 | 讀取 |

## 工作流程工具

工作流程工具是AI代理平台用於處理任何Workfront物件的一般用途動作，包括專案、任務、問題、小時、指派、計畫、投資組合等。

### 物件和欄位

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 搜尋物件 | `workflow_search_any_object` | 使用彈性的篩選引數、順序和分頁來搜尋Workfront物件。 | 讀取 |
| 建立物件 | `workflow_create_any_object` | 建立新的Workfront物件，例如專案、任務、問題、小時、指派、方案或投資組合。 | 寫入 |
| 更新物件 | `workflow_update_any_object` | 更新現有Workfront物件上的欄位。 | 寫入 |
| 刪除物件 | `workflow_delete_any_object` | 依ID刪除Workfront物件。 執行動作前需要明確的使用者確認。 | 寫入 |
| 解析欄位名稱 | `workflow_resolve_field_names_any_object` | 將使用者提供的欄位名稱或標籤轉換為基礎Workfront API欄位名稱，讓AI代理平台可以建置準確的請求。 | 讀取 |

### 註解

| 標題 | 工具名稱 | 作用 | 動作 |
| --- | --- | --- | --- |
| 查詢註解 | `comment-stream_query_comments` | 依物件ID查詢註解，包含分頁。 | 讀取 |
| 取得註解 | `comment-stream_get_comment` | 依ID取得單一註解。 | 讀取 |
| 取得評論計數 | `comment-stream_get_comments_count` | 取得物件的最上層註解總數。 | 讀取 |
| 建立評論 | `comment-stream_create_comment` | 在物件上建立新註解。 | 寫入 |
| 建立回覆 | `comment-stream_create_reply` | 建立現有註解的回覆。 | 寫入 |
| 更新評論 | `comment-stream_update_comment` | 更新現有的註解或回覆。 | 寫入 |
| 刪除評論 | `comment-stream_delete_comment` | 依ID刪除評論。 | 寫入 |
| 新增反應 | `comment-stream_add_reaction` | 新增回應(like)至註解。 | 寫入 |
| 移除反應 | `comment-stream_remove_reaction` | 從註解中移除回應（類似）。 | 寫入 |



## 如何更新工具

當Adobe發行新版Workfront MCP伺服器時，AI代理平台會自動使用更新的工具集。 您不需要重新連線或變更任何專案。



## 即將推出的其他工具

我們日後會致力新增下列工具至Workfront MCP伺服器：

* 展示板


