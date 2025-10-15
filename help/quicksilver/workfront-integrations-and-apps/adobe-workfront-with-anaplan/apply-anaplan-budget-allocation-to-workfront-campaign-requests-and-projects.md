---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 將 [!DNL Anaplan] 預算分配套用至 [!DNL Adobe Workfront] 行銷活動請求或行銷活動專案
description: 此整合案例會同步任何已在 [!DNL Anaplan] 回到 [!DNL Workfront]中進行的預算分配。 此案例會提取所有連結的行銷活動預算專案，然後在預算值已變更時，將預算值傳遞至連結的Workfront專案。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: d3f234313677d916318c181c91cb951948454006
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---

# 將[!DNL Anaplan]預算分配套用至[!DNL Adobe Workfront]行銷活動請求或行銷活動專案

此整合情境會將已在[!DNL Anaplan]中進行的所有預算分配同步回[!DNL Workfront]。 案例會提取所有連結的行銷活動預算專案，然後在預算值已變更時，將預算值傳給連結的[!DNL Workfront]專案。

>[!IMPORTANT]
>
>本文中的「行銷活動」是指此情境所代表的行銷活動使用案例，且絕對未連線至[!DNL Workfront Fusion] Adobe Campaign聯結器或[!UICONTROL 中最近棄用的]行銷活動[!DNL Workfront]物件。


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何Adobe Workfront Workflow套件和任何Adobe Workfront自動化與整合套件</p><p>Workfront Ultimate</p><p>Workfront Prime和Select套件，以及額外購買的Workfront Fusion。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p><p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion授權</td> 
   <td>
   <p>作業型：無Workfront Fusion授權需求</p>
   <p>以聯結器為基礎（舊版）：用於工作自動化和整合的Workfront Fusion </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>如果您的組織有Select或Prime Workfront套件，但不包含Workfront Automation和Integration，則您的組織必須購買Adobe Workfront Fusion。</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

如需此表格中資訊的詳細資訊，請參閱檔案[中的](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)存取需求。

如需Adobe Workfront Fusion授權的相關資訊，請參閱[Adobe Workfront Fusion授權](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration)。

## 觸發中的事件

此情境已排程為每15分鐘執行一次。

## 預期的[!DNL Workfront]組態

若要使用此情境，您在[!DNL Workfront]中必須擁有下列專案：

* [!DNL Workfront]中名為&#x200B;**[!DNL Anaplan Integration]**&#x200B;且擁有系統管理員許可權的使用者設定檔。

  如需在[!DNL Workfront]中建立使用者的詳細資訊，請參閱[新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

## 預期的[!DNL Anaplan]組態

若要使用此情境，您在[!DNL Anaplan]中必須擁有下列專案：

* [!DNL Anaplan]中名為&#x200B;**[!UICONTROL [!DNL Workfront]整合]**&#x200B;的使用者設定檔，具有系統管理員許可權。
* 您要用於此情境的[!DNL Anaplan]模型。
* [!DNL Anaplan]模型中擷取促銷活動預算的清單。

  清單的模組必須支援接收下列屬性：

   * [!UICONTROL [!DNL Workfront]要求GUID]
   * [!UICONTROL [!DNL Workfront]專案GUID]
   * [!UICONTROL 行銷活動名稱]
   * [!UICONTROL 已要求人力資金]
   * [!UICONTROL 預估收入]
   * [!UICONTROL 品牌]

  此清單和模組必須儲存[!DNL Anaplan]正常功能所需的額外詳細資料，包括設定預算並傳達預算清單專案已準備好同步回[!DNL Workfront]的能力。

* [!DNL Anaplan]中名為&#x200B;**[!UICONTROL Campaigns.Update Campaigns in Adobe Workfront]**&#x200B;的檢視。

  此檢視必須包含下列欄，依此順序排列：

   1. [!UICONTROL 專案名稱]

   2. [!UICONTROL [!DNL Workfront]要求GUID]

   3. [!UICONTROL [!DNL Workfront]專案GUID]

   4. [!UICONTROL 行銷活動名稱]

   5. [!UICONTROL 預算]

   6. [!UICONTROL 預估收入]

   7. [!UICONTROL 品牌]

  應篩選檢視以顯示具有[!UICONTROL [!DNL Workfront]專案GUID]的專案以及預算配置應傳輸至Workfront的某些指標。

如需上述任何動作的指示，請參閱[!DNL Anaplan]檔案。

## 部署至Workfront Fusion

完成下列步驟，將此整合案例部署至您的Fusion帳戶。 這應該只有在完成必要的[!DNL Workfront]和[!DNL Anaplan]設定之後才完成。

1. 導覽至[!UICONTROL 中的]範本[!DNL Workfront Fusion]功能表，然後按一下&#x200B;**[!UICONTROL 將[!DNL Anaplan]預算分配套用至Workfront行銷活動要求和專案]**&#x200B;情境範本。
1. 取代下列[!DNL Anaplan]個變數的變數值：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>變數名稱</th> 
      <th>將值取代為</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>您[!DNL Anaplan]帳戶的工作區識別碼。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan]模型識別碼] </td> 
      <td>來自您[!DNL Anaplan]帳戶和所選工作區的模型ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 促銷活動清單名稱]</td> 
      <td>來自您[!DNL Anaplan]帳戶及所選工作區與模型的清單名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan]檢視名稱</td> 
      <td> <p>檢視的名稱，其中包含可傳送給[!DNL Workfront]的行銷活動預算。</p> <p>（範例： [!UICONTROL Campaigns.Load Campaigns.To [!DNL Adobe Workfront]]） </p> </td> 
     </tr> 
    </tbody> 
   </table>

   有關如何設定檔案與程式的詳細資訊，請參閱[!DNL Anaplan]設定檔案。

1. 選取或新增[!DNL Anaplan]連線設定檔。
1. 出現提示時，以[!DNL Anaplan]連線更新所有剩餘的[!DNL Anaplan]模組。
1. 在&#x200B;**[!UICONTROL 將CSV轉換為JSON物件]**&#x200B;模組上，新增新的資料結構以將CSV欄對應到可用的JSON物件。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Request GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. 出現提示時，請為此情境部署中的其他模組選取此資料結構。
1. 在&#x200B;**[!UICONTROL 檢查連結的專案]**&#x200B;模組上，選取或新增[!DNL Workfront]連線設定檔。
1. 出現提示時，以[!DNL Workfront]連線更新所有剩餘的[!DNL Workfront]模組。

## 其他建議的情境範本

若要完成此範本所代表的工作流程，您也必須部署下列其他範本：

* [[!UICONTROL 從 [!DNL Anaplan] 行銷活動要求 [!DNL Adobe Workfront] 建立]清單專案](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

支出最佳化的其他案例包括：

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 專案更新至 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 實際時數更新至 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 費用給 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
