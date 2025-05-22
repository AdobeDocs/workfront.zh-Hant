---
title: Adobe Workfront規劃最佳作法
description: 身為行銷營運領導者，您可以使用Adobe Workfront Planning來組織所有團隊在行銷生命週期中的工作。 這些是我們從Workfront Planning開始建議的一些最佳實務。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6e039b80-e3bf-412c-8c86-8f801f5861e3
source-git-commit: 1926500c76e4f9cfdac829f8d9f0cdfa6231e31d
workflow-type: tm+mt
source-wordcount: '3304'
ht-degree: 0%

---

<!--drafted because Kari Woolf will write something for Field Readiness instead, nothing for ExL, public-facing documentation-->

# Adobe Workfront規劃最佳作法

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

身為行銷營運領導者，您可以使用Adobe Workfront Planning來組織所有團隊在行銷生命週期中的工作。

本文記錄了一些從Workfront規劃開始時，我們建議的常見問題和最佳作法。

## 設定最佳實務

### 工作區

工作區是專案團隊計畫工作的集中位置。 工作區是團隊使用的記錄型別集合，代表團隊的工作生命週期。

以下是有關設定Workfront Planning的一些常見問題。

#### 我應該如何開始？

* ✅當您首次登入Planning時，請遵循我們的應用程式內上線流程，該流程能清楚傳達您的Planning價值，並引導您如何有效導覽及使用產品。 這可確保您瞭解其功能，以及如何輕鬆開始工作。
* ✅首先，探索我們預先定義的工作區範本，以取得現有類似使用案例的想法。 您可以使用範本中預先定義的記錄型別和欄位，也可以新增您自己的記錄型別和欄位。
* ✅識別您要透過Workfront Planning解決的主要使用案例。 例如，大多陣列織想要提高策略活動的可見度，其中可能包括建立更好的「行銷活動行事曆」。 因此，對於該使用案例，您首先想回答幾個問題：

   * 誰在要求？
   * 他們要將哪些專案放在行事曆中？
行銷活動？ 戰術？ 方案？ 活動？ 活動？
   * 他們想要透過此行事曆回答哪些型別的問題？
   * 我們對於相同對象有任何重疊的行銷活動嗎？
   * 我們對於該行銷活動、策略、活動或事件的預算是多少？

  這些問題的答案將決定您需要在Workfront Planning中建置什麼。

  此外，考慮可能有其他規劃人員目前不是Workfront使用者。 這些規劃人員可能會使用Excel試算表、Word檔案、PowerPoints等來執行作業。 考慮他們如何在Workfront Planning中存取您的資訊。

* ✅若要充分利用Workfront Planning，請考慮將Workfront Workflow中的投資組合和程式使用，取代為Workfront Planning中的其他上層結構。

  現在，Workfront客戶透過產品組合和計畫來代表其策略性工作，在某些情況下，是不同型別的專案。 隨著Planning的推出，所有這類策略性工作應透過Workfront Planning中的自訂記錄型別來處理，而Workfront將集中於以專案和任務表示的工作執行階段。


#### 何時應建立新工作區而不要修改現有工作區？

* ✅設計組織層級工作區的最低容量。 您可以建立特定作業組織單位的工作區，以符合每個單位的獨特運作方式。

  在單一Workspace中擁有資訊，以確保可輕鬆管理所有資料之間的關係。

  例如，嘗試為所有Marketing建立單一工作區。

  您可以為具有完全不同營運結構的團隊建立新的工作區：

  例如，**產品開發**&#x200B;工作區應與&#x200B;**行銷**&#x200B;工作區不同。

* ⛔請勿為組織內的每個團隊或程式建立唯一的工作區。

  行銷組織應努力維護一個工作區，以維持可見度，並允許資料在全球計畫層級累積。

  請避免為遵循類似流程的團隊建立類似或重複的工作區（例如，EMEA行銷與APAC行銷），特別是當這些團隊可能會進行的工作可提升到共同策略行銷活動時。

#### 如何使用Workspace區段？

* ✅建立和標籤區段，協助您的使用者瞭解您如何組織您的營運生命週期。

  例如，您可以建立名為&#x200B;**核心記錄**&#x200B;的區段，將您的行銷活動、戰術和交付專案放在工作區中。
