---
content-type: overview
title: 摘要概觀
description: 您可以使用「摘要」面板，直接從任務問題、檔案清單或的其他區域檢閱和更新工作專案資訊。 [!DNL Adobe Workfront] 問題按鈕來顯示任務和問題。
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 5d6e9788ccbae7a8970cff56558233a57ceee1ab
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 2%

---

# [!UICONTROL 摘要] 概述

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

您可以使用 [!UICONTROL 摘要] 面板，直接從任務、問題、檔案清單或從的其他區域檢閱和更新工作專案資訊。 [!DNL Adobe Workfront] 問題按鈕來顯示任務和問題。

您的Workfront或群組管理員可以修改摘要面板中顯示的區域和欄位。 他們最多可以新增16個欄位到摘要面板。

>[!IMPORTANT]
>
>我們建議您新增必須經常更新的欄位至「摘要」面板，這樣您就可以輕鬆存取並更新這些欄位，無需存取物件的首頁面。
>
>例如，您可以將以下經常更新的欄位新增到任務和問題摘要面板：
>
>* 狀態
>* 完成百分比
>* 認可日期
>* 規劃完成日期
>* 狀況



下表顯示您可以找到及使用 [!UICONTROL 摘要] 面板：

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td><b>任務</b></td> 
  </tr> 
  <tr> 
   <td> <p>內的工作清單</p> 
    <ul> 
     <li>專案</li> 
     <li>子任務</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作負載平衡器]的[！UICONTROL未指派]和[！UICONTROL已指派]工作區域中的任務</td> 
  </tr> 
   <tr> 
   <td>[！UICONTROL時程表]中的任務</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><b>問題</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>內的問題清單</p> 
    <ul> 
     <li>專案</li> 
     <li>任務</li> 
     <li>子任務</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL工作負載平衡器]的[！UICONTROL指派的工作]區域發生問題</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL請求]區域的[！UICONTROL已提交]區段中的問題</td> 
  </tr> 
</tr> 
   <tr> 
   <td>[！UICONTROL時程表]中的問題</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td><b>文件</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL檔案]區域</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>任何物件（專案、任務、問題、方案、投資組合、範本、範本任務、使用者）的[！UICONTROL檔案]區段</td> 
  </tr> 
 </tbody> 
</table>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront administrators can customize the Summary in the Layout Template. For more information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
-->

本文說明如何存取及使用 [!UICONTROL 摘要] 清單中任務和問題的面板。

