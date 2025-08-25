---
title: 使用提示或檔案自動填寫請求
content-type: reference
description: 您可以使用AI輸入提示或提供檔案來自動填寫請求欄位。
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 2%

---

# 使用提示或檔案自動填寫請求

>[!NOTE]
>
>* 此功能將作為開放式測試版在以下排程中提供：
>
>   * 每月發行： 2025年9月11日
>   * 每季發行： 2025年10月16日
>
>* 若要使用此功能，您的組織必須符合使用Workfront AI Assistant的需求。 如需詳細資訊，請參閱[ AI助理的必要條件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)。

AI可協助您根據輸入的提示自動填寫請求欄位。 它也可以根據文字（例如電子郵件和已上傳的檔案）填寫欄位。 您可以在提交請求之前核准或拒絕這些建議。

自動填寫不會覆寫您已填寫的任何欄位。

使用者不會收到他們無法存取的資料建議。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>新增：投稿人或更高版本</p>
   或
   <p>目前：要求或以上</p>
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

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

若要使用提示或檔案自動填寫請求，必須套用下列&#x200B;**所有**：

* 貴組織必須使用Adobe IMS (Identity Management系統)
* 必須啟用Adobe Unified Experience
* 貴組織必須有Select、Prime或Ultimate Workfront計畫
* Adobe必須已簽署檔案Adobe Gen AI合約

  如需簽署合約的詳細資訊，請參閱AI助理總覽一文中的[簽署Adobe Gen AI合約](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。
* AI助理必須在您組織的系統設定中啟用。 這項工作由Workfront管理員管理。

  如需有關在系統設定中啟用AI助理的詳細資訊，請參閱[啟用或停用AI助理](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

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
1. 對於每個欄位建議，請為該欄位選取&#x200B;**接受**&#x200B;或&#x200B;**拒絕**。

   ![接受或拒絕建議](assets/accept-reject-suggestion.png)

   或

   在頁面頂端選取「**全部接受**」或「**全部拒絕**」以接受或拒絕所有建議。

   >[!NOTE]
   >
   >當您提交請求時，任何未稽核的建議都會自動被接受。

## 根據您上傳的檔案取得建議

自動填寫可根據您上傳的檔案建議欄位值。

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
<li>JPEG</li>
</ul>
</td>
<td>
<ul>
<li>ODP</li>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>PNG</li>
<li>PPT</li>
</ul>
</td>
<td>
<ul>
<li>PPTX</li>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
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
<td><b>支援的</b><br>自動填寫可以填寫</td>
<td><b>不支援</b> <br>自動填入未填入</td>
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