* ✅個群組「讚」記錄型別在一起。

  例如，您可以建立名為&#x200B;**Geographies**&#x200B;的區段，其中包含記錄型別，例如：地區、國家/地區和城市。

### 記錄類型

記錄型別是Workfront Planning Workspace的建置組塊。 您可以定義記錄型別的互連方式。


#### 如何在我的工作區中定義記錄型別？

* ✅請花一些時間找出您需要追蹤的資訊（我需要哪些記錄型別），以及需要如何連線這些資訊。 與使用工作區的利害關係人溝通，以考慮他們所有的需求。 您也可以建立具有不同記錄型別的自訂區段，以非常方便使用的方式呈現資訊。


* ⛔請勿在不同期間重複記錄型別（例如，請勿為&#x200B;**2024年行銷活動**&#x200B;和&#x200B;**2025年行銷活動**&#x200B;建立個別的記錄型別）。

  每當您想要比較多個年度的資料時，建立不同的記錄型別會中斷資料流程。 今天的檢視是按記錄型別劃分的，因此當一年結束時，該記錄型別的檢視將不再顯示未來的專案。 最佳實務是讓工作型別有一個記錄型別，並視需要使用篩選器或封存資料來劃分資料。

#### 何時應使用單一或多重選取欄位，而不是連結的記錄型別？

* ✅如果物件將用於多個其他記錄型別，請新增記錄型別

  例如，行銷活動可能連線至多個目標對象，而策略可能連線至單一目標對象。 因此，行銷活動、策略和對象應該是記錄型別，而不是多選欄位。

* ✅如果物件需要儲存可能在查詢中有用的其他中繼資料值，請新增記錄型別

  例如，頻道記錄型別（例如&#x200B;**電子郵件**）可能會以原生中繼資料或獨立&#x200B;**傳遞專案**&#x200B;記錄型別的連線，來儲存支援傳遞專案的清單。
* ⛔如果您儲存的資料只與單一記錄型別相關，請勿新增記錄型別。

  例如，**行銷活動**&#x200B;記錄型別可能有一個名為&#x200B;**行銷活動大小**&#x200B;的單選欄位，只有在直接與特定行銷活動關聯時才相關。

#### 如何為我的記錄型別加上標籤？

* ✅請建立代表單一建構或名詞的記錄型別並加上標籤，例如&#x200B;**促銷活動**。
* ⛔請勿建立較適合呈現為檢視的記錄型別。

  例如，**行事曆**&#x200B;對於記錄型別來說是一個糟糕的選擇，因為它不是記錄型別本身，而是記錄的檢視。

### 欄位管理

欄位是記錄型別的屬性，在表格檢視中顯示為欄。 您可以建立記錄型別的自訂欄位，然後將欄位與Workfront Planning記錄建立關聯，以增強記錄資訊。


#### 建議將哪個欄位定義為主要欄位？


* ✅請使用唯一的主要欄位值，以便在建立連線時更容易找到並「挑選」這些記錄。 

  建立連線時，使用者將依照主要欄位中的值進行搜尋，如果它們不是唯一的，使用者將無法知道應該選擇哪一個。 
* ⛔避免使用非唯一值作為主要欄位，因為使用連線選擇器選單時，這會讓必須在主要欄位上搜尋的使用者感到困惑。 

#### 我應如何使用公式？

* ✅請使用公式欄位型別來減少手動輸入。 當您根據表格檢視中已存在的資料輸入資訊時，可以使用公式自動計算該資訊，以節省一些時間。

#### 如何開始連線工作區中的資料？

* ✅建立連線是Workfront規劃最強大的功能之一。 您可以將記錄型別連結至其他應用程式，例如Adobe Workfront （連線至專案、投資組合、方案、公司和群組）和Adobe Experience Manager Assets （連線至資產和資料夾）。

  連線物件與記錄型別可讓您完整概略瞭解公司中所有物件的連線方式。

  例如，您有&#x200B;**行銷活動**&#x200B;記錄型別和&#x200B;**戰術**&#x200B;記錄型別，您可以建立這兩種記錄型別之間的連線，以檢視哪些&#x200B;**戰術**&#x200B;與特定的&#x200B;**行銷活動**&#x200B;相關聯。

  定義連線後，工作區中的所有人員可以開始新增&#x200B;**行銷活動**&#x200B;的值，方法是按兩下連線欄位，在其中會看到所有可用&#x200B;**戰術**&#x200B;的清單。 這可讓您快速找出哪些策略需要與行銷活動相關聯。

