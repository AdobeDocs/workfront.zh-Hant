---
title: 針對Adobe Workfront Planning使用環境升級
description: 您可以使用「環境升級」功能，將Workfront Planning工作區、記錄型別、欄位和檢視從一個Workfront環境複製到另一個環境。 您不需要手動重建所有專案，而是在來源環境中將設定組裝成套件並安裝在目標環境中。
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 00706e8c7ed590cf112f4817da9740a970a4a4b3
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 2%
---

# 針對Adobe Workfront Planning使用環境升級

<!--add to TOC-->
<!--add to miniTOC-->

<!--
Not sure if this bit will ever be needed because this only exists when both Preview and Prod have the features in parity. Features released here always come to both environments at the same time: 

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

<!--if Lilit says this is not for STA, break the intro and specify that; she is checking on this-->

您可以使用「環境升級」功能，將Workfront Planning工作區、記錄型別、欄位和檢視從一個Workfront環境複製到另一個環境。

您不需要手動重建所有專案，而是在來源環境中將設定組裝成套件並安裝在目標環境中。

搭配Planning使用環境升級類似於將其用於Workfront。 如需詳細資訊，請參閱文章[Adobe Workfront測試環境](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-testing-environments.md)中的「環境升級」一節。

## 搭配Planning使用環境升級的相關考量事項

* 您必須是Workfront管理員才能使用「環境升級」。
* 以下專案是透過環境升級匯入：

  * 工作區
  * Workspace區段
  * 記錄類型
  * 欄位
  * 檢視
  * 階層
  * 共用所有物件的設定
  * 自動化<!--this might not be part of it; Lilit is checking-->
  * 請求表單
  * 業務規則
  * 連線的物件
  * 工作區所依賴的物件或其他共用物件的物件，例如群組、專案團隊、工作角色。 存在下列情況：

    * 如果目標環境中已存在同名物件，Workfront會標示衝突，由您決定如何處理。
    * 如果目標環境中不存在共用物件的專案團隊或群組，則推進會建立它。
* 您可以針對每個物件執行下列動作：

  * 將其建立為新物件
  * 使用現有物件，但以新名稱建立它
  * 覆寫現有的物件。 覆寫會取代目標中的設定。

* 安裝可能需要幾分鐘的時間。 您可以視需要從結果頁面復原安裝。
* 建議您儘可能先測試此程式，再繼續進行。 您可以先安裝到沙箱或預覽環境，然後再將它提升到生產環境。

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
<p>Prime或Ultimate Workflow套件搭配Prime或Ultimate計畫套件</p>
<p>以獨立產品形式購買時的Prime或Ultimate Planning套件</p>
   </td> 
   </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>Workflow Standard</p>    
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Planning授權</p></td> 
   <td><p>規劃標準</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>擁有Workflow和Planning套件時，您必須將Workflow和Planning授權型別新增到存取層級</p>  
   <p>您必須是系統管理員</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區的許可權</p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  
   </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用環境升級匯入Planning組態

以下是將Planning組態升級至其他環境的主要步驟：

