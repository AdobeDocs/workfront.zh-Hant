---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 為文檔建立校樣
description: 您可以在將檔案上傳至Workfront時產生檔案校樣。
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 為文檔建立校樣

您可以在將檔案上傳至Workfront時產生檔案校樣。

您也可以為已在Adobe Workfront中上傳的檔案或已在Workfront中的校樣新版本產生校樣。

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Select或Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>管理員或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 上傳檔案並建立校樣

1. 轉到要建立新校樣的項目、任務或問題。
1. 按一下 **檔案** 標籤。
1. 按一下「文檔」 ![](assets/document-icon.png) 中。
1. 按一下 **新增**，然後按一下 **校樣** 中。

   >[!TIP]
   >
   >您可以啟用 **上傳檔案時自動產生校樣** 在您的使用者設定檔中設定，以自動化此程式。 如需詳細資訊，請參閱 [配置我的設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. 在 **新校樣** 頁面，您

   * [使用基本工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自動化工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## 上傳檔案並建立新版校樣

1. 轉到要建立現有校樣的新版本的項目、任務或問題。
1. 按一下 **檔案** 標籤。
1. 選擇要添加新版本的文檔。
1. 按一下 **新增** > **版本** > **校樣**.
1. 在 **新校樣版本** 頁面，您

   * [使用基本工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自動化工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## 使用拖放功能，為新版本產生簡單的校樣

您可以從檔案系統（如案頭）拖放檔案，以建立新校樣或現有校樣的新版本。 校樣包含下列設定，視您要建立新校樣還是新版本而定：

* **新校樣：** 建立僅與您共用的簡單校樣。 校樣建立後，您可以依照 [編輯校樣設定](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **現有校樣的新版本：** 使用與上一版相同的校樣設定建立新版本。

若要使用拖放功能產生新的校樣或新校樣版本：

1. 請確定校樣已設定為自動產生，如中所述。
1. 繼續  [從您的檔案系統將檔案新增至Adobe Workfront](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)，說明新增檔案的拖放方法。 

## 為現有文檔建立校樣

1. 前往您要校樣的專案、任務或問題，然後按一下 **檔案** 區段。
1. 將滑鼠指標暫留在檔案上，然後按一下 **建立校樣** 顯示在文檔名稱下方的連結。

   >[!NOTE]
   >
   >若您有 **上傳檔案時自動產生校樣** 系統會在您的使用者設定檔中啟用，自動建立簡單校樣。

1. 選擇以下選項之一：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">簡單校樣</td> 
      <td>此選項會建立校樣而不附加任何工作流程，並套用預設校樣設定。 您可以在建立校樣後更新預設校樣設定或新增工作流程。 如需校樣設定的詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">編輯校樣設定</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進階校樣</td> 
      <td> <p>此選項可讓您設定基本或進階工作流程，並修改您建立校樣的校樣設定。 如需詳細資訊，請參閱 </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">使用基本工作流程建立進階校樣</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">使用自動化工作流程建立進階校樣</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
