---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在中檢視校樣的進度和狀態 [!DNL Workfront Proof]
description: 校樣進度表示從您將校樣傳送給審核者，到他們決定校樣所完成的校樣工作。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 8fd85595-1403-490e-9d52-2ba5b01457b7
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 1%

---

# 在中檢視校樣的進度和狀態 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

## 了解證明進度

校樣進度表示從您將校樣傳送給審核者，到他們決定校樣所完成的校樣工作。

* [進度表徵圖](#progress-icons)
* [校樣進度等級](#levels-of-proof-progress)

### 進度表徵圖 {#progress-icons}

進度表徵圖S、O、C和D顯示在進度欄中，指示校樣進度。

![proof_edit_existing_progress.png](assets/proof-edit-existing-progress-350x78.png)

它們會指出下列關於證明的資訊：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>進度圖示</strong> </p> </td> 
   <td> <p><strong>說明</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt="proof_progress_sent_icon.png"> </p> </td> 
   <td> <p><strong>已傳送</strong>. 校樣已傳送給審核者。</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-opened-icon.png" alt="proof_progress_opened_icon.png"> </p> <p> </p> </td> 
   <td> <p><strong>已開啟</strong>. 審核者已開啟「校樣」詳細資訊頁面，或在校樣檢視器中開啟校樣本身。</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-comment-icon.png" alt="proof_progress_comment_icon.png"> </p> </td> 
   <td> <p><strong>註解</strong>. 審核者（可評論的使用者）已對校樣發表意見。</p> <p>如果沒有為校樣指定審核者，則不會顯示此表徵圖。</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt="proof_progress_decision_icon.png"> </p> </td> 
   <td> <p><strong>決定</strong>. 審核者已就證明作出決定。</p> <p>如果未為校樣指定批准者（決策者），則不會顯示此表徵圖。 </p> </td> 
  </tr> 
 </tbody> 
</table>

這些圖示可以以下列顏色顯示，以指出校樣進度的特定資訊：

* **綠色**. 已完成.
* **白色**. 未完成。
* **橙色**. 未完成，截止時間小於24小時。
* **紅色**. 沒有完成，而且超過了期限。

### 校樣進度等級 {#levels-of-proof-progress}

Workfront Proof使用進度圖示來追蹤下列每個層級的校樣進度：

* 根據該人對校樣的活動，對每位審核者。
* 對於每個階段，根據測試流程中落後最多的階段審核者的進度。 如需詳細資訊，請參閱 [自動化工作流階段概觀](../../../review-and-approve-work/proofing/proofing-overview/stages.md).
* 對於校樣，根據測試階段（審閱者組）的進度，在校樣過程中最落後。

以取得 [!DNL Workfront Proof] 使用最落後的審核者或階段確定進度，假設有三名審核者需要做出決定。 如果其中兩人已做出決定，但第三人未做出決定，則證明的進度條不會因為未決決定而以綠色顯示D。

若 [!UICONTROL 主要決策者] 在校樣上選擇設定，主決策者提交決策，校樣進度條中的D對所有審閱者變為綠色，因為不需要其他決策。

同樣地，如果 [!UICONTROL 只需一個決定] 在校樣上選取設定，且任何審核者都提交決定，因此校樣進度列中的D會對所有審核者變成綠色，因為不需要其他決定。

## 了解校樣狀態

校樣狀態會顯示校樣所需的決策狀態。

![proof_edit_existing_status.png](assets/proof-edit-existing-status-350x78.png)\
標準狀態選項為：

* 未決
* 已核准
* 變更已核准
* 需要的更改
* 無關

如果您的帳戶已設定自訂決策，狀態選項會反映您的自訂決策設定。

校樣的狀態由「最壞案例」參與者驅動。 例如，假設對證明有三個決定：兩個的狀態為 **已接受** 其中一個的狀態為 **已拒絕**. 被拒絕的「最壞情況」決定對其他決定和證明的整體狀態顯示為 **已拒絕**.

## 查看進度和狀態 {#viewing-progress-and-status}

您可以查看每個階段的校樣、階段和審核者的進度和狀態。

* [校樣摘要](#proof-summary)
* [舞台操作菜單](#stage-actions-menu)
* [在 [!UICONTROL 摘要] 區段中，如果您對校樣具有編輯權限，則也可以訪問審核者操作菜單。 如需詳細資訊，請參閱Workfront校樣中的校樣權限設定檔和Workfront Proof中的管理校樣角色。 此 [!UICONTROL 審核者動作] 菜單(1)將游標暫留在「審閱者」的詳細資訊上，並允許您：](#in-the-summary-section-you-can-also-access-the-reviewer-actions-menus-provided-you-have-edit-rights-on-the-proof-for-more-information-see-proof-permissions-profiles-in-workfront-proof-and-manage-proof-roles-in-workfront-proof-the-reviewer-actions-menu-1-appears-when-you-hover-over-the-reviewer-s-details-and-allows-you-to)
* [校樣動作功能表](#proof-actions-menu)

### 校樣摘要 {#proof-summary}

資料夾中的每個校樣都有可展開的摘要，可讓您快速檢視及編輯校樣的詳細資訊。

要展開或折疊摘要，請執行以下操作：

1. 在控制面板或任何清單檢視中，按一下校樣左側的箭頭。

![Summary_expandable.png](assets/summary-expandable-350x68.png)

摘要包括下列項目：

* 工作流程(2)
* 版本(3)
* 資料夾(4)
* 國家(5)\
   ![summary_2.png](assets/summary-2-350x160.png)

在摘要中，您可以檢視及編輯下列校樣的詳細資訊：

* 證明進度(1)
* 各階段的進展(2)
* 為階段(3)設定的最後期限
* 審核者詳細資訊：

   * 每個審核者的評論和答複數目(4)
   * 每個審閱者的進度(5)
   * 決策（如果決定包含電子簽名，則表示此決定的旁會顯示圖示）。 (6)
   * 證明角色(7)
   * 電子郵件警報設定(8)

>[!NOTE]
>
>編輯校樣詳細資訊的能力取決於您對校樣的權限(請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中管理校樣角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md))。

![summary_details_3.png](assets/summary-details-3-350x160.png)

### [!UICONTROL 階段動作] 功能表  {#stage-actions-menu}

工作流的每個階段都有單獨的菜單，允許您執行與該階段的審閱者相關的批量操作。

此 [!UICONTROL 階段動作] 滑鼠暫留在「階段」區段(1)上時，功能表就會顯示，並允許您

* [!UICONTROL 全部消息] (2)
* [!UICONTROL 共用] (3)
* [!UICONTROL 刪除階段] (4)

>[!NOTE]
>
>這些選項是否可用取決於您對校樣的權利(請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中管理校樣角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md))。

![Stage_actions_menu.png](assets/stage-actions-menu-350x161.png)

在「摘要」區段中，如果您對校樣具有編輯權限，您也可以存取審核者動作功能表。 如需詳細資訊，請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中管理校樣角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md). 將滑鼠游標暫留在「審閱者」的詳細資訊上，並允許您：

* 向審閱者發送消息(2)
* 編輯審閱者的詳細資訊(3) — 可讓您編輯該審閱者的顯示名稱、校樣角色和電子郵件警報
* 讓他們成為證明的所有者(4)
* 使他們成為主要決策者(5)
* 從校樣(6)中刪除

>[!NOTE]
>
>這些選項的可見性取決於您對校樣的權利(請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中管理校樣角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md))。

![Reviewer_actions_menu.png](assets/reviewer-actions-menu-350x135.png)

### 校樣動作功能表 {#proof-actions-menu}

每個校樣也有一個功能表(1)，可讓您執行下列動作：

* 您可以存取「校樣詳細資訊」頁面(2)
* 與他人分享證據(3)
* 向審閱者發送消息(4)
* 建立校樣的新版本(5)
* 複製校樣(6)
* 下載原始檔案(7)
* 共用校樣連結(8)
* 打印注釋(9)
* 請求校樣的Excel摘要(10)
* 鎖定校樣(11)
* 刪除校樣(12)

![Proof_actions_menu__1_.png](assets/proof-actions-menu--1--350x158.png)

>[!NOTE]
>
>這些選項是否可用取決於您對校樣的權利(請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中管理校樣角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md))。

有關在中查看校樣進度和狀態的資訊 [!DNL Workfront]，請參閱 [查看進度和狀態](#viewing-progress-and-status).

有關在案頭校對查看器中查看進度和狀態的資訊，請參見 [在校對檢視器中檢閱工作流程](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-workflow.md).
