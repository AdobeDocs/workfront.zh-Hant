---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 將Outlook電子郵件新增為工作清單
description: 您可以將 [!DNL Outlook] 電子郵件轉換為 [!DNL Adobe Workfront] 個任務。 電子郵件轉換後，任務會顯示在首頁區域的工作清單中。
author: Becky
feature: Workfront Integrations and Apps
exl-id: fcd02116-ffeb-43d3-8541-5e30e6cfdc5e
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# 將[!DNL Outlook]電子郵件新增為您的工作清單

>[!IMPORTANT]
>
>[Microsoft正在停用對舊版Exchange Online權杖](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支援，Workfront Outlook增益集目前使用這些權杖進行驗證。 Microsoft的這項變更已開始影響客戶，並將在2025年10月前持續分階段推出。
>
>* **在Microsoft完全停用這些Token後，適用於Microsoft Outlook整合的Workfront將無法繼續運作。**
>
>在這次變更中，Microsoft已決定變更代號重新啟用的方式。 在&#x200B;**2025年6月30日**&#x200B;之後，管理員將無法再自行重新啟用權杖 — 只有Microsoft支援可授予例外狀況。 **在2025年10月1日，所有租使用者的舊版代號將會關閉。 將不會授與例外。**



您可以將[!DNL Outlook]封電子郵件轉換為[!DNL Adobe Workfront]個任務。 電子郵件轉換後，任務便可在[!UICONTROL 首頁]區域的[!UICONTROL 工作]清單中使用。

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
   <td> <p>[！UICONTROL Work]， [！UICONTROL計畫]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 先決條件

您的[!DNL Workfront]管理員必須以[!DNL Workfront]啟用[!DNL Outlook for Office]，您才能使用此整合。

## 將[!DNL Outlook]電子郵件新增為您的工作清單

1. 在[!DNL Outlook]內選取要轉換為任務的電子郵件。
1. 按一下電子郵件訊息右上角的&#x200B;**[!DNL Workfront]**&#x200B;圖示，以顯示[!DNL Workfront]增益集。\
   您可能需要按一下電子郵件右上角的向下箭頭，才能存取[!DNL Workfront]圖示。

1. 按一下&#x200B;**[!UICONTROL 功能表]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png)圖示以顯示可用[!DNL Workfront]選項清單。\


1. 按一下&#x200B;**[!UICONTROL 新增至工作]**。\

1. 取消選取&#x200B;**[!UICONTROL 新增至專案]**&#x200B;欄位。
1. （選擇性）在儲存為任務之前，您可以從電子郵件更新下列資訊：

   * **[!UICONTROL 工作名稱]：**&#x200B;依預設，工作名稱與電子郵件主旨相同。 您可以視需要修改工作名稱。
   * **[!UICONTROL 描述]：**&#x200B;依照預設，描述與電子郵件內文相同。 您可以視需要修改說明。
   * **[!UICONTROL 附件]：**&#x200B;任何電子郵件附件都會儲存至任務的[!UICONTROL 檔案]區域。 您可以將電子郵件儲存為工作之前刪除任何附件。

1. 按一下&#x200B;**[!UICONTROL 新增]**。\
   任務已新增到首頁區域的[!UICONTROL 工作清單]，但沒有認可日期。

1. （選擇性）按一下[在Workfront中檢視] ****，在新標籤中顯示[!DNL Workfront]應用程式內的工作。

1. （選用）導覽回[!DNL Outlook]，並選取原始電子郵件。\
   在[!DNL Workfront]增益集面板頂端，請注意含有連結的確認訊息，指出電子郵件已新增至Workfront作為工作。 連結包含轉換日期。\
