---
product-area: projects
navigation-topic: convert-issues
title: 在Adobe Workfront中將問題轉換為任務
description: 如果在提交問題後必須完成更多工作，您可以將問題轉換為任務。
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# 在Adobe Workfront中將問題轉換為任務

如果在提交問題後必須完成更多工作，您可以將問題轉換為任務。

如需轉換問題的一般資訊，請參閱[在Adobe Workfront中轉換問題的概觀](../../../manage-work/issues/convert-issues/convert-issues.md)。

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯問題、任務和專案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視問題的許可權</p> <p>貢獻專案的許可權</p> <p>您可在問題轉換後取得任務的管理許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 將問題轉換為任務

1. 前往專案，然後按一下左側面板中的&#x200B;[!UICONTROL **問題**]。
1. 按一下您要轉換的問題，以移至問題的登陸頁面。
1. 按一下問題上的&#x200B;[!UICONTROL **更多**]&#x200B;功能表，然後&#x200B;[!UICONTROL **轉換為任務**]。

   ![問題更多功能表](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >如果問題與核准流程相關，或已經與解決物件相關，Workfront會在[!UICONTROL 轉換為專案]方塊頂端顯示警告，通知您核准已移除，或解決物件在轉換期間遭覆寫。 如需詳細資訊，請參閱[在Adobe Workfront中轉換問題的概觀](../../../manage-work/issues/convert-issues/convert-issues.md)。

1. 更新[!UICONTROL 任務名稱]區段中的任務名稱。 依預設，任務的名稱將與原始問題的名稱相同。

   ![轉換為工作方塊](assets/convert-to-task-box-nwe.png)

1. 按一下&#x200B;[!UICONTROL **目的地專案**]，然後開始輸入您要在&#x200B;[!UICONTROL **目的地專案**]&#x200B;欄位中放置新任務的專案名稱，並在它顯示在清單中時選取它。 依預設，會選取問題的專案。

1. 按一下&#x200B;[!UICONTROL **概述**]，然後輸入工作的&#x200B;[!UICONTROL **描述**]。

   >[!TIP]
   >
   >   系統或群組管理員可能會修改您的版面配置範本，以變更轉換方塊左側面板中區段的順序。

1. （選擇性和條件性）按一下&#x200B;[!UICONTROL **選項**]，選取下列任一選項。

   Workfront管理員或群組管理員必須先啟用這些偏好設定，才能在轉換問題期間顯示：

   * [!UICONTROL **保留原始問題並將其解決方案連結至此任務**]

     如果取消選取，則會刪除原始問題。

     >[!NOTE]
     >
     >無論此設定的狀態為何，沒有存取許可權或刪除問題的使用者在轉換問題時都將無法刪除問題。 如需問題的存取和許可權資訊，請參閱：
     >   
     >   * [授與問題的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     >   * [共用問題](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)
     >   
     >

   * [!UICONTROL **允許（使用者名稱）存取此工作**]

     如果取消選取，問題的主要連絡人將沒有新任務的存取權。

   * [!UICONTROL **保留問題的計畫完成日期**]

     若未選取，新任務的[!UICONTROL 計畫完成日期]將從任務的[!UICONTROL 計劃開始日期]開始計算。 新任務的[!UICONTROL 計劃開始日期]是根據新任務的系統偏好設定所設定。

     >[!NOTE]
     >
     >
     >此處顯示的選項取決於Workfront管理員如何為系統中的每個人設定這些選項。 如需詳細資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。
     >
     >或者，如果您組織中的最上層群組已個別設定這些群組，此處顯示的選項會根據您在步驟6中所選專案相關聯的群組而定。 如需詳細資訊，請參閱[設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

1. （選擇性）按一下&#x200B;[!UICONTROL **自訂Forms**]，然後附加新工作的自訂表單。

   >[!TIP]
   >
   >* 如果附加到問題的多物件自訂表單已設定為同時用於問題和任務，則當您進行轉換時，如果問題和任務的自訂表單上同時存在欄位，則保留表單中儲存的所有資訊。
   >* 如果將具有計算欄位的多物件自訂表單附加到問題和任務，問題和任務必須與表單的計算自訂欄位中參照的所有欄位相容。 如果發生不相容的情況，訊息會警告您進行調整。 如需詳細資訊，請參閱[將計算欄位新增至表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。
   >* 如果目標專案在編輯專案時有任何在任務預設自訂Forms欄位中定義的預設表單，這些任務表單也會新增到新任務中。 原始問題和預設任務表單上的欄位之間的任何共同自訂欄位都會預先填入問題欄位的資訊。


1. 按一下&#x200B;[!UICONTROL **轉換至工作**]。

   如果您決定刪除原始問題，則問題現在為指定專案上的任務。

   或

   問題現在已連結到您所選專案上的新任務，而且如果您決定保留原始問題，它將在任務完成後完成。

   有些問題欄位會傳送至任務。 如需相關資訊，請參閱本文中的[檢視專案與任務的原始問題資訊](#view-original-issue-information-on-projects-and-tasks)一節。

1. （選用）視需要繼續編輯工作。

## 檢視專案和任務的原始問題資訊 {#view-original-issue-information-on-projects-and-tasks}

您可以在專案和工作清單及報告中或在「專案詳細資訊」區域中，檢視原始問題資訊。 如需建立報表的相關資訊，請參閱[建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

下表說明哪些問題欄位可從轉換的專案和任務中看到。

| 問題欄位 | 專案或工作列位 | 專案清單或報告 | 專案詳細資訊區域 | 任務清單或報告 | 任務詳細資訊區域 |
|---|---|---|---|---|---|
| [!UICONTROL 問題名稱] | [!UICONTROL 已轉換問題的名稱] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL 主要連絡人] | [!UICONTROL 轉換的問題建立者名稱] | ✔ | ✔ | ✔ |
| [!UICONTROL 輸入日期] | [!UICONTROL 已轉換問題的輸入日期] | ✔ |  | ✔ |


>[!CAUTION]
>
>如果問題的[!UICONTROL 主要連絡人]變更，或問題在轉換之後與專案或任務解除連結，[!UICONTROL 轉換的問題建立者名稱]不會更新，且會在轉換問題時顯示問題的原始[!UICONTROL 主要連絡人]。