如需有關存取 [!UICONTROL 摘要] 在 [!UICONTROL 工作負載平衡器]，請參閱 [更新中的工作專案 [!UICONTROL 工作負載平衡器] 使用 [!UICONTROL 摘要]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

如需有關存取 [!UICONTROL 摘要] 如需檔案，請參閱 [[!UICONTROL 摘要] 檔案概覽](../../documents/managing-documents/summary-for-documents.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>新增：投稿人或更高版本</p>
   或
   <p>目前：[！UICONTROL要求]或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>[！UICONTROL檢視]或更高的任務、問題、檔案存取權</p> <p>[！UICONTROL檢視]或更高的存取權存取您要檢視其檔案[！UICONTROL摘要]的任何物件</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>[！UICONTROL檢視]或任務、問題或檔案的更高許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請連絡 [!DNL Workfront] 管理員。 如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 檢視 [!UICONTROL 摘要] 任務或問題清單中的面板

1. 前往任務或問題，然後在清單中選取專案。
1. 按一下 **[!UICONTROL 摘要]** 圖示 ![](assets/qs-summary-in-new-toolbar-small.png)

   或

   按一下 **[!UICONTROL 開啟摘要]** 圖示 ![](assets/open-summary-with-text-nwe.png) 在 [!UICONTROL 已提交] 的區段 [!UICONTROL 請求] 區域。

   開啟「摘要」後，當您按一下或選取其他任務或問題時，摘要會保持開啟狀態，直到您手動關閉摘要為止。

   >[!TIP]
   >
   >您一次只能選取一個任務或一個問題，以在 [!UICONTROL 摘要] 面板。

   ![摘要面板](assets/summary-panel-for-task-new-comments.png)

1. （選用）若要關閉 [!UICONTROL 摘要] 面板，執行下列任一項作業：

   * 在任務或問題清單中，按一下 **[!UICONTROL 開啟摘要]** 圖示 ![](assets/summary-panel-icon.png)

     或

     按一下 **X** 圖示於 [!UICONTROL 摘要] 面板。

   * 在 [!UICONTROL 已提交] 的區段 [!UICONTROL 請求] 區域，按一下 **[!UICONTROL 關閉摘要]** 圖示 ![](assets/close-summary-with-text-nwe.png)

     或

     按一下 **X** 圖示加以顯示。

## [!UICONTROL 完成百分比]

使用頂端的進度列 [!UICONTROL 摘要] 更新您選取的任務或問題的完成百分比。 輸入數字或將橫條拖曳到正確的百分比。

![摘要面板中的完成百分比](assets/summary-overview-percent-complete.png)

## [!UICONTROL 更新]

使用 [!UICONTROL 更新] 的區段 [!UICONTROL 摘要] 以檢視最近的更新，並對您選取的任務或問題進行更新。 按一下 **[!UICONTROL 檢視全部]** 直接前往 [!UICONTROL 更新] 標籤中。

![摘要面板中的更新區段](assets/summary-updates-section.png)

## [!UICONTROL 文件]

使用 [!UICONTROL 檔案] 的區段 [!UICONTROL 摘要] 以檢視附加到您所選任務或問題的檔案。 按一下縮圖以開啟檔案預覽。 若要直接前往 [!UICONTROL 檔案] 索引標籤上的任務或問題，按一下 **[!UICONTROL 檔案]** 標題。

![摘要面板中的檔案區段](assets/summary-documents-section.png)

## [!UICONTROL 詳細資料]

使用 [!UICONTROL 詳細資料] 的區段 [!UICONTROL 摘要] 若要檢視高階工作專案詳細資訊、進行指派或新增開始日期。 按一下 **[!UICONTROL 檢視全部]** 直接前往 [!UICONTROL 詳細資料] 標籤上的任務或問題。

>[!NOTE]
>
>此區段中顯示的欄位，與首頁右側面板中顯示的欄位相同。 您可以自訂這些欄位 [自訂 [!UICONTROL 首頁] 和 [!UICONTROL 摘要] 使用版面範本](../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

![摘要面板中的詳細資訊區段](assets/summary-details-section.png)

## [!UICONTROL 子任務]

此區段僅適用於工作。 使用 [!UICONTROL 子任務] 的區段 [!UICONTROL 摘要] 以檢視 [!UICONTROL 新增]， [!UICONTROL 進行中]、和 [!UICONTROL 已關閉] 您選取之任務的子任務。 按一下 **[!UICONTROL 狀態]** 下拉式功能表以切換狀態。 若要直接前往 [!UICONTROL 子任務] 標籤上，按一下 **[!UICONTROL 子任務]**&#x200B;標題&#x200B;。

如果您尚未將任何子任務新增至任務，請按一下 **[!UICONTROL 在這裡新增一個]** 直接前往 [!UICONTROL 子任務] 標籤中。

![摘要面板中的子任務區段](assets/summary-subtasks-section.png)

## [!UICONTROL 小時]

使用 [!UICONTROL 小時] 的區段 [!UICONTROL 摘要] 以記錄所選任務或問題的時數。 按一下 **[!UICONTROL 記錄時間]** 並輸入小時。 若要直接前往任務或問題上的時數索引標籤，請按一下 **[!UICONTROL 小時]** 標題。

中的小時計數 [!UICONTROL 摘要] 顯示您所記錄的時數。 其他使用者在中會有不同的小時總計 [!UICONTROL 摘要] 視他們登入工作的時間而定。

如果沒有計畫 [!UICONTROL 小時] 在任務或問題上，而您已記錄時間，時數列顯示紅色。

![摘要面板中的小時區段](assets/summary-hours-section.png)

## 核准

使用 [!UICONTROL 核准] 的區段 [!UICONTROL 摘要] 以檢視附加至您所選任務或問題的核准。 如果您尚未新增任何核准，請從下拉式選單中選取現有核准，或按一下 **[!UICONTROL 建立單一使用核准程式]** 直接前往 [!UICONTROL 核准] 標籤上的任務或問題。

若要直接前往 [!UICONTROL 核准] 索引標籤上的任務或問題，按一下 **[!UICONTROL 核准]** 標題。

![摘要面板中的核准區段](assets/summary-approvals-section.png)
