---
title: 使用由AI支援的表單填寫功能，使用提示或檔案填寫請求
content-type: reference
description: 您可以使用AI輸入提示或提供檔案來自動填寫請求欄位。
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
source-git-commit: b34d7f48a51acf4bd6ddfa203c9e0024b2e8c280
workflow-type: tm+mt
source-wordcount: '1352'
ht-degree: 3%

---

# 使用由AI支援的表單填寫功能，使用提示或檔案填寫請求

>[!NOTE]
>
>若要使用此功能，您的組織必須符合使用Workfront AI Assistant的需求。 如需詳細資訊，請參閱[ AI助理的必要條件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)。

AI表單填寫可協助您根據輸入的提示自動填寫請求欄位。 它也可以根據文字（例如電子郵件和已上傳的檔案）填寫欄位。 您可以在提交請求之前核准或拒絕這些建議。

AI表單填寫不會覆寫您已填寫的任何欄位。

使用者不會收到他們無法存取的資料建議。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>投稿人或以上</p>
   <p>要求或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯問題的存取權</p>  </td> 
  </tr> 
   <td role="rowheader">物件許可權</td> 
   <td><p>將請求新增至請求佇列的存取權</p> <p>檢視現有請求或更高的許可權</p> <p>如需設定要求佇列的資訊，請參閱<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立要求佇列</a>。 </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

若要使用AI表單填寫來使用提示或檔案填寫請求，必須套用下列&#x200B;**所有**：

