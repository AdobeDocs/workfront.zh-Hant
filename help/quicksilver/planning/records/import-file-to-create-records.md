---
title: 從CSV或Excel檔案匯入資訊，以建立記錄
description: 記錄是記錄型別的個別例項，這些是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以從CSV或Excel檔案匯入資訊，以建立記錄。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 940945df-391c-4672-9d9d-180d5028509b
source-git-commit: 3dfac5ada17248f5c67380b56b9a0969b10b73e6
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 1%

---


# 從CSV或Excel檔案匯入資訊，以建立記錄

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

記錄是記錄型別的個別例項，這些是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以從CSV或Excel檔案匯入資訊，以建立記錄。

如需建立記錄的詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。

## 存取需求

+++ 展開以檢視存取需求。

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
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td> 標準
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p> 
   <p>在Workfront中編輯您想要建立之物件型別（專案、方案和投資組合）的存取權，以便從新記錄連線它們  </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p>對工作區<span class="preview">和要新增記錄的記錄型別</span>貢獻或更高的許可權。 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
   <p>管理Workfront物件（專案組合）的許可權以新增子物件（專案）。</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>在生產環境中，所有使用者（包括系統管理員）都必須指派給包含Planning的版面配置範本。</p>
<p><span class="preview">在預覽環境中，標準使用者和系統管理員預設啟用Planning。</span></p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 使用Excel或CSV檔案匯入記錄時的注意事項

* 每個工作表中的欄標題會成為與記錄關聯的欄位。
* 每一張工作表中的每一列都會成為相關聯的唯一記錄。
* 如果Excel檔案包含多個頁面，則只匯入您在匯入過程中選取的一個頁面的資訊。
* 檔案不應超過下列專案：
   * 25,000列
   * 500欄
* 檔案不應大於5MB。
* 不支援空白工作表。
* 不支援下列型別的欄位，且無法對應至匯入工作表上的欄位：

   * &#x200B;<!--In the Production environment,--> Planning記錄或Workfront和AEM Assets物件的連線欄位

     <!--<span class="preview">In the Preview environment, you can map and import connection fields to Planning records. </span>-->

   * 從連線的Planning記錄或Workfront與AEM Assets物件查詢欄位
   * 公式欄位
   * 建立日期，建立者
   * 上次修改日期，上次修改者：
   * 人員
   * 如果匯入了多重或單一選取欄位，且與Planning中的類似欄位相比，其選擇更多，則會在匯入期間建立其他選項。 只有對工作區具有「管理」許可權的使用者才能匯入新的選擇。

## 透過匯入CSV或Excel檔案來建立記錄

{{step1-to-planning}}

1. 按一下您要建立記錄的工作區，

   或

   從工作區中，展開現有工作區名稱右側的向下箭頭，搜尋工作區，然後在工作區顯示在清單中時選取該工作區。
1. 按一下您要匯入記錄的記錄型別卡片。
1. 按一下熒幕右上角的&#x200B;**新增唱片**。

   ![選擇新增記錄的方式三個按鈕方塊](assets/choose-way-to-add-records-three-button-box.png)
1. 按一下&#x200B;**從檔案上傳**，然後按&#x200B;**繼續**。<!--add screen shot when all three buttons are added - with the Submit a request button-->
1. 拖放先前儲存在電腦上的Excel或CSV檔案，或按一下&#x200B;**選取CSV或Excel檔案**&#x200B;以瀏覽檔案。
1. 按一下&#x200B;**預覽和編輯**。
1. （視條件而定）如果匯入的檔案有多個工作表，請在&#x200B;**選取要匯入的工作表**&#x200B;方塊中選取您要匯入的工作表的選項按鈕，然後按一下&#x200B;**下一步**。 否則，請繼續進行下一個步驟。

   ![選取要匯入記錄的工作表](assets/select-a-sheet-to-import-box.png)
1. 在&#x200B;**將Planning欄位對應到您的欄標題**&#x200B;中，選取最符合每個工作表欄位資訊的&#x200B;**Planning欄位**。

   匯入記錄時![將Planning欄位對應到欄](assets/map-planning-fields-to-columns-when-importing-records.png)

   每一列代表新記錄。 只有前10筆記錄會顯示在「預覽與編輯」方塊中。

1. （選擇性和條件性）如果您擁有工作區的管理許可權，請選取畫面左下角的&#x200B;**建立缺少的選項**。 啟用時，會新增缺少的單選和多選欄位選擇。

   >[!NOTE]
   >
   >例如，如果選取的記錄型別具有單選「狀態」欄位，其中包含「新增」、「進行中」和「已關閉」選項，而從檔案匯入的「狀態」欄位也具有「保留狀態」選項，則也會新增「保留」狀態選項。
   >
   >如果您沒有工作區的「管理」許可權，您可以匯入記錄，但將不會建立其他選項。 相反地，您在[將Planning欄位對應到欄標題]方塊的右上角收到下列訊息： **連線、單一或多重選取欄位中不存在的選擇**。

1. 按一下&#x200B;**匯入**。

   下列資訊會匯入Workfront Planning中：

   * 顯示在所選記錄型別之表格檢視底部的新記錄。
   * 與每個記錄關聯的現有欄位的新欄位值。
   * Planning中沒有的多重或單一選取欄位的新選擇。 <!--when we add connected records - add those here too-->

   您可以在記錄型別頁面中開始管理欄位和記錄。

   有權存取Workfront Planning和工作區的每個人都現在可以檢視及編輯匯入的記錄及其資訊。

   <!--when we add connected records and the info icon in the tool changes, also add those items to the Import step and to the NOTE above it-->
