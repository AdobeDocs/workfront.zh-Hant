---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: 準備將貴組織上線至Adobe Admin Console
description: 由於Adobe Workfront是Adobe產品，因此您可以透過Adobe Admin Console存取。 這可讓您在集中位置管理Workfront，以及其他Adobe帳戶和產品給使用者。
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# 準備將貴組織上線至Adobe Admin Console

由於Adobe Workfront是Adobe產品，因此您可以透過Adobe Admin Console存取。 這可讓您在集中位置管理Workfront，以及其他Adobe帳戶和產品給使用者。

所有Workfront客戶最終都會移至Adobe Admin Console。 您的組織移至Adobe Admin Console後，Workfront驗證便由Adobe Admin Console管理。 更快地準備並實施此項操作為工作管理的效率奠定了基礎，並為貴組織定位，以便在將來更快地進行創新

如需Adobe Admin Console的概觀，請參閱 [Admin Console概述](https://helpx.adobe.com/tw/enterprise/using/admin-console.html).

## 移轉檢查清單

若要確保貴組織可移轉至Adobe Admin Console，您必須執行下列動作

1. 識別您要新增Workfront的Adobe Admin Console。

   * 如果貴組織沒有現有Adobe Admin Console，或您不想使用現有Adobe Admin Console,Workfront支援可協助您建立新的。

   * 如果您有多個AdobeAdmin Console，且不確定哪個最適合將Adobe Workfront新增至，請聯絡Workfront支援。

1. 向Workfront支援確認您要使用現有的Adobe Admin Console，或建立新的。

1. 在Adobe Admin Console上設定身分管理。

   >[!IMPORTANT]
   >
   >準備好就驗證偏好設定(例如單一登入(SSO)或非SSO)與Workfront支援和您的IT團隊溝通。

   如需指示，請參閱Adobe Admin Console部署指南(https://helpx.adobe.com/enterprise/using/deployment-planning.html)中的Identity Management一節。

1. （條件性）如果使用單一登入，請將新Adobe Admin Console連線至您現有的SSO提供者

   如需詳細資訊和指示，請參閱 [設定身分](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >如果您的組織未使用單一登入，任何移轉至Adobe Admin Console的使用者都會收到電子郵件，要求您建立其帳戶和密碼。

1. 確保用戶電子郵件地址已準備好進行遷移：

   1. 從Workfront移除重複的電子郵件

      如需指示，請參閱防止重複使用者中的更新Workfront例項中現有使用者的電子郵件地址。

      如果貴組織中有重複的電子郵件地址，則使用者會以最近的 `lastLoginDate` 將移至Adobe Admin Console組織。 具有該電子郵件地址的任何其他使用者都將停用。

      >[!NOTE]
      >
      >由於指定時間只能有一個具有指定電子郵件地址的使用者處於作用中狀態，如果您需要啟用另一個具有與目前作用中使用者相同電子郵件地址的使用者，您必須先停用目前作用中的使用者，才能啟用停用中的使用者。

   2. （視條件而定）如果您使用自訂API整合，請確認這些使用者擁有他們可存取的有效電子郵件地址。

   3. （選用）建議停用不再需要存取Workfront的使用者，因此不會將他們新增至Adobe Admin Console。
   >[!IMPORTANT]
   >
   >您的組織開始前往Adobe Admin Console之前，必須先完成有關使用者電子郵件的這些動作。

1. （選用）更新所有自訂整合以使用OAuth2。

   如需設定OAuth2整合的指示，請參閱 [建立OAuth2應用程式以進行Workfront整合](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   建立OAuth2整合僅適用於新的Workfront體驗。

   >[!NOTE]
   >
   >此步驟為選用，但強烈建議使用，因為未來將會淘汰其他形式的API驗證和授權。

使用Workfront設定Adobe Admin Console後，您就可以使用它管理使用者。

如需詳細資訊，請參閱 [在Adobe Admin Console中管理使用者](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

如需其他動作的清單(根據貴組織是否已上線至Adobe Admin Console而有所不同)，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
