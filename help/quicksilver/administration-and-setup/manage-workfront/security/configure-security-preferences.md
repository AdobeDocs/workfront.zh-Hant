---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 設定系統偏好設定
description: 身為Adobe Workfront管理員，您可以設定Workfront系統的偏好設定，包括安全性偏好設定。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 1b7964b533093c4eee20d69a74512a145e207e29
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 5%

---

# 設定系統偏好設定

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{important-admin-console-onboard}}

身為Adobe Workfront管理員，您可以設定Workfront系統的偏好設定，包括：

* 從行動應用程式和其他整合式應用程式存取Workfront
* 將Workfront內嵌至iframe的規則

您在系統偏好設定中進行的變更會影響系統中所有使用者，以及他們在Workfront中的體驗。

我們建議您在Workfront實作期間設定系統偏好設定，之後只需偶爾重新造訪一次。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p><p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定您的系統偏好設定

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**系統** > **偏好設定**。

1. 選取下列任一欄位來建立組織的設定：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>啟用快速發佈程序</p> </td> 
      <td>可讓您為貴組織啟用每月Workfront發行，而非每季發行。</p><p>如需快速發行程式的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">為您的組織啟用或停用快速發行</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>允許在iframe中內嵌Workfront</p> </td> 
      <td>可讓您將Workfront內嵌於iframe中。<p>此選項預設為停用。</p><p><b>重要</b>：在iframe中顯示Web應用程式，會使應用程式容易發生點選劫持安全性弱點。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Office 365 增益集允許 SAML 2.0 驗證</td> 
      <td> <p>當Workfront與SAML 2.0單一登入解決方案整合時，可讓您僅將Workfront內嵌在Office 365增益集適用的iframe中。 </p> <p>此選項預設為啟用。</p> <p><b>注意</b>：如果您啟用上述選項<strong>允許在iframe中內嵌Workfront</strong>，則選項<strong>允許Office 365增益集中的SAML 2.0驗證</strong>已啟用且變暗。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">啟用在建立外部頁面URL時使用工作階段資訊</td> 
      <td> <p>允許使用者在將外部頁面新增到儀表板時使用網站的工作階段ID資訊。</p> <p>此選項不安全，預設為關閉。 建議改用OAuth進行整合。</p> <p>如需將外部頁面新增至控制面板的詳細資訊，請參閱<a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">將外部網頁內嵌於控制面板</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">讓人們使用Workfront的行動應用程式和Workfront Outlook增益集</td> 
      <td> <p>允許使用者存取行動應用程式(適用於iPad和行動電話應用程式的Workfront View)和Workfront Outlook應用程式。</p> <p>此選項預設為啟用。 </p> <p>如需Workfront檢視的相關資訊，請參閱<a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">使用Adobe Workfront檢視</a>。 如需行動應用程式的詳細資訊，請參閱<a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">使用Adobe Workfront行動應用程式：文章索引</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>透過使用電子郵件地址與沒有Workfront帳戶的人共同作業</p> </td> 
      <td>可讓Workfront使用者透過包含電子郵件地址而非姓名來與沒有Workfront帳戶的人共用特定專案。 使用者可使用其電子郵件地址與外部使用者共用下列專案：
       <ul>
        <li>文件<br></li>
        <li>檔案請求<br></li>
        <li>檔案核准</li>
        <li>行事曆</li>
       </ul><p>此選項預設為啟用。</p> <p><b>重要</b>：如果停用此選項，您的Workfront執行個體將無法使用外部使用者存取層級。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">內建存取層級</a>。</p> </td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> -->
     <tr> 
      <td role="rowheader">說明 URL</td> 
      <td>可讓您定義主要功能表說明圖示要前往的內部自訂說明網站。 如需詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">設定自訂說明URL</a>。</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">啟用「優先順序」工作清單 </td> 
      <td>可讓您選擇為使用者啟用或停用優先順序工作清單體驗。 使用者仍可在Workfront中看到優先順序圖示，但無法存取該功能。 如需有關優先順序的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">開始使用優先順序</a>。</td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">啟用AI</span> </td> 
      <td><span class="preview">可讓您選擇啟用AI，包括AI助理。 <p><b>注意</b>：您的組織必須符合特定要求才能啟用AI。 如需AI的詳細資訊，包括需求，請參閱<a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">AI助理概述</a>。</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">表單自動完成 </span></td> 
      <td><span class="preview">可讓您選擇啟用根據先前的請求資料自動完成請求表單的功能。 如需表單自動完成的詳細資訊，請參閱<a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">從先前的資料自動填入要求</a>。</span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">選擇加入 AI Beta 版 </span></td> 
      <td><span class="preview">可讓您選擇啟用Beta中目前的AI功能。 如果啟用此選項，您可以接著選取要啟用哪些AI Beta功能。 如需每個AI Beta功能的詳細資訊，請按一下該功能旁的資訊圖示。</span></td> 
     </tr>
     <tr> 
      <td role="rowheader">測試環境</td> 
      <td>可讓您存取Workfront測試環境。 如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Adobe Workfront預覽沙箱環境</a>。</p></td> 
    </tbody> 
   </table>

1. 按一下「**儲存**」。

   您在此處儲存的變更會影響Workfront中所有使用者的體驗，以及任何以外部使用者身分與系統互動的使用者體驗。
