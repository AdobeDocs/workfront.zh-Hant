---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 將請求佇列內嵌在控制面板中
description: 您可以將新請求佇列內嵌在控制面板中，以便讓使用者直接存取請求佇列，而無須前往「請求」區域。
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# 將請求佇列內嵌在控制面板中

您可以將新請求佇列內嵌在控制面板中，以便讓使用者直接存取請求佇列，而無須前往「請求」區域。 

例如，如果您有一個請求隊列，該請求隊列對整個組織開放，例如「服務台隊列」或每個人都必須定期訪問的PTO請求隊列，則將請求隊列直接插入到其中一個控制面板中以方便快速、方便地訪問。 此設定的程式與在控制面板上建立外部頁面的程式類似。

首先，您必須取得要求佇列的URL。 其次，您可以新增外部頁面，將URL內嵌至控制面板。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>管理控制面板的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須先建立下列兩項，才能將請求佇列內嵌在控制面板中：

* **控制面板**:如需建立控制面板的詳細資訊，請參閱 [建立控制面板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).
* **請求佇列**:有關建立請求隊列的資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## 取得請求佇列的URL {#obtain-the-url-of-the-request-queue}

您可以透過多種方式取得請求佇列的URL，端視從控制面板存取請求佇列時，要公開給使用者的請求佇列的哪一部分而定。

* [取得特定佇列主題的連結，並可變更請求類型](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)
* [取得請求佇列的連結，以及變更請求類型的功能](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)
* [取得請求佇列的連結，但無法變更請求類型](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### 取得特定佇列主題的連結，並可變更請求類型 {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

當您與其他使用者共用特定佇列主題的連結時，請求表單會在他們提交請求所需的確切佇列主題中開啟。 當使用者無法確定記錄特定請求佇列的請求時，要選擇哪個佇列主題時，這個方法會很實用。

使用者可以變更請求類型，或視需要選擇其他主題。 「請求」區域的導覽也會顯示。

1. 按一下 **主菜單** > **請求** > **新請求**.
1. 如果要共用特定隊列，請繼續選擇主題組和隊列主題，直到到達要在控制面板上共用的隊列。 如需提交請求的相關資訊，請參閱 [建立及提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >選擇主題組和隊列主題是可選的。

1. 按一下 **共用路徑** 在「新請求」區域的右上角。

   如此會在畫面上顯示請求佇列或佇列主題時複製該連結。 使用者可以更新「請求類型」或任何可用的主題群組和佇列主題。

   ![](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### 取得請求佇列的連結，以及變更請求類型的功能 {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

當您共用請求類型的連結時，系統會為使用者選取請求類型。 當使用者需要針對相同請求類型從多個主題群組或佇列主題中選擇時，此功能會很實用。 使用者可以變更請求類型並選擇其他請求類型。 「請求」區域的導覽也會顯示。

1. 移至指定為請求佇列的專案。

   如需從專案建立請求佇列的相關資訊，請前往 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 前往 **隊列詳細資訊**.
1. 複製您在 **直接存取URL** 欄位。

   程式碼看起來應類似下列：

   ```
   <samp>https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=</samp>
   ```

   這是與所選項目關聯的請求隊列的連結。預先選擇「請求類型」。

   使用者可以選擇任何主題群組或佇列主題，也可以選擇其他請求類型。

   ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### 取得請求佇列的連結，但無法變更請求類型 {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

當您共用預先選取之請求類型的連結時，系統會為使用者選取請求類型，且無法變更（此類型會呈現灰色）。 使用者可以選擇主題群組或將主題排入佇列。 如果您不希望使用者檢視並選取其他請求類型，這個方法會很實用。 「請求」區域的導覽不會顯示。

1. 移至指定為請求佇列的專案。

   如需從專案建立請求佇列的相關資訊，請前往 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 前往 **隊列詳細資訊**.
1. 複製您在 **內嵌程式碼** 欄位。

   程式碼看起來應類似下列：

   ```
   <samp><iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe></samp>
   ```

1. 編輯程式碼，僅保留下列資訊：

   ```
   <samp>https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71</samp>
   ```

   >[!TIP]
   >
   >您可以保留 `<samp>iframe </samp>` 標籤。

   這是與所選專案相關聯的請求佇列連結。 「請求類型」已預先選取，因此無法變更。

   使用者可以選擇所選請求類型所需的任何主題群組或佇列主題。 使用者無法選取其他請求類型。

   ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## 將請求佇列內嵌在控制面板中

您可以將連結內嵌至請求佇列或請求佇列下巢狀的佇列主題，以讓使用者直接存取進入請求。

1. 使用 [取得請求佇列的URL](#obtain-the-url-of-the-request-queue) 本文的一節。
1. 按一下 **主菜單** > **控制面板** > **新控制面板**.
1. 輸入 **名稱** ，以取得Advertising Cloud的說明。 這是必填欄位。
1. 按一下 **新增外部頁面**.

   ![](assets/add-external-page-highlighted---nwe-350x214.png)

1. 在 **新增外部頁面** 框中，編輯以下欄位：

   * **名稱**:輸入您要請求佇列顯示在控制面板上的名稱。 這是必填欄位。

   * **說明**:輸入有關此外部頁面顯示的說明。 這不是必填欄位，此欄位僅用於報表用途。 它不會顯示在控制面板中。
   * **URL**:貼上您使用步驟1所述的其中一種方法取得的URL。

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <MadCap:conditionalText data-mc-conditions="">   
     (NOTE: ensure this stays accurate)   
     </MadCap:conditionalText>   
     </MadCap:conditionalText>   
     -->

   * **高度**:輸入外部頁面的高度。 這會定義包含請求佇列的外部頁面在控制面板上所佔的空間。 這是必填欄位，預設值為500。

1. 按一下&#x200B;**儲存**。
1. 按一下 **儲存+關閉**. 

   請求佇列會以個別控制面板元件的形式顯示在控制面板中。

   ![](assets/new-dashboard-with-embedded-request-queue-nwe-350x260.png)

1. （選用）按一下 **控制面板動作**，然後 **編輯** 將報表、日曆或其他外部頁面新增至相同的控制面板。\
   如需將元件新增至控制面板的相關資訊，請參閱 [建立控制面板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

 

 

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - old information)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> > Requests >&nbsp;<strong>New Request</strong>. </p> </li>
<li class="preview" value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Continue entering the request.&nbsp;For information about submitting requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>. </p> </li>
<li value="3"> <p>Select the <strong>Request Type</strong> for the queue you would like added to the dashboard.</p> </li>
<li value="4"> <p>(Optional) Select a Queue Topic and a Topic Group. Depending on how the project manager set up the request queue, the names of these fields are different in each Workfront instance.</p> </li>
<li class="preview" value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <strong>Share path</strong> to obtain a shared link from the request queue you want to embed on a dashboard.</p> <p>For information about sharing a request queue, see <a href="../../../manage-work/requests/create-requests/share-link-to-request-queue.md" class="MCXref xref">Share a link to a request queue</a></p> </li>
<li value="6"> <p>For example, enter a URL similar to one of the following: </p> </li>
</ol>
-->
