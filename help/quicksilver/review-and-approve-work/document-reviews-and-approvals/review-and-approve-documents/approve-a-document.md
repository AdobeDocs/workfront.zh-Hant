---
product-area: projects
navigation-topic: approvals
title: 在Workfront中核准檔案
description: 如果您被指派為檔案的核准者，則您有多種方式可以做出核准決定。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# 在Workfront中核准檔案

如果您被指派為檔案的核准者，則您有多種方式可以做出核准決定。

如需有關建立新檔案核准的資訊，請參閱[建立檔案稽核或核准要求](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。

>[!IMPORTANT]
>
>本文內容指的更新檔案核准功能僅適用於特定帳戶。 如需有關標準核准程式的資訊，請參閱[工作核准](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)中列出的文章。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>投稿人或以上</p>
   <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視與核准關聯的物件或更高的存取許可權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視與核准相關聯的物件或更高許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從首頁核准檔案

1. 按一下Adobe Workfront左上角的&#x200B;**首頁**&#x200B;圖示![首頁圖示](../assets/home-icon-30x29.png)。

   >[!NOTE]
   >
   >您的Workfront管理員可能會對您環境中的「首頁」圖示進行下列變更：
   >
   >* 以自訂的影像取代，以說明您的組織。 在此情況下，圖示看起來將會與本文中顯示的有所不同。
   >
   >* 使用其他頁面取代連結至該頁面的頁面。 在此情況下，請按一下頁面右上角的&#x200B;**主功能表** ![主功能表圖示](../assets/main-menu-icon.png)，然後按一下&#x200B;**首頁**。

1. 按一下頁面左上方的&#x200B;**篩選器**，並確定已勾選&#x200B;**核准**。

   需要您核准的所有工作專案都會顯示在清單中。

   >[!NOTE]
   >
   >* 指派給工作角色或群組的核准未列在首頁中。
   >* 指派給團隊的核准會顯示在「首頁」中每個個別團隊成員的「我的核准」小工具中。

1. 在清單中按一下要作出核准決定的檔案核准。 有關核准的資訊將顯示在頁面右側。

1. 按一下頁面右上角的以下兩個核准選項之一：

   * **核准**&#x200B;下拉式清單包含兩個選項：

      * **核准**&#x200B;表示此版本的檔案不需要變更，且已獲得核准。

      * **核准變更**&#x200B;表示檔案上仍需要一些小變更，但核准條件為進行這些變更。 如果選取此選項，將會出現一個視窗，其中包含名為&#x200B;**後續步驟**&#x200B;的文字方塊，您可以在其中指定要核准檔案所需的變更。 您可以輸入該資訊並按一下[新增訊息]****，或按一下[略過]**以傳送核准決定，而不需要其他資訊。**

   * **需要工作**&#x200B;表示檔案版本未核准，需要重大變更。

   在首頁檢視檔案核準時，請考慮下列事項：

   * 要求核准的使用者名稱會顯示在「首頁」的檔名稱上方，文字為「*使用者A*&#x200B;希望您核准於……」，以及在選取核准後右側顯示的核准資訊中&#x200B;**提交者**&#x200B;下。

   * 對核准做出決定後，核准會保留在「我的核准」標籤中，並顯示「已做出決定」文字，直到您按一下&#x200B;**重新整理**&#x200B;按鈕或重新整理瀏覽器頁面為止。

## 從檔案頁面核准檔案

1. 按一下檔名稱，移至檔案頁面。

1. 在檔名稱旁的版本下拉式清單中，選取擱置核准的檔案版本。 預設會選取最新版本。

   如果目前選取的檔案版本有您未決的核准，則核准決定按鈕會顯示在頁面的右上角；如果其他版本的檔案有您未決的核准，則版本下拉式選單會顯示紅點。

   <!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. 按一下頁面右上角的以下兩個核准選項之一：

   * **核准**&#x200B;下拉式清單包含兩個選項：

      * **核准**&#x200B;表示此版本的檔案不需要變更，且已獲得核准。

      * **核准變更**&#x200B;表示檔案上仍需要一些小變更，但核准條件為進行這些變更。 如果選取此選項，將會出現一個視窗，其中包含名為&#x200B;**後續步驟**&#x200B;的文字方塊，您可以在其中指定要核准檔案所需的變更。 您可以輸入該資訊並按一下[新增訊息]****，或按一下[略過]**以傳送核准決定，而不需要其他資訊。**

   * **需要工作**&#x200B;表示檔案版本未核准，需要重大變更。

## 從檔案摘要面板核准檔案

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。

1. 按一下需要您核准的檔案，檔案摘要面板隨即開啟。

1. 在版本下拉式清單中選取您要檢閱的檔案版本。 預設會選取最新版本。

   如果目前選取的檔案版本有您未決的核准，則核准決定按鈕會顯示在「檔案摘要」面板的右上角；如果其他版本的檔案有您未決的核准，則版本下拉式選單會顯示紅點。
<!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
 -->
1. 在「檔案摘要」面板的右上角，按一下以下兩個核准選項之一：

   * **核准**&#x200B;下拉式清單包含兩個選項：

      * **核准**&#x200B;表示此版本的檔案不需要變更，且已獲得核准。

      * **核准變更**&#x200B;表示檔案上仍需要一些小變更，但核准條件為進行這些變更。 如果選取此選項，將會出現一個視窗，其中包含名為&#x200B;**後續步驟**&#x200B;的文字方塊，您可以在其中指定要核准檔案所需的變更。 您可以輸入該資訊並按一下[新增訊息]****，或按一下[略過]**以傳送核准決定，而不需要其他資訊。**

   * **需要工作**&#x200B;表示檔案版本未核准，需要重大變更。


## 從校訂檢視器核准檔案

若要檢閱及核准檔案，請執行下列動作：

1. 前往檢閱電子郵件通知，然後按一下&#x200B;**前往檢閱**。

1. 進入Workfront後，按一下&#x200B;**前往校訂**。

1. 檢閱內容，並新增任何註解或標示。 如需如何使用校訂檢視器的詳細資訊，請參閱[在Adobe Workfront中檢閱校訂：文章索引](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)。

1. 選擇下列其中一項決定：

   * **核准**：檔案不需要變更，且已可供使用。
   * **核准變更**：檔案需要變更，而且一旦完成變更即可使用。 不需要額外核准。
   * **需要工作**：檔案需要變更，而且尚未準備好使用。 完成指定的變更後，檔案必須上傳為新版本，並經過另一輪核准。 如需上傳新版本的詳細資訊，請參閱本文中的[視需要建立新版本](#create-a-new-version-as-needed)。

做出決定後，檔案所有者會透過電子郵件收到通知。


