---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 校樣Experience Manager Assets或Assets Essentials的連結資產
description: 從Experience Manager Assets Essentials連結資產後，您可以建立校樣並指派使用者以檢閱並新增註解至資產。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 3b063899c5c7992aad71d1eb8c8fafff7fda84c3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# 校樣Experience Manager Assets或Assets Essentials的連結資產

從Experience Manager Assets Essentials連結資產後，您可以建立校樣並指派使用者以檢閱並新增註解至資產。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或更高</p>
   <p>您必須為使用者啟用校對功能。</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您必須有Experience Manageras a Cloud Service或Assets Essentials，且您必須以Admin Console使用者身分新增至產品。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看訪問權限或更高版本</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，

* 您的Workfront管理員必須設定Experience Manager整合。 如需詳細資訊，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## 建立校訂

您可以建立靜態、視訊或互動式校樣。

建立校樣：

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
      <td role="rowheader"><strong>簡單校樣</strong></td> 
      <td>此選項會建立校樣而不附加任何工作流程，並套用預設校樣設定。 您可以在建立校樣後更新預設校樣設定或新增工作流程。 如需校樣設定的詳細資訊，請參閱 <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">編輯校樣設定</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>進階校樣</strong></td> 
      <td> <p>此選項可讓您設定基本或進階工作流程，並修改您建立校樣的校樣設定。 如需詳細資訊，請參閱 </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">使用基本工作流程建立進階校樣</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">使用自動化工作流程建立進階校樣</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## 管理現有校樣

一旦建立了校樣，您就可以

* 查看當前階段活動
* 更新審核者和截止日期
* 編輯工作流程

如需如何管理現有校樣的詳細資訊，請參閱 [在Adobe Workfront中管理校樣](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## 檢閱證明

指派的審核者可以執行

* 檢視資產並提供意見
* 新增動作至註解
* 比較版本
* 批准或拒絕校樣

如需關於您可以使用校對工具的詳細資訊，請參閱 [在Adobe Workfront中檢閱校樣](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
