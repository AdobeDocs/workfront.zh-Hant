---
title: 開始使用Adobe Workfront Planning Designer
description: 使用Adobe Planning Designer，您可以產生新的工作區、完成Workfront Planning中的記錄型別和欄位，或將物件新增至工作區，或檢視記錄的變更歷史記錄。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bf34bfa2059d227eca3faa3d719adcf4d711e457
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---


# 開始使用Adobe Workfront Planning Designer

{{planning-important-intro}}

使用Adobe Planning Designer，您可以產生新的工作區、完成Workfront Planning中的記錄型別和欄位，或將物件新增至工作區，或檢視記錄的變更歷史記錄。

>[!IMPORTANT]
>
>Planning Designer目前僅適用於參與封閉Beta階段的使用者。

## 存取需求<!--edit theses-->

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<p>任何Workfront和Planning套件</p>
<p>任何工作流程和Planning套件</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 為Planning Designer註冊Closed Beta方案

<!--edit this Or create a new article under Beta programs?? -->

目前，您可以申請參與Planning Designer的封閉Beta計畫。

## Planning Designer的相關考量事項

<!--these are from the AI Assistant - edit these-->

* 若要使用Planning Designer，您必須先為組織啟用AI助理。 必須啟用下列專案，AI助理才能供組織中的每個人使用：

   * AI助理必須先為貴組織啟用，才能供貴公司的使用者使用。 如需詳細資訊，請參閱[AI助理概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。
   * Workfront為貴組織啟用AI助理後，即可供Workfront主要管理員使用。 如需詳細資訊，請參閱[設定您系統的基本資訊](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

   * Workfront管理員必須為所有其他使用者啟用AI助理。 如需詳細資訊，請參閱[啟用或停用AI助理](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

   * AI助理會在每個頁面的內容中運作。 您為AI助理提交的請求必須參考您開啟的頁面中可用的功能。

* 若要使用Planning Designer，系統管理員必須在設定的「系統偏好設定」區域中將其啟用。

* AI助理在「計畫」區域中執行的動作會根據您的Workfront Planning許可權和Workfront存取層級來設定。 如需詳細資訊，請參閱下列文章：

   * [在Adobe Workfront Planning中共用許可權的概觀](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/planning/access/license-type-overview.md)

* AI助理員代表使用者所做的變更會在紀錄的紀錄面板中進行追蹤。

* 您可以使用命令來復原動作。 例如，您可以輸入「復原上次變更」來回覆變更。

* 透過AI助理建立、更新或刪除物件時，AI助理會顯示預期的動作並要求確認。 之後，您可以確認或取消動作。

—>

## 目前適用於Planning Designer的功能

<!--edit these- they are from the Ai Assistant: 

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted

-->

您可以使用Planning Designer或AI助理來執行下列任一動作：

* 建立及設定工作區

* 建立記錄型別

* 設計欄位或公式欄位

* 建立、刪除、複製和還原記錄

* 編輯、更新、附加記錄中的欄位

* 將記錄連結至其他記錄

* 存取記錄變更記錄

* 建置自訂檢視

* 匯入檔案以建立記錄。 從匯入的檔案建立記錄只能在Planning Designer中使用，不能在AI助理中使用。<!--add information about supported files-->

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## 在Workfront Planning中找到Planning Designer

您可以從Workfront Planning首頁面存取Planning Designer。

<!--add screen shot-->

您也可以使用AI助理來利用Planning Designer所提供的相同功能。

## 為您的組織啟用Planing Designer

身為Workfront管理員，您必須先為組織啟用Planning Designer 。

<!--add steps here-->

## 使用Planning Designer建立或更新物件

除非另有指定，否則您可以使用Planning Designer或AI助理在Workfront Planning中建立或更新物件。

1. 登入Workfront，然後按一下熒幕右上角的&#x200B;**主功能表**&#x200B;圖示![點主功能表](assets/dots-main-menu.png)，或左上角的&#x200B;**主功能表**&#x200B;圖示![行主功能表](assets/lines-main-menu.png) （若有）。

1. 按一下&#x200B;**計畫**。 「規劃」區域隨即開啟。

1. 按一下&#x200B;**使用AI設計**。

1. 在提供的空間中，開始輸入AI助理的命令，然後在完成時按一下Enter。

   <!--add screen shot-->

   例如，您可以輸入類似以下的要求：

   * 建立並設定包含五種記錄型別的工作區以管理行銷活動

   * 建立當年每個月的行銷活動

   * 為行銷設計工作區的狀態新增行銷活動欄位

   * 刪除狀態為陳舊的所有記錄

   * 將所有Planning行銷活動更新為作用中狀態

   * 將Campaign連結至行銷設計工作區中的角色

   * 顯示「情人節」行銷活動的變更記錄

   * 在行銷設計工作區中建立行銷活動的時間軸檢視

   * 匯入檔案以建立記錄。 從匯入的檔案建立記錄只能在Planning Designer中使用，不能在AI助理中使用。

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

   視覺預覽會顯示助理可以建置的專案範例。

1. 在收到成功的回應後，請依照命令列中提供的連結來建立、更新或檢閱請求的物件。




