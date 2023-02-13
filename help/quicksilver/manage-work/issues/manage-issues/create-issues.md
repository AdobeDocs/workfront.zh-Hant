---
product-area: projects
navigation-topic: manage-issues
title: 建立問題
description: 處理專案時，您可能會發現發生非預期的事件。 您可以將這些意外事件記錄為特定專案或任務的問題。 具有適當訪問權限的用戶可以查看和監視項目或任務完成時的問題狀態，從而無需進行冗長的電子郵件鏈或狀態會議。 與作業（即計畫事件）不同，問題代表Adobe Workfront中的未計畫工作項目。
author: Alina
feature: Work Management
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# 建立問題

處理專案時，您可能會發現發生非預期的事件。 您可以將這些意外事件記錄為特定專案或任務的問題。 具有適當訪問權限的用戶可以查看和監視項目或任務完成時的問題狀態，從而無需進行冗長的電子郵件鏈或狀態會議。 與作業（即計畫事件）不同，問題代表Adobe Workfront中的未計畫工作項目。

您也可以視要求將問題新增至專案。 如需詳細資訊，請參閱 [建立及提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>問題和要求在Workfront中可互換使用。 您可以記錄項目和任務中的問題，以指明需要解決的未預見的工作。 您也可以提交記錄為問題的請求，此問題會列在指定為「請求佇列」的專案上。

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
   <td> <p>查看或更高版本以向項目或任務添加問題</p> <p>使用「請求佇列」，以請求或更新版本來將問題新增為請求。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯問題的存取權</p> <p>查看或更高程度地訪問項目和任務</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需存取層級問題的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予問題的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>貢獻或更高權限，並能夠將問題新增至您建立問題的工作或專案</p> <p> 如需授予問題權限的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題 </a></p> <p>如需要求其他權限的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## 建立問題的限制

如果您擁有正確的存取權和權限，便可針對專案或任務建立問題。 但是，下列情況可能無法建立問題：

* 您的Workfront管理員或群組管理員必須啟用在您的「專案偏好設定」區域中，將問題新增至處於「完成」或「無效」狀態的專案。 有關設定項目首選項的資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 您無法向處於「待批准」的項目添加問題。

## 準備新問題表單

貴組織應有明確定義的程式，以便記錄問題的時間和方式。 設定此程式時，第一步是建立提交問題所需的表單。 無論您是否允許將問題直接添加到任務和項目中，還是如果您有提交問題的請求隊列，都可以定義哪些Workfront欄位以及用戶在提交新問題時可以使用哪些自定義欄位並必須填寫。 「新問題」表單中可包含有助於快速解決問題的重要資訊。

專案中新問題的欄位會在專案的「佇列詳細資料」區段中定義，並記錄問題。 如需設定專案的「佇列詳細資料」區段的相關資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

如需將問題提交至請求佇列以建立問題的相關資訊，請參閱 [輸入新請求以建立問題](#create-issues-by-entering-a-new-request) 一節。

## 使用「新建問題」按鈕建立任務或項目的問題

在專案中定義新問題表單的欄位後，您就可以開始建立問題。

要在任務或項目上建立問題，請執行以下操作：

1. 前往您要建立問題的專案。
1. （可選）如果要記錄任務的問題，請轉至 **工作** 區域，然後按一下任務的名稱。
1. 按一下 **問題** 區段。

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. 按一下 **新問題**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. （條件性）如果項目建立者在項目上建立了「隊列主題」或「主題組」，則這些主題或主題組將添加到新的問題表單中。 指定 **主題組** 或 **隊列主題** 新版。 它們應具有根據您的環境自訂的名稱。\
   如需建立主題群組的詳細資訊，請參閱 [建立主題群組](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). 如需建立佇列主題的詳細資訊，請參閱 [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * 如果專案上只設定了一個佇列主題，則會自動顯示。
   * 如果主題組下沒有任何隊列主題或主題組，則「主題組」下拉清單中沒有任何內容可用。

1. （條件性）如果專案建立者允許 **問題類型** 欄位以顯示在「新增期刊」表單中，請從下列選項中選取您的期刊類型：

   * 錯誤報告
   * 變更順序
   * 問題
   * 請求\
      根據您的Workfront管理員配置項目首選項的方式，問題類型的名稱可能不同。

1. 指定 **新問題** 表單。 有關在輸入新問題時定義欄位的詳細資訊，請參閱 [編輯問題](../../../manage-work/issues/manage-issues/edit-issues.md).
1. （條件性）如果佇列主題與自訂表單相關聯，該自訂表單會顯示在 **新問題** 表單。\
   或\
   如果專案透過「佇列詳細資料」區域與問題自訂表單相關聯，表單會顯示在 **新問題** 表單中的預設Workfront欄位。

   如需詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 按一下 **儲存新問題。**

問題可指派給多個使用者、工作角色或團隊。 如需指派及管理請求的詳細資訊，請參閱 [管理工作和團隊請求](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## 在內嵌任務或專案上建立問題

>[!IMPORTANT]
>
>項目所有者必須啟用 **允許使用者內嵌新增問題** 定義項目的問題設定時，您才能將問題內嵌到項目或任務中。 如需在專案上設定問題設定的相關資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

想要快速新增多個問題時，您可以內嵌建立任務或專案的問題，將問題新增至問題清單。

>[!NOTE]
>
>內嵌新增問題時，Workfront不會將「新問題」表單套用至新問題。 如果您希望使用者在輸入問題時提供特定資訊，則不建議內嵌新增問題。 這可能會對問題報告，以及之後指派給問題的使用者擁有解決問題所需的所有資訊的能力，造成負面影響。

要建立內聯問題，請執行以下操作：

1. 前往您要建立問題的專案。
1. （可選）如果要記錄任務的問題，請轉至 **工作** ，然後按一下任務的名稱。
1. 按一下 **問題** 區段。
1. 按一下 **新增更多問題**.

   「問題」區段的問題清單中會建立新的行。

   >[!TIP]
   >
   >如果在「編輯專案」方塊中取消選取「允許使用者新增問題內嵌」設定，此選項將呈暗灰色。 如需詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. 開始在「名稱」欄位中輸入問題名稱，然後繼續內嵌有關問題的詳細資訊。

   >[!TIP]
   >
   >可用於內嵌編輯的欄位可由您套用至問題清單的檢視使用。 您可能無法內嵌編輯下列類型的欄位：
   >   
   >* 屬於其他對象的欄位
   >* 您無權編輯的欄位
   >* 計算欄位，由Workfront自動更新


1. 按一下Enter完成內嵌編輯，然後將問題新增至專案或任務。

## 輸入新請求以建立問題 {#create-issues-by-entering-a-new-request}

您可以指定項目作為接收問題的接收器。 這些類型的專案在Workfront中稱為「請求佇列」。 您可以透過主功能表的「請求」區域存取「請求佇列」。

>[!TIP]
>
>在Workfront中，「issue」和「request」兩個詞可互換。

如需如何將專案設定為「請求佇列」以接收問題的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). 如需提交請求的相關資訊，請參閱 [建立及提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md).
