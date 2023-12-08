---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 設定系統安全性偏好設定
description: 身為Adobe Workfront管理員，您可以設定Workfront系統的安全性偏好設定。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: c709ecd8023a0a9ce9c5b4591145d0a70912e003
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 4%

---

# 設定系統偏好設定

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

身為Adobe Workfront管理員，您可以設定Workfront系統的偏好設定：

* 從行動應用程式和其他整合式應用程式存取Workfront
* 將Workfront內嵌至iframe的規則

您在系統偏好設定中進行的變更會影響系統中所有使用者，以及他們在Workfront中的體驗。

我們建議您在Workfront實作期間設定系統偏好設定，之後只需偶爾重新造訪一次。

## 存取需求

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
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 設定您的系統偏好設定

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **系統** > **偏好設定**.

1. 選取下列任一欄位來建立組織的設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>啟用快速複查程式</p> </td> 
      <td>可讓您為貴組織啟用每月Workfront發行，而非每季發行。</p><p>如需快速發行程式的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">啟用或停用組織的快速發行</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>允許內嵌 <strong>Workfront</strong> 在iframe中</p> </td> 
      <td>可讓您將Workfront內嵌於iframe中。<p>此選項預設為停用。</p><p><b>重要</b>：在iframe中顯示Web型應用程式，會使應用程式容易受到點選劫持安全性漏洞的影響。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Office 365 增益集允許 SAML 2.0 驗證</td> 
      <td> <p>當Workfront與SAML 2.0單一登入解決方案整合時，可讓您僅將Workfront內嵌在Office 365增益集適用的iframe中。 </p> <p>此選項預設為啟用。</p> <p><b>注意</b>：如果您啟用上述選項， <strong>允許在iframe中內嵌Workfront</strong>，選項 <strong>允許Office 365增益集中的SAML 2.0驗證</strong> 已啟用且變暗。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">啟用在建立外部頁面URL時使用工作階段資訊</td> 
      <td> <p>允許使用者在將外部頁面新增到儀表板時使用網站的工作階段ID資訊。</p> <p>如需新增外部頁面至控制面板的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">將外部網頁內嵌在控制面板中</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">讓人們使用Workfront的行動應用程式和 <strong>Workfront</strong> Outlook增益集</td> 
      <td> <p>允許使用者存取行動應用程式(適用於iPad和行動電話應用程式的Workfront View)和Workfront Outlook應用程式。</p> <p>此選項預設為啟用。 </p> <p>如需Workfront檢視的相關資訊，請參閱 <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">使用Adobe Workfront檢視</a>. 如需行動應用程式的詳細資訊，請參閱 <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">使用Adobe Workfront行動應用程式</a>.</p> <p>如需有關Outlook外掛程式的詳細資訊，請參閱 <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">設定適用於Outlook的Adobe Workfront</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>透過使用電子郵件地址與沒有Workfront帳戶的人共同作業</p> </td> 
      <td>可讓Workfront使用者透過包含電子郵件地址而非姓名來與沒有Workfront帳戶的人共用特定專案。 使用者可使用其電子郵件地址與外部使用者共用下列專案：
       <ul>
        <li>文件<br></li>
        <li>檔案請求<br></li>
        <li>檔案核准</li>
        <li>行事曆</li>
       </ul><p>此選項預設為啟用。</p> <p><b>重要</b>：如果停用此選項，您的Workfront執行個體將無法使用外部使用者存取層級。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Workfront中的內建存取層級</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求外部使用者使用密碼註冊</td> 
      <td> <p>外部使用者必須先註冊，才能在Workfront中檢視專案。 此選項預設為停用。 當您啟用此選項時，沒有Workfront帳戶但依電子郵件地址包含在特定更新中的人員，將會在檢視其所包含的專案之前，收到建立帳戶的提示。 這會為其建立外部使用者帳戶。</p> <p>此選項預設為停用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">之後自動將使用者登出。</td> 
      <td> 可讓您指定使用者何時在經過一段閒置期間後登出Workfront。 根據預設，使用者會在閒置8小時後登出。 <p>此選項也會影響使用單一登入解決方案的Workfront客戶。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">之後自動將行動使用者登出 </td> 
      <td>可讓您指定使用者在一段閒置時間後何時登出Workfront應用程式。 根據預設，使用者會在閒置7天後登出。 <p>此選項也會影響使用單一登入解決方案的Workfront客戶。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">系統中的使用者預設會看到新首頁體驗 </td> 
      <td>可讓您指定使用者是否預設會看到新首頁體驗。 啟用後，使用者預設將會看到新首頁體驗，但仍可依個人情況選擇啟用或停用新首頁。 停用時，使用者將不會看到可讓他們切換至新首頁的橫幅，但是，他們仍然可以手動輸入以導覽至他們的新首頁 <code>/home/workspaces</code> 執行個體URL結尾處。 此設定預設為啟用。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。

   您在此處儲存的變更會影響Workfront中所有使用者的體驗，以及以外部使用者身分與他們互動的任何人的體驗。
