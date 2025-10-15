---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 將 [!DNL Adobe Workfront] 實際時數更新傳送至 [!DNL Anaplan] 清單專案
description: 此整合情境會共用在具有 [!DNL Adobe Workfront] 預算清單專案的 [!DNL Anaplan] 專案上擷取的實際時數詳細資料。 共用此資訊可讓您更好地利用 [!DNL Anaplan] 提供的支出最佳化與財務分析。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: d3f234313677d916318c181c91cb951948454006
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 0%

---

# 將[!DNL Adobe Workfront]實際時數更新傳送至[!DNL Anaplan]清單專案

此整合情境會共用在具有[!DNL Adobe Workfront]預算清單專案的[!DNL Anaplan]專案上擷取的實際時數詳細資料。 共用此資訊可讓您更好地利用[!DNL Anaplan]提供的支出最佳化和財務分析。

此情境範本提供過去3個月在作用中專案上依專案、日期和角色所記錄的時數清單。

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

如需Adobe Workfront Fusion授權的相關資訊，請參閱[Adobe Workfront Fusion授權](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration)。

## 觸發中的事件

此情境已排程為每15分鐘執行一次。

## 預期的[!DNL Workfront]組態

若要使用此情境，您在[!DNL Workfront]中必須擁有下列專案：

* [!DNL Workfront]中名為&#x200B;**[!UICONTROL Anaplan整合]**&#x200B;且擁有系統管理員許可權的使用者設定檔。

  如需在[!DNL Workfront]中建立使用者的詳細資訊，請參閱[新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

## 預期的[!DNL Anaplan]組態

若要使用此情境，您在[!DNL Anaplan]中必須擁有下列專案：

* [!DNL Anaplan]中名為&#x200B;**[!UICONTROL [!DNL Workfront]整合]**&#x200B;的使用者設定檔，具有系統管理員許可權。
* 您要用於此情境的[!DNL Anaplan]模型。
* 您要用於此情境的[!DNL Anaplan]模型內的清單。
* [!DNL Anaplan]中名為&#x200B;**[!UICONTROL Anaplan實際時數匯入]**&#x200B;的檔案，包含下列資料行，依此順序：

   1. [!UICONTROL Workfront專案GUID]

   2. [!UICONTROL 小時]

   3. [!UICONTROL 小時估計成本]

   4. [!UICONTROL 輸入日期]

   5. [!UICONTROL 角色名稱]

   6. [!UICONTROL 行銷活動名稱]

   7. [!UICONTROL [!DNL Anaplan]清單專案識別碼]

  若要準備[!DNL Anaplan]實際費用報表檔案：

   1. 將下列內容複製並貼到文字編輯器或[!DNL Excel]
   1. 以CSV格式儲存檔案
   1. 將檔案上傳至[!DNL Anaplan]。

      如需指示，請參閱[!DNL Anaplan]檔案，瞭解如何從檔案將資料匯入模組。

   1. 請記下您為檔案指定的名稱；此名稱將會在[!UICONTROL Fusion]情境範本的部署期間使用。

  範例CSV內容

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* 準備執行&#x200B;**[!UICONTROL 專案實際時數匯入]**&#x200B;程式，以執行匯入檔案上傳中傳送的資料。

如需上述任何動作的指示，請參閱[!DNL Anaplan]檔案。

## 部署至[!DNL Workfront Fusion]

完成下列步驟，將此整合情境部署至您的[!DNL Fusion]帳戶。 這應該只有在完成必要的[!DNL Workfront]和[!DNL Anaplan]設定之後才完成。

1. 導覽至[!UICONTROL 中的]範本[!DNL Workfront Fusion]功能表，然後按一下&#x200B;**[!UICONTROL 將Workfront實際時數更新傳送至[!DNL Anaplan]清單專案]**&#x200B;情境範本。
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
      <td role="rowheader">[！UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>您[!DNL Anaplan]帳戶的工作區識別碼。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL [!DNL Anaplan]模型識別碼] </td> 
      <td>來自您[!DNL Anaplan]帳戶和所選工作區的模型ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL促銷活動清單名稱]</td> 
      <td>來自您[!DNL Anaplan]帳戶及所選工作區與模型的清單名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL檔案名稱：實際時數匯入]</td> 
      <td> <p>將接收專案實際時數資料的檔案名稱。</p> <p> （範例：WorkfrontUpdateLinkedProjects_HoursRoles.csv） </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL流程名稱：實際時數匯入]</td> 
      <td> <p>將執行專案時數資料匯入的流程名稱。</p> <p>（範例： WF Int — 依角色載入專案時數）</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL [!DNL Workfront]子網域]</td> 
      <td>您[!DNL Workfront]帳戶的子網域。 這可用來在可能產生的附註中建立回到[!DNL Workfront]專案的連結。</td> 
     </tr> 
    </tbody> 
   </table>

   有關如何設定檔案與程式的詳細資訊，請參閱[!DNL Anaplan]設定檔案。

1. 選取或新增[!DNL Anaplan]連線設定檔。
1. 出現提示時，以[!DNL Anaplan]連線更新所有剩餘的[!DNL Anaplan]模組。
1. 選取或新增[!DNL Workfront]連線設定檔。
1. 出現提示時，以[!DNL Workfront]連線更新所有剩餘的[!DNL Workfront]模組。

## 其他建議的情境範本

此情境範本由以下支出最佳化情境範本補充，這些範本也可部署：

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 專案更新至 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 費用給 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

連結預算請求的其他案例：

* [[!UICONTROL 從 [!DNL Anaplan] 預算請求 [!DNL Adobe Workfront] 建立]清單專案](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 套用 [!DNL Anaplan] 預算配置至 [!DNL Adobe Workfront] 專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

連結行銷活動請求的其他情況：

* [[!UICONTROL 從 [!DNL Anaplan] 行銷活動要求 [!DNL Adobe Workfront] 建立]清單專案](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 將 [!DNL Anaplan] 預算配置套用至 [!DNL Adobe Workfront] 行銷活動請求或行銷活動專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
