---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 為貴組織安裝案頭校對檢視器
description: 案頭校對檢視器主要是為校對互動式內容而設計，是必須安裝在每個使用者本機電腦上的應用程式。 您可以是Adobe Workfront管理員或Workfront Proof管理員，執行此安裝。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 58f976d9f4245e528a4ddf23d39b92d9fa405311
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# 為貴組織安裝案頭校對檢視器

案頭校對檢視器主要是為校對互動式內容而設計，是必須安裝在每個使用者本機電腦上的應用程式。 您可以是Adobe Workfront管理員或Workfront Proof管理員，執行此安裝。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Premium或Select</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須在校樣權限設定檔中選取管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">設定使用者的校對存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 系統需求

下列作業系統支援案頭校對檢視器：

* Windows 7及更新版本、32位元和64位元
* Mac OS X 10.9和更新版本，64位元

## 必要條件

若要讓使用者使用案頭校對檢視器，您必須

* 在安裝之前，將系統配置為將案頭校對查看器作為互動式校樣的預設視圖。

## 將案頭校對檢視器設定為互動式校樣的預設值

為貴組織安裝案頭校對檢視器後，您可以將其設為互動式校樣的預設檢視器。

1. 在Workfront中，按一下主功能表 ![](assets/main-menu-icon.png)，然後按一下「校對」 ![](assets/proofing-in-main-menu.png) 存取Workfront校樣。

1. 按一下 **帳戶設定** 在Workfront Proof的右上角附近，按一下 **設定**&#x200B;標籤。

1. 在 **校樣預設值**，在 **互動式校樣的案頭校樣檢視器** 列，按一下 **設定**.

   ![](assets/proof-defaults-350x265.png)

1. 按一下 **啟用和預設**，然後按一下 **儲存**.

## 為用戶安裝案頭校對查看器

* [在Mac上安裝案頭校對檢視器](#installing-the-desktop-proofing-viewer-on-mac)
* [在Windows上安裝案頭校對檢視器](#installing-the-desktop-proofing-viewer-on-windows)

### 在Mac上安裝案頭校對檢視器 {#installing-the-desktop-proofing-viewer-on-mac}

1. 在使用者的電腦上，執行下列其中一項操作來下載應用程式：

   * 如果您使用的是生產環境，請按一下  [Mac Production Download for the Desktop Prooding Viewer（案頭校對檢視器的生產下載）。](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg)
   * 如果您使用預覽環境，請按一下  [Mac案頭校對檢視器的預覽下載。](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg)
)

1. 開啟剛下載的檔案以開始安裝。
1. 在出現的安裝方塊中，按一下 **繼續**，然後按一下 **安裝**.

   ![00000776.png](assets/00000776-350x244.png)

1. 從Workfront的「檔案」區域開啟互動式校樣，確保每位使用者都能完成安裝。

### 在Windows上安裝案頭校對檢視器 {#installing-the-desktop-proofing-viewer-on-windows}

1. 在使用者的電腦上，執行下列其中一項操作來下載應用程式：

   * 在「生產」環境中，按一下 [用於案頭校對查看器的Windows生產下載。](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe)
   * 在預覽環境中，按一下 [案頭校對查看器的Windows預覽下載](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. 開啟剛下載的檔案以開始安裝。
1. 在出現的安全性警告方塊中，按一下 **執行**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   案頭校對查看器安裝並運行。

1. （條件性）如果您使用Internet Explorer安裝應用程式，請在應用程式安裝後，重新整理瀏覽器中的啟動頁面。
1. 從Workfront的「檔案」區域開啟互動式校樣，確保每位使用者都能完成安裝。
