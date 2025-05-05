---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: ' [!DNL Workfront Proof]中的單一登入： AD FS組態'
description: 如果您是AD伺服器的管理員，則可以安裝和設定AD FS。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: 690b0817dfe4ff200982ffe8d67ad93e563e30ac
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# [!DNL Workfront Proof]中的單一登入： AD FS設定

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

如果您是AD伺服器的管理員，則可以安裝和設定AD FS。

## 安裝和設定AD FS

1. 將Microsoft AD FS 2.0下載至您的電腦。
1. 開啟下載的AdfsSetup.exe檔案，以啟動ADFS (Active Directory Federation Services)安裝精靈。
1. 在[Server Role]畫面上，選取其中一個選項（您至少需要一個Federation Server）。
1. 如果您不想將AD伺服器上的IIS公開至網際網路（HTTP和HTTPS的連線埠80和443），您可以先在防火牆後面設定同盟伺服器，然後建立第二個同盟伺服器Proxy，透過防火牆將請求傳送至同盟伺服器。
1. 完成AD FS安裝之後，請選取&#x200B;**[!UICONTROL 啟動AD FS 2.0管理嵌入式管理單元]**，然後按一下&#x200B;**[!UICONTROL 完成]**。 完成此操作後，「AD FS 2.0管理」視窗應立即開啟。 如果沒有，您可以從&#x200B;**[!UICONTROL 開始]** > **[!UICONTROL 管理工具]** > **[!UICONTROL AD FS 2.0管理]**&#x200B;開啟它。 這是主要的AD FS控制應用程式。

1. 按一下AD FS 2.0 Federation Server組態精靈開始。
這可協助您設定AD FS，並透過IIS和AD將其連線至網際網路。
1. 如果您正在設定新的AD FS伺服器，請選取&#x200B;**[!UICONTROL 建立新的Federation Service]**。
1. 選取&#x200B;**[!UICONTROL 獨立同盟伺服器]** （用於測試和評估目的）。

1. 若要取得高可用性與負載平衡，請按一下[新增同盟伺服器陣列]。
1. 指定您的Federation服務名稱。
依預設，設定精靈會擷取繫結至IIS中預設網站的SSL憑證，並將使用那裡指定的主體名稱。 如果您使用萬用字元憑證，則需要輸入Federation Service名稱。
如果IIS中未設定SSL憑證，則設定精靈會在本機電腦憑證存放區中搜尋任何有效的憑證。 這些引數會顯示在SSL憑證下拉式清單中。 如果沒有找到憑證，您可以使用IIS中的伺服器憑證產生器來建立憑證。

1. 繼續進行組態，完成後按一下[關閉]。**&#x200B;**

## 正在設定[!DNL Workfront Proof]單一登入

如果您是[!DNL Workfront Proof]管理員，可以在[!DNL Workfront Proof]端設定單一登入。 如需詳細資訊，請參閱[單一登入 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md)。

1. 按一下&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 帳戶設定]**，然後開啟&#x200B;**[!UICONTROL 單一登入]**&#x200B;標籤。

1. 在&#x200B;**SSO URL**&#x200B;方塊中，貼上您的實體識別碼。
以下是實體ID的範例：
http://*&lt;adfs.your-company.com>*/adfs/services/trust
您可以在同盟中繼資料XML檔案中找到您的實體ID。
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. 同盟中繼資料位於AD FS 2.0嵌入式管理單元>服務>端點資料夾。 在中繼資料區段中，找出具有同盟中繼資料型別的中繼資料。 若要檢視中繼資料，請在瀏覽器中貼上此端點。 將{adfs.your-company.com}取代為您自己的詳細資料後，您也可以直接前往此連結： https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml。
1. 在&#x200B;**[!UICONTROL 登入URL]**&#x200B;方塊中，貼上您的SSO登入。
1. 以下是SSO登入的範例：
1. http://*&lt;adfs.your-company.com>*/adfs/ls。
1. 此連結可位於同盟中繼資料XML檔案中。
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. 在&#x200B;**[!UICONTROL 登出URL]**&#x200B;方塊中，輸入連結並儲存。
以下是登出URL的範例：
https://*&lt;adfs.your-company.com>*/adfs/ls/？wa=wsignout1.0

   1. 前往您的AD FS管理員>信任關係>信賴方信任 — ProofHQ屬性。
   1. 在[端點]底下，按一下[新增]和[專案] ，其詳細資訊如下：

      * 端點型別= SAML登出
      * 繫結= POST
      * URL = https://*&lt;adfs.your-company.com*>/adfs/ls/？wa=wsignout1.0
      * 在AD FS中設定信賴方信任（請參閱下文）後，即可完成此步驟。
   1. 在&#x200B;**[!UICONTROL 憑證指紋]**&#x200B;方塊中，輸入憑證中的資料。
   1. 前往您的ADFS 2.0嵌入式管理單元，導覽至「服務>憑證>權杖簽署」。
   1. 以滑鼠右鍵按一下此專案以檢視憑證。
   1. 從[!UICONTROL 憑證詳細資料]索引標籤複製指紋，並將其貼到&#x200B;**[!UICONTROL Workfront Proof單一登入]**&#x200B;設定索引標籤中。

   1. 指紋字元可以使用冒號或空格來分隔，但我們建議移除這些字元。 如果您的「單一登入」設定有任何問題，請聯絡客戶支援團隊。


## 新增信賴方信任

完成設定後，您需要在AD FS中的信賴方信任區段中進行工作。

1. 瀏覽至&#x200B;**[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信任]**&#x200B;資料夾，然後按一下&#x200B;**[!UICONTROL 新增信賴方信任]**&#x200B;以啟動設定精靈。

1. 選取您的資料來源。
您[!DNL ProofHQ]帳戶的所有中繼資料都位於如下連結下：
https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq
這將設定大部分信賴方信任。

   >[!NOTE]
   >
   >* 如果您從URL建立連線時遇到任何問題，請將中繼資料儲存為檔案，然後選擇從檔案匯入資料。
   >* 當您在您的[!DNL ProofHQ]帳戶上設定了完整的自訂網域(例如www.your-proofing.com)時，請將整個&quot;{yoursubdomain}.proofhq.com&quot;部分取代為您自己的網域，以建立您的[!DNL ProofHQ]中繼資料連結。


## 設定宣告規則

完成信賴方信任設定後，您就可以設定宣告規則以完成設定。 您將為ProofHQ設定兩個宣告規則：電子郵件和名稱ID。

1. 開啟&#x200B;**[!UICONTROL 編輯宣告規則]**&#x200B;對話方塊。
1. 移至&#x200B;**[!UICONTROL ProofHQ信賴方信任]**，然後按一下&#x200B;**[!UICONTROL 編輯宣告規則]** (1)。\
   如果您在設定信任結束時選取此選項，快顯視窗應該會自動開啟。

1. 按一下&#x200B;**[!UICONTROL 新增規則]** (2)以開啟宣告設定視窗。

   * 電子郵件（傳送LDAP屬性作為宣告規則範本）
   * NameID （轉換傳入宣告規則範本）
