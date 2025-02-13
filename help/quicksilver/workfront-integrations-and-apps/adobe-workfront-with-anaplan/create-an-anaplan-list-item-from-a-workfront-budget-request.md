---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 從 [!DNL Adobe Workfront] 預算請求建立 [!DNL Anaplan] 清單專案
description: 此整合情境會連結 [!DNL Adobe Workfront] 專案（行銷活動）與 [!DNL Anaplan] 預算清單專案。 若要完成此作業，請將預算要求新增至需要取得資金的 [!DNL Workfront] 專案。 此案例會監視未處理的預算請求，然後執行在 [!DNL Anaplan] 中建立空白預算清單專案的程式，以在Anaplan中啟動預算分配程式。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: d6fd224fb8a7b8094946814ae905bc0ff6e8223c
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---

# 從[!DNL Adobe Workfront]預算請求建立[!DNL Anaplan]清單專案

此整合情境連結[!DNL Adobe Workfront]專案（行銷活動）與[!DNL Anaplan]預算清單專案。 若要完成此作業，請將預算要求新增至需要取得資金的[!DNL Workfront]專案。 此案例會監視未處理的預算請求，然後執行在[!DNL Anaplan]中建立空白預算清單專案的程式，以在[!DNL Anaplan]中啟動預算分配程式。

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
   <td> <p>[！UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您的組織必須購買[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文所述的功能。</td> 
  </tr>
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

&#42;&#42;如需[!DNL  Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration)

## 觸發中的事件

此情境已排程為每15分鐘執行一次。

## 預期的[!DNL Workfront]組態

若要使用此情境，您在[!DNL Workfront]中必須擁有下列專案：

* [!DNL Workfront]中名為&#x200B;**[!DNL Anaplan]整合**&#x200B;的使用者設定檔，具有系統管理員許可權。

  如需在[!DNL Workfront]中建立使用者的詳細資訊，請參閱[新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

* **[!UICONTROL 預算請求]**&#x200B;自訂表單已附加至[!UICONTROL 請求]物件。

  自訂表單上必須包括下列必填欄位，以協助對應至[!DNL Anaplan]的資料：

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>欄位名稱</th> 
     <th>欄位型別</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[！UICONTROL預算請求型別]</td> 
     <td> <p>[！UICONTROL下拉式清單]</p> <p>選項：</p> 
      <ul> 
       <li> <p>[！UICONTROL資金調整]</p> </li> 
       <li> <p>[！UICONTROL初始資金]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL申請勞力資金]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL請求的費用基金]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

  如需建立自訂表單的相關資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

* 代表行銷活動和其他需要資金的專案的專案範本，已設定一個[!UICONTROL 預算請求]佇列主題。 已指派[!UICONTROL 預算請求]佇列主題來使用[!UICONTROL 預算請求]自訂表單。
* 專案物件的&#x200B;**[!UICONTROL 行銷活動簡報]**&#x200B;表單。

  此表單必須包含下列欄位：

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
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
     <td>[！UICONTROL RTF欄位]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL金鑰訊息]</td> 
     <td>[！UICONTROL RTF欄位]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL目標對象]</td> 
     <td> <p>[！UICONTROL下拉式清單]</p> <p>包含適合您流程的選項。</p> </td> 
    </tr> 
   </tbody> 
  </table>

  如需建立自訂表單的相關資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 預期的[!DNL Anaplan]組態

若要使用此情境，您在[!DNL Anaplan]中必須擁有下列專案：

* [!DNL Anaplan]中名為&#x200B;**[!UICONTROL [!DNL Workfront]整合]**&#x200B;的使用者設定檔，具有系統管理員許可權。
* 您要用於此情境的[!DNL Anaplan]模型。
* [!DNL Anaplan]模型中擷取促銷活動預算的清單。

  清單的模組必須支援接收下列屬性：

   * [!UICONTROL Workfront專案GUID]
   * [!UICONTROL 行銷活動名稱]
   * [!UICONTROL 已要求人力資金]
   * [!UICONTROL 已要求費用資金]
   * [!UICONTROL 預算要求型別]
   * [!UICONTROL 資金調整原因]

  此清單和模組必須儲存[!DNL Anaplan]正常功能所需的額外詳細資料，包括設定預算並傳達預算清單專案已準備好同步回[!DNL Workfront]的能力。

如需上述任何動作的指示，請參閱[!DNL Anaplan]檔案。

## 部署至[!DNL Workfront Fusion]

完成下列步驟，將此整合情境部署至您的[!DNL Fusion]帳戶。 這應該只有在完成必要的[!DNL Workfront]和[!DNL Anaplan]設定之後才完成。

1. 導覽至[!DNL Workfront Fusion]中的[!UICONTROL 範本]功能表，然後按一下&#x200B;**[!UICONTROL 從Workfront預算請求]**&#x200B;情境範本建立[!DNL Anaplan]清單專案。
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

* [[!UICONTROL 套用 [!DNL Anaplan] 預算配置至 [!DNL Adobe Workfront] 專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

支出最佳化的其他案例包括：

* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 專案更新至 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 實際時數更新至 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL 傳送 [!DNL Adobe Workfront] 費用給 [!DNL Anaplan] 清單專案]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
