---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: '''Adobe Workfront Fusion案例範例：連線電子郵件、文字剖析器和Google表'
description: 此案例可協助您建立所有電子郵件訊息的記錄，並加以標籤，以在試算表中執行進一步動作。 它會使用規則運算式(Regex)作為搜尋模式，擷取試算表中兩個個別表格中的電子郵件內文。 第一模式搜索短語，第二模式搜索相同的短語和電子郵件地址。
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 案例範例：連接電子郵件， [!UICONTROL 文字剖析器]，和 [!DNL Google Sheets]

此案例可協助您建立所有電子郵件訊息的記錄，並加以標籤，以在試算表中執行進一步動作。 它會使用規則運算式(Regex)作為搜尋模式，擷取試算表中兩個個別表格中的電子郵件內文。 第一模式搜索短語，第二模式搜索相同的短語和電子郵件地址。

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
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td> 
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

本教學課程需要對規則運算式有基本的知識。 若要了解Regex，請造訪 [https://regexone.com](https://regexone.com/).

新增第一個模組並加以設定

1. 搜尋電子郵件並選擇 **[!UICONTROL 觀看電子郵件]** 作為觸發器。

   >[!NOTE]
   >
   >當您可以連線 [!DNL Google] 帳戶使用E郵件模組，您也可以使用 [!DNL Gmail] 模組。

1. 連線 [!DNL Google] 帳戶或任何其他基於IMAP的電子郵件客戶端(如 [!DNL Outlook])。
1. 連線後，選取您要監看其傳入電子郵件的資料夾，例如 [!UICONTROL 收件匣].
1. 在 [!UICONTROL 條件]，選擇 **[!UICONTROL 所有電子郵件]** （或縮小至已讀或未讀電子郵件）。

   您也可以選擇將擷取的電子郵件標示為已讀或未讀。

1. 設定 [!UICONTROL 最大結果數] 到1。

   ![](assets/save-max-as-1-350x304.png)

   您可以根據收到的訊息數量來變更此項目。 不過，建議您設定低值，並更頻繁地執行案例。

1. 按一下 **[!UICONTROL 顯示高級設定]** 在底部。

   ![](assets/show-adv-settings-350x332.png)

1. 依 [!UICONTROL 寄件者地址], [!UICONTROL 主旨] 和 [!UICONTROL 片語].

   這可讓您只觀看相關電子郵件。 在此範例中，我們僅新增了「主旨」篩選器，並將其他2留空。

   >[!NOTE]
   >
   >我們將添加路由器，以使用 [!UICONTROL 匹配模式] 運算子和規則運算式(Regex)作為搜尋模式。 這也使我們能夠建立多公用程式案例。

1. 完成設定後，系統會提示您指定從何處開始觀看電子郵件，請按一下 **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. 繼續 [搜尋 [!UICONTROL 流量控制] 並新增 [!UICONTROL 路由器]](#search-for-flow-control-and-add-a-router)

## 搜尋 [!UICONTROL 流量控制] 並新增 [!UICONTROL 路由器]

1. 在任何模組之後添加路由器，以在將資料發送到下一個模組之前分割或複製資料。

   在這裡，我們用了 [!UICONTROL 路由器] 將電子郵件內文傳送至 [!DNL Google Sheet].

   ![](assets/search-for-flow-control-350x220.png)

## 使用 [!UICONTROL 文字剖析器] 模組

1. 新增 [!UICONTROL 匹配模式] 變壓器，在電子郵件中搜尋片語。

   我們將搜索短語「[!UICONTROL 文本解析器模組]「 」，以擷取符合該片語的內文和寄件者名稱。

   1. 將模式寫入為規則運算式：

      text\sparser\smodule

   1. （選用）使用任何其他「模式」選項。

      ![](assets/pattern-350x318.png)

      如果文字包含數行，且您需要搜尋每行中的模式，多行即可派上用場。 在本教學課程中，我們需要搜尋整個電子郵件內文中的模式，因此我們會保留未核取的狀態。

   1. 在 [!UICONTROL 文字] 欄位，按一下屬性 **文字內容** 在清單中。

      ![](assets/text-content-350x264.png)

      這是屬性，可儲存電子郵件內文的文字，我們將在其中搜尋模式。

1. 添加其他 [!UICONTROL 匹配模式] 會搜尋相同的片語和電子郵件地址。

   如果您有多個使用者的客戶帳戶，這特別實用。 若要節省時間，您可以複製 [!UICONTROL 文字剖析器] 模組，並將其連結到路由器。

   ![](assets/clone.png)

1. 編輯模式如下：

   text\sparser\smodule。+\s([\w-]+@[\w-]+)

   ![](assets/text-parser-350x202.png)

   此模式會搜尋片語「[!UICONTROL 文本解析器模組]「 」和john.doe@gmail.com之類的電子郵件地址，且只會傳回電子郵件地址。

   >[!NOTE]
   >
   >請務必根據您接受的電子郵件地址規格來撰寫規則運算式，但以上規則會處理大部分標準電子郵件地址。

   * 如果您只想搜尋電子郵件地址，可以使用以下的規則運算式：

      ([\w-]+@[\w-]+)

   * 您也只能使用下列規則運算式來搜尋電話號碼：

      ^[+]?\(?(\d{1,3})\?[\s-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d{3,4}上述模式涵蓋寫入電話號碼的最常見格式。
   若要測試您的模式，建議您使用 [[!DNL https://regex101.com]](https://regex101.com/) with [!DNL javascript] 作為風味。

   其餘的設定與之前的設定相同。

## 新增 [!DNL Google Sheets] 模組

針對 [!DNL Sheets]，我們必須先建立含有必要標題的試算表。

1. 建立試算表，其中包含您要擷取使用者資料的欄。 （您也可以使用現有檔案）。

   例如，建立名為「電子郵件資料：支援票證」，以「寄件者名稱」、「寄件者電子郵件」和「電子郵件內容」為欄。 將工作表命名為「包含：文本解析器模組。」

1. 新增 [!UICONTROL Google工作表] 模組 **[!UICONTROL 新增列]** 作為動作。

   ![](assets/add-a-row-350x174.png)

1. 連接您的 [!DNL Google] 帳戶（如果尚未）。 選擇您先前建立的檔案，然後選擇您要擷取資料的工作表。

   您的設定應如下所示：

   ![](assets/connect-google-acct-350x279.png)

1. 對應相關欄位（欄）中的屬性以完成模組設定。

   ![](assets/map-attributes-350x282.png)

1. 複製您剛建立的模組，並將其連結至第二個模組 [!UICONTROL 文字剖析器] 模組。

   1. 前往試算表，複製您先前建立的工作表並命名。

      例如，將其命名為「包含：文字剖析器模組和電子郵件。」

   1. 新增另一欄，以儲存電子郵件內文包含的電子郵件地址。

      例如，將其命名為「共用的電子郵件地址」。

   1. 按一下複製的 [!DNL Google Sheets] 設定模組。
   1. 將工作表變更為您剛建立的工作表。
   1. 映射 [!UICONTROL 匹配模式] 模組($1)到要儲存電子郵件地址（共用電子郵件地址）的列。

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. 按一下 **[!UICONTROL 確定]**，儲存情境，然後取用它進行測試執行。

      您需要依下列方式，傳送兩封不同的電子郵件至連線的電子郵件地址：

      * 包含片語&quot;[!UICONTROL 文本解析器模組]&quot;（沒有電子郵件地址）

         ![](assets/text-parser-module-350x103.png)

      * 包含上述片語和電子郵件地址

         ![](assets/above-phrase-and-email-350x106.png)

         如果您的設定中沒有錯誤，您會看到第一個工作表擷取包含片語「[!UICONTROL 文本解析器模組]&quot;，而第二個工作表只會擷取包含片語&quot;[!UICONTROL 文本解析器模組]」和電子郵件地址。 您可以參閱下方的螢幕擷取畫面。

         工作表1:

         ![](assets/worksheet-1-350x57.png)

         工作表2:

         ![](assets/worksheet-2-350x41.png)

## 資源

* [免費練習](https://regexone.com/) 了解規則運算式
* [了解電話號碼匹配](https://regexone.com/problem/matching_phone_numbers) 使用Regex
* [了解電子郵件比對](https://regexone.com/problem/matching_emails) 使用Regex
* [測試規則運算式](https://regex101.com/)
