---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 配置系統的基本資訊
description: 在設定Adobe Workfront系統時，您可以在客戶資訊頁面的基本資訊區段中管理組織的詳細資訊。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 2%

---

# 配置系統的基本資訊

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

在設定Adobe Workfront系統時，您可以在客戶資訊頁面的基本資訊區段中管理組織的詳細資訊。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> <col> 
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
   <td> <p>您必須是Workfront管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 存取客戶資訊

客戶代表貴組織的Workfront例項。 您身為Workfront的客戶，所在區域中的選項都是專屬的。

若要存取「客戶資訊」頁面：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **系統** > **客戶資訊**.

   根據您已購買的Workfront計畫，「客戶資訊」頁面可能會遺漏某些區段。 如果您需要了解貴組織使用的Workfront計畫，請連絡您的客戶代表。

   「客戶資訊」區域中可用的區段為：

   * **基本資訊**

      如需在Workfront中設定基本資訊的詳細資訊，請參閱 [配置基本資訊](#configure-basic-info).

   * **API 金鑰設定**

      如需API金鑰設定的相關資訊，請參閱 [管理API金鑰](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **IP 允許清單**

      如需將IP位址新增至您允許清單，供您的使用者存取Workfront的相關資訊，請參閱 [配置防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **授權**

      有關許可證的資訊，請參閱 [管理系統中的可用許可證](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## 配置基本資訊 {#configure-basic-info}

在「客戶資訊」頁面的「基本資訊」區域內，有關客戶的部分詳細資訊由Workfront設定，並以唯讀模式顯示。 您可以設定其他詳細資訊。 您可以在此區域編輯的任何選項，都會對Workfront中的所有使用者產生全域影響。

若要在「客戶資訊」區域中設定「基本資訊」區段：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **系統** > **客戶資訊**.

1. 在 **基本資訊** 區段 **客戶資訊** 頁面，找到下列關於您使用Workfront的例項的資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名稱</td> 
      <td>組織的名稱，也與公司的名稱相符。 此項目由Workfront新增，且無法編輯。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">群集設定 </td> 
      <td>實例的群集號。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理員電子郵件</td> 
      <td> <p>Workfront管理員的電子郵件地址。 您可以編輯此欄位，以符合您其中一位Workfront管理員的電子郵件地址。 與此電子郵件地址相關聯的使用者被視為您的Workfront系統的主要Workfront管理員。 來自Workfront的任何網站範圍通訊都會導向至此電子郵件地址，因此請務必持續更新。</p> <p><b>注意</b>:您無法停用、刪除或變更與管理員電子郵件相關聯的使用者的存取層級。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">網域</td> 
      <td> <p>建立帳戶時，網域由Workfront設定。</p> <p>網域會在您用來存取Workfront的URL中識別您的唯一子網域。<p>例如，如果貴組織已獲派「mycompany」網域，則您用來存取Workfront的URL為 <i>https://mycompany.my.workfront.com。</i></p><p>您無法自行編輯網域。 如果您想要變更網域，請聯絡Workfront客戶支援。 如需聯絡Workfront客戶支援的詳細資訊，請參閱 <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">聯絡客戶支援</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">時區</td> 
      <td> <p>這是您Workfront執行個體的預設時區。 您可以編輯此欄位，以符合主要Workfront位置的時區。 您選取的時區會決定下列項目： </p> 
       <ul> 
        <li>傳出電子郵件中顯示的日期和時間</li> 
        <li>新使用者建立時的預設時區</li> 
       </ul> <p>使用者可在其設定檔下修改其Workfront例項的時區。 當使用者修改其時區時，來自Workfront的電子郵件中的日期和時間會符合其設定檔偏好設定。 有關修改用戶配置檔案首選項的詳細資訊，請參閱 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">配置我的設定</a>. 建立新計畫時，系統會將其選為預設時區。 如需建立排程的詳細資訊，請參閱 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>.</p> <p>如需如何使用排程來協助使用者在Workfront中跨時區進行共同作業的詳細資訊，請參閱 <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">跨時區工作</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">地區</td> 
      <td>控制傳出電子郵件中使用的語言、日期和數字格式。 新建用戶時，此處選擇的區域設定為預設值。 用戶可以在其用戶配置檔案中修改其區域設定。 當使用者修改其地區設定時，來自Workfront的電子郵件中的語言、日期和數字格式會符合其設定檔偏好設定。 如需修改設定檔偏好設定的詳細資訊，請參閱 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">配置我的設定</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">儲存配額</td> 
      <td> <p>這是Workfront執行個體中可用的檔案儲存空間量。<br>配額包含您直接上傳至Workfront的檔案。<br>其中不包含：</p> 
       <ul> 
        <li>您從任何其他協力廠商服務提供者(SharePoint、Google Drive、Webdam、Box、Dropbox、任何其他檔案資產管理提供者)連結至Workfront的檔案。</li> 
        <li>您的Workfront資料（專案、工作、問題、使用者等）。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">產品版本</td> 
      <td>這是指派給您的Workfront例項類型。 大多數Workfront客戶的產品版本為 <strong>企業</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。