#### 如何使用查詢欄位？

* ✅在您建立記錄或物件型別之間的連線後，可以將個別記錄彼此連線，並在Workfront Planning記錄上顯示連結記錄或物件型別的欄位。 您將減少必須更新相同資訊的地點數量，並確保其完全相符。

  例如，一旦您在&#x200B;**促銷活動**&#x200B;記錄型別和&#x200B;**戰術**&#x200B;記錄型別之間建立連線，您將會看到主要欄位資訊，但當您新增查閱欄位時，您將能夠從該記錄型別帶入其他資訊，例如該&#x200B;**戰術**&#x200B;的&#x200B;**上市日期**。 新增記錄後，系統會自動填入這些查詢欄位的資料。

#### URL建議使用什麼欄位型別？ 

* ✅請使用單行文字欄位，將URL資料新增至記錄。

### 檢視

#### 如何決定檢視與記錄型別應為何？

* ✅對於代表單一建構或名詞的專案（例如&#x200B;**行銷活動**），請建立記錄型別。 

* ⛔請勿建立較適合呈現為檢視的記錄型別。

  例如，**行事曆**&#x200B;對於記錄型別來說是一個糟糕的選擇，因為它不是記錄型別本身，而是記錄的檢視。 

#### 我應該隱藏或刪除和我無關的欄位嗎？

* ✅當此資訊與使用相同記錄型別的不同人員相關時，請隱藏該欄，而不是刪除它。 如果您刪除特定表格檢視中的欄位，此欄位也會在此記錄的其餘檢視中刪除，以及此記錄型別所連結的任何其他位置中刪除。

#### 如何在表格和時間表檢視中使用篩選器和群組？

* ✅使用包含篩選器和群組的檢視來顯示您需要檢視內容的快照。 您可以篩選資料並將資料分組，以更易消耗的方式瞭解計畫內容。 您可以依中繼資料欄位將記錄分組。

  例如，您可以有您的&#x200B;**促銷活動**&#x200B;記錄型別的時間表檢視，而且您可以依&#x200B;**目標對象**&#x200B;分組，並依&#x200B;**日期**&#x200B;篩選以僅顯示目前年份。

#### 為什麼我在時間軸檢視中看不到所有記錄？

* ✅請記得為您的記錄定義2個日期欄位。 您至少有兩個日期欄位與記錄型別相關聯時，才能建立時間表檢視。 當「開始」或「結束」日期或兩者都沒有值，且「開始」日期在「結束」日期之後時，某些記錄可能不會顯示在時間軸檢視中。

#### 如何使用時間軸檢視設定

* ✅定義您的時間表檢視的設定，例如&#x200B;**橫條樣式**&#x200B;和&#x200B;**色彩**，以取得更豐富的視覺效果。 您可以藉由定義您是否想要看到具有有意義的影像的縮圖，並新增更多欄位以顯示於長條圖（例如，**所有者**&#x200B;或&#x200B;**狀態**），自訂&#x200B;**長條圖樣式**。

  依預設，您只會看到主要欄位。 您也可以依欄位值來定義長條的顏色（例如，您可以藉由將長條與「狀態」欄位比對來自訂長條的顏色），或依您套用的群組來定義長條的顏色。 依預設，該顏色與記錄型別的顏色相符。

  只有記錄型別顏色或包含與顏色關聯的選項的欄位才能影響時間軸中記錄列的顏色。

### 許可權和共用

使用共用功能，為員工提供檢視和工作區的適當許可權。

#### 我該如何管理工作區的許可權？

* ✅當您建立&#x200B;**工作區**&#x200B;時，只有您才能使用。 系統管理員以外的任何人將無法找到它。 定義工作區且準備好將您的團隊帶入共同作業後，您需要與他們共用該工作區並定義其許可權層級。

  您可以從下列許可權層級中選擇：

   * **管理**：人員可以編輯、刪除及共用工作區。
   * **Contribute**：人員可以建立、編輯和刪除記錄。
   * **檢視**：人員可以檢視記錄。

