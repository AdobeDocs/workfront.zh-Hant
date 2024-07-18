---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 將 [!DNL Adobe Workfront] 專案更新傳送至 [!DNL Anaplan] 清單專案
description: 此整合情境會共用具有 [!DNL Anaplan] 預算清單專案之 [!DNL Adobe Workfront] 專案的進度、狀態和主要排程詳細資料。 共用此資訊可讓您更好地利用 [!DNL Anaplan] 提供的支出最佳化與財務分析。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 0%

---

# 傳送[!DNL Adobe Workfront]個專案更新至[!DNL Anaplan]清單專案

此整合情境會共用來自具有[!DNL Anaplan]預算清單專案的[!DNL Adobe Workfront]專案的進度、狀態和主要排程詳細資料。 共用此資訊可讓您更好地利用[!DNL Anaplan]提供的支出最佳化和財務分析。

>[!IMPORTANT]
>
>本文中的「行銷活動」是指此情境所代表的行銷活動使用案例，且絕對未連線至[!DNL Workfront Fusion] Adobe Campaign聯結器或[!DNL Workfront]中最近棄用的[!UICONTROL 行銷活動]物件。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td> <p>適用於工作自動化和整合的Workfront Fusion </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您的組織必須購買[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

&#42;&#42;如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 觸發中的事件

此情境已排程為每15分鐘執行一次。

## 預期的[!DNL Workfront]組態

若要使用此情境，您在[!DNL Workfront]中必須擁有下列專案：

* [!DNL Workfront]中名為&#x200B;**[!UICONTROL [!DNL Anaplan]整合]**&#x200B;的使用者設定檔，具有系統管理員許可權。

  如需在[!DNL Workfront]中建立使用者的詳細資訊，請參閱[新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

* **[!UICONTROL 行銷活動簡報]**&#x200B;自訂表單已附加至專案物件，以儲存您選擇傳送至Anaplan的自訂資料值。

  以下欄位代表自訂表單中可包含的欄位範例，有助於將資料對應至Anaplan，但此整合案例不需要這些欄位：

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
     <td>[！UICONTROL日期] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL市場結束日期]</td> 
     <td>[！UICONTROL日期]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL行銷活動概覽]</td> 
     <td>[！UICONTROL段落文字欄位]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL金鑰訊息]</td> 
     <td>[！UICONTROL段落文字欄位]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL目標對象]</td> 
     <td> <p>[！UICONTROL下拉式清單]</p> <p>包含適合您流程的選項。</p> </td> 
    </tr> 
   </tbody> 
  </table>

  如需建立自訂表單的相關資訊，請參閱[建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## 預期的[!DNL Anaplan]組態

若要使用此情境，您在[!DNL Anaplan]中必須擁有下列專案：

* [!DNL Anaplan]中名為&#x200B;**[!UICONTROL [!DNL Workfront]整合]**&#x200B;的使用者設定檔，具有系統管理員許可權。
* 您要用於此情境的[!DNL Anaplan]模型。
* 您要用於此情境的[!DNL Anaplan]模型內的清單。
* 包含下列資料行的&#x200B;**[!UICONTROL 專案更新匯入]**&#x200B;檔案（依此順序）：

1. [!UICONTROL 專案識別碼]

2. [!UICONTROL [!DNL Workfront]專案GUID]

3. [!UICONTROL 行銷活動名稱]

4. [!UICONTROL 完成百分比]

5. [!UICONTROL 計劃開始日期]

6. [!UICONTROL 計畫完成日期]

7. [!UICONTROL 規劃時數]

8. [!UICONTROL 規劃成本]

9. [!UICONTROL 計畫費用成本]

10. [!UICONTROL 實際勞力成本]

11. [!UICONTROL 計畫勞力成本]

12. [!UICONTROL 狀態]

若要準備[!UICONTROL [!DNL Anaplan]計畫費用匯入]檔案：

1. 將下列內容複製並貼到文字編輯器或[!DNL Excel]
1. 以CSV格式儲存檔案
1. 將檔案上傳至Anaplan。

   如需指示，請參閱[!DNL Anaplan]檔案，瞭解如何從檔案將資料匯入模組。

1. 請記下您為檔案指定的名稱；此名稱將會在[!UICONTROL Fusion]情境範本的部署期間使用。

範例CSV內容

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>可選欄可能包括：

1. [!UICONTROL 行銷活動概覽]

2. [!UICONTROL 金鑰訊息]

3. [!UICONTROL 上市開始日期]

4. [!UICONTROL 市場結束日期]

5. [!UICONTROL 目標對象]

也包含您要在對應中設定的任何其他欄位。

* **[!UICONTROL 專案更新匯入]**&#x200B;程式已準備執行匯入檔案上傳中傳遞的資料。

如需上述任何動作的指示，請參閱[!DNL Anaplan]檔案。

## 部署至[!DNL Workfront Fusion]

完成下列步驟，將此整合案例部署至您的Fusion帳戶。 這應該只有在完成必要的[!DNL Workfront]和[!DNL Anaplan]設定之後才完成。

1. 導覽至[!DNL Workfront Fusion]中的[!UICONTROL 範本]功能表，然後按一下&#x200B;**[!UICONTROL 將Workfront專案更新傳送至[!DNL Anaplan]清單專案]**&#x200B;情境範本。
1. 取代下列[!DNL Anaplan]個變數的變數值：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
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
      <td role="rowheader">[！UICONTROL檔案名稱：專案更新匯入]</td> 
      <td>將接收專案更新資料的檔案名稱。<p>（範例：WorkfrontUpdateLinkedProject.csv）</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL流程名稱：專案更新匯入]</td> 
      <td> <p>將執行專案資料匯入的程式名稱。</p> <p>（範例： WF Int — 更新促銷活動詳細資料）</p> </td> 
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

   此篩選器已設定為提取所有未完成的連結專案，以及過去29分鐘內完成的專案。 如果您變更[!DNL Fusion]案例的頻率，則會在部署案例範本後更新此值。

1. 在&#x200B;**[!UICONTROL 建置專案更新CSV]**&#x200B;模組上，新增新的資料結構以將專案屬性對應到CSV欄。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. 出現提示時，以[!DNL Workfront]連線更新所有剩餘的[!DNL Workfront]模組。

## 其他建議的情境範本

此情境範本由以下支出最佳化情境範本補充，這些範本也可部署：

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 實際時數更新至 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 費用給 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

連結預算請求的其他案例：

* [[!UICONTROL 從 [!DNL Adobe Workfront] 預算請求]建立 [!DNL Anaplan] 清單專案](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 套用 [!DNL Anaplan] 預算配置至 [!DNL Adobe Workfront] 專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

連結行銷活動請求的其他情況：

* [[!UICONTROL 從 [!DNL Adobe Workfront] 行銷活動要求]建立 [!DNL Anaplan] 清單專案](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 將 [!DNL Anaplan] 預算配置套用至 [!DNL Adobe Workfront] 行銷活動請求或行銷活動專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
