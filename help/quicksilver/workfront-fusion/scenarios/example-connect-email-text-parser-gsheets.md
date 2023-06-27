---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 「Adobe Workfront Fusion案例範例：連線電子郵件、文字剖析器和Google工作表」
description: 此情境可協助您建立所有電子郵件訊息的記錄，並在試算表中標籤這些訊息以採取進一步動作。 它會使用規則運算式(Regex)作為搜尋模式，在試算表中擷取兩個個別表格中的電子郵件內文。 第一個模式會搜尋片語，第二個模式會搜尋相同的片語和電子郵件地址。
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1214'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 案例範例：連線電子郵件， [!UICONTROL 文字剖析器]、和 [!DNL Google Sheets]

此情境可協助您建立所有電子郵件訊息的記錄，並在試算表中標籤這些訊息以採取進一步動作。 它會使用規則運算式(Regex)作為搜尋模式，在試算表中擷取兩個個別表格中的電子郵件內文。 第一個模式會搜尋片語，第二個模式會搜尋相同的片語和電子郵件地址。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

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
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

本教學課程需要規則運算式的基本知識。 若要瞭解規則運算式，請造訪 [https://regexone.com](https://regexone.com/).

新增第一個模組並進行設定

1. 搜尋電子郵件並選擇 **[!UICONTROL 觀看電子郵件]** 做為觸發程式。

   >[!NOTE]
   >
   >雖然您可以連線 [!DNL Google] 使用E的帳戶郵件模組，您也可以使用 [!DNL Gmail] 模組。

1. 連線至 [!DNL Google] 帳戶或任何其他IMAP電子郵件使用者端(例如 [!DNL Outlook])。
1. 連線後，選取要監視其內送電子郵件的資料夾，例如 [!UICONTROL 收件匣].
1. 下 [!UICONTROL 條件]，選擇 **[!UICONTROL 所有電子郵件]** （或將其縮小至讀取或未讀取的電子郵件）。

   您也可以選擇將擷取的電子郵件標示為已讀取或未讀取。

1. 設定 [!UICONTROL 結果數量上限] 至1。

   ![](assets/save-max-as-1-350x304.png)

   您可以根據收到的訊息數量來變更此設定。 不過，建議設定低值並更頻繁地執行情境。

1. 按一下 **[!UICONTROL 顯示進階設定]** 在底部。

   ![](assets/show-adv-settings-350x332.png)

1. 篩選電子郵件依據 [!UICONTROL 寄件者地址]， [!UICONTROL 主旨] 和 [!UICONTROL 片語].

   這可讓您只觀看相關的電子郵件。 在此範例中，我們僅新增「主旨」篩選條件，並將其他2個保留空白。

   >[!NOTE]
   >
   >我們將新增路由器，以使用在電子郵件中尋找片語。 [!UICONTROL 比對模式] 迭代器和規則運算式(Regex)作為搜尋模式。 這也讓我們能夠建置多公用程式的情境。

1. 完成設定後，系統會提示您指定開始觀看電子郵件的位置時，請按一下 **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. 繼續至 [搜尋 [!UICONTROL 流量控制] 並新增 [!UICONTROL 路由器]](#search-for-flow-control-and-add-a-router)

## 搜尋 [!UICONTROL 流量控制] 並新增 [!UICONTROL 路由器]

1. 在任何模組之後新增路由器，在傳送資料至下一個模組之前分割或複製資料。

   在此，我們使用了 [!UICONTROL 路由器] 若要將電子郵件內文文字傳送至 [!DNL Google Sheet].

   ![](assets/search-for-flow-control-350x220.png)

## 使用 [!UICONTROL 文字剖析器] 模組

1. 新增 [!UICONTROL 比對模式] 轉換器以搜尋電子郵件中的片語。

   我們將搜尋片語「[!UICONTROL 文字剖析器模組]&quot;，以擷取符合該片語的內文和寄件者姓名。

   1. 將模式寫入為規則運算式：

      text\sparser\smodule

   1. （可選）使用任何其他「陣列」選項。

      ![](assets/pattern-350x318.png)

      如果文字包含數行，且您需要搜尋每行中的模式，多行會很有用。 在本教學課程中，我們需要搜尋整個電子郵件內文的模式，因此我們將保留未勾選的狀態。

   1. 在 [!UICONTROL 文字] 欄位，按一下屬性 **文字內容** 在清單中。

      ![](assets/text-content-350x264.png)

      這是儲存電子郵件內文文字的屬性，我們會在其中搜尋模式。

1. 新增另一個 [!UICONTROL 比對模式] 會搜尋相同的片語和電子郵件地址。

   如果您的客戶帳戶有多個使用者，這會特別有用。 若要節省時間，您可以複製 [!UICONTROL 文字剖析器] 您剛建立的模組，並將其連結至路由器。

   ![](assets/clone.png)

1. 編輯模式，如下所示：

   text\sparser\smodule。+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   此模式會搜尋片語「[!UICONTROL 文字剖析器模組]」和電子郵件地址(例如john.doe@gmail.com)並只傳回電子郵件地址。

   >[!NOTE]
   >
   >請務必根據您所接受電子郵件地址的規格來撰寫規則運算式，但上述規格會處理大部分的標準電子郵件地址。

   * 如果您只想搜尋電子郵件地址，可以使用下列規則運算式：

     ([\w.-]+@[\w.-]+)

   * 您也可以使用以下規則運算式搜尋電話號碼：

     ^[+]？\(？(\d{1，3})\)？[\s-]？\(？(\d{3})\)？[\s-]？\d{3}[\s-]？\d{3，4}
上述模式涵蓋寫入電話號碼時最常見的格式。

   若要測試您的模式，我們建議使用 [[!DNL https://regex101.com]](https://regex101.com/) 替換為 [!DNL javascript] 作為Flavor。

   其餘的設定與之前的設定相同。

## 新增 [!DNL Google Sheets] 模組

對象 [!DNL Sheets]，我們需要先建立具有必要標題的試算表。

1. 建立試算表，其中包含您要擷取使用者資料的欄。 （您也可以使用現有的檔案）。

   例如，以寄件者名稱、寄件者電子郵件和電子郵件內容為欄，建立名為「電子郵件資料：支援票證」的票證。 將工作表命名為「包含：文字剖析器模組」。

1. 新增 [!UICONTROL Google工作表] 模組搭配 **[!UICONTROL 新增列]** 作為動作。

   ![](assets/add-a-row-350x174.png)

1. 連線您的 [!DNL Google] 帳戶（如果沒有）。 選擇您先前建立的檔案，然後選擇您要擷取資料的工作表。

   您的設定應如下所示：

   ![](assets/connect-google-acct-350x279.png)

1. 對應相關欄位（欄）中的屬性以完成模組設定。

   ![](assets/map-attributes-350x282.png)

1. 複製您剛才建立的模組，並將其連結至第二個模組 [!UICONTROL 文字剖析器] 模組。

   1. 移至試算表，複製您先前建立的工作表，並為其命名。

      例如，將其命名為「contains： text parser module and email」。

   1. 新增另一欄以儲存電子郵件內文包含的電子郵件地址。

      例如，將其命名為「Email Address Shared」。

   1. 按一下複製的 [!DNL Google Sheets] 設定安裝程式的模組。
   1. 將工作表變更為您剛建立的新工作表。
   1. 將輸出對應 [!UICONTROL 比對模式] 模組($1)至要儲存電子郵件地址（已共用電子郵件地址）的欄。

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. 按一下 **[!UICONTROL 確定]**，儲存情境，然後進行測試回合。

      您需要傳送兩封個別的電子郵件至所連線的電子郵件地址，如下所示：

      * 包含片語&quot;[!UICONTROL 文字剖析器模組]&quot; （沒有電子郵件地址）

        ![](assets/text-parser-module-350x103.png)

      * 包含上述片語和電子郵件地址

        ![](assets/above-phrase-and-email-350x106.png)

        如果您的設定沒有錯誤，您會看到第一個工作表擷取所有包含片語「 」的電子郵件[!UICONTROL 文字剖析器模組]「而第二個工作表只會擷取包含片語」的頁面[!UICONTROL 文字剖析器模組]」和電子郵件地址。 您可以參閱下方的熒幕擷取畫面。

        工作表1：

        ![](assets/worksheet-1-350x57.png)

        工作表2：

        ![](assets/worksheet-2-350x41.png)

## 資源

* [免費練習](https://regexone.com/) 瞭解規則運算式
* [瞭解電話號碼比對](https://regexone.com/problem/matching_phone_numbers) 使用Regex
* [瞭解電子郵件比對](https://regexone.com/problem/matching_emails) 使用Regex
* [測試規則運算式](https://regex101.com/)