* ✅雖然許多客戶覺得他們會將工作區的&#x200B;**管理**&#x200B;許可權授與大部分人員，但確實會將&#x200B;**管理**&#x200B;許可權限製為選取的信任人員群組，以免意外刪除記錄型別或建立不必要的記錄型別和欄位。 他們可以編輯、共用甚至刪除工作區。 此等級的許可權可授予他們對Workspace的完整管理存取權。

  某人若要擁有工作區的管理許可權，必須具備Standard使用者授權。

* ✅如果您希望使用者&#x200B;**Contribute**&#x200B;僅能建立、編輯和刪除記錄，但不希望他們變更工作區的結構和結構描述，請授予這些使用者許可權。 他們具有&#x200B;**Contribute**&#x200B;許可權，無法建立記錄型別或變更現有記錄型別上的欄位。

  某人必須具備Standard使用者授權，才能擁有工作區的&#x200B;**Contribute**&#x200B;許可權。

* 如果您只想讓使用者&#x200B;**檢視**&#x200B;記錄，請✅授予使用者檢視許可權。

  >[!NOTE]
  >
  >目前，我們對於記錄型別或記錄沒有特定的許可權，因此這表示如果您授予某人&#x200B;**檢視**&#x200B;工作區存取權，則任何記錄型別中的所有記錄都會顯示。


#### 我該如何管理記錄型別的許可權？

* ✅請記住，擁有工作區管理許可權的使用者無法降低其記錄型別的許可權。 他們也將繼承記錄型別的管理許可權。 您無法授予使用者對工作區的管理許可權，但授予記錄型別的「貢獻」或「檢視」許可權。
* ✅如果您希望使用者對記錄型別的許可權層級（例如「檢視」許可權）低於對工作區的許可權，我們建議將工作區的貢獻許可權授予他們。 然後，您可以授予他們記錄型別的檢視許可權。
* 將使用者從記錄型別的許可權中移除時，仍會為他們提供至少對工作區的檢視許可權。

#### 我該如何管理檢視的許可權？

* ✅請將&#x200B;**管理**&#x200B;許可權限制在您想要編輯、刪除和共用檢視的許可權範圍內。 這表示他們可以變更檢視的篩選器、分組欄位或某些設定。 這些變更將會影響同時使用該檢視的其他人的檢視主要設定。

  某人若要取得檢視的管理許可權，必須具備Standard使用者授權。

* ✅授予使用者&#x200B;**檢視**&#x200B;存取權以套用檢視。 他們將能夠變更某些篩選器或分組和排序，但這些變更將是暫時的；變更沒有為存取檢視的所有其他使用者儲存。 這些變更不會影響同時使用該檢視的其他人的檢視主要設定。  他們的變更只會顯示給套用已修改設定的使用者。 重新整理畫面後，變更會重設為預設值。

* ✅授予&#x200B;**當您希望所有可以檢視工作區的人檢視該特定檢視中的記錄及其欄位時，工作區中的每個人都可以檢視**&#x200B;許可權。 如此一來，您就不需要手動將任何人新增至檢視的共用許可權方塊。

  >[!NOTE]
  >
  >如果檢視尚未共用，而您與其他人共用該檢視的連結，則他們將能夠在&#x200B;**預設表格檢視**&#x200B;中檢視記錄。 如果他們擁有標準Workfront授權，便能建立自己的檢視。


#### **Workspace共用**&#x200B;與&#x200B;**檢視共用**&#x200B;有何不同？

* **Workspace共用**&#x200B;定義使用者對工作區、其記錄型別、記錄及其欄位的存取權。

* **檢視共用**&#x200B;定義使用者是否可以看見您建立的檢視，以及他們是否可以變更檢視的篩選、分組欄位或其他組態。 「檢視」中顯示之記錄的可見度是由Workspace共用所控制，而非由「檢視」共用所控制。

#### Workfront授權型別如何影響Workfront Planning許可權？

* 針對&#x200B;**Workspace共用**：輕度和Contribute授權使用者只能取得工作區的檢視存取權。 若要授與某人「貢獻」或「管理」工作區許可權，該人員必須擁有「標準」授權。

* **檢視共用**：擁有工作區管理許可權的標準授權使用者將能夠建立檢視。 Light和Contribute授權使用者只能使用Standard使用者已建立並與他們共用的檢視。 否則，如果未共用任何專案，使用者將能夠看到&#x200B;**預設資料表檢視**。


