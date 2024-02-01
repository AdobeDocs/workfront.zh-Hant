---
user-type: Admin
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: 瞭解Workfront移轉至Adobe Admin Console
description: 瞭解Workfront產品和使用者移轉至Adobe Admin Console
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 54d855e6-c387-458c-9cd3-f32318c8ae02
source-git-commit: 99b94c246f14110e37b23c95a178efd5b9042a9d
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# 瞭解Workfront移轉至Adobe Admin Console

Adobe正在改變您管理Adobe Workfront使用者的方式，為您和您的組織帶來更高的生產力。 作為此變更的一部分，Adobe正在將您的Workfront執行個體和使用者移轉至Adobe Admin Console。 這是必要的移轉，不會影響任何報告、核准路徑、內容或資產。 它會影響您管理使用者存取許可權的方式以及使用者登入的方式。

若要瞭解如何使用Adobe Admin Console來管理整個組織的Adobe權益，請參閱 [在Adobe Admin Console中管理使用者](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

## 有什麼改變？

移轉過程中，您的使用者管理將從Workfront應用程式內移至Adobe Admin Console，並具備下列管理角色：

* **系統管理員** 是擁有所有管理員許可權的超級使用者。 他們可指派所有管理角色，並管理整個組織所有產品的使用者。

* **產品設定檔管理員(Workfront系統管理員)** 管理組織中的哪些使用者可存取Workfront。

* **使用者將使用Adobe身分登入。** Adobe將現有使用者移轉至Adobe Admin Console後，使用者將使用其新的Adobe身分識別(Adobe ID或AdobeFederated ID(SSO))登入其Workfront執行個體。

* **您管理所有其他功能的方式不會變更** 在Workfront應用程式本身中，包括功能、使用者角色、工作區、功能和行為的管理。

## 移轉歷程時間表

Adobe會先將您的Workfront執行個體移轉至Adobe Admin Console，然後移轉具有已驗證電子郵件地址的所有現有使用者。 如果您是系統管理員或Workfront產品設定檔管理員(Workfront系統管理員)，您將會收到引導您完成移轉歷程的電子郵件。 以下是您可以期待的時間表：

### Workfront移轉至Adobe Admin Console完成

Workfront移轉至Adobe Admin Console完成後，系統管理員將會收到電子郵件。 此時，系統管理員可能需要完成一些必要的步驟 **使用者移轉開始之前**，將對Workfront使用者造成的影響降至最低。

* **如果您的Workfront使用者目前是以SSO登入**，您必須在Adobe Admin Console上設定SSO，讓您的使用者可以繼續以SSO登入。 如果您的Workfront使用者目前未使用SSO，但您想在Adobe Admin Console上加以設定，您可在移轉歷程中的此時點進行設定。
* **如果您已在您的Adobe Admin Console中管理其他Adobe產品**，Adobe可能會要求您同意自動將使用者移轉至您現有的主控台。 按一下 **開始使用** 電子郵件中的按鈕，以導覽至同意頁面。

目前使用者管理沒有變更。 Workfront管理員將繼續在Workfront中管理使用者，使用者將繼續使用其Workfront ID或SSO登入，直到使用者移轉完成。

### 排程使用者移轉

系統管理員完成上一節所述的先決條件後，Adobe會自動排程您的使用者移轉30天（在這些先決條件完成後），並會與Workfront產品設定檔管理員(Workfront系統管理員)通訊，以管理使用者移轉。

Workfront產品設定檔管理員(Workfront系統管理員)將：

* 收到含有排程使用者移轉開始日期的電子郵件（大約在完成這些先決條件後的30天）
* 取得指定Workfront管理員控制檯的存取權，使用者可選擇在此變更移轉日期

  >[!NOTE]
  >
  >由於移轉的複雜性，日期變更限制在排定日期後30天內有效。 如果您需要更晚的日期，請聯絡支援人員。

* 在使用者移轉開始日期前1天收到提醒電子郵件

### 準備使用者進行移轉日

身為Workfront產品設定檔管理員(Workfront系統管理員)，負責確保所有使用者準備好進行移轉作業。

* 通知所有使用者下列事項，讓他們為即將移轉至Adobe身分識別做好準備：

   * 當使用者移轉時，他們會收到Adobe的電子郵件，通知他們登入Workfront的方式已變更。 使用者將獲邀接受邀請，以使用Adobe身分識別首次登入，方法為使用現有Adobe ID登入，或使用相同的電子郵件地址設定新帳戶。

### 移轉當天的期望

* **使用者移轉將於客戶託管Workfront資料中心的午夜開始。**

* **Adobe將會先自動移轉Workfront管理員。** Workfront管理員移轉至Adobe身分識別時，將會被指派Adobe產品設定檔管理員(Workfront系統管理員)角色。 使用者在移轉前可能擁有的現有角色將不會受到影響。

  >[!NOTE]
  >
  >使用者移轉期間，不會失去對產品的存取權。 如果使用者在其使用者移轉期間登入，則不會有任何影響。 但是，下次登入時，使用者必須使用其Adobe身分識別。



* **使用者移轉後，會收到Adobe的電子郵件，通知他們登入Workfront的方式有所變更。** 使用者將獲邀接受邀請，以使用Adobe身分識別首次登入，方法為使用現有Adobe ID登入，或使用相同的電子郵件地址設定新的Adobe ID。

  如需如何使用Adobe ID登入Workfront的詳細資訊，請參閱 [登入Adobe Experience Cloud](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md#log-in-to-adobe-experience-cloud).

### 使用者移轉完成

所有系統管理員和使用者完成移轉後，Adobe會透過電子郵件通知所有系統管理員和產品設定檔管理員(Workfront系統管理員)。 此時，該執行個體的所有Workfront使用者都會使用Adobe身分登入Workfront。 Workfront系統管理員和產品設定檔管理員(Workfront系統管理員)可能會在Adobe Admin Console中管理使用者存取權。 如果客戶沒有在管理員主控台中使用目錄同步處理形式，他們可能會繼續在Workfront應用程式中管理Workfront的存取許可權。

## 取得支援

如有疑問或疑慮，請依照文章中概述的步驟操作 [聯絡客戶支援](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).




