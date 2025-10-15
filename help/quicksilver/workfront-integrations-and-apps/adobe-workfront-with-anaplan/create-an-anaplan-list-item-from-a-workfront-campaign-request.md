---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 從 [!DNL Anaplan] 行銷活動請求建立 [!DNL Adobe Workfront] 清單專案
description: 此整合案例連結具有 [!DNL Adobe Workfront] 預算清單專案的 [!DNL Anaplan] 專案。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: d3f234313677d916318c181c91cb951948454006
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 2%

---

# 從[!DNL Anaplan]行銷活動請求建立[!DNL Adobe Workfront]清單專案

此整合案例連結具有[!DNL Adobe Workfront]預算清單專案的[!DNL Anaplan]專案。

此情境會監視新增到請求佇列的新行銷活動請求。 行銷活動要求一經記錄，預算明細專案就會新增到[!DNL Anaplan]中，以開始融資程式。

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

* [!DNL Workfront]中名為&#x200B;**[!UICONTROL [!DNL Anaplan]整合]**&#x200B;的使用者設定檔，具有系統管理員許可權。

  如需在[!DNL Workfront]中建立使用者的詳細資訊，請參閱[新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

* **[!UICONTROL 行銷活動簡報]**&#x200B;自訂表單已附加至[!UICONTROL 要求]物件。

  自訂表單上必須包括下列必填欄位，以輔助將資料對應到Anaplan：

  | 欄位名稱 | 欄位型別 |
  |---|---|
  | [!UICONTROL 要求資金總計] |   |
  | [!UICONTROL 已要求人力資金] |   |
  | [!UICONTROL 已要求費用資金] |   |
  | [!UICONTROL 傳送至[!DNL Anaplan]] | 核取方塊 |

  表單上可能會出現下列選用欄位。 此案例僅對應上述欄位，但行銷活動簡介上的任何其他欄位可能會對應。

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>欄位名稱</th> 
     <th>欄位型別</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[！UICONTROL上市日期]</td> 
     <td>日期 </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL市場結束日期]</td> 
     <td>日期</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL行銷活動概覽]</td> 
     <td>段落文字欄位</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL金鑰訊息]</td> 
     <td>段落文字欄位</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL目標對象]</td> 
     <td> <p>下拉</p> <p>包含適合您流程的選項。</p> </td> 
    </tr> 
   </tbody> 
  </table>

  如需建立自訂表單的相關資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

* 設定為要求佇列的專案，用來擷取新的行銷活動要求。 [!UICONTROL 行銷活動簡報]表單必須附加至這些要求。

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
   * [!UICONTROL 已要求費用資金]
   * [!UICONTROL 預算要求型別]

  此清單和模組必須儲存[!DNL Anaplan]正常功能所需的額外詳細資料，包括設定預算並傳達預算清單專案已準備好同步回[!DNL Workfront]的能力。

如需上述任何動作的指示，請參閱[!DNL Anaplan]檔案。

## 部署至[!DNL Workfront Fusion]

完成下列步驟，將此整合情境部署至您的[!DNL Fusion]帳戶。 這應該只有在完成必要的[!DNL Workfront]和[!DNL Anaplan]設定之後才完成。

1. 導覽至[!UICONTROL 中的]範本[!DNL Workfront Fusion]功能表，然後按一下&#x200B;**[!UICONTROL 從Workfront行銷活動請求[!DNL Anaplan]情境範本建立]**&#x200B;清單專案。
1. 取代下列[!DNL Anaplan]個變數的變數值：

   | 變數名稱 | 將值取代為 |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | 您[!DNL Anaplan]帳戶的工作區識別碼。 |
   | [!UICONTROL [!DNL Anaplan]模型識別碼] | 來自您[!DNL Anaplan]帳戶和所選工作區的模型ID。 |
   | [!UICONTROL [!DNL Anaplan]模組名稱] | 描述所選[!DNL Anaplan]清單中促銷活動屬性的模組名稱。 |
   | [!UICONTROL 行銷活動清單名稱] | 來自您[!DNL Anaplan]帳戶及所選工作區與模型的清單名稱。 |

   {style="table-layout:auto"}

   有關如何設定檔案與程式的詳細資訊，請參閱[!DNL Anaplan]設定檔案。

1. 選取或新增[!DNL Anaplan]連線設定檔。
1. 出現提示時，以[!DNL Anaplan]連線更新所有剩餘的[!DNL Anaplan]模組。
1. 選取或新增[!DNL Workfront]連線設定檔。

   部署範本後，如果您想要將預設對應欄位變更為[!DNL Anaplan]，此模組將會更新，以新增或移除欄位屬性值中的自訂欄位參考。

1. 出現提示時，以[!DNL Workfront]連線更新所有剩餘的[!DNL Workfront]模組。

## 其他建議的情境範本

若要完成此範本所代表的工作流程，您也必須部署下列其他範本：

* [[!UICONTROL 將 [!DNL Anaplan] 預算配置套用至 [!DNL Adobe Workfront] 行銷活動請求或行銷活動專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

支出最佳化的其他案例包括：

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 專案更新至 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 實際時數更新至 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 費用給 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
