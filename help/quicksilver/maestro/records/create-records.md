---
title: 建立記錄
description: 在Adobe大師，記錄是記錄型別的例項。 在建立個別記錄之前，您必須先建立記錄型別。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: d3c22c84a9b246d1a45853c5d2825241f58bebe9
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# 建立記錄

>[!IMPORTANT]
>
>本文資訊是指Adobe Maestro，這是Adobe Workfront的新產品。
>
>目前，Adobe大師是測試版計畫的一部分，向有限數量的客戶開放。 您必須是Workfront客戶才能使用Maestro功能。
>
>如需加入Maestro測試版計畫的詳細資訊，請聯絡您的客戶代表。
>
>如需詳細資訊，請參閱 [Adobe大師概觀](../maestro-overview.md).

在Adobe大師，記錄是記錄型別的例項。

您可以擁有下列記錄型別：

* **作業記錄**：代表工作相關物件。 例如，針對名為「行銷活動」的營運記錄，您可以為「每月電子報」或「夏季銷售」等記錄命名。
* **分類法記錄**：它們代表可與作業記錄關聯的屬性。 例如，針對名為「頻道」的分類法記錄型別，您可以命名分類法，例如「電子郵件」、「社群媒體」或「廣告」。

建立作業記錄與建立分類記錄或分類相同。

您可以執行下列其中一項作業，在Maestro中建立記錄：

* 為Maestro記錄型別手動建立它們
* 將它們連線到來自協力廠商應用程式的Maestro記錄。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe產品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>貴組織必須註冊AdobeMaestro封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront計畫</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">存取層級</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">版面配置範本</td>
   <td> <p>您的系統管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/grant-access.md">授與Adobe大師的存取權</a>. </p>  
</td>
  </tr>
 </tbody>
</table>


<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 手動將記錄新增至記錄型別以建立記錄 <!--in a record type table (I don't think you can create them elsewhere right now)-->

您可以在記錄型別頁面的表格檢視中建立記錄。

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-workfront.png) 位於右上角，或 **主要功能表** 圖示 ![](assets/main-menu-shell.png) （如果有的話）按一下 **大師** ![](assets/maestro-icon.png).
您上次存取的工作區預設會開啟。 如需有關建立工作區的資訊，請參閱 [建立工作區](../architecture/create-workspaces.md).
1. 按一下記錄型別卡。 如需有關建立記錄型別的資訊，請參閱 [建立記錄型別](../architecture/create-record-types.md).

   記錄型別頁面會在您上次存取的檢視中開啟。 依預設，會在表格檢視中開啟記錄型別頁面。
所選型別的所有記錄都會顯示在表格檢視中。

1. （視條件而定）如果記錄型別頁面未在表格檢視中開啟，請按一下 **檢視** 下拉式功能表，並選取現有的 **表格檢視** ![](assets/table-view-icon.png) 或按一下 **建立檢視>表格** 以建立表格檢視。

1. 若要新增記錄，請按一下 **新&lt;記錄型別名稱>** 在表格的最後一列

   或

   按一下 **Shift + Enter** 從表格的任一欄或列移至鍵盤上。 這會新增空白列。

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. 開始在新列輸入有關新記錄的資訊。

   >[!NOTE]
   >
   >  * [名稱]欄位不是必要欄位。 不過，我們建議您為記錄新增名稱，因為將記錄連結至彼此時，有助於識別記錄。
   >
   >  * 參考其他記錄型別或計算欄位的欄位為唯讀欄位。

1. 繼續新增每一列的資訊，然後按一下 **輸入** 以儲存變更。

## 從其他應用程式連線記錄以建立記錄

您可以將記錄連結至Maestro連結的記錄，藉此從其他應用程式匯入記錄。

1. 建立Maestro記錄型別，如 [建立記錄型別](../architecture/create-record-types.md).

1. 為您在上一步建立的記錄型別建立Maestro記錄。 如需詳細資訊，請參閱區段 [手動將記錄新增至記錄型別以建立記錄](#create-records-by-manually-adding-them-to-a-record-type) 本文章內容。

1. 針對您建立的Maestro記錄型別，從協力廠商應用程式建立與物件型別的連線。 如需詳細資訊，請參閱 [連線記錄型別](../architecture/connect-record-types.md).

1. 使用您在上一步建立的連結記錄欄位，將第三方應用程式的記錄新增至您在上一步建立的Maestro記錄。 如需詳細資訊，請參閱 [連線記錄](../records/connect-records.md).

   在Maestro中建立下列專案：

   * 唯讀的Maestro記錄型別，參考您在連線記錄欄位中連結的第三方記錄型別。

     例如，如果您將Maestro記錄型別連線至Workfront專案，會在相同工作區中建立名為「Workfront專案」的唯讀記錄型別。
   * 第三方記錄型別頁面中的唯讀記錄。 從協力廠商應用程式匯入的記錄仍維持唯讀狀態，且只能在其原始應用程式中更新。


## 從外部清單複製並貼上資訊，以建立記錄

1. 在Maestro中，開始在「表格」檢視中建立記錄，如區段中所述 [手動將記錄新增至記錄型別以建立記錄](#create-records-by-manually-adding-them-to-a-record-type) 本文章內容。

   請確定Maestro表格檢視具有您要填入新記錄資訊的欄（或欄位）。

1. 按一下 **新&lt;記錄型別名稱>** 在表格的最後一列，新增任意數目的新資料列至表格。

   例如，如果要從另一個應用程式貼上10筆新記錄的資訊，請將10列新增到表格檢視中。

1. 在另一個應用程式中，建立您要匯入Maestro的記錄清單。

   例如，您可以使用Excel試算表來建立清單。

   清單應包含表格格式的資訊。

   >[!TIP]
   >
   > 清單的欄應包含您在Maestro中擁有的現有欄位資訊。
   >
   > 確保您已在Maestro中建立所需的欄位，且工作表中的資訊以符合Maestro中每個欄位之資訊的正確格式顯示。

1. 從第三方應用程式中，選取數個列和欄，然後將資訊貼到記錄型別表格檢視中，從第一個新記錄開始。

   下列資訊會在Maestro中匯入：

   * 列包含新記錄
   * 欄會填入記錄欄位的資訊。
