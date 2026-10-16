---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: 將舊版物件轉換為Adobe雲端儲存空間
description: 瞭解您可以將舊版Workfront儲存物件轉換成Adobe雲端儲存的三種情況，並瞭解每次轉換期間的移動和內容。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---
# 將舊版物件轉換為Adobe雲端儲存空間

在大多數案例中，您只能在類似儲存模式之間移動、複製和轉換Workfront物件。 例如，您可以將任務從一個Adobe雲端儲存空間專案移動至另一個Adobe雲端儲存空間專案。 在三種特定情況下，您可以將舊版Workfront儲存體物件轉換為Adobe雲端儲存體：

* 將舊版Workfront儲存空間任務轉換為Adobe雲端儲存空間專案
* 將舊版Workfront儲存產品組合轉換為Adobe雲端儲存產品組合
* 從舊版Adobe儲存空間範本建立Workfront雲端儲存空間專案

如需移動方向以及Adobe雲端儲存空間上的不同之處，請參閱[在Adobe雲端儲存空間上移至Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)。

<!-- 
need to validate with PM
>[!NOTE]
>
>In all three conversion scenarios, documents and document folders don't move from legacy Workfront storage to Adobe cloud storage. Documents that exist on the legacy object before the conversion remain on legacy storage.
-->

## 將舊版任務轉換為Adobe雲端儲存空間專案

若要將舊版Workfront儲存體任務轉換為Adobe雲端儲存體專案，請在該任務上使用現有的轉換至專案流程。 轉換期間：

* 子任務和問題移至新專案。
* 附加到任務的檔案及其核准工作流程會保留在原始專案上。
* 已移除工作核准和解析物件連結。
* 已刪除原始任務。

## 將舊版產品組合轉換為Adobe雲端儲存產品組合

Workfront管理員可從「設定」區域將舊版Workfront儲存產品組合轉換為Adobe雲端儲存產品組合。 轉換後：

* 您無法再將舊版Workfront儲存專案移至產品組合。
* 產品組合中建立的所有新專案都會使用Adobe雲端儲存空間。
* Frame.io是產品組合Adobe雲端儲存空間專案中檔案的檢視器。
* 使用舊版Workfront儲存空間的子專案會保留在舊版儲存空間。
* 子程式會保留在舊版儲存空間。

>[!NOTE]
>
>只有有人手動將Adobe雲端儲存空間專案新增至子舊版計畫時，才會自動轉換成Adobe雲端儲存空間。

如需詳細資訊，請參閱[將舊版產品組合轉換為Adobe雲端儲存空間](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md)。

## 從舊版範本建立Adobe雲端儲存空間專案

當您從舊版Workfront儲存範本建立專案時，專案建立對話方塊中的&#x200B;**在Adobe雲端儲存空間上建立此專案**&#x200B;核取方塊會決定新專案的儲存型別。 核取方塊行為取決於您建立專案的位置：

* **在投資組合外**：預設會提供並清除核取方塊。 選取它以在Adobe雲端儲存空間上建立新專案。
* **在Adobe雲端儲存產品組合內**：核取方塊已選取並鎖定。 新專案必須符合產品組合的儲存型別。
* **在舊版Workfront儲存產品組合中**：無法使用核取方塊。 新專案使用舊版Workfront儲存空間。

如需詳細資訊，請參閱[建立專案](/help/quicksilver/manage-work/projects/create-projects/create-project.md)。
