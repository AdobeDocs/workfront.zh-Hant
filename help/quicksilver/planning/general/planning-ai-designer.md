---
title: 開始使用Adobe Workfront Planning Designer
description: 使用Adobe Planning Designer，您可以產生新的工作區、完成Workfront Planning中的記錄型別和欄位、將物件新增至工作區，或檢視記錄的變更歷史記錄。
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bd3dde54d986416af847b2f3b2a1e8570d5ce3f2
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 1%

---


<!--add these at release to the metadata:

author: Alina, Becky
feature: Workfront Planning
role: User, Admin -->

# 開始使用Adobe Workfront Planning Designer

{{planning-important-intro}}

您可以使用由AI支援的Adobe Planning Designer來產生新工作區、將物件新增至工作區（記錄型別、記錄、檢視或欄位），或檢視記錄的變更歷史記錄。

>[!IMPORTANT]
>
>Planning Designer目前僅適用於參與「已關閉的Beta」計畫的使用者。

如需Workfront Planning的相關資訊，請參閱下列文章：

* [Adobe Workfront Planning的一般資訊](/help/quicksilver/planning/planning-information.md)
* [開始使用Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning存取權概觀](/help/quicksilver/planning/access/access-overview.md)


## 存取需求<!--edit theses??-->

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

目前，您可以傳送電子郵件至sargism@adobe.com，申請參與Planning Designer的封閉Beta計畫。

收到電子郵件後，我們的工程團隊將在您的Workfront執行個體中開啟規劃Designer 。

>[!IMPORTANT]
>
>您的公司必須先接受AI Assistant合約，系統才能使用Planning Designer。

## Planning Designer的相關考量事項

