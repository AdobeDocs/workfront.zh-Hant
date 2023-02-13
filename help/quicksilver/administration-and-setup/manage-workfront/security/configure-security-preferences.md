---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 配置系統安全首選項
description: 身為Adobe Workfront管理員，您可以為Workfront系統設定安全性偏好設定。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 04cf9d37c681398f5a0e2b9d7d45c0f8b93ab44b
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 3%

---

# 配置系統安全首選項

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

身為Adobe Workfront管理員，您可以為Workfront系統設定安全性偏好設定：

* 從行動應用程式和其他整合式應用程式存取Workfront
* 將Workfront內嵌在iframe中的規則

您在系統偏好設定中所做的變更，會影響您系統中的所有使用者，以及他們在Workfront中的體驗。

建議您在Workfront實作期間設定系統安全性偏好設定，之後偶爾會重新造訪。

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

## 配置系統安全首選項

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **系統** > **偏好設定**.

1. 在 **安全性** 區段，選取下列任一欄位以建立組織的安全設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>允許內嵌 <strong>Workfront</strong> iframe中</p> </td> 
      <td>可讓您將Workfront內嵌在iframe中。<p>預設會停用此選項。</p><p><b>重要</b>:在iframe中顯示Web型應用程式，會使應用程式易於發生點擊劫持安全漏洞。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Office 365 增益集允許 SAML 2.0 驗證</td> 
      <td> <p>可讓您在Workfront與SAML 2.0單一登入解決方案整合時，僅將Workfront內嵌於Office 365增益集的iframe中。 </p> <p>預設會啟用此選項。</p> <p><b>注意</b>:如果您啟用上述選項， <strong>允許在iframe中內嵌Workfront</strong>，選項 <strong>在Office 365增益集中允許SAML 2.0驗證</strong> 已啟用且呈灰色。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">建立外部頁面URL時啟用工作階段資訊的使用</td> 
      <td> <p>可讓使用者在新增外部頁面至控制面板時，使用網站的工作階段ID資訊。</p> <p>如需將外部頁面新增至控制面板的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">在控制面板中內嵌外部網頁</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">讓使用者使用Workfront的行動應用程式和 <strong>Workfront</strong> Outlook載入項</td> 
      <td> <p>可讓使用者存取行動應用程式(適用於iPad和行動電話應用程式的Workfront檢視)和Workfront Outlook應用程式。</p> <p>預設會啟用此選項。 </p> <p>如需Workfront檢視的相關資訊，請參閱 <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">使用Adobe Workfront檢視</a>. 如需行動應用程式的詳細資訊，請參閱 <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">使用Adobe Workfront行動應用程式</a>.</p> <p>有關Outlook插件的詳細資訊，請參見 <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">設定Adobe Workfront for Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>使用電子郵件地址與沒有Workfront帳戶的人員共同作業</p> </td> 
      <td>可讓Workfront使用者透過加入其電子郵件地址（而非姓名），與沒有Workfront帳戶的使用者共用特定項目。 使用者可以使用其電子郵件地址與外部使用者共用下列項目：
       <ul>
        <li>文件<br></li>
        <li>文檔請求<br></li>
        <li>檔案核准</li>
        <li>行事曆</li>
       </ul><p>預設會啟用此選項。</p> <p><b>重要</b>:如果停用此選項，Workfront執行個體中的「外部使用者」存取層級將無法使用。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Workfront中的內建存取層級</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求外部用戶使用密碼註冊</td> 
      <td> <p>需要外部使用者先註冊，才能檢視Workfront中的項目。 依預設，此選項會停用。 當您啟用此選項時，沒有Workfront帳戶的使用者若透過其電子郵件地址加入某些更新中，將會提示他們建立帳戶，然後才能檢視其所包含的項目。 這會為其建立外部使用者帳戶。</p> <p>預設會停用此選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">之後自動將使用者登出。</td> 
      <td> 可讓您指定使用者何時在閒置一段時間後登出Workfront。 依預設，使用者閒置8小時後即會登出。 <p>此選項也會影響使用單一登入解決方案的Workfront客戶。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">之後自動將行動使用者登出 </td> 
      <td>可讓您指定使用者何時在閒置一段時間後登出Workfront應用程式。 依預設，使用者在閒置7天後會登出。 <p>此選項也會影響使用單一登入解決方案的Workfront客戶。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。

   您在此儲存的變更會影響Workfront中所有使用者以及以外部使用者身分與他們互動的使用者體驗。
