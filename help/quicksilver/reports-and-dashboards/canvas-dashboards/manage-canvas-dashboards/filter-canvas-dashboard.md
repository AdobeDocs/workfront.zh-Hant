---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 篩選畫布控制面板
description: 建立畫布控制面板後，您就可以將篩選器套用至控制面板。
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: 156e9d3f-49f6-4372-9749-c7124ff5baee
source-git-commit: 56d0b9281387cc7b35055461e7868c7e4a194f81
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 0%

---

# 篩選畫布控制面板

>[!IMPORTANT]
>
>畫布儀表板功能目前僅適用於參與Beta階段的使用者。 在此階段中，部分功能可能無法完成或如預期般運作。 請依照「畫布控制面板」測試版概觀文章中[提供意見回饋](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)一節的指示，提交有關您體驗的任何意見回饋。<br>
>&#x200B;>如果您對可能的錯誤或技術問題有回饋，請向Workfront支援提交票證。 如需詳細資訊，請參閱[聯絡客戶支援](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>&#x200B;>請注意，以下雲端服務供應商未提供此測試版：
>
>* 自備Amazon Web Services金鑰
>* Azure
>* Google Cloud Platform


您可以將篩選器套用至包含提示的畫布控制面板。 提示會當做篩選器修飾詞使用，套用其他篩選條件，以便您進一步縮小結果的範圍。 每次套用篩選器時都可以修改這些提示，讓您能夠調整顯示的結果，而無需編輯儀表板或每個個別報告的主要篩選條件。

## 存取需求

+++ 展開以檢視存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫</p></td> 
   <td> 
<p>任何 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td> 
<p>目前：計畫 </p> 
<p>新增：標準</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td><p>編輯報告、儀表板和行事曆的存取權</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td><p>管理儀表板的許可權</p>
  </td> 
  </tr> 
</tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先決條件

您必須先建立控制面板，然後才能進行篩選。

如需詳細資訊，請參閱[建立畫布控制面板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)。

## 篩選儀表板

請按列出的順序執行以下步驟，以篩選控制面板：

* [第1部分：建立控制面板篩選](#part-1-create-a-dashboard-filter)
* [第2部分：建立儀表板提示](#part-2-define-a-dashboard-prompt)
* [第3部分：套用儀表板提示](#step-3-apply-a-dashboard-prompt)

>[!NOTE]
>
>儀表板篩選將套用至未停用儀表板層級篩選的所有報表。  您可以展開每個報告的動作功能表，並選取&#x200B;**停用篩選器**&#x200B;選項，以排除套用控制面板層級篩選器的個別報告。


### 第1部分：建立控制面板篩選

有了控制面板篩選，您就可以對控制面板上可用的所有報表套用通用篩選，而無需修改每個個別報表的篩選。

>[!NOTE]
>
>這些篩選器只能由對控制面板具有管理存取許可權的使用者設定。


{{step1-to-dashboards}}

1. 在左側面板中，按一下&#x200B;**畫布控制面板**。

1. 在「**畫布控制面板**」頁面上，選取您要套用篩選器的控制面板。

1. 在儀表板詳細資訊頁面的左上角，按一下&#x200B;**篩選器**。 篩選器側面板隨即開啟。

1. 選取&#x200B;**編輯篩選器**。 **儀表板篩選器**&#x200B;對話方塊開啟。

1. （可選）若要新增規則，請遵循下列步驟：

   1. 選取規則方塊右側的&#x200B;**編輯**&#x200B;圖示。

      ![編輯圖示](assets/edit-icon.png)

   1. 按一下&#x200B;**新增條件**，然後新增下列資訊：
      * 選取您要作為篩選依據的欄位。
      * 選取選項（或篩選器修飾元）以定義欄位必須符合何種條件。

   1. （選擇性）按一下&#x200B;**新增篩選器群組**&#x200B;以新增另一組篩選准則。 集合之間的預設運運算元為AND。 按一下運運算元以將其變更為OR。

1. 繼續進行[第2部分：建立儀表板提示](#part-2-define-a-dashboard-prompt)。


### 第2部分：定義儀表板提示

控制面板提示可讓使用者選擇套用其他自訂篩選器至控制面板上可用的報表。

>[!NOTE]
>
>控制面板提示選項只能由對控制面板具有管理存取許可權的使用者設定。

1. 若要新增提示，請遵循下列步驟：

   1. 選取&#x200B;**新增提示**。 新欄位會出現在畫面右側。

   1. 在&#x200B;**自訂標籤**&#x200B;欄位中輸入標籤。

   1. 輸入欄位名稱，然後在提示出現在清單中時選取該欄位，以選取提示所依據的欄位。 

1. 若要新增自訂提示，請遵循下列步驟：

   1. 選取&#x200B;**新增自訂提示**。 新欄位會出現在畫面右側。

   1. （選擇性）在&#x200B;**自訂標籤**&#x200B;欄位中輸入新標籤。 預設會指派標籤&#x200B;*新自訂提示*。

   1. 按一下&#x200B;**新增選項**。

   1. 在&#x200B;**選項值**&#x200B;欄位中輸入提示名稱。

   1. 按一下&#x200B;**新增條件**，然後指定您要篩選的欄位，以及定義欄位必須符合何種條件的修飾元。

      >[!NOTE]
      >
      >自訂提示的條件只能使用文字模式編輯。 這可在單一欄位中套用多個條件。


   1. （選擇性）按一下&#x200B;**新增篩選器群組**&#x200B;以新增另一組篩選准則。 集合之間的預設運運算元為AND。 按一下運運算元以將其變更為OR。

1. 按一下&#x200B;**儲存**，將篩選器套用至儀表板。

1. 繼續進行[第3部分：套用儀表板提示](#step-3-apply-a-dashboard-prompt)。

### 步驟3：套用控制面板提示

所有有權存取控制面板的使用者可以在建立篩選和提示後，將控制面板提示套用至畫布控制面板。

{{step1-to-dashboards}}

1. 在左側面板中，按一下&#x200B;**畫布控制面板**。

1. 在&#x200B;**畫布控制面板**&#x200B;頁面上，選取您要套用提示的控制面板。

1. 在儀表板詳細資訊頁面的左上角，按一下&#x200B;**篩選器**。 篩選器側面板隨即開啟。

1. 在&#x200B;**顯示記錄位置……**&#x200B;區段中，選擇一個或所有顯示的提示的條件。 已套用提示，且已套用&#x200B;**控制面板篩選器**&#x200B;標籤會顯示在報表Widget的角落。
   ![選取條件](assets/prompts-list.png)

1. 按一下右上角的&#x200B;**關閉**&#x200B;圖示![關閉圖示](assets/close-icon.png)以隱藏面板。
