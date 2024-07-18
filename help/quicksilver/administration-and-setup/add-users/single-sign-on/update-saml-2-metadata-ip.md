---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: 更新身分提供者中的SAML 2.0中繼資料
description: 您可以在身分提供者中更新SAML 2.0中繼資料。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 0%

---

# 更新身分提供者中的SAML 2.0中繼資料

{{important-admin-console-onboard}}

以下各節說明在使用Active Directory Federation Services (ADFS)做為身分提供者時，如何更新您的安全性宣告標籤語言(SAML) 2.0中繼資料。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 使用ADFS作為您的身分提供者

您可以在Adobe Workfront更新SAML 2.0憑證之前或之後更新ADFS中繼資料。 如果您選擇在更新SAML 2.0憑證之前，先更新Workfront中繼資料，則需執行其他步驟。

* [更新您的ADFS中繼資料](#update-your-adfs-metadata)
* [強制更新ADFS中繼資料](#force-your-adfs-metadata-to-update)

### 更新您的ADFS中繼資料 {#update-your-adfs-metadata}

若要將您的ADFS中繼資料設定為自動更新，請完成本節中的步驟。

依預設，ADFS會設定為自動檢查其所有信賴方信任中繼資料的更新；不過，預設值僅設定為每24小時輪詢一次。 您可以使用powershell命令變更此值。

1. 登入ADFS伺服器並開啟ADFS管理主控台。
1. 在左側面板中，展開&#x200B;**ADFS 2.0，**，然後展開&#x200B;**信任關係。**

1. 按一下&#x200B;**信賴方信任**&#x200B;資料夾。
1. 選取您先前設定要與Workfront搭配使用的信賴方信任，然後在右側面板中，按一下&#x200B;**從同盟中繼資料更新**。
1. （條件式）如果此選項變暗（表示先前已使用中繼資料檔案設定信賴方信任），請完成下列操作。

   1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

   1. 按一下&#x200B;**系統** > **單一登入(SSO)**。

   1. 按一下&#x200B;**編輯設定。**
   1. 按一下&#x200B;**編輯組態**，然後在&#x200B;**型別**&#x200B;下拉式清單中選取&#x200B;**SAML 2.0**。

   1. 複製&#x200B;**中繼資料URL**，它應該類似於以下內容：

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. 在ADFS伺服器上，用滑鼠右鍵按一下您先前設定的信賴方信任，然後按一下&#x200B;**[內容]。**
   1. 按一下&#x200B;**監視**&#x200B;標籤，然後將您從Workfront複製的URL貼到&#x200B;**信賴方的同盟中繼資料URL**&#x200B;欄位。

   1. 檢查&#x200B;**監視信賴方**&#x200B;和&#x200B;**自動更新信賴方**&#x200B;的選項。

   1. 按一下&#x200B;**確定。**
   1. 選取您先前設定要與Workfront搭配使用的信賴方信任；然後在右側面板中，按一下&#x200B;**從同盟中繼資料更新。**

1. 按一下[確定]****&#x200B;忽略有關ADFS 2.0不支援同盟中繼資料中某些內容的訊息。
1. 開啟&#x200B;**Windows Powershell模組。**
1. 載入所有模組後，在powershell中執行以下命令：

   `Get-ADFSProperties`

1. 尋找&#x200B;**監視間隔**&#x200B;旁的值。

   它將是一個數字，代表兩次輪詢之間的分鐘數。 預設值應為1440 （1440分鐘= 24小時）。

1. 在powershell中執行下列命令來設定新值：

   `Set-ADFSProperties -MonitoringInterval 1`

   這會將監視間隔從每24小時變更為每分鐘。 如果您希望降低1的輪詢頻率，可將其變更為另一個較大的值。

1. 若要確認此功能正常運作，請使用&#x200B;**事件檢視器**&#x200B;在ADFS2.0記錄檔中尋找下列資訊：

   **事件ID 156和157**

### 強制更新ADFS中繼資料 {#force-your-adfs-metadata-to-update}

若要更新ADFS中繼資料，請完成下節中的步驟。

若要在使用Active Directory Federation Services (ADFS)時強制在Workfront與您的SAML 2.0提供者之間交換中繼資料：

>[!NOTE]
>
>其中有些變更可能需要由您的IT部門執行。

1. 登入ADFS伺服器並開啟&#x200B;**ADFS管理主控台**。
1. 在左側面板中，展開&#x200B;**ADFS 2.0**，然後展開&#x200B;**信任關係**。

1. 按一下&#x200B;**信賴方信任**&#x200B;資料夾。
1. 選取您先前設定要與Workfront搭配使用的信賴方信任，然後在右側面板中，按一下&#x200B;**從同盟中繼資料更新**。

   如果此選項變暗且無法選取，請完成下列操作：

   （只有先前使用中繼資料檔案設定信賴方信任時，選項才會變暗。）

   1. 在Workfront的「設定」區域中，從您的Workfront單一登入設定畫面複製&#x200B;**中繼資料URL**。

      若要存取&#x200B;**中繼資料URL**&#x200B;的資訊：

      1. 按一下全域導覽列上Adobe Workfront右上角附近的&#x200B;**設定**。
      1. 按一下> **系統** > **單一登入(SSO)**。
      1. 按一下&#x200B;**編輯設定。**
      1. 按一下&#x200B;**編輯組態**，然後在&#x200B;**型別**&#x200B;下拉式清單中選取&#x200B;**SAML 2.0**。
      1. 複製&#x200B;**中繼資料URL**，它應該類似於以下內容：

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. 在ADFS伺服器上，用滑鼠右鍵按一下您先前設定的信賴方信任，然後按一下&#x200B;**[內容]。**
   1. 按一下&#x200B;**監視**&#x200B;標籤，然後將您從Workfront複製的URL貼到&#x200B;**信賴方的同盟中繼資料URL**&#x200B;欄位。
   1. 檢查&#x200B;**監視信賴方**&#x200B;和&#x200B;**自動更新信賴方**&#x200B;的選項。
   1. 按一下&#x200B;**確定**。
   1. 選取您先前設定要與Workfront搭配使用的信賴方信任，然後在右側面板中，按一下&#x200B;**從同盟中繼資料更新。**

1. 按一下[確定]****&#x200B;忽略有關ADFS 2.0不支援同盟中繼資料中某些內容的訊息。
1. 按一下&#x200B;**更新**&#x200B;以完成更新同盟中繼資料。

允許透過Workfront登入憑證的原生登入畫面存取Workfront的使用者（這可從&#x200B;**存取**&#x200B;區段中的每個使用者的設定檔頁面進行設定），可透過瀏覽至下列URL，使用其Workfront使用者名稱和密碼登入： `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`。

## 使用其他身分識別提供者

使用ADFS以外的身分提供者（例如Ping、Okta或Centrify）時，必須將Workfront中繼資料重新上傳至身分提供者。

如需有關如何取得新的Workfront中繼資料URL的詳細資訊，請參閱[更新您的ADFS中繼資料](#update-your-adfs-metadata)。

如需在Workfront中使用Active Directory Federation Services (ADFS)搭配SAML 2.0的其他資訊，請參閱[使用ADFS設定Adobe Workfront搭配SAML 2.0 ](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md)。
