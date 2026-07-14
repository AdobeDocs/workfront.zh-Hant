---
product-area: documents;workfront-integrations;system-administration
navigation-topic: adobe-cloud-drive
title: 設定和管理Adobe Cloud Drive
description: 作為管理員，您可以為組織設定Adobe Cloud Drive、將其部署至使用者裝置，並在Adobe Admin Console中管理持續存取。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps, System Setup and Administration
role: Admin
source-git-commit: f1dd9555df2adcf8a1afc48982bc2d52a14df54f
workflow-type: tm+mt
source-wordcount: '3139'
ht-degree: 1%

---

# 為貴組織設定和管理Adobe Cloud Drive

身為管理員，您可以設定Adobe Cloud Drive，讓使用者透過macOS上的Finder和Windows上的File Explorer，直接透過案頭存取Adobe雲端儲存空間中的專案檔案。 本文介紹如何在Adobe Admin Console中啟用存取、將應用程式部署至使用者裝置，以及持續管理存取。

Adobe Cloud Drive是一款企業案頭應用程式，可將Workfront檔案掛載至Adobe雲端儲存空間，作為使用者Mac和Windows電腦上的虛擬磁碟機。 安裝後，使用者可在Finder或File Explorer中檢視其Workfront專案資料夾，並可使用任何案頭應用程式開啟、編輯和儲存專案檔案，無需手動下載檔案或透過瀏覽器工作。

若要使用Adobe Cloud Drive，您的組織必須位於已啟用Adobe雲端儲存空間的工作流程Ultimate套件上。

如需Adobe Cloud Drive的詳細資訊，請參閱下列文章：

