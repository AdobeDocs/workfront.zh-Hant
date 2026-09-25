---
title: Adobe Workfront規劃CX Coworker概觀
description: 您可以使用Workfront Planning中的CX Coworker對Planning中的記錄和其他物件執行類似的動作，這些動作通常會在介面中執行。 使用者的命令和AI對這些命令的執行會共同運作，以確保AI所做的變更正確地反映在您的環境中。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
    internal-label: Workfront Planning
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 3934b1b333f86c8c700617871bfaac23d2b19213
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 1%
---

# Adobe Workfront規劃CX Coworker概觀

<!--replaced information from the AI Assistant for Planning article with CX Coworker-->

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 在「預覽」版發行後，啟用的客戶每月可在「生產」環境中使用相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

CX Coworker是對話式介面，您可在其中以淺白語言描述目標，接著在Workfront Planning和其他連線的Adobe系統中規劃、執行及驗證工作，再重新帶回供您核准。

CX Coworker保留AI Assistant目前的所有功能，同時在新的全熒幕體驗和Workfront右側邊欄中新增更強大的端對端功能。

它會在您組織現有的產品層級存取控制項內運作，因此使用者只能採取已在Workfront中獲准採取的動作，且預設為唯讀存取權，以及由Workfront管理員控制的寫入存取權。

>[!IMPORTANT]
>
>CX Coworker目前不適用於保健、金融或某些具有敏感資料的其他行業的組織。 AI助理可供這些組織使用。
>
>如需詳細資訊，請參閱[AI助理概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。


## 存取權要求

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
<p>具有Planning套件的任何Workfront或工作流程</p>
或
<p>以獨立產品形式購買時的任何Planning套件</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe計畫授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td>  
   <p>您的管理員必須執行下列操作，以允許在Planning中存取CX Coworker：</p>
   <ul>
   <li><p>當您同時具有Workflow和Planning套件時，將Workflow和Planning授權型別新增到您的存取層級</p></li>
   <li><p>取消選取存取層級中的「在Workfront中停用CX Coworker面板」設定。 預設會選取此選項。</p></li></ul>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>系統設定</p></td> 
   <td>   <p>您的Workfront管理員必須在「設定」的「系統偏好設定」區域中選取「唯讀」和「唯寫」MCP工具。 依預設，會選取唯讀MCP工具。</p> 
    </td> 
  </tr> 
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## CX Coworker的考量事項

* 貴公司使用者必須先為貴組織啟用CX Coworker，才能使用。

  如需詳細資訊，請參閱[CX Coworker概觀](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)。

* 在Workfront為您的Workfront執行個體啟用代理程式後，Workfront主要管理員可以使用此代理程式，他們可以為您的組織啟用它。 如需詳細資訊，請參閱[設定系統偏好設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

* Workfront管理員也必須在存取層級中為您啟用CX Coworker 。 如需詳細資訊，請參閱[建立和修改存取層級](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* CX Coworker可處理Workfront或Workfront Planning中您有存取許可權的資訊和物件。 在Planning右側邊欄中，「同事」面板會在您已開啟的工作區、記錄型別或記錄頁面的內容中運作。

* CX Coworker在Planning區域中執行的動作會根據您的Workfront Planning許可權和Workfront存取層級來設定。 如需詳細資訊，請參閱下列文章：

  * [在Adobe Workfront Planning中共用許可權的概觀](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [使用Adobe Workfront Planning時的授權型別概觀](/help/quicksilver/planning/access/license-type-overview.md)

* CX Coworker代表使用者所做的變更會在紀錄的紀錄面板中進行追蹤。

* CX Coworker執行的動作是永久性的，且無法復原。 例如，刪除欄位後便無法還原。 在接受之前，請先檢閱CX Coworker提出的所有動作。

* 透過CX Coworker建立、更新或刪除物件時，CX Coworker會顯示預期動作並要求確認。 之後，您可以確認或取消動作。

## 目前適用於CX Coworker的功能

目前，CX Coworker可在Workfront的Planning區域中使用，它使用一組技能來存取和控制Planning物件的資訊。 如需詳細資訊，請參閱[CX Coworker技能](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-skills.md)。

您可以使用CX Coworker來執行下列動作：

* 搜尋記錄。 您可以依據任何記錄欄位中包含的資訊進行搜尋。
* 建立記錄。 含有新記錄連結的ID會在建立記錄後顯示。 您可以指定要在建立過程中更新的欄位，例如日期或說明。
* 根據您上傳的檔案建立記錄。 Workfront支援下列CX Coworker檔案格式：

  PPTX、PDF、DOCX、XLSX、PPT、DOC、TXT和大部分影像格式
* 更新您在畫面上看到的記錄欄位
* 刪除、複製或還原記錄
* 將記錄連結至其他記錄
* 檢視記錄的變更記錄


## 在Workfront Planning中找到CX Coworker

您可以在Workfront Planning的下列區域中找到CX Coworker：

* 熒幕右上角的主要導覽列。
* 在新的索引標籤中開啟記錄時，將其置於記錄的詳細資訊區域中。

## 存取「規劃」區域中的CX Coworker

1. 登入Workfront，然後按一下左上角的&#x200B;**主功能表**&#x200B;圖示![行主功能表](assets/lines-main-menu.png)，然後按一下&#x200B;**規劃**。

   「規劃」區域隨即開啟。

   在頁面的右上角找到&#x200B;**同事**&#x200B;圖示![同事圖示](assets/coworker-icon.png)，或繼續下列步驟。

1. 按一下&#x200B;**工作區卡片**。

1. 按一下&#x200B;**記錄型別卡片**。

1. 按一下&#x200B;**記錄**&#x200B;以開啟記錄的&#x200B;**詳細資料**&#x200B;頁面，然後按一下&#x200B;**在新索引標籤中開啟**&#x200B;圖示![在新索引標籤中開啟](assets/open-workspace-on-new-tab-icon.png) 。

1. 按一下畫面右上角的&#x200B;**CX Coworker圖示** ![同事圖示](assets/coworker-icon.png)。

1. 在提供的空白處，開始輸入CX Coworker的命令，然後在完成後按一下Enter 。

   ![含空白命令方塊的CX Coworker面板](assets/cx-coworker-right-rail.png)

   例如，您可以鍵入下列其中一項：

   * 建立名為「2026年夏季優惠」的新行銷活動記錄
   * 將夏季行銷活動記錄中的預算欄位更新為$75,000
   * 刪除名為「舊促銷」的行銷活動記錄
   * 還原我意外刪除的行銷活動

   >[!TIP]
   >
   >在要求Workfront對物件執行編輯動作之前，請確定您的CX Coworker管理員已在系統偏好設定中啟用僅限寫入的MCP工具。

   CX Coworker處理命令時會顯示視覺指示器，設定回應時間的預期值。

   收到成功回應後，請遵循提供的連結或注意左側的變更。


1. （選擇性）按一下&#x200B;**展開全熒幕**&#x200B;圖示![展開全熒幕圖示](assets/expand-full-screen-icon.png)，以開啟全瀏覽器標籤中的「同事聊天」方塊。