#### 當Workspace擁有者變更時，怎麼辦？

* Workfront會將工作區建立者設為擁有者，但就功能而言，擁有者與任何具有「管理」許可權的使用者具有相同的許可權。
* 如果擁有者已停用，其他成員可以在工作區中繼續工作，而不會造成任何中斷。
* 系統管理員可存取任何工作區，因此，如果擁有者是唯一具有管理許可權的人員，則管理員可以新增其他人員並授予他們管理許可權，以處理工作區的管理。

### 在Workfront規劃中提交請求

當您想要使用者在記錄型別的頁面外新增記錄時，您可以為每個記錄型別建立請求表單。 提交表單會將新記錄新增到記錄型別。

#### 何時應該開始建立記錄型別的要求表單？

* ✅您應該先將必要的欄位新增至資料表，以確保已設定記錄型別結構。 這些欄位說明您的記錄，並可在表單產生器中存取。

  理想情況下，在記錄型別結構完成後建立請求或輸入表單，以避免遺漏任何關鍵欄位。

#### 誰可以建立申請表單？

* ✅任何擁有工作區管理存取許可權的使用者都可以建立或編輯請求表單。 請確定已正確指派使用者的許可權，以允許此功能。

#### 如何建立或編輯記錄型別的要求表單？

* ✅任何具有工作區管理存取許可權的使用者都可以遵循文章[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)中所述的步驟。


#### 誰能使用申請表提交新記錄？

* ✅提交許可權取決於您為每個表單設定的設定。

  在表單產生器中，發佈表單後，您可以管理許可權以控制誰可以提交請求。

  您可以從下列三個共用選項中選擇：

   * **擁有工作區檢視許可權或更高存取許可權的任何人：**&#x200B;允許所有擁有工作區檢視許可權或更高許可權的使用者提交建立記錄的請求。
   * **任何擁有貢獻者或以上工作區存取權的使用者**：限制向擁有貢獻者或以上工作區許可權的使用者提交內容。
   * **擁有連結的任何人：**&#x200B;讓擁有表單連結的任何人能夠提交要求。
   * **到期日：**&#x200B;請確定您設定公用連結的到期日，以增強安全性。

### 管理請求表單的最佳作法

以下是管理請求表單的建議：

* 預先計畫：在建立表單之前，請明確定義要求者需要或需要的資訊，以避免日後過度修訂。
* 使用清楚的標籤：確保欄位標籤和說明清晰易懂，可供所有使用者使用。
* 測試表單：在將新表單轉出給更廣大的受眾之前，請使用表單連結和表單預覽選項來測試表單，以確保所有欄位和邏輯都如預期般運作。
* 保持表單更新：定期稽核並更新表單，以符合記錄型別結構或操作流程中的任何變更。

<!-- this is hidden, per Andrea:  

2.2 Migration  

Migrating your data from external <span style="text-decoration:underline;">s~~S~~</span>ystems to Workfront Planning unlocks new ways to create important connections in your workflow and uncover insights that you might not have been able to identify with your previous tools. 

By having all your data in one central location, you can more easily form connections between your Workfront data than if they all existed in separate tools. 

We have some options that will help you to accelerate the migration process:  

