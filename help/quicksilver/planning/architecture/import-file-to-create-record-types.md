---
title: 從CSV或Excel檔案匯入資訊，以建立記錄型別
description: 記錄型別是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以建立自訂記錄型別，藉由從CSV或Excel檔案匯入資訊，說明組織生命週期中所需的工作專案。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# 從CSV或Excel檔案匯入資訊，建立記錄型別

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

記錄型別是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以建立自訂記錄型別，藉由從CSV或Excel檔案匯入資訊，說明組織生命週期中所需的工作專案。

## 存取權要求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<p>任何Workfront和任何Planning套件</p>
或
<p>任何工作流程與任何Planning套件</p>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區的許可權</p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
 
</tbody> 
</table>-->


## 有關使用Excel或CSV檔案匯入記錄型別的考量事項

* Excel檔案的每一頁都會變成記錄型別。 工作表的名稱會變成記錄型別的名稱。
* 如果只有一張工作表，或者如果匯入CSV檔案，則檔案的名稱會變成記錄型別的名稱。
* 每個工作表中的欄標題會成為與每個記錄型別相關聯的欄位。
* 欄位對於其各自的記錄型別來說都是唯一的。
* 每個工作表中的每一列都會成為與其個別記錄型別相關聯的唯一記錄。
* 每個Excel檔案工作表不應超過下列專案：
   * 25,000列
   * 500欄
* 檔案不應大於5MB。
* 不支援空白工作表。
* 不支援下列型別的欄位，且無法對應至匯入工作表上的欄位：

   * Workfront、AEM Assets物件型別或GenStudio品牌的連線欄位。
   * 從連線的Planning記錄、Workfront、AEM Assets物件或GenStudio品牌中查詢欄位。
   * 公式欄位
   * 建立日期，建立者
   * 上次修改日期，上次修改者：
   * 核准日期，核准者
   * 人員

若要使用Excel或CSV檔案匯入記錄型別：

{{step1-to-planning}}

1. 按一下您要建立記錄型別的工作區，

   或

   從工作區中，展開現有工作區名稱右側的向下箭頭，搜尋工作區，然後在工作區顯示在清單中時選取該工作區。
1. 按一下&#x200B;**新增記錄型別**。
1. 按一下&#x200B;**從檔案**&#x200B;上傳。
1. 拖放先前儲存在電腦上的Excel或CSV檔案，或按一下&#x200B;**選取CSV或Excel檔案**&#x200B;來瀏覽並選取檔案。
1. 按一下&#x200B;**預覽和編輯**。

   **預覽和編輯**&#x200B;方塊會顯示下列資訊：

   * 工作表或未來記錄型別的名稱會顯示在左側面板中。 根據預設，Workfront Planning會選取每個新記錄型別的圖示和顏色。
   * 選擇第一個工作表或記錄型別，並且與其關聯的欄位名稱顯示為欄標題。 依預設，會選取每個欄位的型別。
   * 每一列代表新記錄。 只有前10筆記錄會顯示在「預覽與編輯」方塊中。

   ![預覽和編輯方塊](assets/preview-and-edit-box.png)

1. （選擇性）按一下左側面板中每個工作表的名稱，以檢閱其中包含的資訊。

   >[!NOTE]
   >
   >不支援空白的頁面，這些頁面會變暗。

1. （選擇性）從左側面板取消選取您不想要匯入的頁面。

   ![選取要匯入的工作表並取消選取](assets/select-sheets-to-import-drop-down-with-unselected.png)

   取消選取的頁面會以灰色背景顯示。

1. （選擇性）按一下欄標題右側的向下箭頭，在&#x200B;**欄位**&#x200B;索引標籤中執行下列其中一項作業：

   ![記錄型別對應匯入方塊上的欄位索引標籤](assets/field-tab-on-record-type-import-mapping-box.png)

   * 重新命名其中一個欄位
   * 變更&#x200B;**欄位型別**
   * 更新欄位&#x200B;**描述**

1. （選擇性）按一下&#x200B;**連線**&#x200B;索引標籤，將資料行中的資訊對應到其他記錄型別的連線欄位。

   ![記錄型別匯入對應方塊上的連線標籤](assets/connection-tab-on-record-type-import-mapping-box.png)

   >[!TIP]
   >
   >您只能對應至Workfront Planning連線記錄中的欄位。 您無法對應至Workfront、AEM Assets或GenStudio Brands連線的欄位。 如需詳細資訊，請參閱本文中[關於使用Excel或CSV檔案匯入記錄型別的考量事項](#considerations-about-importing-record-types-using-an-excel-or-csv-file)一節。

1. （視條件而定）更新欄位相關資訊後，按一下&#x200B;**儲存**。

1. 當您準備好匯入您的檔案時，請按一下[匯入]。****

   下列資訊會匯入Workfront Planning中：

   * 新記錄型別
   * 與每個記錄型別關聯的新欄位
   * 與每個記錄型別關聯的新記錄

   您可以開始管理記錄型別頁面上的欄位和記錄。

   有權存取Workfront Planning和工作區的每個人都現在可以檢視及編輯匯入的記錄型別及其資訊。