* [在來源環境中建立封裝](#create-a-package-in-the-source-environment)
* [讓封裝準備就緒，可供安裝](#make-the-package-ready-to-install)
* [在目標環境中安裝套件](#install-the-package-in-the-target-environment)
* [驗證結果](#verify-the-results)

請依照以下章節的指示，在兩個Workfront環境之間複製Planning設定。

### 在來源環境中建立套件

1. 擁有已備妥所需設定的來源環境。
1. 在來源環境中，按一下&#x200B;**主要功能表** ![主要功能表](assets/main-menu-shell.png)，然後前往&#x200B;**設定** > **系統** > **環境升級**。
**設定套件**&#x200B;清單會顯示現有套件的狀態、來源環境及其部署位置。
1. 按一下&#x200B;**建立封裝**。

   >[!TIP]
   >
   >套件至少需要一個物件才能組裝和安裝。
1. 在&#x200B;**封裝詳細資料**&#x200B;索引標籤上，輸入封裝的&#x200B;**名稱**&#x200B;和&#x200B;**描述**。 來源環境已填入目前的（來源）環境。
1. 在左側的物件型別清單中，選取&#x200B;**規劃工作區**。
1. 搜尋您要提升的工作區，選取其核取方塊，然後按一下&#x200B;**新增Planning工作區**。 工作區會顯示在&#x200B;**封裝內容**&#x200B;下。

   已針對環境升級選取![Workspace](assets/workspace-selected-for-environment-promotion.png)
1. 按一下&#x200B;**儲存並組裝**。

   Workfront會組合套件並在套件的&#x200B;**更新**&#x200B;標籤上新增專案。 您可以檢閱封裝在「內容」標籤上的內容。
1. （條件式與選擇性）如果您要稍後完成，請按一下[儲存]並關閉&#x200B;**。**
1. （選擇性）按一下&#x200B;**內容**&#x200B;以檢閱封裝的內容，或按一下&#x200B;**部署**&#x200B;以檢視此封裝是否已部署多次。

   繼續讓封裝準備安裝。

### 讓封裝準備就緒，可供安裝

在目標環境中安裝套件之前，我們建議您先在測試環境中測試套件。

1. 依照上一節所述完成封裝建置後，按一下&#x200B;**封裝詳細資料**，然後按一下&#x200B;**編輯**，將&#x200B;**狀態**&#x200B;設定為&#x200B;**測試**，然後按一下&#x200B;**儲存並關閉**。

   >[!TIP]
   >
   >建置封裝後，其狀態會設為&#x200B;**草稿**。 必須先測試封裝，才能使用&#x200B;**作用中**&#x200B;狀態。
1. （建議使用）按一下[安裝]****，然後選擇其中一個可用的測試環境來部署它並測試組態。

   >[!TIP]
   >
   >當狀態設定為&#x200B;**測試**&#x200B;時，生產環境不能作為其中一個選項使用。

1. 在測試環境中安裝它之後，再按一下[編輯]，然後將&#x200B;**[狀態]**&#x200B;設定為&#x200B;**[使用中]**，再按一下[儲存]**，然後關閉**。****

   >[!TIP]
   >
   >在測試環境中安裝套件類似於在生產環境中安裝，如下節所述。

   請繼續下一節，以在您的目標環境中安裝套件。


### 在目標環境中安裝套件

1. 在封裝頁面上，驗證封裝後，按一下[安裝]。****
1. 在&#x200B;**目標環境**&#x200B;清單中，選取要部署到的環境（例如您的生產環境），然後按一下&#x200B;**繼續**。 預設目標是目前的環境。
1. 在&#x200B;**封裝資訊**&#x200B;頁面上，確認您要部署到的來源環境與環境。
1. 在&#x200B;**物件對應**&#x200B;區段中，展開每個物件群組（例如&#x200B;**群組**&#x200B;和&#x200B;**規劃工作區**）以檢閱物件。
1. 檢閱每個物件的&#x200B;**衝突**&#x200B;和&#x200B;**狀態**&#x200B;資料行，然後從清單中選擇&#x200B;**部署動作**。 從下列選項中選擇:

   * **建立新的**：將物件新增至目標。 當未偵測到衝突時，請使用此選項。
   * **使用existing**：將物件對應到目標中已存在的物件，例如具有相同名稱的群組。
   * **以新名稱建立**：以您指定的名稱新增物件。
   * **覆寫**：以封裝中的物件取代目標中的現有物件。
1. （選擇性）若要一次變更數個物件，請選取物件的核取方塊，在群組頂端的「建置」動作清單中選擇動作，然後按一下「套用至選取的專案」。 使用清單上方的篩選器（例如「僅顯示錯誤」）來聚焦於特定物件。
1. 解決任何錯誤指示器。 如果您選取&#x200B;**使用物件現有的**，您也必須選取物件對應到的物件。  否則，狀態會顯示錯誤，**部署**&#x200B;仍無法使用。
1. 按一下&#x200B;**部署**，然後按一下&#x200B;**部署**&#x200B;以確認。

   Workfront會顯示一個安裝頁面，訊息為&#x200B;**此封裝正在安裝**。 這可能需要幾分鐘的時間。

   安裝完成時，頁面會顯示成功訊息、安裝套件的環境，以及已安裝物件的清單，每個物件的狀態為，例如&#x200B;**Used existing**&#x200B;或&#x200B;**Installed （新建）**。
1. （選擇性）如果需要還原安裝並從目標環境中移除組態，請按一下&#x200B;**復原安裝**。

   繼續驗證安裝結果。

### 驗證結果

1. 前往目標環境> **主要功能表** > **計畫**，然後尋找匯入的工作區。
1. 開啟記錄型別和檢視以確認欄位和版面配置符合來源。 記錄不包含在內，因此表格是空的。