* [Adobe Cloud Drive概述](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md)
* [安裝Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md)
* [使用Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront版本</td> 
   <td>工作流程Ultimate，已啟用Adobe雲端儲存空間</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe管理員許可權</td> 
   <td>您必須是Adobe Admin Console中Workfront的系統管理員</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在Adobe Admin Console中指派Adobe Cloud Drive的存取權

啟用Adobe雲端儲存空間時，Workflow Ultimate套件會包含Adobe Cloud Drive。 它在Admin Console的&#x200B;**產品**&#x200B;區段中不會顯示為獨立產品。 而是透過&#x200B;**使用者**&#x200B;下的&#x200B;**角色**&#x200B;區段來管理。

當您前往&#x200B;**使用者** > **角色**，您會看到兩個與Workfront產品相關的角色：

| 角色 | 自動指派給 | 與Adobe Cloud Drive的相關性 |
| --- | --- | --- |
| **成員** | 組織中的所有使用者 | 包含組織層級Adobe Cloud Drive功能開關。 預設為開啟。 |
| **ACD使用者** | 無使用者，預設為 | 當組織層級切換器關閉時，授予個別存取權。 |

Admin Console中的![角色](assets/admin-console-roles.png)

### 存取控制

**控制項1：組織層級功能控制項（在成員角色中）**

**成員**&#x200B;角色會自動指派給貴組織中的每位使用者。 在此角色中，有&#x200B;**Adobe雲端磁碟機**&#x200B;功能引數。 當此開關開啟時，每個具有Workflow Ultimate授權的使用者都可以存取Adobe Cloud Drive。 關閉後，無論授權為何，使用者都無法存取Adobe Cloud Drive。

Adobe為您的組織啟用Adobe Cloud Drive時，切換器預設為開啟。

**控制項2： ACD使用者角色**

**ACD使用者**&#x200B;角色只有在組織層級切換開關關閉時才相關。 如果您關閉組織層級切換器以執行受控試驗，您仍可透過將特定使用者新增至&#x200B;**ACD使用者**&#x200B;角色來授予其存取權。 即使組織層級切換已關閉，此角色的使用者仍可存取Adobe Cloud Drive。 如果組織層級切換器已開啟，**ACD使用者**&#x200B;角色就沒有作用。

**基礎需求：工作流程Ultimate授權**

Adobe Cloud Drive僅適用於Workflow Ultimate套件。 角色選項無法在任何其他套件中使用。

工作流程Ultimate套件中的授權可以是任何授權型別：標準、輕度或貢獻者。 如需授權的相關資訊，請參閱[授權總覽](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)。

下表顯示這些控制項如何互動：

| 組織層級交換器 | ACD使用者角色中的使用者 | 工作流程Ultimate授權 | 存取結果 |
| --- | --- | --- | --- |
| 開啟 | 非必要 | 是 | 已授予 |
| 關閉 | 是 | 是 | 已授予 |
| 關閉 | 無 | 是 | 已拒絕 |
| 兩者之一 | 兩者之一 | 無 | 已拒絕 |

<!-- Sarah said to delete the second line. Commenting it out within the table messed up the display for the rest of the table, so keeping the line here until I can delete it. | On | Not required | No | Denied | -->

## 先決條件

開始之前，請先確認下列事項：

* 您計畫布建的使用者已獲指派Workfront工作流程授權。
* 您已與您的IT團隊檢閱[網路需求](#network-requirements)。
* 您已經起草通訊內容，以傳送給使用者來說明Adobe Cloud Drive顯示的內容（僅限Workfront專案資產）以及如何安裝。

  >[!NOTE]
  >
  >具有已啟用存取許可權但未存取任何Workfront專案的使用者登入後會看到空的已掛載磁碟機。 這是預期中的情形。 Workfront專案存取權在Workfront中另行管理。 如需詳細資訊，請參閱[共用專案](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。
  >
  >此外，Creative Cloud權益必須與Workfront位於相同的IMS組織中，專案才能顯示在磁碟機中。

## 在Adobe Admin Console中設定存取權

Adobe Cloud Drive存取需在Adobe Admin Console中設定。 選擇符合轉出策略的選項。

### 選項A：啟用整個組織的存取權

當Adobe為您的組織啟用Adobe Cloud Drive時，組織層級功能切換預設為開啟，且所有使用者都能立即存取。 在部署應用程式之前，請使用此程式確認切換器已開啟。

1. 登入[adminconsole.adobe.com](https://adminconsole.adobe.com/)。
1. 按一下頂端導覽列中的&#x200B;**使用者**。
1. 按一下左側面板中的&#x200B;**角色**。
1. 按一下角色清單中的&#x200B;**成員**。
1. 在右側開啟的&#x200B;**成員**&#x200B;面板中，確認&#x200B;**Adobe雲端磁碟機**&#x200B;出現在&#x200B;**許可權**&#x200B;下方，且其開關已開啟。

   已開啟Adobe Cloud Drive的![成員角色詳細資料面板](assets/member-permissions.png)

   >[!NOTE]
   >
   >如果Adobe Cloud Drive未出現在&#x200B;**成員**&#x200B;角色的&#x200B;**許可權**&#x200B;之下，則可能尚未為您的組織啟用Adobe Cloud Drive。 聯絡Adobe支援以確認。

1. 如果您做了任何變更，請按一下[儲存]。****

### 選項B：啟用特定使用者群組的存取權

如果您想要限制對一組已定義使用者的存取權（例如，在較廣泛的轉出之前進行試驗），請使用此選項。 這涉及關閉組織層級切換器，然後將您的試驗使用者新增至&#x200B;**ACD使用者**&#x200B;角色。

>[!IMPORTANT]
>
>關閉組織層級交換器會立即移除組織中所有使用者的Adobe Cloud Drive存取權，包括目前登入的使用者。 您必須關閉組織層級功能，並在相同作業階段中新增試驗使用者。

若要關閉組織層級功能：

1. 登入[adminconsole.adobe.com](https://adminconsole.adobe.com/)。
1. 按一下頂端導覽列中的&#x200B;**使用者**，然後按一下左側面板中的&#x200B;**角色**。
1. 按一下角色清單中的&#x200B;**成員**。
1. 在&#x200B;**成員**&#x200B;面板中，在&#x200B;**許可權**&#x200B;下找到&#x200B;**Adobe Cloud Drive**，然後將其關閉。
1. 按一下「**儲存**」。

若要將試驗使用者新增至ACD使用者角色：

1. 在左側面板中，按一下&#x200B;**角色**&#x200B;以返回角色清單。
1. 按一下角色清單中的&#x200B;**ACD使用者**。

   ![ACD使用者詳細資料面板](assets/acd-user-panel.png)

1. 按一下&#x200B;**新增使用者**。
1. 輸入每個試驗使用者的電子郵件地址。
1. 按一下「**儲存**」。

   新增至&#x200B;**ACD使用者**&#x200B;角色的使用者會立即取得存取權。 除非您將使用者新增至角色或開啟組織層級切換開關，否則沒有此角色的使用者將無法存取。

   >[!TIP]
   >
   >若要隨著時間擴展存取權，請返回&#x200B;**ACD使用者**&#x200B;角色，並視需要新增使用者。 當您準備好進行完整轉出時，請在&#x200B;**成員**&#x200B;角色中重新開啟組織層級切換開關。 一旦開啟組織層級切換器，**ACD使用者**&#x200B;角色就沒有作用，不需要維護。

## 部署Adobe雲端硬碟應用程式

在Adobe Admin Console中設定存取權會建立權益。 部署應用程式會將其安裝在使用者的裝置上。 這是兩個獨立的必要步驟。

Adobe Cloud Drive為獨立應用程式。 它不會透過Creative Cloud案頭應用程式發佈，也不會出現在Creative Cloud封裝管理員中。 不過，Adobe Cloud Drive的使用者設定檔已繫結至Creative Cloud應用程式權利。 這表示使用者若要在磁碟機中存取Workfront專案，Creative Cloud應用程式必須在與Workfront相同的IMS組織中取得許可權。

選擇符合您組織裝置管理實務的部署方法。

### 方法A：透過Admin Console套件進行IT管理的部署

當您的組織使用集中式部署工具（例如Microsoft Intune、SCCM、Jamf Pro或Apple遠端案頭）時，請使用此方法。 這是標準的Adobe企業部署工作流程，會依照用於其他Adobe應用程式的相同套件建立流程進行。

若要在Adobe Admin Console中建立套件：

1. 登入[adminconsole.adobe.com](https://adminconsole.adobe.com/)。
1. 按一下頂端導覽列中的&#x200B;**封裝**。
1. 按一下左側面板中的&#x200B;**預先產生的封裝**。
1. 按一下「**範本**」標籤。

   Adobe Cloud Drive在範本清單中顯示兩次：一次適用於macOS，另一次適用於Windows。

   ![預先產生的封裝範本](assets/pre-generated-packages.png)

1. 找出符合目標平台的&#x200B;**Adobe Cloud Drive**&#x200B;列，然後按一下該列的詳細資訊圖示。

   側面板會顯示封裝中繼資料。

   ![封裝詳細資料和中繼資料](assets/template-details-and-metadata.png)

1. 按一下&#x200B;**自訂**。

   封裝自訂精靈開啟，包含四個步驟： **設定**、**選擇應用程式**、**選項**&#x200B;和&#x200B;**完成**。

1. 在&#x200B;**設定**&#x200B;步驟中，選取目標電腦的架構，然後確認語言設定並按一下&#x200B;**下一步**。

   * **macOS：**&#x200B;選擇&#x200B;**macOS (Intel)**&#x200B;或&#x200B;**macOS (Apple Silicon)**。
   * **Windows：**&#x200B;選擇&#x200B;**Windows （64位元）**&#x200B;或&#x200B;**Windows (ARM)**。

   ![在封裝精靈中設定步驟](assets/configure-step-in-wizard.png)

1. 在&#x200B;**選擇應用程式**&#x200B;步驟中，確認已使用您想要的版本選取Adobe Cloud Drive。

   已預先選取Adobe Cloud Drive的最新可用版本。 若要使用較舊的版本，請按一下&#x200B;**其他版本**，然後選取&#x200B;**較舊的版本**。

   ![在封裝精靈中選擇應用程式步驟](assets/choose-apps-step-in-wizard.png)

1. 按一下「**下一步**」。
1. 在&#x200B;**選項**&#x200B;步驟中，按一下&#x200B;**下一步**，而不選取任何選項。

   這些設定會套用至Creative Cloud案頭應用程式，不會套用至Adobe Cloud Drive。

   封裝精靈中的![選項步驟](assets/options-step-in-wizard.png)

1. 在&#x200B;**完成**&#x200B;步驟中，輸入封裝的名稱，並選取&#x200B;**平面封裝**。
1. 檢閱摘要，然後按一下&#x200B;**建立封裝**。

   在封裝精靈中![完成步驟](assets/finalize-step-in-wizard.png)

   精靈會關閉。 您的新封裝會在建置時，以&#x200B;**正在準備**&#x200B;狀態出現在封裝清單頂端。 準備就緒後，狀態會變更為&#x200B;**最新**，並顯示下載連結。

   ![封裝正在準備狀態](assets/package-is-preparing.png)

1. 按一下&#x200B;**下載**&#x200B;並將封裝檔案儲存到您選擇的位置。

### 方法B：從Software Distribution自助直接下載

在較小組織、自我管理裝置，或引導個別使用者自行安裝應用程式時，請使用此方法。

開始之前，請確認下列事項：

* Adobe Admin Console中的使用者存取許可權已啟用。
* 使用者已收到軟體發佈URL和登入指示的通知。
* 已驗證所需端點的網路連線。 如需詳細資訊，請參閱本文中的[網路需求](#network-requirements)。

若要自行安裝Adobe Cloud Drive：

1. 確認已在Adobe Admin Console中為該使用者啟用存取權。
1. 將使用者導向至[experience.adobe.com/#/downloads](https://experience.adobe.com/#/downloads)。

   >[!NOTE]
   >
   >使用者必須在Adobe Admin Console中啟用Adobe Cloud Drive存取權，才能檢視Adobe Cloud Drive安裝程式。 沒有存取權的使用者將不會看到安裝程式列出。

1. 使用者使用其Enterprise ID或Federated ID登入。 Adobe Cloud Drive安裝程式出現在Software Distribution的&#x200B;**Workfront**&#x200B;標籤中。
1. 使用者下載其平台的安裝程式，並遵循[安裝Adobe雲端磁碟機](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md)中的安裝步驟。

   適用於Workfront的![Adobe Cloud Drive安裝程式](assets/wf-downloads.png)

部署後，在測試裝置上完成此驗證：

1. 從&#x200B;**應用程式**&#x200B;資料夾(macOS)或&#x200B;**開始**&#x200B;功能表(Windows)啟動Adobe Cloud Drive。
1. 使用已在Adobe Admin Console中啟用Adobe Cloud Drive存取許可權的使用者帳戶登入。
1. 確認Workfront專案資料夾出現在Finder或File Explorer中已掛載的磁碟機中。

   >[!NOTE]
   >
   >成功登入但未看到任何資料夾的使用者，無權存取任何Workfront專案。 將使用者新增至Workfront中的專案以填入磁碟機。

1. 導覽至專案資料夾，並建立小型測試檔案。
1. 在瀏覽器中開啟Workfront，並確認測試檔案會顯示在對應的專案中。
1. 驗證後刪除測試檔案。

## 管理使用者對Adobe Cloud Drive的持續存取

您的組織使用Adobe Cloud Drive後，請按照以下步驟新增使用者，或移除不再需要存取的使用者。

### 新增使用者

如果組織層級切換器為開啟，則不需執行Adobe Admin Console動作。 要求使用者下載並安裝Adobe Cloud Drive。 如果授權使用者仍無法存取Adobe Cloud Drive，請聯絡Adobe支援，確認其帳戶已正確移轉。

如果組織層級切換器已關閉：

1. 登入[adminconsole.adobe.com](https://adminconsole.adobe.com/)。
1. 按一下頂端導覽列中的&#x200B;**使用者**，然後按一下左側面板中的&#x200B;**角色**。
1. 按一下角色清單中的&#x200B;**ACD使用者**。
1. 按一下&#x200B;**新增使用者**，輸入使用者的電子郵件地址，然後按一下&#x200B;**儲存**。

### 移除使用者

如果組織層級交換器已開啟，則任何授權使用者都可以存取Adobe Cloud Drive。 若要移除特定使用者的存取權而不移除其Workfront授權，請關閉組織層級切換器，並將所有其他使用者新增至&#x200B;**ACD使用者**&#x200B;角色，排除您要封鎖的使用者。

如果組織層級切換器已關閉，且使用者處於&#x200B;**ACD使用者**&#x200B;角色：

1. 登入[adminconsole.adobe.com](https://adminconsole.adobe.com/)。
1. 按一下頂端導覽列中的&#x200B;**使用者**，然後按一下左側面板中的&#x200B;**角色**。
1. 按一下角色清單中的&#x200B;**ACD使用者**。
1. 選取使用者並按一下&#x200B;**移除**。

使用者會立即失去已掛載磁碟機的存取權。 不會刪除儲存在Workfront中的檔案。 使用者的本機快取會保留在其裝置上，直到解除安裝應用程式為止。

>[!IMPORTANT]
>
>從&#x200B;**ACD使用者**&#x200B;角色中移除使用者，並不會將他們從Workfront或任何Workfront專案中移除。 分別管理Workfront專案存取權。

## 管理Workfront專案存取權

Adobe Cloud Drive會向使用者顯示他們有權存取的Workfront專案。 專案存取權在Workfront中管理，而非在Adobe Admin Console中管理。 擁有Adobe Cloud Drive存取權但屬於Workfront專案的使用者登入後會看到空的已掛載磁碟機。 這是預期的行為。

如需有關管理專案存取許可權的資訊，請參閱[管理專案](/help/quicksilver/manage-work/projects/manage-projects/manage-projects-overview.md)和[共用專案](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。

## 網路需求

Adobe Cloud Drive需要輸出HTTPS （連線埠443）存取一組Adobe端點。 不需要輸入防火牆規則。 如需端點清單，請參閱[Adobe網路端點](https://helpx.adobe.com/in/enterprise/kb/network-endpoints.html)。

Adobe Cloud Drive會讀取macOS和Windows上的系統層級Proxy設定。 支援已驗證的代理。

## 安全性考量

### Authentication

Adobe Cloud Drive會透過Adobe IMS (Identity Management System)驗證使用者。 使用者使用其Enterprise ID或Federated ID登入。 如果您的組織使用Adobe Admin Console中設定的SSO，使用者會透過您的身分提供者進行驗證，而不需要個別的Adobe憑證。

>[!NOTE]
>
>Adobe Cloud Drive在企業部署中不支援個人Adobe ID （個別建立、未管理的帳戶）。 使用者必須使用貴組織目錄中的Enterprise ID或Federated ID登入。

### 傳輸中及閒置的資料

* Adobe Cloud Drive與Adobe服務之間的所有通訊皆使用TLS 1.2或更新版本。
* 儲存在Adobe雲端儲存空間中的檔案會在閒置時加密。
* 當裝置上啟用FileVault (macOS)或BitLocker (Windows)時，本機快取的檔案會使用作業系統層級的磁碟加密。

### 檔案存取控制

檔案存取權依照Workfront專案許可權執行。 使用者只會在其Workfront存取層級允許的情況下，看見自己有許可權的專案並與專案互動。

在案頭檢視中，每個Workfront專案的根資料夾都是唯讀的。 使用者無法從Finder或File Explorer重新命名、移動或刪除專案根資料夾。 他們可以不受限於其Workfront許可權，在專案資料夾內任何深度建立資料夾、子資料夾和檔案。

## 疑難排解常見問題

如需使用者疑難排解步驟，請參閱[疑難排解Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/troubleshoot-adobe-cloud-drive.md)。 以下所列的問題是管理員特有的問題。

### 使用者在Software Distribution中找不到Adobe雲端磁碟機安裝程式

**原因：** Adobe Admin Console未針對使用者啟用Adobe雲端磁碟機存取。

**解析度：**

1. 登入[adminconsole.adobe.com](https://adminconsole.adobe.com/)並按一下&#x200B;**使用者**。
1. 搜尋使用者並按一下其名稱。
1. 按一下「**角色**」標籤，然後確認Adobe Cloud Drive是否已啟用。

**原因：** Creative Cloud所有應用程式已布建在與Workfront不同的IMS組織。

**解析度：**&#x200B;目前沒有可用的解析度。

### 使用者已安裝應用程式並登入，但磁碟機中沒有資料夾

**原因：**&#x200B;使用者沒有任何Workfront專案的許可權。

**解析度：**

1. 在Workfront中，確認使用者擁有至少一個專案的許可權。
1. 如果沒有，則與使用者共用專案。
1. 要求使用者最多等候5分鐘，讓專案資料夾顯示。
1. 如果資料夾在五分鐘後仍未顯示，請要求使用者結束Adobe Cloud Drive並重新啟動。

### 使用者無法登入Adobe Cloud Drive

**原因：**&#x200B;使用者的Adobe Admin Console帳戶為非使用中，或其身分未正確設定。

**解析度：**

1. 在Adobe Admin Console中，按一下&#x200B;**使用者**&#x200B;並搜尋該使用者。
1. 確認使用者的帳戶狀態為&#x200B;**作用中**。
1. 確認使用者的電子郵件網域是您Admin Console目錄中已宣告的網域。
1. 如果您的組織使用SSO，請確認使用者帳戶在您的身分提供者中有效。
1. 要求使用者嘗試再次登入。

### 檔案在使用者儲存後未同步

**原因：**&#x200B;檔案未明確儲存，或是網路連線有問題。

**解析度：**

1. 向使用者確認他們已在應用程式中使用&#x200B;**檔案** > **儲存**&#x200B;儲存檔案。 關閉應用程式或依賴自動儲存不會觸發同步。
1. 確認使用者可以存取網際網路，並可以連線`*.adobe.com`和`*.workfront.com`。
1. 要求使用者檢查功能表列(macOS)或系統匣(Windows)中的Adobe Cloud Drive圖示，以取得錯誤指標。
1. 如果發生錯誤，請要求使用者結束Adobe Cloud Drive、重新啟動它，然後再次儲存檔案。
1. 如果問題仍然存在，請收集應用程式記錄：

   * **macOS：** `~/Library/Logs/Adobe/AdobeCloudDrive/`
   * **Windows：** `C:\Users\<username>\AppData\Local\Temp\Adobe\AdobeCloudDrive\`

### 專案資料夾中出現了檔案的衝突副本

**原因：**&#x200B;在任一版本同步至雲端之前，有兩個使用者儲存對相同檔案的變更。 Adobe Cloud Drive會自動保留兩個版本。

衝突的副本使用此命名格式： `filename (Conflicted copy from device_name on date_time).extension`
例如： `project_brief (Conflicted copy from jsmith's MacBook Pro on 2026-06-15-10-45-19).docx`

**解析度：**

1. 詢問兩個使用者哪個版本具有權威性。
1. 將衝突副本中任何需要的內容複製到主要檔案中。
1. 協調兩個版本後，刪除衝突的復本。

   >[!NOTE]
   >
   >Adobe Cloud Drive不使用檔案鎖定。 若要防止多個使用者編輯相同檔案時發生衝突，請在多個使用者從案頭存取相同檔案之前，先透過Workfront任務指派或核准工作流程協調編輯。

### 使用者無法在專案中建立資料夾或檔案

**原因A：**&#x200B;使用者嘗試在專案根層級建立資料夾或檔案。 Adobe Cloud Drive中的專案根資料夾目前是唯讀的。 根層級資料夾代表在Workfront中建立和管理的Workfront專案。

**解析度：**

1. 要求使用者導覽至專案內任何現有的子資料夾，並在那裡建立檔案或資料夾。
1. 如果使用者需要在專案中新的頂層資料夾，請要求他們先在Workfront中建立該資料夾。 然後會顯示在Adobe Cloud Drive中。

**原因B：**&#x200B;使用者沒有Workfront專案的編輯許可權。

**解析度：**

1. 在Workfront中，檢查使用者對專案的許可權（**檢視**、**貢獻**&#x200B;或&#x200B;**管理**）。
1. 更新使用者對&#x200B;**Contribute**&#x200B;或&#x200B;**管理**&#x200B;的許可權（如果他們需要建立或編輯檔案）。
