---
title: 使用AI自動填寫請求
content-type: reference
description: 您可以使用AI自動填寫請求欄位。
author: Becky
feature: Get Started with Workfront
exl-id: d053e604-5a28-4fd3-8f89-4467b6e46f02
source-git-commit: a3e93311277bc5b68063e0ec1cbdcce3a40eb3dd
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

---

# 使用AI自動填寫請求

>[!NOTE]
>
>此功能目前是封閉測試版的一部分。 若要啟用此功能，請連絡sargism@adobe.com。
>
>若要符合封閉Beta版的資格，您的組織必須符合使用Workfront AI Assistant的需求。 如需詳細資訊，請參閱[ AI助理的必要條件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)。

AI可協助您自動填寫請求欄位。 它可以根據先前的請求來建議欄位值，或從文字（例如電子郵件和已上傳的檔案）中剖析欄位值。

您可以在提交請求之前核准或拒絕這些建議。

自動填寫不會覆寫您已填寫的任何欄位。

## 填寫表單時取得建議

自動填寫可在您填寫表單時建議欄位值。 當您在請求欄位中輸入值時，Workfront會將這些值與先前的請求進行比較。 如果輸入的值與先前請求中類似內容中的其他欄位值緊密相關，Workfront會建議這些值。

例如，如果診所一律使用相同的計費代碼，Workfront會在輸入診所名稱時，建議在適當的欄位中輸入計費代碼。

若要根據先前的請求使用建議：

1. 開始建立請求。

   如需指示，請參閱[建立及提交要求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 開始填寫欄位。

   當您填寫欄位時，其他欄位可能會顯示建議。

1. 對於每個欄位建議，請在該欄位下方選取&#x200B;**接受**&#x200B;或&#x200B;**拒絕**。

   或

   在頁面頂端選取「**全部接受**」或「**全部拒絕**」以接受或拒絕所有建議。

## 從文字提示取得建議

自動填寫可根據文字（例如電子郵件）建議欄位值。 您貼入文字區塊，Workfront會處理文字，以根據文字建議欄位值。

例如，如果電子郵件包含「此到期日為6月1日」，而請求表單有到期日的欄位，則Workfront會建議該欄位值在6月1日。

此型別的建議也會檢查先前是否有類似內容的請求。 例如，如果提示指出請求是針對特定使用者端，Workfront可以根據先前的請求，自動尋找並輸入該使用者端的帳單地址。

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
1. 對於每個欄位建議，請在該欄位下方選取&#x200B;**接受**&#x200B;或&#x200B;**拒絕**。

   或

   在頁面頂端選取「**全部接受**」或「**全部拒絕**」以接受或拒絕所有建議。

## 根據您上傳的檔案取得建議

自動填寫可根據您上傳的檔案建議欄位值。

此型別的建議也會檢查先前是否有類似內容的請求。 例如，如果提示指出請求是針對特定使用者端，Workfront可以根據先前的請求，自動尋找並輸入該使用者端的帳單地址。

### 檔案上傳護欄

#### 支援的檔案類型

支援的檔案型別如下：

* BMP
* CSV
* DOC
* DOCX
* GIF
* JPEG
* JPG
* ODP
* ODS
* ODT
* PDF
* PNG
* PPT
* PPTX
* RTF
* TIFF
* TXT
* XLS
* XLSX

#### 支援的檔案大小

每個檔案的大小最多可達100 MB

#### 檔案數

您最多可上傳50個檔案（頁面、幻燈片或工作表）。

>[!IMPORTANT]
>
>檔案會轉換為一系列影像，每個影像都視為個別檔案。
>
>例如，您可以上傳一個含有50張幻燈片的PowerPoint，或是5個各有10頁的Word檔案。

#### 其他最佳實務

上傳要求自動填寫的檔案時，請考量下列事項：

* 自動填色目前已針對拉丁字母最佳化。
* 我們建議使用8點或更大的文字大小。
* 自動填色可能對檔案中的影像造成困難，例如旋轉或扭曲影像、圖形、計算或利用影像中物件的空間原因。
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
1. 對於每個欄位建議，請在該欄位下方選取&#x200B;**接受**&#x200B;或&#x200B;**拒絕**。

   或

   在頁面頂端選取「**全部接受**」或「**全部拒絕**」以接受或拒絕所有建議。

