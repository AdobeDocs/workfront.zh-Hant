---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 傳送 [!DNL Adobe Workfront] 專案更新至 [!DNL Anaplan] 清單項目
description: 此整合案例會分享進度、狀態和關鍵排程詳細資訊，來自 [!DNL Adobe Workfront] 包含 [!DNL Anaplan] 預算清單項。 共用此資訊可讓您更好地利用支出優化和財務分析， [!DNL Anaplan] 提供。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 2%

---

# 傳送 [!DNL Adobe Workfront] 專案更新至 [!DNL Anaplan] 清單項目

此整合案例會分享進度、狀態和關鍵排程詳細資訊，來自 [!DNL Adobe Workfront] 包含 [!DNL Anaplan] 預算清單項。 共用此資訊可讓您更好地利用支出優化和財務分析， [!DNL Anaplan] 提供。

>[!IMPORTANT]
>
>本文中的「促銷活動」是指此案例所代表的行銷活動使用案例，且與 [!DNL Workfront Fusion] Adobe Campaign連接器或最近淘汰的 [!UICONTROL 行銷活動] 物件 [!DNL Workfront].

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

&#42;&#42;如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 觸發事件

此情境排程每15分鐘執行一次。

## 預期 [!DNL Workfront] 設定

您必須在 [!DNL Workfront] 若要使用此案例：

* 中的使用者設定檔 [!DNL Workfront] 已命名 **[!UICONTROL [!DNL Anaplan]整合]**，具有系統管理員權限。

   如需在 [!DNL Workfront]，請參閱 [新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL 行銷活動簡報]** 附加到項目對象的自定義表單，以儲存您選擇發送到Anaplan的自定義資料值。

   下列欄位代表自訂表單中可能包含的欄位範例，以輔助將資料對應至Anaplan，但此整合案例並非必要欄位：

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>欄位名稱</th> 
     <th>欄位類型</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[！市場開始日期中的UICONTROL]</td> 
     <td>[!UICONTROL日期] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL在市場結束日期]</td> 
     <td>[!UICONTROL日期]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL促銷活動概述]</td> 
     <td>[!UICONTROL段落文本欄位]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL密鑰消息]</td> 
     <td>[!UICONTROL段落文本欄位]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL目標對象]</td> 
     <td> <p>[!UICONTROL下拉式清單]</p> <p>納入適合您流程的選項。</p> </td> 
    </tr> 
   </tbody> 
  </table>

   如需建立自訂表單的詳細資訊，請參閱 [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## 預期 [!DNL Anaplan] 設定

您必須在 [!DNL Anaplan] 若要使用此案例：

* 中的使用者設定檔 [!DNL Anaplan] 已命名 **[!UICONTROL [!DNL Workfront]整合]**，具有系統管理員權限。
* 此 [!DNL Anaplan] 要用於此案例的模型。
* 清單 [!DNL Anaplan] 要用於此案例的模型。
* A **[!UICONTROL 項目更新導入]** 檔案，依順序包含下列各欄：

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] 項目GUID]

3. [!UICONTROL 行銷活動名稱]

4. [!UICONTROL 完成百分比]

5. [!UICONTROL 計畫開始日期]

6. [!UICONTROL 計畫完成日期]

7. [!UICONTROL 計畫小時]

8. [!UICONTROL 計畫成本]

9. [!UICONTROL 計畫費用成本]

10. [!UICONTROL 實際勞力成本]

11. [!UICONTROL 計畫勞力成本]

12. [!UICONTROL 狀態]

準備 [!UICONTROL [!DNL Anaplan] 計畫費用導入] 檔案：

1. 將下列項目複製並貼到文字編輯器或 [!DNL Excel]
1. 將檔案儲存為CSV格式
1. 將檔案上傳至Anaplan。

   如需指示，請參閱 [!DNL Anaplan] 關於從檔案將資料匯入模組的檔案。

1. 記下您給檔案的名稱；將在部署 [!UICONTROL 融合] 方案範本。

範例CSV內容

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

1. [!UICONTROL 促銷活動概觀]

2. [!UICONTROL 關鍵訊息]

3. [!UICONTROL 市場開始日期]

4. [!UICONTROL 在市場結束日期]

5. [!UICONTROL 目標對象]

也包括您要在對應中設定的任何其他欄位。

* A **[!UICONTROL 項目更新導入]** 準備執行匯入檔案上傳中傳送之資料的程式。

如需這些動作的指示，請參閱 [!DNL Anaplan] 檔案。

## 部署至 [!DNL Workfront Fusion]

請完成下列步驟，將此整合案例部署至您的Fusion帳戶。 這必須在完成必要項目後才能完成 [!DNL Workfront] 和 [!DNL Anaplan] 設定。

1. 導覽至 [!UICONTROL 範本] 功能表 [!DNL Workfront Fusion] 並按一下 **[!UICONTROL 將Workfront專案更新傳送至 [!DNL Anaplan] 清單項目]** 方案範本。
1. 取代下列變數值 [!DNL Anaplan] 變數：

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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 工作區ID]</td> 
      <td>來自您 [!DNL Anaplan] 帳戶。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 模型ID] </td> 
      <td>來自您 [!DNL Anaplan] 帳戶和所選工作區。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL促銷活動清單名稱]</td> 
      <td>清單的名稱 [!DNL Anaplan] 帳戶和選取的工作區與模型。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL檔案名：項目更新導入]</td> 
      <td>將接收項目更新資料的檔案的名稱。<p>(範例：WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL進程名稱：項目更新導入]</td> 
      <td> <p>執行項目資料導入的進程的名稱。</p> <p>(範例：WF整合 — 更新促銷活動詳細資訊)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] 子網域]</td> 
      <td>您的 [!DNL Workfront] 帳戶。 這可用來建立回您 [!DNL Workfront] 項目（在可能生成的注釋中）。</td> 
     </tr> 
    </tbody> 
   </table>

   有關如何設定檔案和程式的詳細資訊，請參閱 [!DNL Anaplan] 設定檔案。

1. 選取或新增 [!DNL Anaplan] 連線設定檔。
1. 更新所有剩餘 [!DNL Anaplan] 具有 [!DNL Anaplan] 連線時顯示。
1. 選取或新增 [!DNL Workfront] 連線設定檔。

   篩選器設定為提取所有不完整的連結專案以及過去29分鐘內完成的專案。 如果您變更 [!DNL Fusion] 方案部署方案範本後，您將要更新此值。

1. 在 **[!UICONTROL 建立專案更新CSV]** 模組，新增資料結構以將專案屬性對應至CSV欄。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 更新所有剩餘 [!DNL Workfront] 模組 [!DNL Workfront] 連線時顯示。

## 其他建議的方案範本

此方案模板由下列也可部署的支出優化方案模板所補充：

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 實際更新小時數 [!DNL Anaplan] 清單項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 費用 [!DNL Anaplan] 清單項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

連結預算請求的其他方案：

* [[!UICONTROL 建立 [!DNL Anaplan] 清單項 [!DNL Adobe Workfront] 預算請求]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 套用 [!DNL Anaplan] 預算分配至 [!DNL Adobe Workfront] 專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

連結促銷活動請求的其他案例：

* [[!UICONTROL 建立 [!DNL Anaplan] 清單項 [!DNL Adobe Workfront] 行銷活動請求]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 套用 [!DNL Anaplan] 預算分配至 [!DNL Adobe Workfront] 行銷活動要求或行銷活動專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
