---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 從Outlook電子郵件建立 [!DNL Adobe Workfront] 要求
description: 您可以從Outlook中的電子郵件建立 [!DNL Adobe Workfront] 要求。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# 從[!UICONTROL Outlook]電子郵件建立[!DNL Adobe Workfront]要求

>[!IMPORTANT]
>
>[Microsoft正在停用對舊版Exchange Online權杖](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支援，Workfront Outlook增益集目前使用這些權杖進行驗證。 Microsoft的這項變更已開始影響客戶，並將在2025年10月前持續分階段推出。
>
>* **在Microsoft完全停用這些Token後，適用於Microsoft Outlook整合的Workfront將無法繼續運作。**
>
>在這次變更中，Microsoft已決定變更代號重新啟用的方式。 在&#x200B;**2025年6月30日**&#x200B;之後，管理員將無法再自行重新啟用權杖 — 只有Microsoft支援可授予例外狀況。 **在2025年10月1日，所有租使用者的舊版代號將會關閉。 將不會授與例外。**

您可以從Outlook中的電子郵件建立[!DNL Adobe Workfront]要求。

當您根據電子郵件建立[!DNL Workfront]要求時，預設情況下要求中包含電子郵件內容（包括主旨與內文）。

>[!NOTE]
>
>您無法從共用的[!UICONTROL Outlook]信箱建立[!DNL Workfront]要求。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL Work]， [!UICONTROL 計畫]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 先決條件

您的[!DNL Workfront]管理員必須以[!DNL Workfront]啟用[!DNL Outlook for Office]，您才能使用此整合。

## 從[!DNL Outlook]電子郵件建立請求

若要從[!DNL Outlook]建立[!DNL Workfront]要求：

1. 選取包含您要包含在[!DNL Workfront]要求中的資訊的電子郵件。
1. 按一下電子郵件訊息右上角的&#x200B;**[!DNL Workfront]**&#x200B;圖示，以顯示Workfront增益集。\
   您可能需要按一下電子郵件右上角的向下箭頭，才能存取[!DNL Workfront]圖示。

1. 按一下&#x200B;**[!UICONTROL 功能表]**&#x200B;圖示![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png)以顯示可用[!DNL Workfront]選項清單。

1. 按一下&#x200B;**[!UICONTROL 送出要求]**。
1. 在&#x200B;**[!UICONTROL 選取要求型別]**&#x200B;欄位中，選取您要提交要求的要求佇列。

1. 指定下列資訊：\
   可用欄位可能會因請求佇列的設定方式而異。 如需可能欄位的完整清單和說明，請參閱[建立和提交 [!DNL Adobe Workfront] 要求](../../manage-work/requests/create-requests/create-submit-requests.md)文章。

   * **[!UICONTROL 主旨]：**&#x200B;指定要求的主旨。 預設會使用電子郵件主旨。
   * **[!UICONTROL 描述]：**&#x200B;指定要求的描述。 預設會使用電子郵件內文。
   * **[!UICONTROL 檔案]：**&#x200B;附加您要包含在要求中的任何檔案。 您可以透過拖放或按一下&#x200B;**[!UICONTROL 選取檔案]**&#x200B;並瀏覽及選取檔案來附加檔案。\

     依預設，任何附加到電子郵件的檔案都會包含在請求中。

1. 按一下&#x200B;**[!UICONTROL 送出要求]**。\
   要求已提交至[!DNL Workfront]，位於指定的要求佇列中。

1. （選用）導覽回[!DNL Outlook]，並選取原始電子郵件。\
   在[!DNL Workfront]增益集面板頂端，請注意含有連結的確認，表示電子郵件已新增至Workfront作為請求。 連結包含轉換日期。\
