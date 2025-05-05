---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 在Microsoft Exchange中設定POP
description: ' [!DNL Microsoft Exchange] 中的POP電子郵件帳戶已停用。'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# 在[!DNL Microsoft Exchange]中設定POP

## 問題

[!DNL Microsoft Exchange]中的POP電子郵件帳戶已停用。

## 解決方案

在花費時間疑難排解問題之前，請先確定使用者的POP帳戶已正確設定。 如果您在確認POP帳戶已正確設定之後仍然遇到問題，請連絡[!DNL Microsoft]支援或其中一個合作夥伴以取得其他協助。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在[!DNL Microsoft Exchange]中設定POP

>[!NOTE]
>
>下列步驟可作為一般指南，用於為生產[!DNL Workfront]系統設定[!DNL Microsoft Exchange]中的POP。 根據Exchange的版本或Microsoft所做的程式碼變更，這些步驟可能會有顯著差異。

1. 在Exchange 2010伺服器上啟動並啟用POP3服務。

   >[!NOTE]
   >
   >預設不會啟動POP3服務。

   1. 啟動[!DNL Microsoft]的伺服器管理員。
   1. 導覽： **[!UICONTROL 伺服器管理員]** > **[!UICONTROL 組態]** >**[!UICONTROL 具有進階安全性的Windows防火牆]** > **[!UICONTROL 服務]**。

   1. 用滑鼠右鍵按一下&#x200B;**[!DNL Microsoft Exchange]POP3**，然後按一下&#x200B;**[!UICONTROL 內容]**。

   1. （條件式）若要確保POP服務自動啟動，請在&#x200B;**[!UICONTROL 一般]**&#x200B;標籤上將&#x200B;**[!UICONTROL 啟動]**&#x200B;型別設定為[!UICONTROL 自動]。

1. 設定伺服器的POP3。

   1. 啟動[!DNL Microsoft Exchange]管理主控台。
   1. 導覽： [!DNL Microsoft] **[!UICONTROL Exchange內部部署]** > **[!UICONTROL 伺服器組態]** > **[!UICONTROL 使用者端存取]**。

   1. 選擇&#x200B;**[!UICONTROL POP3]**。

      POP3在[!UICONTROL POP3]與[!UICONTROL IMAP4]索引標籤下的清單中。

   1. 在右側的&#x200B;**[!UICONTROL 動作]**&#x200B;下方，選取&#x200B;**[!UICONTROL POP3]**，然後選擇&#x200B;**[!UICONTROL 屬性]**。

   1. 按一下「**[!UICONTROL POP3屬性]**」，然後開啟「**[!UICONTROL 繫結]**」標籤。

      為POP3伺服器顯示設定的所有可用IP位址和連線埠號碼。 頂端方塊顯示未加密，而底部方塊顯示SSL/TLS連線的IP和連線埠。

   1. 按一下「**[!UICONTROL POP3屬性]**」，然後開啟「**[!UICONTROL 驗證]**」標籤。

   1. **[!UICONTROL 選取Secure]**&#x200B;登入。

      使用者端需要TLS連線才能向伺服器驗證。

1. 啟用或允許使用者連線至POP。

   1. 啟動[!DNL Microsoft Exchange]管理主控台。
   1. 導覽： [!DNL Microsoft] **[!UICONTROL Exchange內部部署]** > **[!UICONTROL 收件者組態]** > **[!UICONTROL 信箱]**。

      顯示信箱或使用者清單。

   1. 反白標示[!DNL Workfront]內正在使用的電子郵件。
   1. 在右側的&#x200B;**[!UICONTROL 動作]**&#x200B;下方，選取&#x200B;**[!UICONTROL 內容]**，然後開啟&#x200B;**[!UICONTROL 信箱功能]**&#x200B;索引標籤。

   1. （視條件而定）如果POP3已停用，請按一下&#x200B;**[!UICONTROL POP3]**，然後按一下&#x200B;**[!UICONTROL 啟用]**。

      顯示信箱或使用者清單。

1. 設定接收聯結器。

   1. 啟動[!DNL Microsoft Exchange]管理主控台。
   1. 導覽： [!DNL Microsoft] **[!UICONTROL Exchange內部部署]** > **[!UICONTROL 伺服器組態]** > **[!UICONTROL 集線傳輸]**。

      隨即顯示接收聯結器的清單。

   1. 確認接收聯結器&#x200B;*使用者端* *EX01*&#x200B;已啟用。

      其中&#x200B;*使用者端* *EX01*&#x200B;是您的Exchange伺服器名稱。

   1. 選取&#x200B;*使用者端EX01*，然後在右邊的&#x200B;**[!UICONTROL 動作]**&#x200B;下，選取&#x200B;**[!UICONTROL 屬性]**。

   1. 開啟&#x200B;**[!UICONTROL 驗證]**&#x200B;標籤，然後確定已核取&#x200B;**[!UICONTROL 傳輸層安全性(TLS)]**。

      >[!NOTE]
      >
      >若要使用基本驗證，您可能需要啟動TLS和整合式Windows驗證。
