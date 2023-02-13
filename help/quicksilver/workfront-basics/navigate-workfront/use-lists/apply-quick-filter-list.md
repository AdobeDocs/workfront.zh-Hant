---
navigation-topic: use-lists
title: 將快速篩選器應用於清單
description: 您可以使用對象清單中的快速篩選器來幫助您僅查找對您來說很重要的項目，以便快速查看、更新或與他人共用這些項目。
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# 將快速篩選器應用於清單

<!--
{{highlighted-preview}}
-->

您可以使用對象清單中的快速篩選器來幫助您僅查找對您來說很重要的項目，以便快速查看、更新或與他人共用這些項目。

>[!IMPORTANT]
>
>您可以使用快速篩選找到包含搜尋字詞的項目，無論該項目是實際顯示在您的螢幕上，還是在您捲動至頁面底部後會顯示。 使用瀏覽器的搜尋功能時，您只能尋找實際顯示在畫面上的項目。 如果您的清單有多個頁面，快速篩選找不到頁面上未顯示的項目。

如果您想要儲存快速篩選，建議您改為建立清單的永久篩選。\
如需如何在中建立篩選器的相關資訊 [!DNL Adobe Workfront]，請參閱文章 [篩選器概觀，於 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

快速篩選目前適用於下列區域


您可以在所有清單中使用臨時快速篩選，但下列項目除外：

* 此 [!UICONTROL 報表] 區域
* 文檔清單和報告
* 數個 [!UICONTROL 設定] 地區
   >[!NOTE]
   >
   >下列設定區域提供快速篩選： [!UICONTROL 群組], [!UICONTROL 團隊], [!UICONTROL 公司], [!UICONTROL 排程], [!UICONTROL 版面範本]，和 [!UICONTROL 自訂Forms].


將快速篩選套用至清單時，請考量下列事項：

* 您可以使用關鍵字來篩選清單檢視中顯示的任何欄位。 這包括自訂欄位或複雜欄位，例如 [!UICONTROL 前置任務], [!UICONTROL 分配], [!UICONTROL 分配] 和 [!UICONTROL 狀態], [!UICONTROL 核准者] 和 [!UICONTROL 狀態]、等
* 如果您的清單已收合群組，當您使用快速篩選時，這些群組會自動展開。 移除快速篩選時，群組會再次收合。
* 無論應用的快速篩選器或對清單上的對象所做的任何更改，分組都會保留原始清單的聚合資訊。
* 快速篩選是暫時的。 變更分組、檢視、篩選或清單排序，會移除快速篩選條件。
* 無法保存快速篩選器。 如果您想要儲存篩選器以再次使用，請考慮為清單建立永久篩選器。
* 如果清單中有多個分組，而快速篩選器只在一個分組中查找項目，則只有該分組與找到的項目一起顯示。 所有其他群組皆隱藏。
* 在任務或子任務清單中，當快速篩選結果顯示時，將刪除任務層次。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] 計劃*</b></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] 授權*</b></td> 
   <td> <p>[!UICONTROL Request]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>訪問級別配置*</b></td> 
   <td> <p>查看對清單所在區域的訪問</p> <p>例如，若要將快速篩選套用至專案，您需要[!UICONTROL檢視]的專案存取權。</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。<br>若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>物件權限</b></td> 
   <td> <p>[!UICONTROL視圖]</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 將快速篩選套用至清單

1. 前往支援快速篩選的清單或報表，然後按一下 **[!UICONTROL 快速篩選] 圖示** ![](assets/qs-quick-filter-icon.png) 的下一頁。

   或

   根據您的作業系統或瀏覽器以及使用標準QWERTY鍵盤時，按下列命令集以啟動快速篩選器：

   * ALT+F [!DNL Windows] 電腦
   * ALT/選項+F [!DNL Mac] 電腦

      >[!TIP]
      >
      >如果按下CTRL+F或CMD+F，快速篩選器旁會顯示工具提示，提醒您這些命令。 命令也顯示在快速篩選搜索框內。

1. 在 **[!UICONTROL 篩選頁面]** 框中，輸入要篩選的關鍵字。

   您可以使用清單檢視中目前顯示的任何字詞。

   >[!NOTE]
   >
   >如果您使用可能顯示在清單其他頁面上的字詞，快速篩選器將不會找到任何結果。

   當您輸入並隱藏所有其他項目時，符合搜尋准則的項目清單會動態地顯示在清單中。 在所有獨立且複雜的欄位中，您在搜尋中使用的關鍵字會以黃色反白顯示。 複雜欄位的某些範例為共用欄，或下列任一欄： [!UICONTROL 分配], [!UICONTROL 分配] 和 [!UICONTROL 狀態], [!UICONTROL 完成百分比], [!UICONTROL 前置任務], [!UICONTROL 批准者和狀態], [!UICONTROL 資源管理器], [!UICONTROL 類別], [!UICONTROL 條件], [!UICONTROL 條件更新]、等

1. （可選）要批量編輯快速篩選找到的項目：

   1. 選取清單中的全部或數個項目，然後按一下 **[!UICONTROL 編輯]** 來批量編輯項目。
   1. 完成編輯後，按一下 **[!UICONTROL 儲存變更]**.

1. （可選）要導出快速篩選找到的項目，請選擇清單中的全部或數個項目，然後按一下 **[!UICONTROL 匯出]**.

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >只有您在快速篩選搜索中找到的項目才會導出到所選檔案。 如果在導出清單之前未選擇任何項目，則會導出完整、未篩選的清單。\
   >如需詳細資訊，請參閱 [匯出清單](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. （可選）若要清除篩選結果，請按一下 **[!UICONTROL 快速篩選]** 表徵圖。\
   或\
   重新整理該頁面。
