---
navigation-topic: use-lists
title: 將快速篩選套用至清單
description: 您可以使用物件清單中的快速篩選來協助您僅找出對您而言重要的專案，以便快速檢閱、更新或與他人共用這些專案。
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# 將快速篩選套用至清單

<!--
{{highlighted-preview}}
-->

您可以使用物件清單中的快速篩選來協助您僅找出對您而言重要的專案，以便快速檢閱、更新或與他人共用這些專案。

>[!IMPORTANT]
>
>您可以使用快速篩選來尋找包含搜尋字詞的專案，無論該專案已實際顯示在您的熒幕上，還是在您捲動至頁面底部之後顯示。 使用瀏覽器的搜尋功能時，您只能尋找實際顯示在熒幕上的專案。 如果您的清單有多個頁面，快速篩選器會找不到未顯示頁面上的專案。

如果您想要儲存快速篩選，建議您改為為清單建立永久篩選。\
若要瞭解如何在[!DNL Adobe Workfront]中建立篩選器，請參閱文章[篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

快速篩選器目前在以下區域可用


您可以在所有清單中使用暫時的快速篩選，但下列專案除外：

* [!UICONTROL 報表]區域
* 檔案清單與報告
* 多個[!UICONTROL 設定]區域
  >[!NOTE]
  >
  >快速篩選器可用於下列設定區域： [!UICONTROL 群組]、[!UICONTROL 團隊]、[!UICONTROL 公司]、[!UICONTROL 排程]、[!UICONTROL 配置範本]以及[!UICONTROL 自訂Forms]。


將快速篩選套用至清單時，請考量下列事項：

* 您可以使用關鍵字來篩選顯示在清單檢視中的任何欄位。 這包括自訂欄位或複雜欄位，例如[!UICONTROL 前置任務]、[!UICONTROL 指派]、[!UICONTROL 指派]和[!UICONTROL 狀態]、[!UICONTROL 核准者]和[!UICONTROL 狀態]等。
* 如果您的清單已摺疊群組，當您使用快速篩選器時，這些群組會自動展開。 當您移除快速篩選器時，群組會再次摺疊。
* 無論套用快速篩選或對清單上的物件所做的任何變更，群組都會保留原始清單的彙總資訊。
* 快速篩選是暫時性的。 變更清單的分組、檢視、篩選或排序會移除快速篩選條件。
* 您無法儲存快速篩選。 如果要儲存篩選器以再次使用，請考慮為清單建立永久篩選器。
* 如果清單中有多個群組，且快速篩選器僅在一個群組中找到專案，則只有該群組會與找到的專案一起顯示。 所有其他群組都已隱藏。
* 在任務或子任務清單中，當快速篩選的結果顯示時，會移除任務階層。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] 計畫*</b></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] 授權*</b></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>存取層級設定*</b></td> 
   <td> <p>檢視清單所在區域的存取權</p> <p>例如，若要將快速篩選套用至專案，您需要[！UICONTROL檢視]專案的存取權。</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。<br>如需[!DNL Workfront]管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>物件許可權</b></td> 
   <td> <p>[！UICONTROL檢視]</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 將快速篩選套用至清單

1. 移至支援快速篩選的清單或報告，然後按一下工具列中的&#x200B;**[!UICONTROL 快速篩選]圖示** ![](assets/qs-quick-filter-icon.png)。

   或

   視您的作業系統或瀏覽器而定，在使用標準QWERTY鍵盤時，請按下列指令集以啟動快速篩選：

   * [!DNL Windows]部電腦的ALT+F
   * [!DNL Mac]部電腦的ALT/ Option+F

     >[!TIP]
     >
     >如果您按下CTRL+F或CMD+F，快速篩選旁會顯示工具提示，提醒您有關這些指令的資訊。 這些命令也會顯示在快速篩選搜尋方塊內。

1. 在&#x200B;**[!UICONTROL 篩選頁面]**&#x200B;方塊中，輸入您要依據的關鍵字。

   您可以使用目前顯示在清單檢視中的任何單字。

   >[!NOTE]
   >
   >如果您使用可能顯示在清單其他頁面上的單字，快速篩選將找不到任何結果。

   當您輸入時，符合搜尋條件的專案清單會動態地顯示在清單中，而所有其他專案則會隱藏。 您在搜尋中使用的關鍵字在所有獨立和複雜欄位中都會以黃色反白顯示。 某些複雜欄位的範例為共用欄，或以下任何一項： [!UICONTROL 指派]、[!UICONTROL 指派]及[!UICONTROL 狀態]、[!UICONTROL 完成百分比]、[!UICONTROL 前置任務]、[!UICONTROL 核准者和狀態]、[!UICONTROL 資源管理員]、[!UICONTROL 類別]、[!UICONTROL 條件]、[!UICONTROL 條件更新]等。

1. （可選）若要大量編輯快速篩選找到的專案：

   1. 選取清單中的所有或數個專案，然後按一下&#x200B;**[!UICONTROL 編輯]**&#x200B;以大量編輯專案。
   1. 完成編輯之後，請按一下&#x200B;**[!UICONTROL 儲存變更]**。

1. （選擇性）若要匯出快速篩選找到的專案，請選取清單中的所有或數個專案，然後按一下[匯出]。****

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >只有您在快速篩選搜尋中找到的專案會匯出至您選取的檔案。 如果您在匯出清單之前未選取任何專案，則會匯出完整、未篩選的清單。\
   >如需詳細資訊，請參閱[匯出清單](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md)。

1. （選擇性）若要清除篩選的結果，請按一下視窗右上角的&#x200B;**[!UICONTROL 快速篩選]**&#x200B;圖示。\
   或\
   重新整理該頁面。
