---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: 使用SAML 2.0設定Adobe Workfront
description: 身為Adobe Workfront管理員，您可以設定Workfront網頁和行動應用程式，以整合單一登入(SSO)的安全宣告標籤語言(SAML) 2.0解決方案。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '1011'
ht-degree: 7%

---

# 使用SAML 2.0設定Adobe Workfront

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

<!-- Audited: 12/2023 -->

{{important-admin-console-onboard}}

身為Adobe Workfront管理員，您可以設定Workfront網頁和行動應用程式，以整合單一登入(SSO)的安全宣告標籤語言(SAML) 2.0解決方案。

在Workfront中設定SAML 2.0後（如以下區段所述），您可以維持設定（如所述） [更新身分提供者中的SAML 2.0中繼資料](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

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
   <td><p>新增：標準 </p>
       <p>或</p> 
       <p>目前：計畫 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 啟用使用SAML 2.0對Workfront的驗證

{{step-1-to-setup}}

1. 按一下 **系統** > **單一登入(SSO)。**

1. 在 **型別** 下拉式清單，選取 **SAML 2.0。**

1. 在顯示的選項頂端附近，按一下 **下載SAML 2.0中繼資料** 將檔案下載到電腦上。

   您的SAML 2.0身分提供者需要XML檔案，其中包含在Workfront執行個體中產生的資訊。 下載檔案後，您必須存取您的SAML 2.0 Identity Provider伺服器，並在該處上傳Workfront SAML 2.0 Metadata XML檔案。

1. 在Workfront中指定下列資訊：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">服務提供者 ID </td>
      <td> 此URL已為您填入，可將Workfront識別給您的身分提供者。 例如： <code>&lt;yourcompany&gt;.com/SAML2</code>.</td>
     </tr>
     <tr>
      <td role="rowheader">繫結型別</span> </td>
      <td> <p>選取您的IDP伺服器支援用來傳送驗證資訊的方法：</p>
       <ul>
       <li>張貼</li>
       <li>重新導向</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">從身份提供者中繼資料填入欄位 </td> 
      <td>在您的SAML 2.0 Identity Provider解決方案中，匯出Service Provider中繼資料XML檔案，並將其儲存到您電腦上的暫存位置。 選取 <strong>選擇檔案</strong>，然後尋找並選取您儲存的檔案，以將其新增至您的Workfront設定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">登入入口網站URL</span> </td> 
      <td>輸入您組織的通用登入入口網站。 這是使用者登入以存取Workfront和與SAML 2.0整合的所有其他應用程式的URL。</td> 
     </tr>
     <tr>
      <td role="rowheader">登出URL</span> </td> 
      <td> <p>輸入IDP伺服器的登出URL。 Workfront會在登出Workfront之前傳送HTTP要求至此URL。 當Workfront工作階段關閉時，這會關閉遠端伺服器上的使用者工作階段。</p> <p><b>注意</b>：只有在您有選項的情況下，系統才會將您重新導向至登出URL <strong>僅允許SAML 2.0驗證</strong> 已在您的使用者設定檔中啟用。</p> </td>
     </tr>
     <tr>
      <td role="rowheader">變更密碼 URL </td> 
      <td> <p> 指定要重新導向使用者以變更其密碼的URL。 </p> <p>由於SAML 2.0認證是用來存取Workfront，因此必須將使用者重新導向至可以變更其SAML 2.0密碼的頁面，而非透過Workfront完成此活動。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">安全雜湊演算法 </td> 
      <td> <p>選取IDP支援的安全雜湊演演算法(SHA)：</p> 
       <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自動布建使用者</span> </td> 
      <td> <p>當具有目錄使用者名稱和密碼的新使用者嘗試首次登入Workfront時，此選項會自動在系統中建立使用者。</p> <p>若要在Workfront中建立使用者，您必須將Workfront資料屬性與目錄提供者中的下列使用者資料屬性對應：</p> 
       <ul> 
       <li>名字</li> 
       <li>姓氏</li> 
       <li>電子郵件地址</li> 
       </ul> 
       <p>當您選取核取方塊時，會顯示下列選項：</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>從下拉式清單中選取您要對應的Workfront使用者屬性，然後在使用者目錄中指定對應的目錄屬性。</p> 
       <p>此 <strong>目錄屬性</strong> 欄位應包含您成功測試SAML 2.0組態時儲存之「使用者屬性」表格中的「目錄屬性名稱」。</p> 
       <p>您可以在「 」中設定預設Workfront值 <strong>預設值</strong> 欄位。 您也可以根據SAML 2.0身分提供者的值來設定規則。</p> 
       <p><b>警告</b>：每次使用者登入系統時，Workfront都會嘗試對應下列屬性。 因此，我們不建議對應存取層級。 如果屬性對應不正確，您可以輕鬆移除管理存取權。 按一下 <strong>新增對應</strong> 以新增其他規則。
       </p> 
       <p>您可以對應下列Workfront屬性：</p> 
      <ul> 
      <li> <p>存取層級</p> </li> 
      <li> <p>地址</p> </li> 
      <li> <p>地址 2</p> </li> 
      <li> <p>每小時計費</p> </li> 
      <li> <p>城市</p> </li> 
      <li> <p>公司</p> </li> 
      <li> <p>每小時成本</p> </li> 
      <li> <p>電子郵件地址</p> </li> 
      <li> <p>分機</p> </li> 
      <li> <p>名字</p> </li> 
      <li> <p>主群組</p> </li> 
      <li> <p>主團隊</p> </li> 
      <li> <p>職務角色</p> </li> 
      <li> <p>姓氏</p> </li> 
      <li> <p>版面配置範本</p> </li> 
      <li> <p>經理</p> </li> 
      <li> <p>行動電話</p> </li> 
      <li> <p>電話號碼</p> </li> 
      <li> <p>郵遞區號</p> </li> 
      <li> <p>排程</p> </li> 
      <li> <p>州/省</p> </li> 
      <li> <p>時程表設定檔</p> </li> 
      <li> <p>標題</p> </li> 
      </ul>
      <p>按一下 <strong>儲存</strong> 完成對應使用者屬性時。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">憑證 </td> 
      <td> <p>上傳有效的SSL憑證，以確保驗證服務與Workfront之間的安全連線。 對於OnDemand帳戶，一律需要憑證。 您可以向SAML 2.0系統管理員取得此憑證。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理豁免 </td> 
      <td> <p>可讓Workfront管理員使用其Workfront登入資料存取Workfront。 如果未選取此選項，Workfront管理員必須使用其SAML 2.0使用者名稱和密碼。</p> 
      <p>Workfront會先嘗試透過SAML 2.0為具有Workfront系統管理員存取層級的使用者登入Workfront。 如果SAML 2.0驗證失敗，Workfront會為Workfront管理員使用本機驗證。</p> 
      <p>如果您的SAML 2.0提供者暫時無法使用，建議您一律選取此選項，以便讓Workfront管理員可以登入Workfront。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">啟用 </td> 
      <td> <p>在Workfront系統上啟用SSO。 確定您已向使用者傳達登入指示。</p> <p>在Workfront中啟用SSO設定後，您必須啟用 <strong>僅允許SAML 2.0驗證</strong> 為所有使用者進行設定，以便他們可以使用SSO。</p> <p>如需更新SSO使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">更新單一登入的使用者</a>.</p> <p>如需使用者設定的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者設定檔</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">確認設定 </td> 
      <td> 
      <p>按一下 <strong>測試連線</strong> 確認Workfront和SAML 2.0身分提供者可互相通訊。 只有當您交換XML檔案時，此連線才會成功。
      </p> 
      <p>成功測試SAML 2.0身分提供者與Workfront之間的連結後，您會看到類似下圖的畫面。</p>
      <p><b>注意</b>：此畫面會以瀏覽器快顯視窗顯示，因此請務必停用瀏覽器中的快顯封鎖程式。</p>
      <p>儲存表格中顯示的資訊以供稍後使用。</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **儲存** 儲存SAML 2.0設定。
