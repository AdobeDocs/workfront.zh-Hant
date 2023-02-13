---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: 設定使用者的校對存取權
description: 身為Adobe Workfront管理員或Workfront Proof管理員，您可以設定使用者的存取權，以在Workfront和Workfront Proof中建立和檢視校樣。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# 設定使用者的校對存取權

身為Adobe Workfront管理員或Workfront Proof管理員，您可以設定使用者的存取權，以在Workfront和Workfront Proof中建立和檢視校樣。

有關可用於基本和整合校對的校對功能的資訊，請參見 [存取Workfront中的校對功能](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是Workfront管理員或Workfront校樣管理員。 如需Workfront管理員的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 啟用和停用使用者的校對功能（僅限舊版計畫） {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

如果您的組織使用舊版Select或Premium Workfront計畫，以Workfront管理員身分，您可以啟用和停用使用者的校對功能。

當您為使用者啟用校對功能時，Workfront會啟用自動產生使用者校樣的選項。

雖然您可以讓使用者成為測試使用者，但他/她必須擁有管理員權限，才能從Workfront主功能表直接導覽至Workfront Proof介面。 如需如何為Workfront系統中所有校對使用者啟用此選項的詳細資訊，請參閱 [透過Workfront主功能表為所有使用者設定Workfront校樣存取](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. 在 **主菜單**，選取 **使用者**.

1. 選取使用者，然後按一下 **編輯** 表徵圖。
1. 在 **存取** 部分，選擇或取消選擇 **使用者可產生校樣**.

## 設定使用者的校樣權限設定檔

您選取的權限設定檔會針對組織記憶體在的每個校樣授予使用者。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).
1. 選取一或多個使用者，然後按一下 **編輯**.

1. 在 **存取** 區段中，按一下以下其中一個Workfront校樣權限選項： **校樣權限設定檔** 下拉式功能表：

   >[!NOTE]
   >
   >如果您是舊版Workfront計畫，請確定 **使用者可產生校樣** 選項，如上節所述 [啟用和停用使用者的校對功能（僅限舊版計畫）](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>主管</strong> </td> 
      <td>使用者可以管理並檢視在您組織帳戶上建立的所有校樣。 他們也可以編輯新增至這些校樣的審核者。 擁有此權限設定檔的使用者無法管理使用者或編輯Workfront校樣設定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>經理</strong> </td> 
      <td> <p> 使用者可以管理並檢視在您組織帳戶上建立或擁有的校樣。 只有新增為審核者時，他們才能檢視其他使用者的校樣。 這是預設設定。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>管理員</strong> </td> 
      <td> 在Workfront Proof中為使用者授予管理員權限，並可編輯帳戶設定。 使用者可以管理並檢視在您組織帳戶上建立的所有校樣。 這包括新增和移除審核者、校樣和註解。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自訂</strong> </td> 
      <td> <p>只有在您已在Workfront Proof中設定自訂權限設定檔時才可用。</p> <p><b>附註</b>:  <p>請確定您在這裡授予的權限設定檔不會提供比Workfront中使用者的存取層級設定更高的存取權(請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>)。 如果提供較高的存取權，使用者可以存取Workfront Proof內證明，證明無法在Workfront記憶體取。</p> <p>如果您打算允許所有Workfront使用者直接從Workfront存取Workfront Proof，這點尤其重要，如 <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">從Adobe Workfront存取Workfront校樣</a>.</p> <p>依預設，只有Workfront管理員可從Workfront全域導覽列存取Workfront校樣網站的直接連結。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   您選取的權限設定檔會針對組織記憶體在的每個校樣授予使用者。

1. 按一下 **儲存變更** 完成對用戶設定的更新。

   >[!NOTE]
   >
   >當您在Workfront中建立或更新使用者，且使用者的Workfront電子郵件地址與授權的Workfront Proof使用者的電子郵件地址相符時，系統會在Workfront中為使用者啟用校對功能。 如需詳細資訊，請參閱 [Adobe Workfront和Workfront Proof之間的使用者同步](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### 考量事項

設定權限時，請考量下列資訊：

* 如果您將使用者的權限設定檔變更為具有較少權限的設定檔，則使用者可能會失去Workfront中現有校樣的可見性。 當某人與Workfront內的使用者共用工作，但未共用附加至該工作的校樣時，就會發生此情況(請參閱 [在Adobe Workfront內共用證明](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [在Adobe Workfront內共用證明](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md))。
* 只有在您的Workfront環境已與Workfront Proof Premium帳戶整合時，才可從Workfront設定Roof權限。 如果您無法如本節所述使用校對功能，請聯絡您的Workfront管理員。
* 您的Workfront環境中至少必須有一名使用者具有校對的管理員權限。 如果您嘗試從所有用戶中刪除校對的管理員權限，則會顯示錯誤消息。
* 當您將使用者的Workfront存取層級變更為系統管理員以外的任何層級時，使用者的Workfront校樣權限設定檔會預設為Manager。

* 將「Workfront存取」層級變更為「系統管理員」時，「證明權限」設定檔會變更為「管理員」。

## 透過Workfront主功能表為所有使用者設定Workfront校樣存取 {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

依預設，只有Workfront內具有管理權限的使用者才能存取Workfront Proof，如所述  [從Adobe Workfront存取Workfront校樣](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

您可以聯絡Workfront支援並提交請求，借此授與所有使用者對Workfront主功能表中「Workfront校樣」按鈕的存取權。

>[!IMPORTANT]
>
> 如果您打算允許所有Workfront使用者直接從Workfront全域導覽列存取Workfront Proof，請確定每位使用者的權限設定檔所提供的存取權限，不會超過使用者在Workfront內的存取層級。 這會讓使用者無法存取Workfront Proof內無法在Workfront記憶體取的校樣。 如需詳細資訊，請參閱 [啟用和停用使用者的校對功能（僅限舊版計畫）](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## 配置用戶對案頭校對查看器的訪問

如果您組織中的使用者偏好使用案頭打樣檢視器，而非網頁打樣檢視器來檢視互動式內容，您可以設定案頭打樣檢視器，讓使用者在開啟互動式內容校樣時自動啟動。 有關Desktop Pooting Viewer及其與Web Pooting Viewer的不同之處的資訊，請參閱 [了解案頭打樣檢視器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) 和 [Web校對查看器與Desktop Pooting Viewer之間的差異概述](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. 在Workfront中，按一下全域導覽列中的Workfront校樣圖示以存取Workfront Proof。

   ![](assets/proof-access-proofhq-350x39.png)

1. 按一下 **帳戶設定** 在Workfront Proof的右上角附近，按一下 **設定** 標籤。

1. 在 **校樣預設值**，在 **互動式校樣的案頭校樣檢視器** 列，按一下 **設定**.

1. 修改案頭校對檢視器設定，如 [案頭校對檢視器](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) 在文章中 [為貴組織配置校樣設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. 按一下&#x200B;**儲存**。

## 設定互動式校樣的自訂裝置

您可以向系統添加任何自定義設備，允許用戶查看交互內容，並模擬當他們使用案頭校對查看器時，該內容在特定設備上的顯示方式。 （網頁校對檢視器中無法使用此功能，使用者可以檢閱互動式內容，但只能依不同解析度顯示，不能依不同裝置顯示。）

如需詳細資訊，請參閱 [變更校對檢視器中的互動式校樣解析度](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. 從Workfront存取Workfront Proof介面，如 [從Adobe Workfront存取Workfront校樣](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. 修改案頭校對檢視器設定，如 [設定校樣的自訂裝置](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) 在文章中 [為貴組織配置校樣設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
