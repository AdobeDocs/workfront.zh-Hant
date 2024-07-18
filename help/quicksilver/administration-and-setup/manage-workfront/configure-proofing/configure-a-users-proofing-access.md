---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: 設定使用者的校訂存取權
description: 身為Adobe Workfront管理員或Workfront Proof管理員，您可以設定使用者在Workfront和Workfront Proof中建立和檢視校訂的存取權。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# 設定使用者的校訂存取權

身為Adobe Workfront管理員或Workfront Proof管理員，您可以設定使用者在Workfront和Workfront Proof中建立和檢視校訂的存取權。

如需可用於基本與整合校訂之校訂功能的相關資訊，請參閱[存取Workfront中的校訂功能](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是Workfront管理員或Workfront Proof管理員。 如需Workfront管理員的相關資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 為使用者啟用和停用校訂（僅限舊版計畫） {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

如果您的組織使用舊版Select或Premium Workfront計畫，您作為Workfront管理員，可以為使用者啟用和停用校訂功能。

當您啟用使用者校訂時，Workfront會啟用自動產生使用者校訂的選項。

雖然您可以將使用者啟用為校訂使用者，但他或她必須擁有管理員許可權，才能直接從Workfront主功能表導覽至Workfront Proof介面。 如需如何在Workfront系統中為所有校訂使用者啟用此選項的相關資訊，請參閱[透過Workfront為所有使用者設定Workfront Proof存取權](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users)。

1. 在&#x200B;**主功能表**&#x200B;中，選取&#x200B;**使用者**。

1. 選取使用者，然後按一下&#x200B;**編輯**&#x200B;圖示。
1. 在&#x200B;**存取**&#x200B;區段中，選取或取消選取&#x200B;**使用者可以產生校樣**。

## 設定使用者的校訂許可權設定檔

您選取的許可權設定檔會針對組織內存在的每個校訂授予使用者。

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**使用者** ![](assets/users-icon-in-main-menu.png)。
1. 選取一或多個使用者，然後按一下[編輯]。****

1. 在&#x200B;**存取**&#x200B;區段中，按一下&#x200B;**校訂許可權設定檔**&#x200B;下拉式功能表中的下列Workfront Proof許可權選項之一：

   >[!NOTE]
   >
   >如果您在舊版Workfront計畫中，請確定已啟用&#x200B;**使用者可以產生校樣**&#x200B;選項，如上方[為使用者啟用和停用校樣（僅限舊版計畫）](#enable-and-disable-proofing-for-a-user-legacy-plans-only)一節中所述。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>監督員</strong> </td> 
      <td>使用者可以管理和檢視在您組織帳戶上建立的所有校訂。 他們也可以編輯新增到這些校訂的稽核者。 具有此許可權設定檔的使用者無法管理使用者或編輯Workfront Proof設定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>管理員</strong> </td> 
      <td> <p> 使用者可以管理和檢視在您組織帳戶上建立或擁有的校樣。 他們只有在新增為檢閱者時才能檢視其他使用者的校樣。 這是預設設定。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>管理員</strong> </td> 
      <td> 使用者在Workfront Proof中擁有管理員許可權，可以編輯帳戶設定。 使用者可以管理和檢視在您組織帳戶上建立的所有校訂。 這包括新增和移除稽核者、校樣和註解。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自訂</strong> </td> 
      <td> <p>僅當您在Workfront Proof中設定了自訂許可權設定檔時才可用。</p> <p><b>附註</b>：  <p>確定您在此處授與的許可權設定檔提供的存取許可權不會高於Workfront中使用者的存取層級設定（請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>）。 如果它提供更高的存取權，使用者可以在Workfront Proof中存取他或她無法在Workfront中存取的校訂。</p> <p>如果您打算依照<a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">從Adobe Workfront存取Workfront Proof</a>中的說明，允許所有Workfront使用者直接從Workfront存取Workfront Proof，這一點尤其重要。</p> <p>依預設，只有Workfront管理員有權存取Workfront全域導覽列中Workfront Proof網站的直接連結。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   您選取的許可權設定檔會針對組織內存在的每個校訂授予使用者。

1. 按一下&#x200B;**儲存變更**&#x200B;以完成使用者設定的更新。

   >[!NOTE]
   >
   >當您在Workfront中建立或更新使用者，並且該使用者的Workfront電子郵件地址與授權的Workfront Proof使用者的電子郵件地址相符時，系統會在Workfront中啟用該使用者的校訂。 如需詳細資訊，請參閱[ Adobe Workfront與Workfront Proof之間的使用者同步](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md)。

### 考量事項

設定許可權時，請考慮下列資訊：

* 如果您將使用者的許可權設定檔變更為許可權較少的設定檔，使用者可能會失去Workfront中現有校訂的可見度。 當有人在Workfront中與使用者共用工作，但未共用附加至工作的校訂(請參閱[在Adobe Workfront中共用](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)的校訂](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)的校訂[在Adobe Workfront中共用)時，就會發生這種情況。
* 您必須將Workfront Proof環境與Workfront Premium帳戶整合，才能從Workfront Proof設定Workfront許可權。 如果您無法依照本節所述使用校訂，請聯絡Workfront管理員。
* 在您的Workfront環境中，必須至少有一個使用者擁有校訂的管理員許可權。 如果您嘗試從所有使用者中移除校訂的管理員許可權，則會出現錯誤訊息。
* 當您將使用者的Workfront存取層級變更為系統管理員以外的任何層級時，該使用者的Workfront Proof許可權設定檔預設為「管理員」。

* 當您將Workfront存取層級變更為系統管理員時，校訂許可權設定檔會變更為管理員。

## 透過Workfront主要功能表為所有使用者設定Workfront Proof存取權 {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

依預設，只有在Workfront內具有管理許可權的使用者才能存取Workfront Proof，如所述[從Adobe Workfront存取Workfront Proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)。

您可以聯絡Workfront Proof支援並提交請求，藉此向所有使用者授予Workfront主功能表內Workfront按鈕的存取權。

>[!IMPORTANT]
>
> 如果您打算允許所有Workfront使用者直接從Workfront全域導覽列存取Workfront Proof，請確認每位使用者的許可權設定檔所提供的存取權，不會超過該使用者在Workfront中的存取層級。 這可防止使用者存取Workfront Proof中他們無法在Workfront中存取的校訂。 如需詳細資訊，請參閱[啟用和停用使用者的校訂（僅限舊版計畫）](#enable-and-disable-proofing-for-a-user-legacy-plans-only)。

## 設定案頭校訂檢視器的使用者存取權

如果您組織中的使用者偏好使用「案頭校訂檢視器」而不是「網頁校訂檢視器」來檢閱互動式內容，您可以將「案頭校訂檢視器」設定為在使用者開啟互動式內容校訂時自動啟動。 如需有關這個案頭校訂檢視器的資訊，以及它與Web校訂檢視器的差異，請參閱[瞭解案頭校訂檢視器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)和[網頁校訂檢視器與案頭校訂檢視器之間的差異](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)。

1. 從Workfront，按一下全域導覽列中的Workfront Proof圖示以存取Workfront Proof。

   ![](assets/proof-access-proofhq-350x39.png)

1. 按一下Workfront Proof右上角附近的&#x200B;**帳戶設定**，然後按一下&#x200B;**設定**&#x200B;標籤。

1. 在&#x200B;**校訂預設值**&#x200B;下，在&#x200B;**互動式校訂的案頭校訂檢視器**&#x200B;列的結尾處，按一下&#x200B;**設定**。

1. 修改案頭校訂檢視器設定，如[案頭校訂檢視器](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer)文章[設定組織的校訂設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)中所述。

1. 按一下「**儲存**」。

## 設定互動式校樣的自訂裝置

您可以將任何自訂裝置新增到系統中，讓使用者檢閱互動式內容，並模擬內容在使用「案頭校訂檢視器」時顯示在特定裝置上的方式。 (此功能無法在Web Proofing Viewer （使用者可以在其中檢閱互動式內容）中使用，但只能以各種解析度顯示，不能用於各種裝置。)

如需詳細資訊，請參閱[在校訂檢視器中變更互動式校訂解析度](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)。

1. 從Workfront存取Workfront Proof介面，如[從Adobe Workfront存取Workfront Proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)中所述。
1. 修改案頭校訂檢視器設定，如[設定組織的校訂設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)文章中的[設定校訂的自訂裝置](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs)中所述。
