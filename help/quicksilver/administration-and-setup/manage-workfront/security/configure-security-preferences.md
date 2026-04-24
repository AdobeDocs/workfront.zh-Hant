---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configure System Preferences
description: As an Adobe Workfront administrator, you can configure preferences for your Workfront system, including security preferences.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 77b78c5905736092c972e08283fdabf321bfa580
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 7%

---

# 設定系統偏好設定

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

{{important-admin-console-onboard}}

As an Adobe Workfront administrator, you can configure preferences for your Workfront system, including:

* Access to Workfront from mobile apps and other integrated applications
* Rules for embedding Workfront in an iframe

Changes that you make in the system preferences impact all users in your system, and their experience in Workfront.

We recommend that you configure your system preferences during the Workfront implementation and only occasionally revisit them after that.

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
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

## Configure your system preferences

{{step-1-to-setup}}

1. In the left panel, click **System** > **Preferences**.

1. Select any of the following fields to establish the settings for your organization:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>啟用快速發佈程序</p> </td> 
      <td>Lets you enable monthly Workfront releases for your organization instead of quarterly releases.</p><p>For more information about the fast release process, see <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">Enable or disable fast releases for your organization</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Allow embedding of Workfront in an iframe</p> </td> 
      <td>Lets you embed Workfront in an iframe.<p>此選項預設為停用。</p><p><b>IMPORTANT</b>: Displaying a web-based application in an iframe makes the application susceptible to a click-jacking security vulnerability.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Office 365 增益集允許 SAML 2.0 驗證</td> 
      <td> <p>Lets you embed Workfront in an iframe only for Office 365 add-ins when Workfront is integrated with a SAML 2.0 single sign-on solution. </p> <p>This option is enabled by default.</p> <p><b>NOTE</b>:  If you enable the option above, <strong>Allow embedding of Workfront in an iframe</strong>, the option <strong>Allow SAML 2.0 authentication in Office 365 add-ins</strong> is enabled and dimmed.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enable the use of session information when creating External Page URLs</td> 
      <td> <p>Allows users to use the Session ID information of a site when adding an External Page to a Dashboard.</p> <p>This option is insecure and off by default. 建議改用OAuth進行整合。</p> <p>如需將外部頁面新增至控制面板的詳細資訊，請參閱<a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">將外部網頁內嵌於控制面板</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">讓人們使用Workfront的行動應用程式</td> 
      <td> <p>允許使用者存取行動應用程式（適用於iPad和行動電話應用程式的Workfront檢視）</p> <p>此選項預設為啟用。 </p> <p>如需Workfront檢視的相關資訊，請參閱<a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">使用Adobe Workfront檢視</a>。 如需行動應用程式的詳細資訊，請參閱<a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">使用Adobe Workfront行動應用程式：文章索引</a>。</p> </td> 
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
     <!--
     <tr> 
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
     </tr>
     -->
     <tr> 
      <td role="rowheader">說明 URL</td> 
      <td>可讓您定義主要功能表說明圖示要前往的內部自訂說明網站。 如需詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">設定自訂說明URL</a>。</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">啟用「優先順序」工作清單 </td> 
      <td>可讓您選擇為使用者啟用或停用優先順序工作清單體驗。 使用者仍可在Workfront中看到優先順序圖示，但無法存取該功能。 如需有關優先順序的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">開始使用優先順序</a>。</td> 
     </tr>
      <tr> 
      <td role="rowheader">啟用Adobe企業儲存空間 </td> 
      <td>可讓您選擇為整個組織或特定群組啟用或停用Adobe企業儲存空間。 如需Adobe企業儲存空間的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md">為您的組織啟用Adobe企業儲存空間</a>。</td> 
     </tr>
     <tr> 
      <td role="rowheader">啟用 AI </td> 
      <td>可讓您選擇啟用AI，包括AI助理。 <p><b>注意</b>：您的組織必須符合特定要求才能啟用AI。 如需AI的詳細資訊，包括需求，請參閱<a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">AI助理概述</a>。</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">表單自動完成 </td> 
      <td>可讓您選擇啟用根據先前的請求資料自動完成請求表單的功能。 如需表單自動完成的詳細資訊，請參閱<a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">從先前的資料自動填入要求</a>。</td> 
     </tr>
     <tr> 
      <td role="rowheader">選擇加入 AI Beta 版 </td> 
      <td>&gt;可讓您選擇啟用Beta中的目前AI功能。 如果啟用此選項，您可以接著選取要啟用哪些AI Beta功能。 如需每個AI Beta功能的詳細資訊，請按一下該功能旁的資訊圖示。</td> 
     </tr>
     <tr> 
      <td role="rowheader">測試環境</td> 
      <td>可讓您存取Workfront測試環境。 如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Adobe Workfront預覽沙箱環境</a>。</p></td> 
    </tbody> 
   </table>

1. 按一下「**儲存**」。

   您在此處儲存的變更會影響Workfront中所有使用者的體驗，以及任何以外部使用者身分與系統互動的使用者體驗。
