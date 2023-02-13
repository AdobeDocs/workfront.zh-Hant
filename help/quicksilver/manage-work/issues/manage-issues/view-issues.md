---
product-area: projects
navigation-topic: manage-issues
title: 檢視問題
description: 您可以查看與項目、任務或小版本關聯的問題。
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 0%

---

# 檢視問題

您可以查看與項目、任務或小版本關聯的問題。

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
   <td> <p>要求或更高版本</p> <p>檢閱或更高授權，以在專案的「問題」區段中檢視問題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視問題的存取權</p> <p>查看或更高程度地訪問項目和任務</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需存取層級問題的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予問題的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視問題的權限</p> <p> 如需授予問題權限的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題 </a></p> <p>如需要求其他權限的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 根據狀態檢視問題

要查看項目、任務或小版本的問題，請執行以下操作：

1. 開啟包含問題的專案、任務或小版本，然後按一下 **問題** 中。

1. 若要顯示所有、開啟或關閉的問題，請按一下以下所列的任何篩選器(位於 **篩選** 下拉式功能表。

>[!TIP]
>
>篩選器清單會依您的系統或群組管理員選取要顯示的項目而有所不同。

* **開啟：** 顯示未結的問題。

   這包括與解析對象關聯的對象，以及處於「已關閉 — 待批准」狀態的對象。

   有關解析對象的資訊，請參見 [解析和可解析對象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **已完成：** 顯示有實際完成日期的所有問題。
* **全部** 顯示所有問題。

## 了解有關問題的資訊

您可以在存取問題時檢視其相關資訊。

若要存取問題並檢視相關資訊：

1. 開啟包含問題的專案、任務或小版本，然後按一下 **問題** 中。
1. 從 **篩選** 下拉式選單中，選取篩選器以顯示您嘗試檢視的問題。

   從以下項目中選取：

   * 開啟
   * 已完成
   * 全部

1. 按一下問題名稱。

   當您對期刊有管理權限時，可以編輯期刊中任何可編輯的欄位，並將核准、小時數或檔案新增至期刊。

1. 從左側面板，按一下下列任一項，以檢視有關問題的詳細資訊：

* **更新**:您可以執行下列動作：

   * 對問題發表評論，或回復現有評論。
   * 記錄時間。
   * 更改問題的狀態。

      如需更新Workfront中工作的詳細資訊，請參閱 [更新工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **檔案**:將文檔附加到問題。 如需將檔案新增至Workfront的詳細資訊，請參閱 [從您的檔案系統將檔案新增至Adobe Workfront](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **問題詳細資訊**:展開此連結以顯示 **概述** 和 **自訂Forms** 區域。

   如果您擁有期刊的管理權限，且擁有自訂表單的編輯權限，您可以在此處編輯部分資訊。

   在 **概述** 區域：

   * **名稱**
   * **路徑**:將問題記錄到項目的路徑。

      如果以請求隊列中的請求形式提交問題，則此處將列出項目名稱、主題組和隊列主題。 無法編輯此欄位。

      如需提交請求的詳細資訊，請參閱 [建立及提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **說明**
   * **URL**:與問題相關的任何網址。
   * **優先順序**:視覺標幟，可讓您排定問題的優先順序。
   * **嚴重性**:可視標幟，指出問題中說明的問題嚴重程度。
   * **主要連絡人**:預設的「主要連絡人」是建立問題的使用者。 可編輯此欄位。
   * **計畫小時數**:顯示某人完成問題所花的時間。 預設為8小時。 可編輯此欄位。
   * **實際小時數**:顯示完成問題所花的時間。 這是某人記錄問題的實際時間。
   * **計劃開始日期**:計劃開始問題的日期。 預設值為建立問題的日期和時間。
   * **實際開始日期**:問題狀態更改為「In Progress（進行中）」的日期和時間。
   * **計畫完成日期**:計畫完成問題的日期。
   * **實際完成日期**:實際完成問題的日期。 當問題狀態變更為「已關閉」或「已解決」時，將自動填入此欄位，或者可以手動編輯。
   * **實際成本**:根據問題上記錄的實際小時數計算的成本。 此欄位不可編輯。 系統會根據下列公式計算問題的實際成本，其中，用戶成本比率是與記錄問題時間的用戶關聯的成本比率：

      問題實際成本=記錄小時數*用戶成本率

   * **輸入者**:這是建立問題的使用者。 此欄位不可編輯。
   * **上次更新者**:這是上次更新問題任何欄位的使用者。 此欄位不可編輯。

      在 **自訂Forms** 區域，選取一或多個要與問題關聯的自訂表單的檢視。

* **小時**:顯示問題的小時條目清單。
* **核准：** 顯示與問題相關聯的核准路徑。

   如需有關將核准與問題關聯的詳細資訊，請參閱 [將審批流程與工作項目關聯](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) 區段 [建立工作項的審批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 查看哪些項目和任務存在問題

您可以在專案或任務報表或清單的檢視中新增圖示，以顯示其是否附加問題。 將圖示新增至報表或清單的檢視，對於專案和任務類似。

若要新增顯示專案報表中是否有問題的圖示：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 按一下 **報表** > **新增報表** > **專案報表**.
1. 在 **顯示在此列中** 欄位，開始鍵入 **狀態表徵圖**，然後在清單中出現時選取它。

1. 按一下 **儲存+關閉** .

   問題圖示會顯示在 **狀態表徵圖** 欄。

   ![project_list_with_issue_icon.png](assets/project-list-with-issue-icon-350x132.png)