* **Fusion** – You can create a Scenario in Fusion that runs after certain criteria and connects objects. 
* **Bulk Data Operations** _through the new functionality -[ [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE)  (Q3 2024)_ -  
* **Copy and paste – **You can copy and paste directly from a spreadsheet. This is best suited to a simple table of data from tools like Excel or Google Sheets.  
* **Upload a C<span style="text-decoration:underline;">SV~~VS~~</span> or Excel **- The CSV (comma-separated values) format or Excel is one of the most common ways to move data between applications, and tools. This functionality is not available yet, but we are planning to work on it in Q4 2024.  

-->

<!--
     

1. Data Flow  

Currently the metadata modelling in Workfront Planning is done by Ops Admins through adding various data points to the record type from the table view, including: 



* Fields added directly on the current record type 
* Connections with custom defined operational and taxonomical record types 
* Connections with execution work captured in Workfront 
* Connections with deliverables stored as assets in AEM 
* Any lookup fields captured in any of the above connections. 

Here is a summary of how you can define the data flow within Workfront Planning and other applications.  


     



* **Connections and Lookup fields. **Creating **connections** is one of the most powerful features of Workfront Planning. You can connect record types to one another or record types with object types from other applications like Adobe Workfront (connection to Project, Portfolios, Programs, Companies, and Groups) or Adobe Experience Manager Assets (connection to assets and folders).  Connections give you a full overview of how everything in your company is connected.  

    - e.g.: You have a Campaign record type, and a Tactics record type, then you can create a connection between these two record types to see to see which Tactics are associated to a specific Campaign. After defining the connection, all the people in the workspace can start adding values by double-clicking into the connection field that displays the tactic where they will see a list of all the Tactics available and you can quickly select the tactics to be associated with each campaign. 


    After you establish the connection between records or object types, you can connect individual records to one another, and display fields from the linked record or object types on a Workfront Planning record. The connected fields are called **Lookup fields**. You will reduce the number of places you have to update the same piece of information and ensure that they match perfectly.  


    - e.g.: Once you have a connection between a Campaign record type and a Tactics record type, you will see the primary field information when you add the tactic, but when you add lookup fields, you will be able to bring additional information from the tactic, like the Launch date for that Tactic. The data for these lookup fields is auto populated. Find more information in the Adobe Experience League documentation in the article about Connecting records.  


     

* **Planning (or Connections) tab** **in Workfront _-[ [E] Global Connect capability in Planning connections area](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6617d7760001e250f5ffb9ebf04baacc/overview?source-id=unifiedShareMFE)_** 

    When you go to the Planning section of Adobe Workfront objects, you can display both connections with linked records or any available connections with Planning record types. With that, you can view and edit any connection field without having to navigate away from the current section in Workfront to other areas. The Planning section is available for the following Workfront objects: Project, Portfolio and Program. For more information, see [Manage records in the Planning section of Adobe Workfront objects](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/manage-records-in-planning-section).   


* Create new records within the connection fields - In-context creation of connected records https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6656c1a30026b903c6edf0210b8cbb23/overview?source-id=unifiedShareMFE  When you need to link records through a connection field but cannot find the required records in the connected record type, you can also create new records in the connected record type directly within the connection fields, with that you can efficiently establish necessary links without having to leave the current record type context. For more information, see Create records https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-records/create-records.   

     

* **Field on Customer Form** (CF)[ - [E] Make connected Planning data consumable through WF forms](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/6641b040000b880ccd74aab6365c3361/overview?source-id=unifiedShareMFE) _(Planned completion date Sep 15, 2024 10:00 PM)._ Considering that the Workfront Project metadata modeling is done through forms, you are also able to add Planning connections to your custom forms. You can embed any lookup field value from the connected Planning record types within the custom form of your Workfront object. With that capability, when you are managing objects in Workfront, you can present any taxonomies or operational records connected to the Workfront object in custom forms, alongside other details, so that your teams can easily consume and update all the relevant information through a unified interface.  They should not need to navigate to different areas to view and update the information relevant for their work.  

     

* **Connection between Workspaces with Record types accessible from multiple workspaces** – ~~Epic – "[Connect to record types across workspaces](https://experience.adobe.com/@adobeinternalworkfront/so:hub-Hub/workfront/project/64dfad3100027190324dcc35b2176e76/overview?source-id=unifiedShareMFE)"~~ When you are creating a workspace in Planning, you can define certain record types once and then configure them to be accessible from multiple workspaces so you can create connections with them from anywhere. This way, you can streamline the data management process, eliminate duplicative work, and ensure data consistency across teams. As a result, your teams can tag their records with common taxonomies and unlock better visualization, filtering, grouping, and reporting of cross-team work.  For more information, see [Edit record types](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/edit-record-types). 

     

* **Fusion connector – You can create a connection to your Workfront Planning account from inside a Workfront Fusion module. **With this connector, you can trigger a scenario when events occur in Workfront Planning. You can also create, read, update, and delete records, or perform a custom API call to your Adobe Workfront Planning account. More information in Experience League in[ Adobe Workfront Planning modules](https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-moduleshttps:/experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-fusion/fusion-apps-and-modules/workfront-planning-modules) article.  

-->
