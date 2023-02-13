---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: 使用SAML 2.0設定Adobe Workfront
description: 身為Adobe Workfront管理員，您可以設定Workfront網頁和行動應用程式，以整合單一登入(SSO)的安全斷言標籤語言(SAML)2.0解決方案。
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 7%

---

# 使用SAML 2.0設定Adobe Workfront

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

{{important-admin-console-onboard}}

身為Adobe Workfront管理員，您可以設定Workfront網頁和行動應用程式，以整合單一登入(SSO)的安全斷言標籤語言(SAML)2.0解決方案。

在Workfront中設定SAML 2.0後（如下節所述），您可以依照 [在您的身分提供者中更新SAML 2.0中繼資料](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

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

## 使用SAML 2.0啟用Workfront驗證

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** > **單一登入(SSO)。**

1. 在 **類型** 下拉式清單，按一下 **SAML 2.0。**

1. 在顯示的選項頂端附近，按一下 **下載SAML 2.0中繼資料** 下載電腦上的檔案。

   您的SAML 2.0身分提供者需要XML檔案，且其中包含在您的Workfront執行個體中產生的資訊。 下載檔案後，您需前往SAML 2.0身分提供者伺服器，並在該處上傳Workfront SAML 2.0中繼資料XML檔案。

1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">服務提供者 ID </td> 
      <td> 此URL已填入您，會將Workfront識別給您的身分提供者。 例如： <code>&lt;yourcompany&gt;.com/SAML2</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">繫結類型</span> </td> 
      <td> <p>選取IDP伺服器支援的傳送驗證資訊的方法：</p> 
       <ul> 
        <li>張貼</li> 
        <li>重新導向</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">從身份提供者中繼資料填入欄位 </td> 
      <td>在您的SAML 2.0身分提供者解決方案中，匯出服務提供者中繼資料XML檔案，並將其儲存至電腦上的暫存位置。 選擇 <strong>選擇檔案</strong>，然後尋找並選取您儲存的檔案，以將其新增至您的Workfront設定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">登入入口網站 URL</span> </td> 
      <td>指定貴組織的通用登入入口網站。 這是使用者登入以存取Workfront和與SAML 2.0整合的所有其他應用程式的URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">登出 URL</span> </td> 
      <td> <p>指定IDP伺服器的登出URL。 Workfront在登出Workfront之前會傳送HTTP要求至此URL。 這會在Workfront工作階段關閉時，關閉遠端伺服器上的使用者工作階段。</p> <p><b>注意</b>:只有在使用者設定檔中啟用「僅允許SAML 2.0驗證」選項時，系統才會將您重新導向至登出URL。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">變更密碼 URL </td> 
      <td> <p> 指定URL，系統會將使用者重新導向以變更其密碼。 </p> <p>由於SAML 2.0認證是用來存取Workfront，因此系統需要將使用者重新導向至頁面，讓使用者可以變更其SAML 2.0密碼，而非透過Workfront完成此活動。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">安全雜湊演算法 </td> 
      <td> <p>選取您的IDP支援的安全雜湊演算法(SHA):</p> 
       <ul> 
        <li>SHA-1</li> 
        <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自動提供使用者</span> </td> 
      <td> <p>當使用目錄使用者名稱和密碼的新使用者首次嘗試登入Workfront時，系統會自動建立使用者。</p> <p>若要在Workfront中建立使用者，您需要將Workfront資料屬性與目錄提供者中的下列使用者資料屬性對應：</p> 
       <ul> 
        <li>名字</li> 
        <li>姓氏</li> 
        <li>電子郵件位址</li> 
       </ul> 
       <p>下列選項可讓您執行此操作：</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>從下拉式清單中選取您要對應的Workfront使用者屬性，然後在使用者目錄中指定對應的目錄屬性。</p> 
       <p>此 <strong>目錄屬性</strong> 欄位應包含您在成功測試SAML 2.0設定時，所儲存之「使用者屬性」表格的「目錄屬性名稱」。</p> 
       <p>您可以在 <strong>預設值</strong> 欄位。 您也可以根據SAML 2.0身分提供者的值來設定規則。</p> 
       <p><b>警告</b>:Workfront會在使用者每次登入系統時，嘗試對應下列屬性。 因此，我們不建議對應存取層級。 如果屬性映射不正確，您可以輕鬆刪除管理訪問。 按一下「新增對應」以新增其他規則。
       </p> 
       <p>您可以對應下列Workfront屬性：</p> 
      <ul> 
      <li> <p>存取層級</p> </li> 
      <li> <p>地址</p> </li> 
      <li> <p>地址 2</p> </li> 
      <li> <p>記帳/小時</p> </li> 
      <li> <p>城市</p> </li> 
      <li> <p>公司</p> </li> 
      <li> <p>成本/小時</p> </li> 
      <li> <p>電子郵件位址</p> </li> 
      <li> <p>分機</p> </li> 
      <li> <p>名字</p> </li> 
      <li> <p>主群組</p> </li> 
      <li> <p>主團隊</p> </li> 
      <li> <p>職務角色</p> </li> 
      <li> <p>姓氏</p> </li> 
      <li> <p>配置範本</p> </li> 
      <li> <p>經理</p> </li> 
      <li> <p>行動電話</p> </li> 
      <li> <p>電話號碼</p> </li> 
      <li> <p>郵遞區號</p> </li> 
      <li> <p>排程</p> </li> 
      <li> <p>狀況</p> </li> 
      <li> <p>時間表設定檔</p> </li> 
      <li> <p>標題</p> </li> 
      </ul> </td> 
          <td> </td> 
         </tr> 
        </tbody> 
        <p>按一下 <strong>儲存</strong> 完成對應用戶屬性時。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">憑證 </td> 
      <td> <p>上傳有效的SSL憑證，以確保驗證服務與Workfront之間有安全的連線。 對於OnDemand帳戶，始終需要證書。 您可以向SAML 2.0系統管理員取得此憑證。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理豁免 </td> 
      <td> <p>可讓Workfront管理員使用其Workfront登入存取Workfront。 如果未選取此選項，Workfront管理員必須使用其SAML 2.0使用者名稱和密碼。</p> 
      <p>Workfront會先嘗試透過SAML 2.0，為具有Workfront系統管理員存取層級的使用者登入Workfront。 如果SAML 2.0驗證失敗，Workfront會為Workfront管理員使用本機驗證。</p> 
      <p>建議您一律選取此選項，以便在您的SAML 2.0提供者暫時無法使用時，您的Workfront管理員可登入Workfront。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">啟用 </td> 
      <td> <p>在Workfront系統上啟用SSO。 請確定您已將登入指示傳送給使用者。</p> <p>在Workfront中啟用SSO設定後，您必須啟用 <strong>僅允許SAML 2.0驗證</strong> 為所有使用者設定，以便他們能使用SSO。</p> <p>如需更新SSO使用者的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">更新單一登入的使用者</a>.</p> <p>如需使用者設定的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">確認設定 </td> 
      <td> 
      <p>按一下 <strong>測試連線</strong> 驗證Workfront和SAML 2.0身分提供者可以彼此通訊。 只有在交換XML檔案時，此連接才成功。
      </p> 
      <p>成功測試SAML 2.0身分提供者與Workfront之間的連結後，您會看到類似下方的畫面。</p>
      <p><b>注意</b>:此畫面會顯示在瀏覽器快顯視窗中，因此請務必停用瀏覽器中的快顯封鎖程式。</p>
      <p>儲存表格中顯示的資訊以供稍後使用。</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **儲存** 儲存SAML 2.0設定。
