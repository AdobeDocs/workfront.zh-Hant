---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 設定組織的校訂設定
description: 身為Adobe Workfront管理員或Workfront Proof管理員，您可以為貴組織自訂預設校訂設定。 這些設定包含預設共用選項、品牌化等。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 29405172-c3dd-431f-a242-fd38b53a307d
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '1221'
ht-degree: 0%

---

# 為您的組織設定校訂設定

身為Adobe Workfront管理員或Workfront Proof管理員，您可以為貴組織自訂預設校訂設定。 這些設定包含預設共用選項、品牌化等。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前計畫：Pro或更高版本</p> <p>或</p> <p>舊版計畫：Premium或選取</p> <p>如需有關不同方案的校訂存取許可權的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前計畫：工作或計畫</p> <p>舊版計畫：任何（您必須為使用者啟用校訂）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須在校訂許可權設定檔中選取管理員。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">設定使用者的校訂存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

+++

## 設定動作

如需有關在校訂檢視器中使用動作的資訊，請參閱[對校訂評論使用動作](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)。

您可以透過下列方式設定組織的動作：

* [新增或重新命名動作](#add-or-rename-an-action)
* [停用或重新啟用動作](#deactivate-or-reactivate-an-action)
* [重新排序動作](#reorder-actions)

### 新增或重新命名動作 {#add-or-rename-an-action}

{{step1-to-proofing}}

1. 按一下Workfront Proof介面右上角的&#x200B;**設定** > **帳戶設定**，然後按一下&#x200B;**設定**&#x200B;標籤。

1. 執行下列任一項作業：

   * 若要建立新動作，請在&#x200B;**動作**&#x200B;區段中，按一下&#x200B;**新增動作**。

     您可以在帳戶中設定的動作數量沒有限制。

   * 若要重新命名現有的動作，請按一下動作旁的&#x200B;**設定**。

1. 輸入動作的名稱，然後按一下[儲存]。****
1. 按一下&#x200B;**儲存。**

### 停用或重新啟用動作 {#deactivate-or-reactivate-an-action}

{{step1-to-proofing}}

1. 按一下Workfront Proof介面右上角的&#x200B;**設定** > **帳戶設定**，然後按一下&#x200B;**設定**&#x200B;標籤。

1. 按一下您要停用或重新啟用的動作旁的&#x200B;**設定**。
1. 選取「**啟用**」或「**停用**」，然後按一下「**儲存**」。

### 重新排序動作 {#reorder-actions}

{{step1-to-proofing}}

1. 按一下Workfront Proof介面右上角的&#x200B;**設定** > **帳戶設定**，然後按一下&#x200B;**設定**&#x200B;標籤。

1. 按一下&#x200B;**設定**&#x200B;旁的藍色上下箭頭，以重新排序動作。

   ![Re-order_actions.png](assets/re-order-actions-350x103.png)

## 設定校樣的自訂裝置

您可以將任何自訂裝置新增到系統中，讓使用者檢閱互動式內容並模擬內容在特定裝置上的顯示方式。

如需有關使用者在檢閱互動式內容時如何選取裝置的資訊，請參閱[在校訂檢視器中變更互動式校訂解析度](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)

若要新增自訂裝置：

{{step1-to-proofing}}

1. 按一下Workfront Proof介面右上角的&#x200B;**設定** > **帳戶設定**，然後按一下&#x200B;**設定**&#x200B;標籤。

1. 在&#x200B;**校訂的自訂裝置**&#x200B;區段中，按一下&#x200B;**新增裝置**。

1. 在出現的&#x200B;**新增裝置**&#x200B;方塊中，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">姓名</td> 
      <td>使用者在案頭校訂檢視器中選取裝置時看到的名稱，如<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">變更校訂檢視器中的互動式校訂解析度</a>中所述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">尺寸</td> 
      <td>指定要用於此裝置的尺寸。 使用者可以看到裝置名稱下方顯示的維度。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">比例</td> 
      <td>指定裝置的比例。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">類型</td> 
      <td>選取裝置為行動裝置、平板電腦或桌上型電腦。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">使用者代理字串</td> 
      <td>輸入裝置的使用者代理程式，以提供讓我們的軟體按照裝置設計執行及顯示的資訊。<p>您可以從裝置前往<a href="https://www.whatismybrowser.com/detect/what-is-my-user-agent">https://www.whatismybrowser.com/detect/what-is-my-user-agent</a>取得使用者代理程式。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">已停用</td> 
      <td>如果選取此選項，使用者檢閱互動式校樣時，將無法選取裝置。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**建立**」。

## 設定校樣的快顯訊息

您可以設定校樣上的快顯訊息，將一般資訊傳達給組織中的所有稽核者。

您可以設定要在下列情況下顯示的訊息：

* **載入訊息**：在校訂首次開啟時顯示。 適用於向使用者說明如何檢閱校樣或提供免責宣告或其他法律文字。
* **在決定訊息**&#x200B;上：當使用者在校訂上選取決定時顯示。 非常實用，可為您的使用者提供品牌或法規遵循等專案的核對清單。 如需決定的相關資訊，請參閱[在校訂檢視器中對校訂做出決定](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)。

* **確認按鈕文字**：在上述「載入時」快顯訊息的按鈕上顯示的標籤。

若要為校樣建立快顯訊息：

1. 按一下您要自訂之訊息右側的&#x200B;**編輯**。
1. 指定訊息並包含適當的格式，然後按一下[儲存]。****
1. （選擇性）如果您自訂[載入時]訊息，而且您想要自訂確認按鈕標籤，請按一下&#x200B;**確認按鈕文字**&#x200B;右側的&#x200B;**編輯**，指定標籤，然後按一下&#x200B;**儲存**。

## 設定校訂預設值

如需有關設定組織校訂預設值的資訊，請參閱[設定預設校訂設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md)。


## 設定共用預設值

您可以指定可與誰共用您組織的校訂、哪些版本可供檢閱者使用，以及與指定階段相關聯的使用者何時可看到具有自動化工作流程的校訂。

如需在Workfront Proof中共用設定的詳細資訊，請參閱[設定使用者的共用設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md)。

## 為Workfront Proof網站建立品牌

如果您使用Workfront Proof，您可以為網站的下列區域設定品牌：

* 載入校訂時顯示的啟動顯示頁面
* 登入和登出畫面
* 電子郵件通知

如需如何品牌化Workfront Proof網站的詳細資訊，請參閱[品牌化Workfront Proof網站](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md)。

## 設定進階密碼設定

>[!IMPORTANT]
>
>此選項僅適用於舊版Workfront計畫。 如果您使用Pro、Business或Enterprise Workfront計畫，就無法再設定進階密碼設定。

在&#x200B;**進階密碼設定**&#x200B;下，您可以增強使用者的密碼安全性。

1. 按一下您要設定的右側&#x200B;**設定**：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">密碼長度下限</td> 
      <td>預設Workfront Proof密碼長度為6個字元。 您可能想要根據組織的原則增加數量。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>字元組合</strong> </td> 
      <td>您可以強制使用者在其密碼中混合使用小寫、大寫、數字和符號。 您可以決定密碼應包含多少個字元。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>重複字元數上限</strong> </td> 
      <td>您可以指定每個使用者密碼中可重複使用的字元數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自動密碼過時</td> 
      <td>強制使用者定期變更密碼。 由您決定他們執行此動作的頻率。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不允許密碼重複次數</strong> </td> 
      <td>設定您的帳戶中不允許的密碼重複次數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>設定檔鎖定</strong> </td> 
      <td>在您指定的幾次失敗登入嘗試後，將您的使用者鎖定在帳戶之外。 您也可以指定使用者要等候多久才能再次存取帳戶。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">若密碼未在30天後重設，則鎖定使用者</td> 
      <td>如果您的使用者未在啟動設定檔後30天內變更其初始密碼，則他們將被鎖定在帳戶之外。<br><p>帳戶管理員可解除鎖定系統自動鎖定的使用者（重新啟用）。 這將讓他們額外獲得七天的時間來變更密碼。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">若非使用中達120天，則鎖定使用者帳戶</td> 
      <td>如果您的使用者120天未登入Workfront Proof或需要登入的校訂，則他們將被鎖定在帳戶之外。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>第一次登入後變更密碼</strong> </td> 
      <td>要求使用者在首次登入後變更其暫時密碼。<p>帳戶管理員可以解除鎖定系統自動鎖定的使用者（重新啟用）。</p><p>如需密碼資訊，請參閱<a href="../../../workfront-proof/wp-getstarted/faqs/log-in-change-password.md" class="MCXref xref">登入並變更Workfront Proof的密碼和電子郵件</a>。</p></td> 
     </tr> 
    </tbody> 
   </table>
