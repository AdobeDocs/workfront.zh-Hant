---
product-area: projects
navigation-topic: approvals
title: 核准檔案
description: 如果您被指派為檔案的核准者，則有多種方式可以做出核准決定。
author: Nolan
feature: Work Management
source-git-commit: 967e599376714c600d4c920582938a90d8399dc0
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---


# 核准檔案

如果您被指派為檔案的核准者，則有多種方式可以做出核准決定。

如需有關建立新檔案核准的資訊，請參閱 [建立檔案核准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>本文內容指的更新檔案核准功能僅適用於特定帳戶。 如需有關標準核准流程的資訊，請參閱下列文章： [工作核准](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視與核准相關聯的物件或更高存取權</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視與核准相關聯之物件的或更高許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 從首頁核准檔案

1. 按一下 **首頁** 圖示 ![](../assets/home-icon-30x29.png) Adobe Workfront左上角。

   >[!NOTE]
   >
   >您的Workfront管理員可能會對您環境中的「首頁」圖示進行下列變更：
   >
   >* 以自訂的影像取代，以說明您的組織。 在此情況下，圖示看起來將會與本文中所顯示的有所不同。
   >
   >* 以其他頁面取代連結至該頁面的頁面。 在此情況下，請按一下 **主要功能表** ![](../assets/main-menu-icon.png) 然後按一下「 」 **首頁**.

1. 按一下 **篩選器** ，並確保 **核准** 已勾選。

   清單中會顯示需要您核准的所有工作專案。

   >[!NOTE]
   >
   >指派給工作角色或群組的核准未列在首頁中。 指派給專案團隊的核准會顯示在工作清單的專案團隊請求分組中。

1. 在清單中按一下您要對其做出核准決定的檔案核准。 有關核准的資訊將顯示在頁面右側。

1. 按一下頁面右上角的以下兩個核准選項之一：

   * 此 **核准** 下拉式清單包含兩個選項：

      * **核准** 表示此檔案版本不需要變更，且已獲得核准。

      * **核准，但有變更** 表示檔案上仍需要一些小變更，但在進行這些變更的條件下會提供核准。 如果您選取此選項，將會出現一個視窗，其中包含名為的文字方塊 **後續步驟** 您可以在此指定要核准檔案所需的變更。 您可以輸入該資訊，然後按一下 **新增訊息**，或您可以按一下 **略過** 傳送核准決定，而不需要其他資訊。

   * **需要工作** 表示檔案版本未核准，且需要重大變更。

   在首頁檢視檔案核準時，請考量下列事項：

   * 請求核准的使用者名稱顯示在首頁的檔名稱上方，並帶有文字&quot;*使用者A* 希望您核准於……」，以及在 **提交者** 在選取核准後右側顯示的核准資訊中。

   * 對核准做出決定後，核准會保留在我的核准索引標籤中，並帶有文字「已做出決定」，直到您按一下 **重新整理** 按鈕，或直到您重新整理瀏覽器頁面為止。

## 從檔案頁面核准檔案

1. 按一下檔名稱，前往檔案頁面。

1. 在檔名稱旁的版本下拉式清單中，選取擱置核准的檔案版本。 預設會選取最新版本。

   如果目前選取的檔案版本有您未決的核准，則核准決定按鈕會顯示在頁面的右上角；如果其他版本的檔案有您未決的核准，則版本下拉式選單會顯示紅點。

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. 按一下頁面右上角的以下兩個核准選項之一：

   * 此 **核准** 下拉式清單包含兩個選項：

      * **核准** 表示此檔案版本不需要變更，且已獲得核准。

      * **核准，但有變更** 表示檔案上仍需要一些小變更，但在進行這些變更的條件下會提供核准。 如果您選取此選項，將會出現一個視窗，其中包含名為的文字方塊 **後續步驟** 您可以在此指定要核准檔案所需的變更。 您可以輸入該資訊，然後按一下 **新增訊息**，或您可以按一下 **略過** 傳送核准決定，而不需要其他資訊。

   * **需要工作** 表示檔案版本未核准，且需要重大變更。

## 從[檔案摘要]窗格核准檔案

1. 前往包含檔案的專案、任務或問題，然後選取 **檔案**.

1. 按一下需要您核准的檔案，檔案摘要窗格隨即開啟。

1. 在版本下拉式清單中選取您要檢閱的檔案版本。 預設會選取最新版本。

   如果目前選取的檔案版本有您未決的核准，則核准決定按鈕會顯示在「檔案摘要」窗格的右上角；如果其他版本的檔案有您未決的核准，則版本下拉式選單會顯示紅點。

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. 在「檔案摘要」窗格的右上角，按一下下列兩個核准選項之一：

   * 此 **核准** 下拉式清單包含兩個選項：

      * **核准** 表示此檔案版本不需要變更，且已獲得核准。

      * **核准，但有變更** 表示檔案上仍需要一些小變更，但在進行這些變更的條件下會提供核准。 如果您選取此選項，將會出現一個視窗，其中包含名為的文字方塊 **後續步驟** 您可以在此指定要核准檔案所需的變更。 您可以輸入該資訊，然後按一下 **新增訊息**，或您可以按一下 **略過** 傳送核准決定，而不需要其他資訊。

   * **需要工作** 表示檔案版本未核准，且需要重大變更。