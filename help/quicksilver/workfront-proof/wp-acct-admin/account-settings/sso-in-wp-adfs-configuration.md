---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: '''單一登入 [!DNL Workfront Proof]:AD FS配置'
description: 如果您是AD伺服器上的管理員，則可以安裝和配置AD FS。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# 單一登入 [!DNL Workfront Proof]:AD FS配置

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

如果您是AD伺服器上的管理員，則可以安裝和配置AD FS。

## 安裝和配置AD FS

1. 下載 [AD FS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) 到電腦。
1. 開啟下載的AdfsSetup.exe檔案以啟動ADFS（Active Directory聯合身份驗證服務）安裝嚮導。
1. 在「伺服器角色」螢幕上，選擇其中一個選項（至少需要聯合伺服器）。
1. 如果您不想將AD伺服器上的IIS公開到Internet（HTTP和HTTPS的埠80和443），可以先在防火牆後設定聯合伺服器，然後建立第二個聯合伺服器代理，該代理將請求通過防火牆傳遞到聯合伺服器。
1. 完成AD FS設定後，請選擇 **[!UICONTROL 啟動AD FS 2.0管理管理單元]**，然後按一下 **[!UICONTROL 完成]**. 完成此操作後，應立即開啟AD FS 2.0管理窗口。 否則，您可從 **[!UICONTROL 開始]** > **[!UICONTROL 管理工具]** > **[!UICONTROL AD FS 2.0管理]**. 這是主要的AD FS控制應用程式。

1. 首先，按一下AD FS 2.0聯合伺服器配置嚮導。
這將幫助您配置AD FS，並通過IIS和AD將其連接到Internet。
1. 如果要配置新的AD FS伺服器，請選擇 **[!UICONTROL 建立新的聯合身份驗證服務]**.
1. 選擇 **[!UICONTROL 獨立聯合伺服器]** （用於測試和評估用途）。

1. 要獲得高可用性和負載平衡，請按一下「新建聯合伺服器場」。
1. 指定您的聯合身份驗證服務名稱。
預設情況下，配置嚮導將檢索綁定到IIS中預設網站的SSL證書，並將使用該處指定的主題名稱。 如果使用通配符證書，則需要輸入聯合身份驗證服務名稱。
如果IIS中未配置SSL證書，則配置嚮導將在本地電腦證書儲存中搜索任何有效證書。 這些資訊會顯示在SSL憑證下拉式清單中。 如果找不到證書，則可以使用IIS中的伺服器證書生成器來建立證書生成器。

1. 繼續進行設定，然後按一下 **[!UICONTROL 關閉]** 完成後。

## 設定 [!DNL Workfront Proof] 單一登入

如果您是 [!DNL Workfront Proof] 管理員，您可以在 [!DNL Workfront Proof] 側。 如需詳細資訊，請參閱 [單一登入 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. 按一下 **[!UICONTROL 設定]** > **[!UICONTROL 帳戶設定]**，然後開啟 **[!UICONTROL 單一登入]** 標籤。

1. 在 **SSO URL** ，然後貼上實體ID。
以下是實體ID的範例：http://*&lt;adfs.your-company.com>*/adfs/services/trust您的實體ID可在聯合元資料XML檔案中找到。
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. 在AD FS 2.0管理單元>服務>端點資料夾中找到聯合元資料。 在「元資料」部分，找到具有「聯合元資料」類型的元資料。 若要檢視中繼資料，請將此端點貼到您的瀏覽器中。 您也可以直接前往此連結：https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml。
1. 在 **[!UICONTROL 登入URL]** 框中，貼上SSO登錄名。
1. 以下是SSO登入的範例：
1. http://*&lt;adfs.your-company.com>*/adfs/ls。
1. 此連結可以位於聯合元資料XML檔案中。
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. 在 **[!UICONTROL 註銷URL]** 框中，輸入連結並保存。
以下是登出URL的範例：https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. 轉到您的AD FS管理員>信任關係>信賴方信任 — ProofHQ屬性。
   1. 在「端點」下，按一下 [!UICONTROL 新增和登入] 以及下列詳細資料：

      * 端點類型= SAML註銷
      * 綁定=POST
      * URL = https://*&lt;adfs.your-company.com span=&quot;&quot; id=&quot;1&quot; translate=&quot;no&quot; />>/adfs/ls/?wa=wsignout1.0*
      * 在AD FS中配置信賴方信任後（請參見下面）可完成此步驟。
   1. 在 **[!UICONTROL 證書指紋]** 框中，輸入證書中的資料。
   1. 前往ADFS 2.0管理單元，導覽至「服務>憑證>代號簽署」。
   1. 以滑鼠右鍵按一下此項目以檢視憑證。
   1. 從 [!UICONTROL 證書詳細資訊] 頁簽複製指紋，然後貼到 **[!UICONTROL Workfront校樣單一登入]** 設定標籤。

   1. 指紋字元可以用冒號或空格分隔，但建議您移除這些字元。 如果您的單一登入配置有任何問題，請聯繫客戶支援團隊。


## 添加信賴方信任

配置完成後，您需要在AD FS的「信賴方信任」部分中工作。

1. 導覽至 **[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信託]** ，然後按一下 **[!UICONTROL 添加信賴方信任]** 啟動配置嚮導。

1. 選取您的資料來源。
您 [!DNL ProofHQ] 帳戶位於連結下，如下所示：https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq這將配置大多數信賴方信任。

   >[!NOTE]
   >
   >* 如果您在從URL建立連線時遇到任何問題，請將中繼資料儲存為檔案，然後選擇從檔案匯入資料。
   >* 當您的 [!DNL ProofHQ] 帳戶會將整個「{yoursubdomain}.proofhq.com」部分替換為您自己的網域，以建立您的 [!DNL ProofHQ] 中繼資料連結。



## 配置聲明規則

完成信賴方信任配置後，您就可以配置聲明規則以完成設定。 您將為ProofHQ配置兩個聲明規則：電子郵件和名稱ID。

1. 開啟 **[!UICONTROL 編輯聲明規則]** 對話框。
1. 前往 **[!UICONTROL ProofHQ信賴方信任]**，然後按一下 **[!UICONTROL 編輯聲明規則]** (1)。\
   如果您在設定信任結束時選取了此選項，則快顯視窗會自動開啟。

1. 按一下 **[!UICONTROL 新增規則]** （二）開啟理賠配置窗口。

   * 電子郵件（以聲明規則模板發送LDAP屬性）
   * NameID（轉換傳入的聲明規則模板）
