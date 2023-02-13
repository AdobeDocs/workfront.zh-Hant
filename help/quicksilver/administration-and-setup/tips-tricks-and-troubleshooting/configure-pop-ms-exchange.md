---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 在Microsoft Exchange中配置POP
description: 中的POP電子郵件帳戶 [!DNL Microsoft Exchange] 已停用。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 在中配置POP [!DNL Microsoft Exchange]

## 問題

中的POP電子郵件帳戶 [!DNL Microsoft Exchange] 已停用。

## 解決方案

在花時間診斷問題之前，請確保正確配置了用戶的POP帳戶。 如果在確認POP帳戶配置正確後繼續遇到問題，請聯繫 [!DNL Microsoft] 支援或其合作夥伴，以獲得更多幫助。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 在中配置POP [!DNL Microsoft Exchange]

>[!NOTE]
>
>以下步驟可作為配置POP的一般指南，在 [!DNL Microsoft Exchange] 為製作 [!DNL Workfront] 系統。 步驟可能會因Exchange版本或Microsoft所做的程式碼變更而有顯著差異。

1. 在Exchange 2010伺服器上啟動並啟用POP3服務。

   >[!NOTE]
   >
   >預設情況下，POP3服務不啟動。

   1. 開始 [!DNL Microsoft]的伺服器管理員。
   1. 導覽： **[!UICONTROL 伺服器管理員]** > **[!UICONTROL 設定]** >**[!UICONTROL 具有高級安全性的Windows防火牆]** > **[!UICONTROL 服務]**.

   1. 按一下右鍵 **[!DNL Microsoft Exchange]POP3**，然後按一下 **[!UICONTROL 屬性]**.

   1. （條件性）為確保POP服務自動啟動，請在 **[!UICONTROL 一般]** 頁簽，設定 **[!UICONTROL 啟動]** 類型 [!UICONTROL 自動].

1. 為伺服器配置POP3。

   1. 啟動 [!DNL Microsoft Exchange] 管理控制台。
   1. 導覽： [!DNL Microsoft] **[!UICONTROL 內部部署的Exchange]** > **[!UICONTROL 伺服器配置]** > **[!UICONTROL 用戶端存取]**.

   1. 選擇 **[!UICONTROL POP3]**.

      POP3在 [!UICONTROL POP3] 和 [!UICONTROL IMAP4] 標籤。

   1. 右側下方 **[!UICONTROL 動作]**，選取 **[!UICONTROL POP3]**，然後選擇 **[!UICONTROL 屬性]**.

   1. 按一下 **[!UICONTROL POP3屬性]**，然後開啟 **[!UICONTROL 綁定]** 標籤。

      顯示為POP3伺服器配置的所有可用IP地址和埠號。 頂端方塊顯示未加密，底部方塊顯示SSL/TLS連線的IP和埠。

   1. 按一下 **[!UICONTROL POP3屬性]**，然後開啟 **[!UICONTROL 驗證]** 標籤。

   1. **[!UICONTROL 選擇安全]** 登入。

      用戶端需要TLS連線才能驗證伺服器。

1. 啟用或允許用戶連接到POP。

   1. 啟動 [!DNL Microsoft Exchange] 管理控制台。
   1. 導覽： [!DNL Microsoft] **[!UICONTROL 內部部署的Exchange]** > **[!UICONTROL 收件者設定]** > **[!UICONTROL 郵箱]**.

      郵箱或用戶的清單隨即顯示。

   1. 反白顯示中使用的電子郵件 [!DNL Workfront].
   1. 右側下方 **[!UICONTROL 動作]**，選取 **[!UICONTROL 屬性]**，然後開啟 **[!UICONTROL 郵箱功能]** 標籤。

   1. （條件性）如果POP3已禁用，請按一下 **[!UICONTROL POP3]**，然後按一下 **[!UICONTROL 啟用]**.

      郵箱或用戶的清單隨即顯示。

1. 配置接收連接器。

   1. 開始 [!DNL Microsoft Exchange] 管理控制台。
   1. 導覽： [!DNL Microsoft] **[!UICONTROL 內部部署的Exchange]** > **[!UICONTROL 伺服器配置]** > **[!UICONTROL 集線器傳輸]**.

      接收連接器清單隨即顯示。

   1. 確認接收連接器 *用戶端* *EX01* 啟用。

      其中 *用戶端* *EX01* 是Exchange伺服器的名稱。

   1. 選擇 *客戶端EX01*，然後在右下方 **[!UICONTROL 動作]**，選取 **[!UICONTROL 屬性]**.

   1. 開啟 **[!UICONTROL 驗證]** 標籤，然後確定 **[!UICONTROL 傳輸層安全性(TLS)]** 已勾選。

      >[!NOTE]
      >
      >若要進行基本驗證，您可能需要啟動TLS和整合式Windows驗證。
