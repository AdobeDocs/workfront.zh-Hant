---
product-area: documents
navigation-topic: manage-documents
title: 檢查檔案儲存限制
description: 身為Adobe Workfront管理員，您可在客戶資訊頁面上檢視檔案儲存使用量和配額。 儲存空間的顯示方式取決於您的組織是使用舊版Workfront儲存空間或Adobe雲端儲存空間。
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/vOjgBLxX5rFIGHBCHB2a6Q3Bs3KE5x-opXUMvANjI1E
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 09dff59503604894e61f2a62af7ae1c2e8a39068
workflow-type: tm+mt
source-wordcount: 491
ht-degree: 3%

---

# 檢查檔案儲存限制

雖然使用者可上傳至您的Workfront執行個體的個別檔案型別和大小沒有限制，但您的Workfront計畫包含總儲存配額。 身為Workfront管理員，您可以從「客戶資訊」頁面的「設定」區域監控使用情況和配額。

儲存空間的顯示方式取決於您的組織是使用舊版Workfront儲存空間或Adobe雲端儲存空間：

* 如果您使用舊版Workfront儲存空間，請參閱本文中的[舊版Workfront儲存空間](#legacy-workfront-storage)。
* 如果您使用Adobe雲端儲存空間，請參閱本文中的[Adobe雲端儲存空間](#adobe-cloud-storage)。

  如需Adobe雲端儲存空間的詳細資訊，請參閱[Adobe雲端儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Workfront計畫</td> 
   <td> <p>使用舊版儲存空間管理檔案的任何Workfront套件</p>
      <p>使用Adobe雲端儲存空間管理檔案的任何Workflow套件</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>您必須是Workfront管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 舊版 Workfront 儲存空間

如果您的組織使用舊版Workfront儲存空間，客戶資訊頁面會顯示直接上傳至Workfront的檔案的單一儲存配額。

若要檢查舊版Workfront檔案儲存：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**系統** > **客戶資訊**。
1. 在&#x200B;**基本資訊**&#x200B;區段中，尋找&#x200B;**儲存配額**。 在這裡，您可以檢視目前使用的儲存空間，以及Workfront計畫中包含的儲存空間總數。

儲存配額會每天重新整理，以顯示最新的計數。

>[!NOTE]
>
>此限制不適用於您從任何其他第三方服務提供者（SharePoint、Google Drive、Webdam、Box、Dropbox或任何其他檔案資產管理提供者）連結至Workfront的檔案。

## Adobe 雲端儲存空間


如果您的組織使用Adobe雲端儲存空間，您的儲存配額會報告為單一集區配置，其結合透過Workfront授權布建的儲存空間以及透過Frame.io Enterprise附加元件布建的任何儲存空間。 儲存空間使用量沒有硬性上限；即使使用量超過您的配額，使用者也可以繼續上傳檔案。

### 檢視客戶資訊的儲存空間使用量

若要檢查檔案的Adobe雲端儲存空間：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**系統** > **客戶資訊**。
1. 移至&#x200B;**儲存概述**&#x200B;區段。
1. 檢閱您的使用情形。 「儲存空間概覽」會顯示您的集區儲存空間配額，並將使用量分為：

   * Workfront舊版專案和Adobe雲端儲存空間專案會顯示在藍色列中。
   * 框架獨立專案會以綠色列顯示。 這些專案與Workfront不同，僅在您擁有Frame.io Enterprise授權時可用。


![客戶資訊上的Adobe雲端儲存空間使用量](assets/storage-usage.png)

使用量數字會定期重新整理，以便您檢視最新計數。

### 給管理員的電子郵件通知

當使用量超過儲存配額的75%、90%或100%時，Workfront會傳送電子郵件通知給系統管理員。