* 貴組織必須已移轉至Adobe IMS (Identity Management系統)
* 必須啟用Adobe Unified Experience
* 貴組織必須有Select、Prime或Ultimate Workfront計畫
* Adobe必須已簽署檔案Adobe Gen AI合約

  如需簽署合約的詳細資訊，請參閱AI助理總覽一文中的[簽署Adobe Gen AI合約](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。
* AI助理必須在您組織的系統設定中啟用。 這項工作由Workfront管理員管理。

  如需有關在系統設定中啟用AI助理的詳細資訊，請參閱[啟用或停用AI助理](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

## 從文字提示取得建議

AI表單填寫可根據文字（例如電子郵件）建議欄位值。 您貼入文字區塊，Workfront會處理文字，以根據文字建議欄位值。

例如，如果電子郵件包含「這在6月1日到期」，並且請求表單有到期日期的欄位，則AI表單填寫將建議該欄位值在6月1日。

填寫表單時，Workfront也會檢查先前是否有類似內容的請求。 例如，如果提示指出請求是針對特定使用者端，Workfront可以根據先前的請求，自動尋找並輸入該使用者端的帳單地址。

您可以貼上文字以套用至整個表單或表單的單一區段。

若要根據貼上的文字提示使用建議：

1. 開始建立請求。

   如需指示，請參閱[建立及提交要求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 若要將文字提示套用至整個表單，請按一下表單名稱下方的AI圖示![AI圖示](assets/request-prompt-icon.png)。

   或

   若要套用單一區段的文字提示，請按一下區段名稱旁的AI圖示![AI圖示](assets/request-prompt-icon.png)。

1. 將文字貼到提示方塊中。
1. 按一下&#x200B;**填寫表單**。

   Workfront會產生表單的建議。
1. 對於每個欄位建議，請為該欄位選取&#x200B;**接受**&#x200B;或&#x200B;**拒絕**。

   ![接受或拒絕建議](assets/accept-reject-suggestion.png)

   或

   在頁面頂端選取「**全部接受**」或「**全部拒絕**」以接受或拒絕所有建議。

   >[!NOTE]
   >
   >當您提交請求時，任何未稽核的建議都會自動被接受。

### 文字提示範例

這些範例顯示AI可參考其他專案的各種方式的提示。

#### 參考過去的客戶行銷活動

>[!BEGINSHADEBOX]

建立類似的行銷活動要求，就像我們（客戶公司）在第二季上市時所做的那樣，但這次是針對他們的汽車部門。 保留相同的傳遞集和受眾設定檔。

>[!ENDSHADEBOX]

#### 在現有專案上建置

>[!BEGINSHADEBOX]

使用我們去年春天在（專案名稱）專案啟動中所使用的相同設定。 我想要進行以相同執行對象為目標的數位廣告行銷活動，但包含本季的更新日期。

>[!ENDSHADEBOX]

#### 重複使用過去交付專案的樣式

>[!BEGINSHADEBOX]

準備與我們去年執行的（客戶公司）夏季促銷活動類似的請求。 專注於社群媒體資產，保持西班牙語為主要語言，並將預算調整為75,000美元。

>[!ENDSHADEBOX]

#### 展開舊版行銷活動型別

>[!BEGINSHADEBOX]

請參考Q1的（行銷活動名稱）網路研討會系列行銷活動。 我想要相同的註冊工作流程和資產，但這次主題是「財務規劃的人工智慧」，對象是年輕的專業人士。

>[!ENDSHADEBOX]

#### 重複不同產品的請求

>[!BEGINSHADEBOX]

設定行銷活動請求，就像我們處理的（客戶公司）品牌重塑專案一樣，但取代為（新客戶公司）作為客戶。 讓所有交付專案與企業品牌保持一致。

>[!ENDSHADEBOX]

#### 含隱含參照的敘述風格

>[!BEGINSHADEBOX]

我們正在策劃一場類似於去年所推出的假日社交廣告的促銷活動。 預算應約為5萬，目標是創造銷售機會，交付成果應包含Instagram和TikTok資產。

>[!ENDSHADEBOX]


## 根據您上傳的檔案取得建議

由AI支援的表單填寫可使用提示填寫請求，或檔案可以根據您上傳的檔案建議欄位值。

此型別的建議也會檢查先前是否有類似內容的請求。 例如，如果提示指出請求是針對特定使用者端，Workfront可以根據先前的請求，自動尋找並輸入該使用者端的帳單地址。

### 檔案上傳護欄

#### 支援的檔案類型

支援的檔案型別如下：

<table>
<tr style="border: 0;">
<td>
<ul>
<li>BMP</li>
<li>CSV</li>
<li>DOC</li>
<li>DOCX</li>
<li>GIF</li>
<li>JPEG</li>
<li>ODP</li>
</ul>
</td>
<td>
<ul>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>PNG</li>
<li>PPT</li>
<li>PPTX</li>
</ul>
</td>
<td>
<ul>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
<li>WEBP</li>
<li>XLS</li>
<li>XLSX</li>
</ul>
</td>
</tr>
</table>

#### 支援的檔案大小

每個檔案的大小最多可達100 MB

#### 檔案數

您最多可上傳50個檔案（頁面、幻燈片或工作表）。

>[!IMPORTANT]
>
>檔案會轉換為一系列影像，每個影像都視為個別檔案。
>
>例如，您可以上傳一個含有50張幻燈片的PowerPoint，或是5個各有10頁的Word檔案。

#### 支援的欄位型別

Workfront欄位型別會影響指定欄位是否可自動填入。

<table>
<tr>
<td><b>支援的</b><br>由AI支援的表單填寫可以填寫</td>
<td><b>不支援</b> <br>由AI支援的表單填寫未填寫</td>
</tr>
<tr>
<td>
<ul>
<li>單行文字</li>
<li>文字區域或段落</li>
<li>日期欄位</li>
<li>核取方塊</li>
<li>選項按鈕</li>
<li>單選與多選下拉式清單</li>
</ul>
</td>
<td><li>自動提示</li>
<li>外部查詢</li>
<li>內部查詢</li>
<li>參考</li>
<li>WF Planning內嵌欄位</li>
</ul>
</td>
</tr>
</table>

#### 其他最佳實務

將檔案上傳至AI表單填寫時，請考量下列事項：

* AI表單填入目前已針對拉丁字母最佳化。
* 我們建議使用8點或更大的文字大小。
* AI Form Fill可能難以處理檔案中的影像，例如旋轉或扭曲的影像、圖形、計數或利用影像中物件的空間原因。
* 一如既往，我們建議在提交請求前先檢查結果的準確性。

### 上傳檔案以自動填寫請求

您可以上傳要套用至整個表單或表單單一區段的檔案。

1. 開始建立請求。

   如需指示，請參閱[建立及提交要求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 若要將檔案套用至整個表單，請按一下表單名稱下方的AI圖示![AI圖示](assets/request-prompt-icon.png)。

   或

   若要將檔案套用至單一區段，請按一下區段名稱旁的AI圖示![AI圖示](assets/request-prompt-icon.png)。

1. 按一下&#x200B;**上傳檔案**，然後從檔案管理員中選取檔案。

   或

   將檔案從您的檔案管理員拖曳至&#x200B;**上傳檔案以自動填寫請求表單**&#x200B;方塊。
1. 按一下&#x200B;**填寫表單** （共&#x200B;**份）填寫區段**。

   Workfront會產生表單的建議。
1. 對於每個欄位建議，請為該欄位選取&#x200B;**接受**&#x200B;或&#x200B;**拒絕**。

   ![接受或拒絕建議](assets/accept-reject-suggestion.png)

   或

   在頁面頂端選取「**全部接受**」或「**全部拒絕**」以接受或拒絕所有建議。

   >[!NOTE]
   >
   >當您提交請求時，任何未稽核的建議都會自動被接受。

## 疑難排解

如果您沒有收到預期的建議，可能是因為下列其中一個原因：

* 您必須在系統中擁有至少一個月的請求資料，然後才能建議來自先前請求的欄位值。
* 您在上傳要從中提取建議的檔案時，可能未依循檔案上傳護欄。 如需詳細資訊，請參閱本文中的[檔案上傳護欄](#document-upload-guardrails)。