* 若要使用Planning Designer，您必須先為組織開啟AI助理。 AI助理必須具備下列條件，組織中的所有人都能使用：

   * Workfront必須將AI助理提供給您的組織使用。

     如需詳細資訊，請參閱[ AI助理的必要條件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)。
   * Workfront讓您的AI助理可以使用後，Workfront的主要管理員就可以存取它。

     如需詳細資訊，請參閱[設定您系統的基本資訊](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)。
   * Workfront管理員必須接受AI助理合約，然後為所有其他使用者開啟AI助理。

     如需詳細資訊，請參閱[啟用或停用AI助理](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。
* 系統管理員為您的組織開啟AI助理之後，如果已經為您的組織提供Planning助理，預設情況下，所有使用者都可以使用。
* 當您在Planning區域使用Planning Designer時，AI助理也可以執行由Planning助理執行的動作。
* AI助理在「計畫」區域中執行的動作或Planning Designer執行的動作會與Workfront Planning許可權和Workfront存取層級相關。

  如需詳細資訊，請參閱下列文章：

   * [在Adobe Workfront Planning中共用許可權的概觀](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/planning/access/license-type-overview.md)

* AI助理或Planning Designer代表使用者所做的變更會在紀錄的紀錄面板中進行追蹤。

* Planning Designer所做的動作是永久性的，且可能不可逆轉。 例如，刪除欄位後便無法還原。 在接受之前，請先檢閱Designer提出的所有動作。

  >[!IMPORTANT]
  >
  >透過Planning Designer建立、更新或刪除物件時，提示只會要求確認不可逆的動作。 例如，刪除記錄型別或工作區是不可逆的。 刪除記錄則否。 只有在嘗試刪除記錄型別或工作區時，Planning Designer才會要求確認。

* 當您使用Planning Designer建立工作區和記錄型別時，也會自動建立檢視和欄位。

## 目前適用於Planning Designer的功能

您可以使用Planning Designer或AI助理來執行下列任一動作：

* 建立及設定工作區

* 建立記錄型別，包括定義及新增全域記錄型別至工作區

* 設計欄位或公式欄位

* 建立、刪除、複製和還原記錄

* 編輯、更新、附加記錄中的欄位

* 將記錄連結至其他記錄

* 存取記錄變更記錄

* 建置自訂檢視

* 匯入檔案以建立記錄

  例如，您可以上傳公司中的組織圖圖片，而Planning Designer可以據此建立工作區。

  從匯入的檔案中建立物件只能在Planning Designer中使用，不能在AI助理中使用。

  >[!IMPORTANT]
  >
  >雖然我們支援.XLSX和.CSV檔案型別，但無法透過Planning Designer用於大規模記錄匯入。
  >如果您目前需要匯入大量記錄，建議您使用Planning中提供的手動功能進行匯入。
  >
  >如需詳細資訊，請參閱[從CSV或Excel檔案匯入資訊，以建立記錄](/help/quicksilver/planning/records/import-file-to-create-records.md)。
  >如需檔案型別限制，請參閱[使用由AI支援的表單填寫功能來使用提示或檔案填寫請求](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md)中的「根據上傳的檔案取得建議」一節。


  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## 使用Planning Designer建立或更新物件

除非另有指定，否則您可以使用Planning Designer或AI助理在Workfront Planning中建立或更新物件。

1. 登入Workfront，然後按一下左上角的&#x200B;**主功能表**&#x200B;圖示![行主功能表](assets/lines-main-menu.png)，然後按一下&#x200B;**規劃**。

   **規劃**&#x200B;區域隨即開啟。

   ![Design with AI按鈕（在Workspaces頁面上）](assets/design-with-ai-button-on-workspaces-page.png)

1. 按一下&#x200B;**使用AI設計**。

   **計畫Designer**&#x200B;視窗隨即開啟。

   ![規劃Designer視窗](assets/planning-designer-window.png)

1. 在提供的空白處，開始輸入AI助理的提示，然後在完成時按一下Enter。

   <!--add screen shot-->

   例如，您可以鍵入類似以下提示的提示：

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

1. 在收到成功的回應後，請依照提示區中提供的連結建立、更新或檢閱請求的物件。

   當您同意建立物件時，您的變更會顯示在提示區域的右側。

   您可以在提示右側的預覽區域中檢視工作區、記錄型別、欄位、檢視和記錄。

   >[!TIP]
   >
   >某些物件會立即建立，不需要確認。

1. （選擇性）輸入其他提示以進一步編輯物件。
1. （選擇性）按一下&#x200B;**顯示或隱藏預覽畫面**&#x200B;圖示![隱藏或顯示預覽畫面圖示](assets/hide-show-preview-screen-in-planning-designer.png)以開啟或關閉右側的預覽畫面。
1. 按一下&#x200B;**在新標籤中開啟工作區** ![在新標籤中開啟工作區](assets/open-workspace-on-new-tab-icon.png)，以在新標籤中開啟您正在更新的工作區。
1. 按一下&#x200B;**關閉**&#x200B;圖示&#x200B;**X**&#x200B;以關閉Planning Designer並開啟「工作區」區域。
1. 開啟您使用Planning Designer編輯的工作區，然後對其物件進行進一步的變更。

## 關閉貴組織的Planing Designer

在您的Workfront管理員接受AI Assistant合約後，會依預設為組織中的每個人開啟Planning Designer 。

若要將其關閉：

1. 以系統管理員身分登入Workfront。
1. 按一下熒幕左上角的&#x200B;**主功能表** ![主功能表圖示](assets/main-menu-shell.png)，然後按一下&#x200B;**設定**。
1. 按一下左側面板中的&#x200B;**系統** >，然後移至&#x200B;**AI偏好設定**&#x200B;區域。
1. 關閉&#x200B;**規劃Designer**&#x200B;設定。<!--add new screen shot with info icon-->

   系統偏好設定中的![規劃Designer設定](assets/planning-designer-toggle-in-system-preferences.png)
1. 按一下「**儲存**」。

   這會移除系統中所有使用者的Planning Designer。






