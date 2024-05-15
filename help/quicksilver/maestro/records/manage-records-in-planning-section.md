---
title: 在Adobe Workfront物件的Planning區段中管理記錄
description: 您可以在左側面板的Adobe Workfront物件的Planning區段中，顯示連線至Workfront物件的記錄。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 9b1b8d8661917946230033b661ca652f5edef734
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 1%

---

<!--add this to the main TOC and the mini TOC-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--add also Group and Company when they are available-->


# 在Adobe Workfront物件的Planning區段中管理記錄

{{maestro-important-intro}}

您可以在左側面板的Adobe Workfront物件的Planning區段中，顯示連線至Workfront物件的記錄。

「規劃」區段適用於下列Workfront物件：

* 專案
* 專案組合
* 方案
<!--* Group
* Company-->

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 產品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>貴組織必須註冊Adobe Workfront Planning測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront計畫</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權*</p></td>
   <td>
   <p>新增：標準</p>
   或
   <p>目前：計畫</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>檢視專案、方案和Portfolio的或更高存取權</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>在Workfront中，檢視專案、專案組合或方案的或更高許可權</a> </p> 
   <p>在Workfront Planning中，檢視或更高的工作區許可權</a> </p>  
   <p>系統管理員擁有所有Workfront Planning工作區的許可權，包括他們未建立的工作區</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在主功能表中新增Planning區域，並在左側面板中新增Planning區段至您的版面配置範本。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 關於Workfront物件Planning區段的考量事項

* 首先，您必須將記錄型別連線至Workfront物件型別，並將記錄連線至Workfront物件，才能在Workfront中檢視它們。

  如需詳細資訊，請參閱下列文章：

   * [連線記錄型別](/help/quicksilver/maestro/architecture/connect-record-types.md)
   * [連接記錄](/help/quicksilver/maestro/records/connect-records.md)
* 即使沒有與Workfront物件相關聯的記錄，您仍可以在Workfront物件中檢視Planning區段。
* 您可以在Planning區段中，將Planning記錄與Workfront的Workfront物件連線。

## 管理Planning區段中的記錄

{{step1-to-maestro}}

預設會開啟上次存取的工作區。

1. 按一下連線到Workfront專案、投資組合或方案的記錄型別的卡片。
1. 從中選擇表格檢視 **檢視** 下拉式功能表。
1. （視條件而定）前往表格中的已連線記錄欄位並新增Workfront物件，然後按一下欄位中的Workfront物件名稱。 如需詳細資訊，請參閱 [連線記錄](/help/quicksilver/maestro/records/connect-records.md).
物件的頁面會在Workfront Planning中開啟。
1. 按一下 **移至來源**，位於畫面的右上角。

   物件的頁面會在Workfront中開啟。
1. 按一下 **規劃** 在左側面板中。

   >[!NOTE]
   >
   >   您的Workfront或群組管理員必須先將Planning區段新增到您的版面配置範本中，才能為Workfront專案、投資組合或方案顯示該區段。

   Planning區段會顯示下列資訊：

   * 連線的記錄會顯示在包含以下資訊的個別卡片上：
      * 記錄名稱
      * 記錄縮圖
      * 在Workfront Planning中顯示的連線記錄欄位名稱。
   * 記錄會顯示在各自的工作區下。

   ![](assets/planning-section-on-project.png)

1. 按一下記錄卡以顯示有關記錄的更多資訊。 記錄預覽方塊隨即顯示。
1. （選用）開始修改記錄預覽方塊中的欄位。 您的變更會自動儲存。
1. （可選）按一下 **在新標籤中開啟** 圖示 ![](assets/open-details-in-a-new-tab-icon.png) 在預覽方塊的右上角，開啟記錄的詳細資訊頁面。
1. 暫留在記錄卡上，然後按一下中斷連線記錄圖示 **-**，然後按一下 **中斷連線**.
會發生下列情況：
   * 記錄不再連線至Workfront物件。
   * Workfront物件也會從Workfront Planning的記錄連線欄位中移除。
   * 連線至Planning記錄的Workfront欄位值也會一併刪除。
1. 按一下 **連線** 以連線更多記錄。

   <!--checking with the team on the below note - not sure if if should stay Manage or be changed to Contribute??-->

   >[!NOTE]
   >
   >   只有您擁有管理許可權的工作區才會顯示「連線」按鈕。

1. 按一下您要連線的記錄。 會發生下列情況：

   * 記錄會立即連線至Workfront物件，並顯示在Planning區段中。
   * Workfront物件會新增至Workfront Planning記錄的已連線欄位。
   * 與Planning記錄連線之Workfront欄位的值會在Workfront Planning中填入。

<!--add more steps here for what happens after clicking Connect-->


