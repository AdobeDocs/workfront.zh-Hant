---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: 在您的身分提供者中更新SAML 2.0中繼資料
description: 您可以在身分提供者中更新SAML 2.0中繼資料。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 96f1d50024605328713ca2019f3b726e27dc569c
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# 在您的身分提供者中更新SAML 2.0中繼資料

{{important-admin-console-onboard}}

以下各節將說明當使用Active Directory聯合身份驗證服務(ADFS)作為身份提供程式時，如何更新您的安全斷言標籤語言(SAML)2.0元資料。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用ADFS作為身分提供者

您可以在Adobe Workfront更新SAML 2.0憑證之前或之後更新ADFS中繼資料。 如果您選擇在Workfront更新SAML 2.0憑證之前更新ADFS中繼資料，則需要執行其他步驟。

* [更新ADFS中繼資料](#update-your-adfs-metadata)
* [強制更新ADFS中繼資料](#force-your-adfs-metadata-to-update)

### 更新ADFS中繼資料 {#update-your-adfs-metadata}

若要設定要自動更新的ADFS中繼資料，請完成本節中的步驟。

預設情況下，ADFS配置為自動檢查其所有信賴方信任元資料的更新；不過，預設設定為僅每24小時輪詢一次。 可以使用powershell命令更改此值。

1. 登錄到ADFS伺服器並開啟ADFS管理控制台。
1. 在左側面板中，展開 **ADFS 2.0、** 然後展開 **信任關係。**

1. 按一下 **信賴方信託** 檔案夾。
1. 選取您先前設定為搭配Workfront使用的信賴方信任，然後在右側面板中，按一下&#x200B;**從聯合元資料更新**.
1. （條件性）如果此選項呈暗灰色（這表示信賴方信任先前是使用中繼資料檔案設定的），請完成以下操作。

   1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

   1. 按一下 **系統** > **單一登入(SSO)**.

   1. 按一下 **編輯設定。**
   1. 按一下 **編輯配置**，然後選取 **SAML 2.0** 在 **類型** 下拉式清單。

   1. 複製 **中繼資料URL**，其應類似下列：

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. 在ADFS伺服器上，按一下右鍵以前配置的信賴方信任，然後按一下 **屬性。**
   1. 按一下 **監控** 標籤，然後將您從Workfront複製的URL貼到 **信賴方的聯合元資料URL** 欄位。

   1. 勾選 **監視信賴方** 和 **自動更新信賴方**.

   1. 按一下 **好。**
   1. 選取您先前設定為搭配Workfront使用的信賴方信任；然後，在右側面板中，按一下 **從聯合元資料更新。**

1. 按一下 **確定** 忽略ADFS 2.0不支援的聯合元資料中某些內容的相關訊息。
1. 開啟 **Windows Powershell模組。**
1. 在載入所有模組後，在powershell中運行以下命令：

   `Get-ADFSProperties`

1. 尋找旁邊的值 **監控間隔。**

   它將代表兩次投票之間的分鐘數。 預設值應為1440（1440分鐘= 24小時）。

1. 在powershell中運行以下命令以設定新值：

   `Set-ADFSProperties -MonitoringInterval 1`

   這會將監控間隔從每24小時變更為每分鐘。 如果您想讓輪詢頻率較低，可將1變更為另一個較大的值。

1. 若要確認運作正常，請使用 **事件檢視器** 在ADFS2.0日誌中查找以下資訊：

   **事件ID 156和157**

### 強制更新ADFS中繼資料 {#force-your-adfs-metadata-to-update}

若要更新ADFS中繼資料，請完成下節中的步驟。

在使用Active Directory聯合身份驗證服務(ADFS)時，要強制在Workfront和您的SAML 2.0提供程式之間交換元資料：

>[!NOTE]
>
>您的IT部門可能需要完成其中一些變更。

1. 登錄到ADFS伺服器並開啟 **ADFS管理控制台**.
1. 在左側面板中，展開 **ADFS 2.0**，然後展開 **信任關係**.

1. 按一下 **信賴方信託** 檔案夾。
1. 選取您先前設定為搭配Workfront使用的信賴方信任，然後在右側面板中，按一下 **從聯合元資料更新**.

   如果此選項暗顯且無法選取，請完成下列操作：

   （只有在信賴方信任先前已使用中繼資料檔案設定時，選項才會暗顯。）

   1. 在Workfront中，在「設定」區域中，複製 **中繼資料URL** 從「Workfront單一登入」設定畫面。

      若要存取 **中繼資料URL**:

      1. 按一下 **設定** 在全域導覽列上Adobe Workfront的右上角附近。
      1. 按一下> **系統** > **單一登入(SSO)**.
      1. 按一下 **編輯設定。**
      1. 按一下 **編輯配置**，然後選取 **SAML 2.0** 在 **類型** 下拉式清單。
      1. 複製 **中繼資料URL**，其應類似下列：

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`
   1. 在ADFS伺服器上，按一下右鍵以前配置的信賴方信任，然後按一下 **屬性。**
   1. 按一下 **監控** 標籤，然後將您從Workfront複製的URL貼到 **信賴方的聯合元資料URL** 欄位。
   1. 勾選 **監視信賴方** 和 **自動更新信賴方**.
   1. 按一下 **確定**.
   1. 選取您先前設定為搭配Workfront使用的信賴方信任，然後在右側面板中，按一下 **從聯合元資料更新。**


1. 按一下 **確定** 忽略ADFS 2.0不支援的聯合元資料中某些內容的相關訊息。
1. 按一下 **更新** 完成聯合元資料的更新。

允許使用Workfront登入憑證透過原生登入畫面存取Workfront的使用者(這可從 **存取** 區段)可導覽至下列URL，使用其Workfront使用者名稱和密碼登入： `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## 使用其他身分提供者

使用ADFS以外的身分提供者時（例如Ping、Okta或Centrify），您必須將Workfront中繼資料重新上傳至身分提供者。

如需如何取得新Workfront中繼資料URL的詳細資訊，請參閱 [更新ADFS中繼資料](#update-your-adfs-metadata).

有關在Workfront中將Active Directory聯合身份驗證服務(ADFS)與SAML 2.0搭配使用的其他資訊，請參見 [使用ADFS以SAML 2.0設定Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
