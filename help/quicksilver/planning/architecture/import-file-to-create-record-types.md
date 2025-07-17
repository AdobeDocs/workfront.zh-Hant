---
title: 從CSV或Excel檔案匯入資訊，以建立記錄型別
description: 記錄型別是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以建立自訂記錄型別，藉由從CSV或Excel檔案匯入資訊，說明組織生命週期中所需的工作專案。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# 從CSV或Excel檔案匯入資訊，建立記錄型別

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

記錄型別是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以建立自訂記錄型別，藉由從CSV或Excel檔案匯入資訊，說明組織生命週期中所需的工作專案。

## 存取需求

+++ 展開以檢視存取需求。

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront規劃<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> 
<p>下列任一Workfront計畫：</p> 
<ul><li>選取</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準</p>
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>

</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


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

   * Workfront和AEM Assets物件型別的連線欄位。
   * 從連線的Planning記錄或Workfront與AEM Assets物件查詢欄位
   * 公式欄位
   * 建立日期，建立者
   * 上次修改日期，上次修改者：
   * <span class="preview">核准日期，核准者：</span>
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
   >您只能對應至Workfront Planning連線記錄中的欄位。 您無法從Workfront或AEM Assets連線對應到欄位。 如需詳細資訊，請參閱本文中[關於使用Excel或CSV檔案匯入記錄型別的考量事項](#considerations-about-importing-record-types-using-an-excel-or-csv-file)一節。

1. （視條件而定）更新欄位相關資訊後，按一下&#x200B;**儲存**。

1. 當您準備好匯入您的檔案時，請按一下[匯入]。****

   下列資訊會匯入Workfront Planning中：

   * 新記錄型別
   * 與每個記錄型別關聯的新欄位
   * 與每個記錄型別關聯的新記錄

   您可以開始管理記錄型別頁面上的欄位和記錄。

   有權存取Workfront Planning和工作區的每個人都現在可以檢視及編輯匯入的記錄型別及其資訊。
