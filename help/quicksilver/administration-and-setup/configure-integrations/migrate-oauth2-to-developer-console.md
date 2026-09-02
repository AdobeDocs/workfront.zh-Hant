---
title: 從Workfront OAuth2移轉至Adobe Developer Console
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Workfront的舊版自訂OAuth2應用程式服務即將淘汰。 瞭解變更內容、受影響者以及如何將自訂整合移轉至Adobe Developer Console。
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: db7e6a6fa0c5fc5332213c388d9b4db3a5c59f53
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 1%

---

# 從Workfront OAuth2移轉至Adobe Developer Console

Workfront的舊版自訂OAuth2應用程式服務（您在&#x200B;**設定** > **系統** > **OAuth2**&#x200B;下設定的整合）正在淘汰。 日後，所有針對Workfront驗證的自訂整合都必須改用Adobe Developer Console (developer.adobe.com)驗證流程。

此變更會影響任何自訂整合、指令碼或協力廠商工具，這些工具目前會使用Workfront發行的OAuth2使用者端ID和密碼進行驗證。 它不會影響您登入Workfront的方式，也不會影響Adobe管理的標準整合，例如封裝的Microsoft Teams或Slack整合（Adobe正在個別移轉）。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront存取層級設定</td> 
   <td><p>系統管理員</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Developer Console許可權</td> 
   <td><p>存取適用於Workfront的Adobe Developer Console需要完整IMS組織管理許可權。 此角色比Workfront產品管理員角色更廣泛，因為可管理整個Adobe組織及其下所有產品。</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## 關鍵日期

| 日期 | 里程碑 | 這對您有何意義 |
|---|---|---|
| 2026年11月1日 | 已停用新應用程式建立 | 您無法再在Workfront中建立新的自訂OAuth2應用程式。 現有應用程式可繼續運作。 |
| 2027年2月1日 | 舊版服務已淘汰 | 現有的自訂OAuth2應用程式會完全停止運作。 此時，任何尚未移轉至Adobe Developer Console的整合都會失去Workfront API的存取權。 |

>[!IMPORTANT]
>
>我們強烈建議您在2026年11月1日之前規劃並完成移轉，讓您的整合作業持續執行而不會中斷，這樣您就不會在2027年2月1日硬性期限之前進行移轉。

## 受影響的組織

如果您的組織有任何整合、指令碼或工具，會使用透過Workfront舊版OAuth2設定畫面核發的自訂OAuth2使用者端ID和密碼連線至Workfront，則會受到此變更的影響。 常見範例包括：

* 您的工程團隊會針對Workfront API維護的自訂整合功能。
* 協力廠商或合作夥伴建立的聯結器已設定為Workfront簽發的使用者端ID。 如果您不確定其整合的驗證方式，建議您洽詢供應商。
* 直接呼叫Workfront API的內部自動化、報告或資料同步指令碼。

如果您不知道貴組織是否有這些專案，您的Workfront管理員可以檢查&#x200B;**設定** > **系統** > **OAuth2**&#x200B;底下的OAuth2應用程式清單，以檢視目前登入的專案。 如需詳細資訊，請參閱[檢視及管理自訂OAuth2應用程式](/help/quicksilver/administration-and-setup/configure-integrations/manage-custom-oauth2-apps.md)。

## 瞭解Adobe Developer Console驗證型別

Adobe Developer Console支援多種驗證方式。 您可以選取符合整合運作方式的型別：

* **伺服器對伺服器驗證**：對於在您後端執行的應用程式，它會代表您的組織呼叫Adobe API，但未涉及一般使用者。 這是與使用使用者端ID和密碼的舊版Workfront OAuth2模式最相符的型別，也是大部分自訂Workfront整合、指令碼和自動化都應該使用的型別。
* **使用者驗證**：若是Adobe使用者需要登入並授與同意，應用程式才能檢視或編輯其資料的情況。 如果您的整合需要代表特定的已登入Workfront使用者（而非整個組織）採取行動，請改用此型別。

  如果您選擇「使用者驗證」，則根據您應用程式的架構，還有三個選項：

  * **OAuth網頁應用程式**：適用於具有前端UI和後端伺服器的應用程式。 伺服器會安全地儲存使用者端密碼並擷取權杖。
  * **OAuth單頁應用程式**：適用於沒有後端伺服器的僅限瀏覽器網頁應用程式。 網頁應用程式本身會擷取Token。
  * **OAuth原生應用程式**：適用於在裝置上原生執行而沒有後端伺服器的行動或案頭應用程式。 原生應用程式會擷取Token。

將後端整合、指令碼或自動化移出舊版OAuth2服務的組織大多想要伺服器對伺服器驗證。

## 功能比較：舊版OAuth2與Adobe Developer Console

舊版Workfront OAuth2服務（在&#x200B;**Setup** > **System** > **OAuth2應用程式**&#x200B;中植入）提供三種應用程式型別，每個Workfront執行個體最多可有10個OAuth2應用程式。 以下為這些方面與Adobe Developer Console的比較：

