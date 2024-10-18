---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: 委派任務和問題
description: 您不在辦公室時，可以暫時委派指派給您的工作。 本文介紹如何委派任務和問題指派。
author: Alina
feature: Work Management
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 9d0caff0381ee50bf8dd7060bebafb5354c0f0d8
workflow-type: tm+mt
source-wordcount: '1518'
ht-degree: 0%

---

# 委派任務和問題

<!-- Audited: 10/2024 -->


<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote this as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

您不在辦公室時，可以暫時委派指派給您的工作。

您可以委派任務和問題指派，也可以委派核准。 本文介紹如何委派任務和問題指派。

如需委派工作的一般資訊，請參閱[委派工作概覽](../../manage-work/delegate-work/delegate-work-overview.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

>[!IMPORTANT]
>
>* 您選取為委派的使用者會獲得與您委派給他們的任務和問題之許可權相同的許可權。
>* 這些許可權必須在其存取層級內運作，有時其存取層級可能低於您的存取層級。
>
>   
>   例如，如果使用者對其存取層級中的任務只有「檢視」存取權，而您對您委派給他們的任務具有「管理」許可權，則他們可獲得您委派給他們的任務的「管理」許可權。 但是，他們將無法對委派的任務執行與您相同的動作。 若要在缺勤時更新任務，他們必須向系統管理員請求任務的編輯存取權。
>
>   
>   如需系統管理員如何修改存取層級的資訊，請參閱[建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。
>
>* 對於在委派開始後指派的專案，在指派專案給[!DNL Workfront]後，最多可能需要一小時才能與委派共用新指派的專案。


您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>新增：投稿人或更高版本</p><p>或</p><p>目前：檢閱或以上</p>

>[!NOTE]
>
>雖然您可以在擁有Request授權時獲得工作指派，但您無法將工作委派給其他人。 [!DNL Workfront]不建議將工作指派給檢閱、請求或貢獻者使用者。

</tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務和問題的存取權 
     </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視或更高的許可權給您指派的任務或問題</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## 先決條件

您必須先確定下列事項，才能執行本文所述的活動：

* 您的[!DNL Workfront]或群組管理員已啟用[!DNL Workfront]執行個體之[!UICONTROL 設定]區域的[!UICONTROL 任務和問題偏好設定]區段中的&#x200B;[!UICONTROL **允許使用者委派其任務和問題**]&#x200B;設定。

  如需詳細資訊，請參閱[設定全系統的任務和問題偏好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

## 將任務和問題委派給其他使用者

將工作委派給他人之前，建議您聯絡他們並通知他們他們將被指定為您工作專案的代理人。 在委派工作前要求他們口頭核准，以確保他們有必要的時間，在您外出時完成工作。

如需委派任務和問題的一般資訊，請參閱[委派任務和問題總覽](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md)。

若要將您的任務和問題委派給其他人：

1. 移至&#x200B;[!UICONTROL **首頁**]&#x200B;區域。
1. 確定您已將&#x200B;[!UICONTROL **我的工作**]、[!UICONTROL **我的任務**]&#x200B;或&#x200B;[!UICONTROL **我的問題**] Widget新增到您的&#x200B;[!UICONTROL **首頁**]。

   如需詳細資訊，請參閱[在首頁新增、編輯或移除Widget](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md)

1. 按一下&#x200B;[!UICONTROL **我的工作**]、[!UICONTROL **我的任務**]&#x200B;或&#x200B;[!UICONTROL **我的問題**] Widget左上角的&#x200B;[!UICONTROL **代理人**]。

   ![](assets/delegate-button-on-my-work-widget.png)

1. 更新下列專案：

   * [!UICONTROL **將您的任務和問題委派給**]：開始輸入您要將您的任務和問題委派給的使用者名稱，然後在其顯示在清單中時選取它。 您只能選取一個使用者。

     您選取作為委派的使用者會收到與您委派給他們的任務和問題之許可權相同的許可權。

   * [!UICONTROL **開始日期**]：從行事曆選取工作專案應該開始委派的日期。

     >[!TIP]
     >
     >開始日期不能是過去。

   * [!UICONTROL **沒有結束日期**]：如果您不想指定委派的結束日期，請選取此選項。

   * [!UICONTROL **結束日期**]：從行事曆選取委派應該停止的日期。

     >[!TIP]
     >
     >如果您將「結束日期」欄位保留空白，而未選取「無結束日期」選項，則委派僅會針對當天設定。

     ![](assets/delegate-box-expanded-in-home.png)
     <!--check screen shot - submitted bug for casing-->

1. 按一下「[!UICONTROL **儲存**]」。

   會發生下列情況：

   * 您的工作已委派給指定的使用者。 任何日期在您選取的時間範圍內（包括啟用委派後新指派的任務）的未完成任務或問題都會被委派。

     >[!TIP]
     >
     >   日期在委派時間範圍內的已完成工作專案不會委派。


   * 您會在畫面底部收到訊息，確認您已啟用將您的工作委派給其他使用者。 委派使用者的名稱會顯示在確認訊息中。

   * 大部分割槽域都會顯示您的任務和問題已委派給其他使用者，而您可以在[!DNL Workfront]中看到這些工作分派。 如需哪些區域不包含代理人名稱的詳細資訊，請參閱[代理人工作概觀](delegate-work-overview.md)。

   * [!UICONTROL **首頁**]&#x200B;區域中的&#x200B;[!UICONTROL **委派**]&#x200B;按鈕變更為&#x200B;[!UICONTROL **編輯委派**]，表示已有委派。
     <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
      </MadCap:conditionalText>
      -->

     ![](assets/edit-delegation-button-on-my-work-widget.png)

   * 如果已啟用事件通知和個人通知，您也會收到委派電子郵件確認。

   * 如果您選取作為委派的使用者已啟用其事件通知，則該使用者會收到有關委派的電子郵件。

     如需有關啟用個人電子郵件通知的資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

## 編輯或停止委派

如果您選取了「結束日期」，您可以讓委派過期，也可以手動停止委派。 如果委派日期已變更，您也可以修改委派的時間範圍。

1. 移至&#x200B;[!UICONTROL **首頁**]&#x200B;區域，然後按一下下列任一Widget中的&#x200B;[!UICONTROL **編輯委派**]： **我的工作**、**我的任務**&#x200B;或&#x200B;**我的問題**。
1. 在[!UICONTROL 停止委派任務和問題]方塊中，執行下列任一項作業：
   * 修改開始日期&#x200B;[!UICONTROL **或[!UICONTROL **&#x200B;結束日期&#x200B;**]**]
   * 按一下&#x200B;[!UICONTROL **停止委派**]

   >[!TIP]
   >
   >    如果委派已開始，則只能編輯委派的「結束」日期。

   ![](assets/stop-delegation-box-new-home-tasks-and-issues.png)

1. （視條件而定）按一下&#x200B;[!UICONTROL **儲存**]&#x200B;以儲存新的委派日期

   或

   在確認方塊中按一下&#x200B;[!UICONTROL **停止委派**]&#x200B;以確認停止委派。

   委派已更新日期或已停止，並且委派的使用者已從您的任務和問題中移除。 他們對任務和問題的許可權維持不變。

## 找出委派的工作和委派資訊

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

委派任務和問題時，[!DNL Workfront]中有數個區域可供您檢視委派的工作或委派者。

* [在「工作總攬」方塊中找出委派](#locate-delegates-in-the-assignments-box)
* [在[!UICONTROL 首頁]找到委派的工作](#locate-delegated-work-in-home)


### 在[!UICONTROL 工作總攬]方塊中找出代理人

當您的系統或群組管理員在您的系統中啟用工作委派時，[!UICONTROL 工作總攬]方塊會在您可以存取它的任何地方顯示以下標籤：

* [!UICONTROL **指派**]：指派給任務或問題的使用者會顯示在這裡。
* [!UICONTROL **委派**]：由任務或問題受指派人指定為委派的使用者會顯示在這裡。

您可以在下列區域中存取[!UICONTROL 工作總攬]方塊：

* 任務或問題標題

  任務或問題標題中的[!UICONTROL 指派]欄位變更為[!UICONTROL 指派和委派]。

  ![](assets/assignments-and-delegates-panel-in-task-header.png)

* 手動指派任務或問題時的[!UICONTROL 工作負載平衡器]

  ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> 您無法在任務或問題編輯方塊的[!UICONTROL 工作總攬]區段中檢視委派。

如果任務或問題已委派，且[!UICONTROL 委派]子標籤是空的，則可能存在下列其中一種情況：

* 您未指派給任務或問題。
* 任務或問題日期不在委派時間範圍內。

>[!TIP]
>
>委派的任務和問題的計畫或實際時數未納入資源管理工具中，例如[!UICONTROL 工作負載平衡器]或委派使用者的[!DNL Resource Planner]。 時數僅與指派的使用者相關聯。

### 在[!UICONTROL 首頁]找到委派的工作

1. 移至&#x200B;[!UICONTROL **我的工作**] Widget中的&#x200B;[!UICONTROL **首頁**]&#x200B;區域。
1. 按一下篩選器下拉式功能表，然後選取下列一或多個選項：
   * [!UICONTROL **已委派**]：檢視委派給您或由您委派的任務和問題。
   * [!UICONTROL **已委派給我**]：檢視其他使用者委派給您的任務和問題。
   * [!UICONTROL **由我委派**]：檢視您委派給其他使用者的任務和問題。

     ![](assets/delegated-tasks-and-issues-new-home-filter.png)

1. （選擇性）按一下&#x200B;[!UICONTROL **排序**]&#x200B;下拉式功能表，依下列條件排序清單：
   * [!UICONTROL 到期日期]。 這是預設的排序選項。
   * [!UICONTROL 名稱]
   * [!UICONTROL 完成百分比]
   * [!UICONTROL 狀態]
1. （可選）展開&#x200B;[!UICONTROL **我的工作**] Widget右上角的群組下拉式功能表，然後依下列其中一個條件進行群組：
   * 沒有內容。 這是預設分組選項。
   * [!UICONTROL 專案]
   * [!UICONTROL 狀態]
   * [!UICONTROL 到期日期]

1. 若要檢視您委派或已委派給您的專案，請檢視下列其中一項：

   * 對於您委派給其他人的專案，請在&#x200B;[!UICONTROL **委派給**]&#x200B;之後，在任務或問題的狀態下找到委派者的名稱。

   * 對於委派給您的專案，在&#x200B;[!UICONTROL **由**]&#x200B;委派給您之後，在任務或問題的狀態下找到受指派人的名稱。

     >[!TIP]
     >
     >    如果委派設定在今天日期之後的某個日期開始，則委派的開始日期也會顯示在[!UICONTROL 工作清單]中。 委派的專案會根據群組的型別，顯示在您為[!UICONTROL 工作清單]選取的群組中。 例如，如果您依[!UICONTROL 計畫完成日期]分組，則委派的專案會顯示在符合其計畫完成日期的分組中。
