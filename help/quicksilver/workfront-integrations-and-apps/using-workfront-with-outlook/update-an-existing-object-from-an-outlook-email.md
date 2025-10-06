---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 從Outlook電子郵件更新現有的物件
description: 您可以從Outlook電子郵件更新現有的專案、任務或問題。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 從[!DNL Outlook]電子郵件更新現有的物件

>[!IMPORTANT]
>
>[Microsoft已停用對舊版Exchange Online權杖](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支援，這些權杖是由Workfront Outlook增益集用於驗證。 Microsoft的這項變更會分階段推出，並於2025年10月1日完成。
>
>**由於Microsoft已停用這些權杖，適用於Microsoft Outlook整合的Workfront已停止運作。**

您可以從[!DNL Outlook]電子郵件更新資訊的現有專案、任務或問題。

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

您的[!DNL Workfront]管理員必須以[!DNL Outlook for Office]啟用[!DNL Workfront]，您才能使用此整合。

## 從[!DNL Outlook]電子郵件更新現有的物件

1. 在[!DNL Outlook]中，選取包含您要包含在[!DNL Adobe Workfront update]中的資訊的電子郵件。
1. 按一下電子郵件訊息右上角的&#x200B;**[!DNL Workfront]**&#x200B;圖示，以顯示Workfront增益集。\
   您可能需要按一下電子郵件右上角的向下箭頭，才能存取[!DNL Workfront]圖示。

1. 按一下&#x200B;**[!UICONTROL 功能表]**&#x200B;圖示![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png)以顯示可用[!DNL Workfront]選項的清單。\


1. 在Workfront **[!UICONTROL 中按一下]更新**。\
   在儲存為任務之前，您可以從電子郵件更新以下資訊：

   * **[!UICONTROL 型別]**：選取您要更新的物件型別。 您可以選取&#x200B;**[!UICONTROL 專案]**、**[!UICONTROL 任務]**&#x200B;或&#x200B;**[!UICONTROL 問題]**。 您選取的物件會決定顯示在下方&#x200B;**[!UICONTROL 名稱]**&#x200B;欄位中的結果。 如果您不確定物件型別，請選取&#x200B;**[!UICONTROL 全部]**&#x200B;以同時搜尋專案、任務和問題。

   * **[!UICONTROL 名稱]**：開始輸入您要更新的專案、任務或問題的名稱。 當名稱出現在下拉式清單中時，按一下該名稱。
   * **[!UICONTROL 更新]**：依預設，更新與電子郵件內文相同。 您可以視需要修改更新。\

     此[!UICONTROL 更新]在Workfront中顯示為更新狀態。

   * **[!UICONTROL 附件]**：任何電子郵件附件都會儲存至任務的[!UICONTROL 檔案]區域。 提交更新之前，您可以刪除任何附件。

1. （選擇性）按一下&#x200B;**[!UICONTROL 包含其他]**，開始輸入您要包含在更新中的使用者名稱，然後當名稱出現在下拉式清單中時按一下該名稱。\
   重複此程式以包含其他使用者，然後按一下&#x200B;**[!UICONTROL 完成]**。\
   依預設，無論您是否納入通知，您要回覆的使用者都會收到通知。\

1. （選擇性）按一下&#x200B;**[!UICONTROL 鎖定]**&#x200B;圖示，將此更新限制在您公司內的使用者。 當更新被鎖定時，您公司外部的使用者看不到更新。

   * **[!UICONTROL 已解除鎖定]：**&#x200B;任何具有專案、任務或更新所在問題的存取許可權的使用者都可以檢視更新。\

     依預設，會解除鎖定更新。\
      ![o365_addin_unlock.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL 已鎖定]：**&#x200B;只有您公司內的使用者可以檢視更新。\

     ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. 按一下&#x200B;**[!UICONTROL 更新]**。
1. （選擇性）按一下[在Workfront中檢視&#x200B;**&#x200B;**]以檢視[!DNL Workfront]Outlook[!UICONTROL 中與]整合的更新專案。