| 舊版Workfront型別 | 流量/驗證方法 | Developer Console對等函式 | 符合 |
|---|---|---|---|
| 機器對機器應用程式（CLI、精靈、後端指令碼） | 使用公開/私密金鑰組的JWT | 伺服器對伺服器驗證 | 相同的目的是不讓一般使用者參與，但機制會改變。 舊版流程使用公開/私密金鑰組和JWT，而伺服器對伺服器則使用使用者端ID和使用者端密碼，並授予OAuth使用者端憑證。 這不是插入式認證交換。 整合的驗證代碼需要變更，而不只是認證值。 如需詳細資訊，請參閱[使用自訂OAuth 2應用程式的JWT流程](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)。 |
| Web應用程式（伺服器端應用程式：Go、Java、.NET、節點、PHP） | OAuth 2.0授權代碼流程 | OAuth網頁應用程式（在「使用者驗證」下） | 最接近的1:1相符。 此路徑與後端伺服器儲存使用者端密碼的基本形狀相同，流程也相同。 如需詳細資訊，請參閱自訂OAuth 2應用程式的[授權代碼流程](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)。 |
| 單頁網頁應用程式(JS、Angular、React、Vue) | 授權代碼流程與PKCE，無使用者端密碼 | OAuth單頁應用程式（在「使用者驗證」下） | 最接近的1:1相符此項具有相同的PKCE式、無密碼流程。 如需詳細資訊，請參閱[使用OAuth 2應用程式的PKCE流程](/help/quicksilver/wf-api/api/oauth-app-pkce-flow.md)。 |
| （無舊版同等專案） | — | OAuth原生應用程式（在「使用者驗證」下） | 這是一項新功能。 舊版Workfront OAuth2沒有原生行動或案頭應用程式的專用型別。 |

<!--

>[!NOTE]
>
>A few legacy capabilities don't have a confirmed equivalent yet in Adobe Developer Console, and are being validated with the Developer Console team:
>
>* Per-app controls the legacy UI offers: refresh token rotation toggle, absolute vs. inactivity refresh token expiration, custom logo, privacy policy URL, and developer contact fields.
>* Whether Developer Console enforces a cap on credentials or projects similar to the legacy 10-app-per-instance limit.
>* Whether a JWT/key pair-based option remains available anywhere in Developer Console for Machine to Machine customers, or whether all such integrations must move to the client-secret-based Server-to-Server grant.

-->

## 移轉程式

### 如果您是Workfront系統管理員

>[!NOTE]
>
>如果您是Workfront產品管理員但不是組織管理員，則需與組織管理員合作以完成此移轉，或要求完成移轉。

1. 登入[developer.adobe.com](https://developer.adobe.com)並建立新專案。 專案是主控台組織不同整合或使用者端應用程式的方式。
1. 從專案新增API，然後選取&#x200B;**Adobe Workfront**。 此API位於Experience Cloud類別下。 所有Workfront API （包括規劃、工作流程以及檢閱和核准）都會共用此單一API。
1. 選取&#x200B;**伺服器對伺服器**&#x200B;驗證選項，然後如果您的IMS組織有一個以上的Workfront執行個體，請選擇正確的執行個體。

   如需選擇驗證型別的指南，請參閱本文中的[瞭解Adobe Developer Console驗證型別](#understand-adobe-developer-console-authentication-types)。
1. 在「專案」頁面上，開啟新OAuth伺服器對伺服器認證的詳細資料，以尋找您的使用者端ID、使用者端密碼和產生存取權杖所需的資訊。
1. 更新您的整合、指令碼或工具，以使用這些新憑證來驗證身分，取代舊的Workfront OAuth2使用者端ID和密碼。
1. 在Workfront中確認存取權。 建立API使用者端會自動將其新增為Workfront使用者&quot;`techacct`&quot;。 預設會將其新增為具有有限存取權的投稿人，但您可以像調整任何其他使用者的存取層級一樣調整其存取層級。
1. （選用）若要授予`techacct`使用者管理員許可權，請新增技術帳戶的電子郵件，作為Admin Console中相關產品設定檔的管理員。
1. 端對端測試整合。
1. 在您確認新連線正常運作後，請淘汰Workfront中的舊OAuth2應用程式專案。

如需完整的逐步詳細資訊和熒幕擷取畫面，請參閱Adobe的Developer Console檔案中的[取得存取權](https://developer.adobe.com/workfront-apis/guides/gaining_access/)。

### 如果您不是系統管理員

由於在Adobe Developer Console中設定新憑證需要該存取層級，因此您需要在貴組織的IMS組織管理員中執行回圈才能完成移轉。 如果您管理或維護整合，但清楚您組織的IMS組織管理員是誰，請聯絡下列其中一項：

* 您的Workfront客戶團隊
* 您的內部IT團隊
* 您的工程連絡人

## 如果您不移轉

在2027年2月1日之後，仍使用舊版OAuth2使用者端ID/密碼模式的整合服務無法針對Workfront API進行驗證，且任何相依的工作流程、同步或自動化都會失敗。 由於此日期尚未規劃任何擴充功能，因此請及早移轉您的整合。

## 常見問題

**這是否會影響Adobe提供的封裝整合，例如Slack或Microsoft Teams？**

否。 Adobe管理的全域應用程式正由Adobe直接移轉，不需要您採取任何動作。

**我現有的整合服務會在2027年2月1日之前停止運作嗎？**

否。 現有的自訂OAuth2應用程式可繼續正常運作至2027年2月1日。 自2026年11月1日起，只有建立新自訂OAuth2應用程式的功能會受到影響。

**移轉是否有成本？**

不需要，透過Adobe Developer Console驗證不會產生額外費用。

**我可以在哪裡取得協助？**

如果您對特定整合或時間表有任何疑問，請聯絡您的Workfront帳戶團隊或開啟支援案例。 如需使用熒幕擷取畫面進行正式的最新設定逐步解說，請參閱Adobe的Developer Console檔案中的[取得存取權](https://developer.adobe.com/workfront-apis/guides/gaining_access/)。
