---
product-area: projects
navigation-topic: manage-issues
title: 檢視問題
description: 您可以檢視與專案、任務或反複專案關聯的問題。
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# 檢視問題

<!--Audited: 10/2025-->

您可以檢視與專案、任務或反複專案關聯的問題。

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
   <td> <p>要求或更高版本</p> <p>檢視或更高授權以檢視專案問題區段中的問題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視問題的存取權</p> <p>檢視專案和任務的或更高存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需存取您存取層級中問題的相關資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授與問題的存取權</a>。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視問題的許可權</p> <p> 如需授與問題許可權的相關資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題</a></p> <p>如需請求其他許可權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 根據狀態檢視問題

若要檢視專案、任務或反複專案的問題：

1. 開啟包含問題的專案、任務或反複專案，然後按一下左側面板中的&#x200B;**問題**。

1. 若要顯示所有、開啟或關閉的問題，請從&#x200B;**篩選器**&#x200B;下拉式功能表按一下下列任何篩選器。

>[!TIP]
>
>篩選器清單會依您的系統或群組管理員選取要在其中顯示的內容而有所不同。

* **開啟：**&#x200B;顯示開啟的問題。

  其中包括與解析物件相關的專案，以及那些處於已關閉 — 未決核准狀態的專案。

  如需解析物件的相關資訊，請參閱[解析和可解析物件概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

* **已完成：**&#x200B;顯示所有具有實際完成日期的問題。
* **全部**&#x200B;顯示所有問題。

## 瞭解問題的相關資訊

您可以在存取時檢視問題的相關資訊。

若要存取問題並檢視其相關資訊：

1. 開啟包含問題的專案、任務或反複專案，然後按一下左側面板中的&#x200B;**問題**。
1. 從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取篩選器以顯示您嘗試檢視的問題。

   從下列選項中選取：

   * 開啟
   * 已完成
   * 全部

1. 按一下問題的名稱。

   當您擁有問題的管理許可權時，您可以編輯問題中的任何可編輯欄位，並將核准、時數或檔案新增到問題。

1. 從左側面板，按一下以下任一專案以檢視問題的詳細資訊：

* **更新**：您可以執行下列動作：

   * 對問題進行註解，或回覆現有註解。
   * 記錄時間。
   * 變更問題的狀態。

     如需有關在Workfront中更新工作的詳細資訊，請參閱[更新工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

* **檔案**：附加檔案至問題。 如需將檔案新增至Workfront的詳細資訊，請參閱[從您的檔案系統新增檔案至Adobe Workfront](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)。

* **問題詳細資料**：展開此連結以顯示&#x200B;**總覽**&#x200B;和&#x200B;**自訂Forms**&#x200B;區域。

  如果您有問題的管理許可權和自訂表單的編輯許可權，您可以在此處編輯某些資訊。

  檢視或編輯&#x200B;**概觀**&#x200B;區域中的下列欄位：

   * **名稱**
   * **路徑**：將問題記錄到專案的路徑。

     如果問題以請求佇列的形式提交，此處會列出專案名稱、主題群組和佇列主題。 無法編輯此欄位。

     如需有關提交請求的詳細資訊，請參閱[建立並提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

   * **說明**
   * **URL**：與問題相關的任何網址。
   * **優先順序**：視覺化旗標，可讓您排定問題的優先順序。
   * **嚴重性**：視覺化旗標，指出問題中描述的問題嚴重程度。
   * **主要連絡人**：預設的主要連絡人是建立問題的使用者。 此欄位可編輯。
   * **計畫時數**：顯示某人完成問題所需的時間長度。 預設值為8小時。 此欄位可編輯。
   * **實際時數**：顯示完成問題所花費的時間。 這是某人記錄問題的實際時間。
   * **計劃開始日期**：問題計劃開始的日期。 預設為建立問題的日期和時間。
   * **實際開始日期**：問題狀態變更為進行中的日期和時間。
   * **計畫完成日期**：計畫完成問題的日期。
   * **實際完成日期**：問題實際完成的日期。 當問題狀態變更為「已關閉」或「已解決」時，或可手動編輯時，此欄位會自動填寫。
   * **實際成本**：以問題記錄的實際時數為基礎的成本。 此欄位不可編輯。 問題的實際成本是根據下列公式來計算，其中「使用者成本費率」是與記錄問題時間的使用者相關的成本費率：

     問題實際成本=記錄時數*使用者成本費率

   * **輸入者**：這是建立問題的使用者。 此欄位不可編輯。
   * **上次更新者**：這是上次更新問題任何欄位的使用者。 此欄位不可編輯。

     在&#x200B;**自訂Forms**&#x200B;區域中，檢視選取一或多個要與問題相關聯的自訂表格。

* **小時**：顯示問題的小時專案清單。
* **核准：**&#x200B;顯示與問題相關的核准路徑。

  如需將核准與問題相關聯的詳細資訊，請參閱[建立工作專案的核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object)中的[將核准流程與工作專案相關聯](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)區段。

## 檢視有問題的專案和任務

您可以在專案或任務報告或清單的檢視中新增圖示，以顯示它們是否附加了問題。

在報表或清單的檢視中新增圖示對專案和任務而言是類似的。

若要新增顯示專案在專案報告中是否有問題的圖示：

{{step1-click-main-menu}}

1. 按一下&#x200B;**報告** > **新報告** > **專案報告**。
1. 在&#x200B;**顯示在此欄**&#x200B;欄位中，開始輸入&#x200B;**狀態圖示**，然後當它出現在清單中時選取它。

1. 按一下「**儲存+關閉**」。

   問題圖示會顯示在&#x200B;**狀態圖示**&#x200B;欄中有問題的專案上。

   ![含有問題圖示的專案清單](assets/project-list-with-issue-icon-350x132.png)
