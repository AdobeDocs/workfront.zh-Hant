---
title: 使用版面配置範本自訂物件標頭
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 身為Adobe Workfront管理員或群組管理員，您可以使用版面配置範本來設定使用者在開啟物件頁面時，在物件標頭中看到的欄位。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# 使用版面配置範本自訂物件標頭

身為Adobe Workfront管理員或群組管理員，您可以使用版面配置範本來設定使用者在開啟物件頁面時，在物件標頭中看到的欄位。

>[!IMPORTANT]
>
>自訂物件標題目前可用於專案、任務和問題。

![](assets/object-header-fields.png)

如需有關建立版面範本的資訊，請參閱 [建立和管理版面範本](../use-layout-templates/create-and-manage-layout-templates.md).

如需有關群組版面配置範本的資訊，請參閱 [建立和修改群組的版面配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

設定版面範本後，您必須將其指派給使用者，才能讓其他人看見您所做的變更。 如需將版面配置範本指派給使用者的詳細資訊，請參閱 [將使用者指派至版面配置範本](../use-layout-templates/assign-users-to-layout-template.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：


<table>
  <tr>
   <td><strong>Adobe Workfront計畫</strong>
   </td>
   <td>任何
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront授權</strong>
   </td>
   <td>計劃
   </td>
  </tr>
  <tr>
   <td><strong>存取層級設定</strong>
   </td>
   <td>您必須是Workfront或群組管理員。
<p>
   </td>
  </tr>
</table>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 [建立或修改自訂存取層級](../../add-users/configure-and-grant-access/create-modify-access-levels.md).

## 自訂物件標頭

1. 開始使用版面範本，如所述 [建立和管理版面範本](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 在 **自訂使用者看到的內容** 下拉式功能表，選取 **專案**， **任務** 或 **問題**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. 在 [!UICONTROL 標題欄位] 區段，將滑鼠移至顯示的欄位上，然後執行下列任一項作業：
   * 按一下 **x** 圖示以移除欄位

     或

   * 按一下並按住 **抓取** 圖示以將欄位拖放至新位置。

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. 一個物件的標頭中最多可以有五個欄位。
如果您已選取五個欄位，則必須先移除欄位，才能新增欄位。
1. 在 **新增欄位** 方塊中，開始輸入您要新增的不可編輯Workfront欄位名稱，然後在其顯示在清單中時選取它。 欄位會新增至新增欄位方塊的緊鄰右側，並顯示為物件標頭左上角的第一個欄位。

   >[!TIP]
   >
   >* 您只能新增顯示在物件「詳細資訊」區段的「概觀」區域中且不可編輯的欄位。 不可編輯的欄位是使用者無法手動編輯的欄位。 Workfront會自動計算這些值。
   >
   >* 您可以新增已屬於預設標題的可編輯欄位（例如，專案所有者、狀態、完成百分比、指派）。
   >
   >* 當您將「解決者」欄位新增到問題的標題時，當存在與問題關聯的解決物件時，欄位會變更為「解決問題、任務或專案」。


   ![](assets/add-field-to-header-in-lt-list.png)


1. （選用）拖放以不同順序新增的欄位。

1. 繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下 **儲存**.

   >[!TIP]
   >
   >您可以隨時按一下「儲存」以儲存進度，然後繼續稍後修改範本。
