---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 設定系統的基本資訊
description: 在設定Adobe Workfront系統時，您可以在客戶資訊頁面的「基本資訊」區段中管理有關組織的詳細資訊。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: 01a80f6140650ca12aaee14115f79449dcfa2a18
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 2%

---

# 設定系統的基本資訊

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

在設定Adobe Workfront系統時，您可以在客戶資訊頁面的「基本資訊」區段中管理有關組織的詳細資訊。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p> <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是Workfront管理員。 </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 存取客戶資訊

客戶代表貴組織的Workfront執行個體。 身為Workfront的客戶，此區域的選項是您專屬的。

若要存取「客戶資訊」頁面：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**系統** > **客戶資訊**。

   根據您購買的Workfront套件，客戶資訊頁面中可能遺漏某些區段。 如果您需要瞭解您的組織使用哪個Workfront套件，請聯絡客戶代表。

   「客戶資訊」區域中提供的區段包括：

   * **基本資訊**

     如需有關在Workfront中設定基本資訊的資訊，請參閱[設定基本資訊](#configure-basic-info)。

   * **API金鑰設定**

     如需API金鑰設定的相關資訊，請參閱[管理API金鑰](../../administration-and-setup/manage-workfront/security/manage-api-keys.md)。

   * **IP允許清單**

     如需將IP位址新增至您的允許清單(您的使用者可存取Workfront)的相關資訊，請參閱[設定防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

   * **電子郵件允許清單**

     如需新增電子郵件至允許清單的詳細資訊，請參閱[設定電子郵件允許清單](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)。

   <!--
   * **License**

     For information about licenses, see [Manage available licenses in your system](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).-->

## 設定基本資訊 {#configure-basic-info}

在「客戶資訊」頁面的「基本資訊」區域中，Workfront會設定有關客戶的一些詳細資料，這些詳細資料將以唯讀模式顯示。 其他詳細資料可由您設定。 您可以在此區域中編輯的任何選項都會對Workfront中的所有使用者產生全域影響。

若要在「客戶資訊」區域中設定「基本資訊」區段：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**系統** > **客戶資訊**。

1. 在&#x200B;**客戶資訊**&#x200B;頁面頂端的&#x200B;**基本資訊**&#x200B;區段中，尋找有關您使用Workfront的執行個體的下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td>組織名稱，也會符合公司的名稱。 此專案由Workfront新增，無法編輯。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">群集設定 </td> 
      <td>您執行個體的叢集編號。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理員電子郵件</td> 
      <td> <p>Workfront管理員的電子郵件地址。 您可以編輯此欄位以符合其中一個Workfront管理員的電子郵件地址。 與此電子郵件地址相關聯的使用者會視為Workfront系統的主要Workfront管理員。 來自Workfront的任何全網站通訊都會導向此電子郵件地址，因此保持更新非常重要。</p> <p><b>注意</b>：您無法停用、刪除或變更與管理員電子郵件相關聯之使用者的存取層級。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">網域</td> 
      <td> <p>網域是在建立帳戶時由Workfront設定。</p> <p>網域會識別您用來存取Workfront之URL的唯一子網域。<p>例如，如果您的組織已被指派網域「mycompany」，則您用來存取Workfront的URL為<i>https://mycompany.my.workfront.com。</i></p><p>您無法自行編輯網域。 如果您想要變更網域，請聯絡Workfront客戶支援。 如需聯絡Workfront客戶支援的詳細資訊，請參閱<a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">聯絡客戶支援</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">時區</td> 
      <td> <p>這是Workfront執行個體的預設時區。 您可以編輯此欄位以符合主要Workfront位置的時區。 您選取的時區會決定下列專案： </p> 
       <ul> 
        <li>外寄電子郵件中顯示的日期和時間</li> 
        <li>新使用者建立時的預設時區</li> 
       </ul> <p>使用者可以在個人資料下修改其Workfront執行個體的時區。 當使用者修改他們的時區時，他們來自Workfront的電子郵件中的日期和時間符合他們的設定檔偏好設定。 如需有關修改使用者設定檔偏好設定的詳細資訊，請參閱<a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">設定我的設定</a>。 當您建立新排程時，系統會選取預設時區作為預設時區。 如需建立排程的詳細資訊，請參閱<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>。</p> <p>如需使用排程協助使用者在Workfront中跨時區共同作業的詳細資訊，請參閱<a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">跨時區工作</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預設電子郵件地區設定</td> 
      <td>控制用於外寄電子郵件訊息的語言、日期和數字格式。 此處選取的地區設定是建立新使用者時的預設設定。 使用者可以在他們的使用者設定檔中修改他們的地區設定。 當使用者修改他們的地區設定時，他們來自Workfront的電子郵件中的語言、日期和數字格式符合他們的設定檔偏好設定。 如需有關修改設定檔偏好設定的詳細資訊，請參閱<a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">設定我的設定</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">儲存配額</td> 
      <td> <p>這是您的Workfront執行個體中可用的檔案儲存空間量。<br>配額包含您直接上傳至Workfront的檔案。<br>它不包含：</p> 
       <ul> 
        <li>檔案會從任何其他第三方服務提供者(SharePoint、Google Drive、Webdam、Box、Dropbox、任何其他檔案資產管理提供者)連結至Workfront。</li> 
        <li>您的Workfront資料（專案、任務、問題、使用者等）。</li> 
       </ul> </td> 
     </tr>
    </tbody> 
   </table>

1. 按一下「**儲存**」。
