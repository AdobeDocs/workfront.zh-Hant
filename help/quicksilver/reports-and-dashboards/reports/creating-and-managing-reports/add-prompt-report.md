---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 新增提示至報表
description: 篩選器和提示很類似，因為它們都會限制您在報表中顯示的資訊量。
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 93fca2a98a8b9d4370841b10be10ed2ba15283c9
workflow-type: tm+mt
source-wordcount: '1363'
ht-degree: 0%

---

# 新增提示至報表

<!-- Audited: 11/2024 -->

## 提示和篩選器之間的差異

篩選器和提示很類似，因為它們都會限制您在報表中顯示的資訊量。

當您希望每次執行報告時，都以相同的條件篩選報告中顯示的資訊時，可以建立篩選器。 篩選器只建立一次，並在報表中進行硬式編碼。 如需建立篩選的詳細資訊，請參閱文章[篩選概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

提示是開啟的篩選器，每次執行報表時都可以以不同方式自訂和套用。

當您將提示新增到報表中時，可以透過在每次執行報表時編輯提示條件來自訂篩選資訊。 根據您選擇的修飾元，報表每次都會以不同的篩選器執行，而不是在報表的篩選器中硬性編碼修飾元一次。

提示可做為報告的可自訂篩選器，您可在執行報告之前加以更新。 您可以建立一般報表，然後根據當天想要檢視的資訊或與您個人的一組條件相關的資訊來縮小結果。 例如，如果您有「小時」報表，而且您想根據下列條件變更報表的資訊：

* 記錄時數的日期
* 輸入時數的使用者
* 輸入的小時數

您可以建立三個提示，其中的條件為所需的條件，而每次執行報告時，報告都會根據您為提示選擇的資訊而有所不同。

篩選器可告知Adobe Workfront只顯示今年6月至8月之間輸入的小時。 不過，每次執行報表時（例如，在一月和二月之間，或十月和十二月之間），透過提示字元，您可以使用不同的時間範圍。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
    <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>規劃</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權*</td> 
   <td> <p>管理報表的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須先建立報表，才能在其中新增提示。

如需建立報告的指示，請參閱[建立報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## 建立提示

1. 前往您要新增提示的報表。
1. 展開&#x200B;**報告動作**，然後按一下&#x200B;**編輯**。

1. 按一下&#x200B;**報表設定**&#x200B;按鈕。
1. 按一下&#x200B;**報告提示**&#x200B;索引標籤，然後按一下&#x200B;**新增提示**。\
   ![](assets/create-report-prompt-tab.png)

1. （視條件而定）選取提示所依據的欄位。 開始輸入欄位名稱，然後按一下以在清單中出現時選取它。\
   使用者可執行報告的選項會因您選取的欄位而異。\
   例如，如果您在任務報告上選取了日期欄位（如實際完成日期），「實際完成日期」是提示的名稱。 當您在執行此報表時編輯此提示時，可以從一組修飾元中選擇，以建立您的篩選陳述式。 此程式等同於建立篩選器。 如需修飾元的詳細資訊，請參閱[篩選和條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

1. （視條件而定）按一下&#x200B;**自訂提示**&#x200B;以建立自訂提示。

   自訂提示是預先定義的提示，可在執行報表之前先對篩選條件進行硬式編碼。 從這個角度來看，自訂提示比提示更接近篩選器。

   不過，提示仍會像一般提示一樣有彈性，因為您可以從數個預先定義的陳述式中進行選擇，而不是在報表中只有一個硬式編碼篩選器。

   為自訂提示指定下列資訊：自訂提示的條件只能使用文字模式編輯。 這可在單一欄位中套用多個條件。

   * **欄位名稱：**&#x200B;這是提示的名稱，您在執行報表之前看到它。
   * **下拉式清單專案標籤：**&#x200B;這是您執行報表前，在提示中看到的其中一個選項名稱。
   * **條件：**&#x200B;輸入定義提示的條件。
   * **預設值：**&#x200B;您可以選取一個專案作為此提示的預設選項。

   使用與輸入文字模式篩選時相同的語法，並透過「&amp;」加入您的陳述式。 如需以文字模式編輯篩選的詳細資訊，請參閱[使用文字模式編輯篩選](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)。

   例如，下列案例的自訂提示的&#x200B;**條件**&#x200B;欄位可能如下所示：

   * 專案狀態為「構想」、「已請求」、「已計畫」和「目前」的未來專案上的所有任務：

     ```
     project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
     ```

   * 在已完成（過去）專案中，專案狀態為已完成或廢棄的所有任務：

     ```
     project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
     ```

   如需文字模式修飾元的詳細資訊，請參閱[篩選和條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   >[!NOTE]
   >
   >當您執行報表時，無法變更自訂提示的條件，就像變更標準提示一樣。 您可以視需要為自訂提示設定多個預先定義的條件。

1. （可選）重複步驟4或步驟5，視需要建立任意數目的提示。
1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存+關閉**&#x200B;以儲存報告。

## 在報表上套用提示

當您將提示新增到報告時，報告的預設標籤始終是提示標籤。

若要執行帶有提示的報告：

1. 前往報表並出現提示。

   ![](assets/run-report-prompts.png)

1. 為&#x200B;**提示**&#x200B;索引標籤上顯示的一個或所有提示選擇條件。\
   （選擇性）您可以讓提示保持空白，而不根據提示條件篩選報告。

1. 按一下&#x200B;**「執行報表」**。\
   （條件式）如果填入提示，則報表會依您為提示選擇的條件進行篩選。\
   （條件式）如果您將提示保留為空白，則報表不會依提示條件篩選。 報表會如未篩選般顯示。

   >[!NOTE]
   >
   >除了提示之外還包含篩選器的報表，會根據篩選器中定義的條件和組合的提示來篩選結果。

## 共用提示報表的限制

>[!CAUTION]
>
>當您共用提示的報告時，登入和未登入的使用者使用公開共用連結檢視報告無法使用其提示執行報告。 在這種情況下，顯示報告結果時不會套用任何提示，而是會根據使用者的存取層級和許可權，或報告的「以使用者身分執行」存取層級和許可權（如果已設定）來顯示資訊。

以下是從Workfront共用提示報表的限制：

* 公開共用報告時，使用者無法執行具有已套用提示的報告，除非他們：擁有Workfront認證、先登入，並直接在Workfront中導覽至報告（而非透過公開共用連結）。

  如需共用報表的詳細資訊，請參閱文章[在Adobe Workfront中共用報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)。

* 當您排程要傳送的提示報告時，電子郵件附件中的報告會包含未提示的報告資料。 當使用者按一下電子郵件中的連結存取報告時，他們必須先登入才能檢視報告並自行執行提示。

  如需排程傳送報表的詳細資訊，請參閱[排程自動報表傳送](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)。

* 執行含有日期型提示的報告時，系統會根據瀏覽器的時區設定來篩選報告結果。 這可能會造成在已提示報表中顯示的日期範圍（位於月份的開始或結束日期）出現細微差異。 如果您的瀏覽器時區設定繫結至特定位置，則該位置當地時間的變化（例如遵循日光節約時間）也會納入到提示報表所顯示的日期中。 這可能會導致位於相同時區但位置設定不同的使用者之間出現細微的日期範圍差異。
