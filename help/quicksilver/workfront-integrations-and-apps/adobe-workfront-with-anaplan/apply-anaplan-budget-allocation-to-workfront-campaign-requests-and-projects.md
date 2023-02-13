---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 套用 [!DNL Anaplan] 預算分配至 [!DNL Adobe Workfront] 行銷活動要求或行銷活動專案
description: 此整合方案會同步在 [!DNL Anaplan] 返回 [!DNL Workfront]. 情境會提取所有連結的促銷活動預算項目，然後如果預算值已變更，則將預算值傳遞至連結的Workfront專案。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 套用 [!DNL Anaplan] 預算分配至 [!DNL Adobe Workfront] 行銷活動要求或行銷活動專案

此整合方案會同步在 [!DNL Anaplan] 返回 [!DNL Workfront]. 方案會提取所有連結的促銷活動預算項目，然後將預算值傳遞至連結的 [!DNL Workfront] 項目。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
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

* 中的使用者設定檔 [!DNL Workfront] 已命名 **[!DNL Anaplan Integration]**，具有系統管理員權限。

   如需在 [!DNL Workfront]，請參閱 [新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 預期 [!DNL Anaplan] 設定

您必須在 [!DNL Anaplan] 若要使用此案例：

* 中的使用者設定檔 [!DNL Anaplan] 已命名 **[!UICONTROL [!DNL Workfront]整合]**，具有系統管理員權限。
* 此 [!DNL Anaplan] 要用於此案例的模型。
* 清單 [!DNL Anaplan] 擷取促銷活動預算的模型。

   清單的模組必須支援接收以下屬性：

   * [!UICONTROL [!DNL Workfront] 請求GUID]
   * [!UICONTROL [!DNL Workfront] 項目GUID]
   * [!UICONTROL 行銷活動名稱]
   * [!UICONTROL 所申請的勞動資金]
   * [!UICONTROL 估計收入]
   * [!UICONTROL 品牌]

   此清單和模組必須儲存正常功能所需的其他詳細資訊 [!DNL Anaplan]，包括設定預算並傳達預算清單項目已準備好同步回的功能 [!DNL Workfront].

* 檢視 [!DNL Anaplan] 呼叫 **[!UICONTROL Campaigns.更新Adobe Workfront中的促銷活動]**.

   此檢視必須依此順序包含下列欄：

   1. [!UICONTROL 項目名稱]

   2. [!UICONTROL [!DNL Workfront] 請求GUID]

   3. [!UICONTROL [!DNL Workfront] 項目GUID]

   4. [!UICONTROL 行銷活動名稱]

   5. [!UICONTROL 預算]

   6. [!UICONTROL 估計收入]

   7. [!UICONTROL 品牌]
   應篩選檢視，以顯示具有 [!UICONTROL [!DNL Workfront] 項目GUID] 還有一些指標表明，應將預算撥款轉給Workfront。

如需這些動作的指示，請參閱 [!DNL Anaplan] 檔案。

## 部署至Workfront Fusion

請完成下列步驟，將此整合案例部署至您的Fusion帳戶。 這必須在完成必要項目後才能完成 [!DNL Workfront] 和 [!DNL Anaplan] 設定。

1. 導覽至 [!UICONTROL 範本] 功能表 [!DNL Workfront Fusion] 並按一下 **[!UICONTROL 套用 [!DNL Anaplan] 預算分配給Workfront促銷活動請求和專案]** 方案範本。
1. 取代下列變數值 [!DNL Anaplan] 變數：

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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 查看名稱]</td> 
      <td> <p>包含要傳送至之促銷活動預算的檢視名稱 [!DNL Workfront].</p> <p>(範例：[!UICONTROL Campaigns.Load促銷活動至 [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   有關如何設定檔案和程式的詳細資訊，請參閱 [!DNL Anaplan] 設定檔案。

1. 選取或新增 [!DNL Anaplan] 連線設定檔。
1. 更新所有剩餘 [!DNL Anaplan] 具有 [!DNL Anaplan] 連線時顯示。
1. 在 **[!UICONTROL 將CSV轉換為JSON物件]** 模組，新增資料結構以將CSV欄對應至可用的JSON物件。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 出現提示時，為此方案部署中的其他模組選擇此資料結構。
1. 在 **[!UICONTROL 檢查連結的項目]** 模組，選擇或添加 [!DNL Workfront] 連線設定檔。
1. 更新所有剩餘 [!DNL Workfront] 模組 [!DNL Workfront] 連線時顯示。

## 其他建議的方案範本

要完成此模板表示的工作流，您還必須部署以下附加模板：

* [[!UICONTROL 建立 [!DNL Anaplan] 清單項 [!DNL Adobe Workfront] 行銷活動請求]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

花費最佳化的其他案例包括：

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 專案更新至 [!DNL Anaplan] 清單項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 實際更新小時數 [!DNL Anaplan] 清單項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 費用 [!DNL Anaplan] 清單項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
