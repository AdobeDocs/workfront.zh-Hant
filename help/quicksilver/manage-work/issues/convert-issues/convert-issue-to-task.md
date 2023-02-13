---
product-area: projects
navigation-topic: convert-issues
title: 將問題轉換為Adobe Workfront中的任務
description: 如果在提交問題後必須完成更多工作才能完成問題，您可以將問題轉換為任務。
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 2%

---

# 將問題轉換為Adobe Workfront中的任務

如果在提交問題後必須完成更多工作才能完成問題，您可以將問題轉換為任務。

如需轉換問題的一般資訊，請參閱 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯問題、任務和專案的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視問題的權限</p> <p>為專案貢獻權限</p> <p>在轉換問題後，您可以取得任務的「管理」權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 將問題轉換為任務

1. 前往專案，然後按一下 [!UICONTROL **問題** ] 中。
1. 按一下您要轉換的問題，前往問題的登陸頁面。
1. 按一下 [!UICONTROL **更多**] ，然後 [!UICONTROL **轉換為任務**].

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >如果問題與核准程式相關聯，或已與解決物件相關聯，Workfront會在 [!UICONTROL 轉換為專案] 框，通知您在轉換期間已刪除批准或已覆蓋解析對象。 如需詳細資訊，請參閱 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

1. 更新 [!UICONTROL 任務名稱] 區段。 預設情況下，任務的名稱將與原始問題的名稱相同。

   ![](assets/convert-to-task-box-nwe.png)

1. 按一下 [!UICONTROL **目的地專案**]，然後開始鍵入要將新任務放在 [!UICONTROL **目的地專案**] 欄位，並在清單中顯示時加以選取。 預設會選取問題的專案。

1. 按一下 [!UICONTROL **概述**]，然後輸入 [!UICONTROL **說明**] 的URL。

   >[!TIP]
   >
   >   系統或群組管理員可能會修改您的配置範本，以變更轉換方塊左側面板中各區段的順序。

1. （選用和條件式）按一下 [!UICONTROL **選項**]，請選取下列任一選項。

   Workfront管理員或群組管理員必須先啟用這些偏好設定，才能在問題轉換期間顯示這些偏好設定：

   * [!UICONTROL **保留原始問題，並將其解決辦法與此任務聯繫起來**]

      如果未選中，則刪除原始問題。

      >[!NOTE]
      >
      >無權存取或刪除問題的使用者在轉換問題時，無法刪除問題，無論此設定的狀態為何。 如需關於問題的存取權和權限的資訊，請參閱：
      >   
      >   * [授予問題的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
      >   * [共用問題](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


   * [!UICONTROL **允許（用戶名）有權訪問此任務**]

      如果未選中，則問題的主要聯繫人無權訪問新任務。

   * [!UICONTROL **維持規劃的問題完成日期**]

      若未選取， [!UICONTROL 計畫完成日期] 新任務的 [!UICONTROL 計劃開始日期] 任務。 此 [!UICONTROL 計劃開始日期] 根據新任務的系統首選項設定新任務的。

      >[!NOTE]
      >
      >
      >此處顯示的選項取決於Workfront管理員為系統中每個人設定這些選項的方式。 如需詳細資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
      >
      >或者，如果您組織中的頂層群組已個別設定，此處顯示的選項取決於哪個群組與您在步驟6中選取的專案相關聯。 如需詳細資訊，請參閱 [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. （選用）按一下 [!UICONTROL **自訂Forms**] 並附加新任務的自定義表單。

   >[!TIP]
   >
   >如果已將附加至問題的多物件自訂表單設定為搭配問題和任務使用，則預設會附加該表單。 進行轉換時，系統會為任務保留問題表單中保存的所有資訊。
   >
   >如果目標項目在編輯項目時在「任務預設自定義Forms」欄位中定義了任何預設表單，則這些任務表單也將添加到新任務中。 原始問題和預設任務表單上欄位之間通用的任何自定義欄位都將預先填充問題欄位中的資訊。

1. 按一下 [!UICONTROL **轉換為任務**].

   如果您決定刪除原始問題，則問題現在是指定項目上的任務。

   或

   現在，問題已連結到您所選項目上的新任務，如果您決定保留原始問題，則任務完成後問題將完成。

   某些問題欄位會轉移至任務。 如需詳細資訊，請參閱 [查看有關項目和任務的原始問題資訊](#view-original-issue-information-on-projects-and-tasks) 一節。

1. （可選）視需要繼續編輯任務。

## 查看有關項目和任務的原始問題資訊 {#view-original-issue-information-on-projects-and-tasks}

您可以在項目和任務清單和報表中或在「項目詳細資訊」區域中查看原始問題資訊。 如需建立報表的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

下表說明了從轉換的項目和任務中可看到的問題欄位。

| 問題欄位 | 項目或任務欄位 | 專案清單或報表 | 項目詳細資訊區域 | 任務清單或報告 | 任務詳細資訊區域 |
|---|---|---|---|---|---|
| [!UICONTROL 問題名稱] | [!UICONTROL 轉換的問題名稱] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL 主要連絡人] | [!UICONTROL 轉換的問題創作者名稱] | ✔ | ✔ | ✔ |
| [!UICONTROL 輸入日期] | [!UICONTROL 轉換的問題輸入日期] | ✔ |  | ✔ |


>[!CAUTION]
>
>若 [!UICONTROL 主要連絡人] 問題變更，或問題轉換後從專案或任務中取消連結，則 [!UICONTROL 轉換的問題創作者名稱 ]不會更新，而會顯示原始 [!UICONTROL 主要連絡人] 的問題。
