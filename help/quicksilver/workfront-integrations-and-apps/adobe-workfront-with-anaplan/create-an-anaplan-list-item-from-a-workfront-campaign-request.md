---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 建立 [!DNL Anaplan] 清單項 [!DNL Adobe Workfront] 行銷活動請求
description: 此整合案例會連結 [!DNL Adobe Workfront] 包含 [!DNL Anaplan] 預算清單項。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 2%

---

# 建立 [!DNL Anaplan] 清單項 [!DNL Adobe Workfront] 行銷活動請求

此整合案例會連結 [!DNL Adobe Workfront] 包含 [!DNL Anaplan] 預算清單項。

此情境會監視新增至請求佇列的促銷活動請求。 一旦記錄了促銷活動請求，就會在 [!DNL Anaplan] 來啟動資金流程。

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
   <td role="rowheader">[!UICONTROL Adobe Workfront]計畫*</td> 
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

* 中的使用者設定檔 [!DNL Workfront] 已命名 **[!UICONTROL [!DNL Anaplan]整合]**，具有系統管理員權限。

   如需在 [!DNL Workfront]，請參閱 [新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL 行銷活動簡報]** 附加至的自訂表單 [!UICONTROL 要求] 物件。

   自訂表單中必須包含下列必填欄位，以輔助將資料對應至Anaplan:

   | 欄位名稱 | 欄位類型 |
   |---|---|
   | [!UICONTROL 請求資金總額] |  |
   | [!UICONTROL 所申請的勞動資金] |  |
   | [!UICONTROL 請求的費用資金] |  |
   | [!UICONTROL 已傳送至 [!DNL Anaplan]] | 核取方塊 |

   表單上可能有下列選用欄位。 此情境僅對應上述欄位，但行銷活動簡報上的任何其他欄位皆可對應。

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
     <td>日期 </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL在市場結束日期]</td> 
     <td>日期</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL促銷活動概述]</td> 
     <td>段落文字欄位</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL密鑰消息]</td> 
     <td>段落文字欄位</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL目標對象]</td> 
     <td> <p>下拉</p> <p>納入適合您流程的選項。</p> </td> 
    </tr> 
   </tbody> 
  </table>

   如需建立自訂表單的詳細資訊，請參閱 [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* 設為請求佇列的專案，可擷取新的促銷活動請求。 此 [!UICONTROL 行銷活動簡報] 表單必須附加至這些請求。

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
   * [!UICONTROL 請求的費用資金]
   * [!UICONTROL 預算請求類型]

   此清單和模組必須儲存正常功能所需的其他詳細資訊 [!DNL Anaplan]，包括設定預算並傳達預算清單項目已準備好同步回的功能 [!DNL Workfront].

如需這些動作的指示，請參閱 [!DNL Anaplan] 檔案。

## 部署至 [!DNL Workfront Fusion]

完成下列步驟，將此整合案例部署至您的 [!DNL Fusion] 帳戶。 這必須在完成必要項目後才能完成 [!DNL Workfront] 和 [!DNL Anaplan] 設定。

1. 導覽至 [!UICONTROL 範本] 功能表 [!DNL Workfront Fusion] 並按一下 **[!UICONTROL 建立 [!DNL Anaplan] Workfront促銷活動請求中的清單項目]** 方案範本。
1. 取代下列變數值 [!DNL Anaplan] 變數：

   | 變數名稱 | 將值取代為 |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] 工作區ID] | 來自您 [!DNL Anaplan] 帳戶。 |
   | [!UICONTROL [!DNL Anaplan] 模型ID] | 來自您 [!DNL Anaplan] 帳戶和所選工作區。 |
   | [!UICONTROL [!DNL Anaplan] 模組名稱] | 說明所選促銷活動屬性的模組名稱 [!DNL Anaplan] 清單。 |
   | [!UICONTROL 促銷活動清單名稱] | 清單的名稱 [!DNL Anaplan] 帳戶和選取的工作區與模型。 |

   {style=&quot;table-layout:auto&quot;}

   有關如何設定檔案和程式的詳細資訊，請參閱 [!DNL Anaplan] 設定檔案。

1. 選取或新增 [!DNL Anaplan] 連線設定檔。
1. 更新所有剩餘 [!DNL Anaplan] 具有 [!DNL Anaplan] 連線時顯示。
1. 選取或新增 [!DNL Workfront] 連線設定檔。

   部署範本後，如果您要將預設對應欄位變更為，則要更新此模組，以從欄位屬性的值新增或移除自訂欄位參考 [!DNL Anaplan].

1. 更新所有剩餘 [!DNL Workfront] 模組 [!DNL Workfront] 連線時顯示。

## 其他建議的方案範本

要完成此模板表示的工作流，您還必須部署以下附加模板：

* [[!UICONTROL 套用 [!DNL Anaplan] 預算分配至 [!DNL Adobe Workfront] 行銷活動要求或行銷活動專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

花費最佳化的其他案例包括：

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 專案更新至 [!DNL Anaplan] 清單項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 實際更新小時數 [!DNL Anaplan] 清單項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 費用 [!DNL Anaplan] 清單項目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
