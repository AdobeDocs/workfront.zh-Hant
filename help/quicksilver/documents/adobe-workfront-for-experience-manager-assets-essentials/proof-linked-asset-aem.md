---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 校訂Experience Manager Assets或Assets Essentials的連結資產
description: 從Experience Manager Assets Essentials連結資產後，您可以建立校訂並指派使用者以在資產中檢閱和新增評論。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 5d818b2e3c3314c6af076df46f7f806214f97bab
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 1%

---

# 校訂Experience Manager Assets或Assets Essentials的連結資產

從Experience Manager Assets Essentials連結資產後，您可以建立校訂並指派使用者以在資產中檢閱和新增評論。

## 存取需求

<!-- Audited: 4/2025 -->

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：工作或以上</p>
   <p>您必須為使用者啟用校樣。</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您必須擁有Experience Manager as a Cloud Service或Assets Essentials，並且您必須在Admin Console中作為使用者新增到產品中。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視存取許可權或更高</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前：

* 您的Workfront管理員必須設定Experience Manager整合。 如需詳細資訊，請參閱[設定Experience Manager Assets as a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[設定Experience Manager Assets Essentials整合](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。

## 建立校樣

您可以建立靜態、視訊或互動式校樣。

若要建立校訂：

1. 前往您要校訂的專案、任務或問題，然後按一下「**檔案**」區段。
1. 暫留在檔案上，然後按一下出現在檔名稱下方的&#x200B;**建立校訂**&#x200B;連結。

   >[!NOTE]
   >
   >如果您在使用者設定檔中啟用&#x200B;**上傳檔案時自動產生校訂**，則系統會自動建立簡易校訂。

1. 從下拉式清單中選擇下列其中一項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>簡單校訂</strong></td> 
      <td>此選項會建立未附加工作流程的校訂，並套用預設校訂設定。 您可以更新預設校訂設定，或在建立校訂後新增工作流程。 如需校訂設定的詳細資訊，請參閱<a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">編輯校訂設定</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>進階校訂</strong></td> 
      <td> <p>此選項可讓您設定基本或進階工作流程，並修改您建立之校訂的校訂設定。 如需詳細資訊，請參閱： </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">使用基本工作流程建立進階校訂</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">使用自動化工作流程建立進階校訂</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## 管理現有校訂

建立校訂後，您可以執行以下操作：

* 檢視目前階段活動
* 更新稽核者和截止日期
* 編輯工作流程

如需有關如何管理現有校訂的詳細資訊，請參閱[在Adobe Workfront中管理校訂：文章索引](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md)。

## 檢閱校訂

指派的稽核者可以執行下列動作：

* 檢視資產並進行註解
* 將動作新增至註解
* 比較版本
* 核准或拒絕證明

如需校訂工具可執行的詳細資訊，請參閱[在Adobe Workfront中檢閱校訂：文章索引](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)。
