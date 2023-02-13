---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 傳送 [!DNL Adobe Workfront] 費用 [!DNL Anaplan] 清單項目
description: 此整合案例會從 [!DNL Adobe Workfront] 包含 [!DNL Anaplan] 預算清單項。 共用此資訊可讓您更好地利用支出優化和財務分析， [!DNL Anaplan] 提供。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# 傳送 [!DNL Adobe Workfront] 費用 [!DNL Anaplan] 清單項目

此整合案例會從 [!DNL Adobe Workfront] 包含 [!DNL Anaplan] 預算清單項。 共用此資訊可讓您更好地利用支出優化和財務分析， [!DNL Anaplan] 提供。

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

* 中的使用者設定檔 [!DNL Workfront] 命名*[!UICONTROL *[!DNL Anaplan] 整合]**，具有系統管理員權限。

   如需在 [!DNL Workfront]，請參閱 [新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL 行銷活動簡報]** 附加至專案物件的自訂表單，以儲存您選取要傳送至的自訂資料值 [!DNL Anaplan].

   表單必須包含下列欄位：

   | 欄位名稱 | 欄位類型 |
   |---|---|
   | [!UICONTROL 上次傳輸日期] | 日期 |
   | [!UICONTROL 整合說明] | 段落文字欄位 |

   如需建立自訂表單的詳細資訊，請參閱 [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## 預期 [!DNL Anaplan] 設定

您必須在 [!DNL Anaplan] 若要使用此案例：

* 中的使用者設定檔 [!DNL Anaplan] 已命名 **[!UICONTROL [!DNL Workfront ]整合]**，具有系統管理員權限。
* 此 [!DNL Anaplan] 要用於此案例的模型。
* 清單 [!DNL Anaplan] 您要擷取促銷活動預算的模型。
* 安 **[!UICONTROL Anaplan實際費用導入]** 檔案，依順序包含下列各欄：

   1. [!UICONTROL [!DNL Workfront] 費用GUID]

   2. [!UICONTROL [!DNL Workfront] 項目GUID]

   3. [!UICONTROL 實際數量]

   4. [!UICONTROL 說明]

   5. [!UICONTROL 費用類型]

   6. [!UICONTROL 生效日期]

   7. [!UICONTROL 行銷活動名稱]

   8. [!UICONTROL [!DNL Anaplan] 清單項目ID]
   準備 [!UICONTROL [!DNL Anaplan] 實際費用導入] 檔案：

   1. 將下列項目複製並貼到文字編輯器或 [!DNL Excel].
   1. 將檔案儲存為CSV格式。
   1. 將檔案上傳至 [!DNL Anaplan].

      如需指示，請參閱 [!DNL Anaplan] 關於從檔案將資料匯入模組的檔案。

   1. 記下您給檔案的名稱；將在部署 [!UICONTROL 融合] 方案範本。

   範例CSV內容

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* 安 **[!UICONTROL [!DNL Anaplan]計畫費用導入]** 檔案，依順序包含下列各欄：

   1. [!UICONTROL [!DNL Workfront] 費用GUID]

   2. [!UICONTROL [!DNL Workfront] 項目GUID]

   3. [!UICONTROL 實際數量]

   4. [!UICONTROL 說明]

   5. [!UICONTROL 費用類型]

   6. [!UICONTROL 生效日期]

   7. [!UICONTROL 行銷活動名稱]

   8. [!UICONTROL [!DNL Anaplan] 清單項目ID]
   準備 [!UICONTROL [!DNL Anaplan] 計畫費用導入] 檔案：

   1. 將下列項目複製並貼到文字編輯器或 [!DNL Excel]
   1. 將檔案儲存為CSV格式
   1. 將檔案上傳至Anaplan。

      如需指示，請參閱 [!DNL Anaplan] 關於從檔案將資料匯入模組的檔案。

   1. 記下您給檔案的名稱；將在部署 [!UICONTROL 融合] 方案範本。

   範例CSV內容

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>


* A **[!UICONTROL 項目更新導入]** 準備執行匯入檔案上傳中傳送之資料的程式。

>[!NOTE]
>
>計畫費用和實際費用有單獨的導入檔案，以便分別在計畫費用和有效日期獨立報告。

如需這些動作的指示，請參閱 [!DNL Anaplan] 檔案。

## 部署至 [!DNL Fusion]

完成下列步驟，將此整合案例部署至您的 [!DNL Fusion] 帳戶。 這必須在完成必要項目後才能完成 [!DNL Workfront] 和 [!DNL Anaplan] 設定。

1. 導覽至 [!UICONTROL 範本] 功能表 [!DNL Workfront Fusion] 並按一下 **[!UICONTROL 將Workfront支出更新傳送至 [!DNL Anaplan] 清單項目]** 方案範本。
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
      <td>來自您 [!DNL Anaplan] 帳戶和您要用於此案例的所選工作區。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL促銷活動清單名稱]</td> 
      <td>清單的名稱 [!DNL Anaplan] 帳戶以及您要用於此案例的所選工作區和模型。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL檔案名：實際費用導入]</td> 
      <td> <p>將接收項目實際費用資料的檔案的名稱。</p> <p> (範例：WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL檔案名：計畫費用導入]</td> 
      <td> <p>將接收項目計畫費用資料的檔案的名稱。</p> <p> (範例：WorkfrontUpdateLinkedProjects_PlannededExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL進程名稱：項目更新導入]</td> 
      <td> <p>將執行項目費用資料導入的進程的名稱。</p> <p>(範例：WF整合 — 載入項目費用)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有關如何設定檔案和程式的詳細資訊，請參閱 [!DNL Anaplan] 設定檔案。

1. 選取或新增 [!DNL Anaplan] 連線設定檔。
1. 更新所有剩餘 [!DNL Anaplan] 具有 [!DNL Anaplan] 連線時顯示。
1. 選取或新增 [!DNL Workfront] 連線設定檔。
1. 更新所有剩餘 [!DNL Workfront] 模組 [!DNL Workfront] 連線時顯示。
1. 在 **[!UICONTROL 建立實際費用CSV]** 模組，新增資料結構以將專案屬性對應至CSV欄。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 在 **[!UICONTROL 建立計畫費用CSV]** 模組，新增資料結構以將專案屬性對應至CSV欄。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

## 其他建議的方案範本

此方案模板由下列也可部署的支出優化方案模板所補充：

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 專案更新至 [!DNL Anaplan] 清單項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 實際更新小時數 [!DNL Anaplan] 清單項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

連結預算請求的其他方案：

* [[!UICONTROL 建立 [!DNL Anaplan] 清單項 [!DNL Adobe Workfront] 預算請求]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 套用 [!DNL Anaplan] 預算分配至 [!DNL Adobe Workfront] 專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

連結促銷活動請求的其他案例：

* [[!UICONTROL 建立 [!DNL Anaplan] 清單項 [!DNL Adobe Workfront] 行銷活動請求]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 套用 [!DNL Anaplan] 預算分配至 [!DNL Adobe Workfront] 行銷活動要求或行銷活動專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
