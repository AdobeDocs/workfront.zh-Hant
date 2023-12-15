---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: 準備將您的組織加入Adobe Admin Console
description: 由於Adobe Workfront是Adobe產品，因此您可以透過Adobe Admin Console存取。 這可讓您集中管理Workfront，以及使用者的其他Adobe帳戶和產品。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# 準備將您的組織加入Adobe Admin Console

<!-- Audited: 12/2023 -->

由於Adobe Workfront是Adobe產品，因此您可以透過Adobe Admin Console存取。 這可讓您集中管理Workfront，以及使用者的其他Adobe帳戶和產品。

所有Workfront客戶最終都會移至Adobe Admin Console。 您的組織移至Adobe Admin Console後，Workfront驗證會由主控台管理。 為這項工作做好準備，並加快進度，為工作管理效率奠定基礎，並為貴組織未來更快創新做好準備

如需Adobe Admin Console的概要介紹，請參閱 [Admin Console概觀](https://helpx.adobe.com/tw/enterprise/using/admin-console.html).

## 移轉檢查清單

為確保您的組織可移轉至Adobe Admin Console，您必須執行下列動作。

1. 識別您要在其中新增Workfront的所需Adobe Admin Console。

   * 如果貴組織沒有現有的Adobe Admin Console，或您不想使用現有的Adobe Admin Console，Workfront支援可協助您建立新架構。

   * 如果您有多個AdobeAdmin Console，但不確定哪一個最適合新增Workfront，請聯絡Workfront支援。

1. 向Workfront支援確認您要使用現有的Adobe Admin Console，或建立一個新的系統。

1. 在Adobe Admin Console上設定身分管理。

   >[!IMPORTANT]
   >
   >請準備好與Workfront支援和您的IT團隊討論驗證偏好設定，例如單一登入(SSO)或非SSO。

   Identity Management如需操作說明，請參閱 [Adobe Admin Console的部署指南](https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. （視條件而定）如果使用單一登入，請將新的Adobe Admin Console連線至您現有的SSO提供者。

   如需詳細資訊與指示，請參閱 [設定身分](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >如果您的組織未使用單一登入，則任何移轉至Adobe Admin Console的使用者都會收到電子郵件，要求建立其帳戶和密碼。

1. 確保使用者電子郵件地址準備好進行移轉：

   1. 從Workfront移除重複的電子郵件。

      如需指示，請參閱 [更新Workfront執行個體中現有使用者的電子郵件地址](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) 在 [防止重複使用者](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).

      如果您的組織中存在重複的電子郵件地址，則以電子郵件地址表示的使用者具有最近的 `lastLoginDate` 將會移至Adobe Admin Console組織。 將停用使用該電子郵件地址的任何其他使用者。

      >[!NOTE]
      >
      >由於在指定時間只能有一個具有指定電子郵件地址的使用者處於作用中狀態，因此如果您需要啟用另一個與目前作用中使用者具有相同電子郵件地址的使用者，則必須先停用目前作用中的使用者，才能啟用該已停用的使用者。

   1. （視條件而定）如果您正在利用自訂API整合，請確認這些使用者擁有可以存取的有效電子郵件地址。

   1. （選用）我們建議停用不再需要存取Workfront的任何使用者，因此不會將他們新增至Adobe Admin Console。

   >[!IMPORTANT]
   >
   >有關使用者電子郵件的這些動作必須在您的組織開始移至Adobe Admin Console之前完成。

1. （選用）更新所有自訂整合以使用OAuth2。

   如需設定OAuth2整合的說明，請參閱 [為Workfront整合建立OAuth2應用程式](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   >[!NOTE]
   >
   >此步驟為選用步驟，但強烈建議使用，因為未來將不再使用其他形式的API驗證和授權。

在使用Workfront設定Adobe Admin Console後，您就可以用它來管理使用者。

如需詳細資訊，請參閱 [在Adobe Admin Console中管理使用者](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

如需根據貴組織是否已上線至Adobe Admin Console而有所不同的其他動作清單，請參閱 [平台型管理差異(Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
