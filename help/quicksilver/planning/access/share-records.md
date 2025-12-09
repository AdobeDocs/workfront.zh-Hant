---
title: 共用記錄
description: 您可以使用「共用」按鈕共用記錄，以提升Adobe Workfront Planning中的協同合作。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: e6fc6def1553df3faa8e1200f7ec2ca2bb97eb04
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 2%

---


<!--update metadata with real information at release-->

# 共用記錄

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

您可以調整人員對記錄型別中個別記錄的許可權。

您可以透過下列方式共用Adobe Workfront Planning記錄：

* 共用記錄的連結。

  如需詳細資訊，請參閱[使用連結](/help/quicksilver/planning/records/share-records.md)共用記錄。

* 透過共用工作區和記錄型別，與其他使用者共用工作區中的所有記錄。

  如需詳細資訊，請參閱下列文章：

   * [共用工作區](/help/quicksilver/planning/access/share-workspaces.md)

   * [共用記錄型別](/help/quicksilver/planning/access/share-record-types.md)

* 使用&#x200B;**共用**&#x200B;選項共用記錄。

  本文說明如何使用&#x200B;**共用**&#x200B;選項與其他人共用記錄。

>[!IMPORTANT]
>
>有權存取工作區的使用者至少會自動取得對工作區中所有記錄的檢視許可權。
>共用檢視不會提供使用者記錄許可權。 只有共用工作區才能授予使用者記錄型別和記錄的許可權。
>
>如需在Workfront Planning中共用物件的一般資訊，另請參閱[在Adobe Workfront Planning中共用許可權概觀](/help/quicksilver/planning/access/sharing-permissions-overview.md)。


## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<p>任何Workfront和Planning套件</p> 
或
<p>任何工作流程和Planning套件</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>任何</p> 
   <p><b>附註</b></p>
   <p>只有具有Standard授權的使用者才能被授與記錄的「管理」許可權。 所有其他授權只能具有「檢視」許可權，而且這些授權的「管理」選項會變暗。</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>  <p>管理工作區、記錄型別和記錄的許可權</p>  
   <p><b>重要</b></p>
   <p>只有對工作區具有管理許可權的使用者才能共用記錄</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> 必須為具有輕度或貢獻者授權的使用者指派包含Planning的版面配置範本。
   <p>標準使用者和系統管理員預設會啟用Planning區域。</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共用記錄時的注意事項

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

<!--checking on the below with Lilit-->

* 您可以與下列實體共用記錄：人員、群組、團隊、公司或職務角色。
* 當您與使用者共用工作區時，預設情況下，他們也會收到工作區中記錄的相同許可權。
* 當您從工作區中移除實體時，所有共用許可權都會從記錄型別及其中的所有記錄中移除。
* 使用者對記錄的存取權取決於以下3個設定的組合：

   * 其許可權繼承自記錄型別和工作區
   * 在記錄共用對話方塊中個別新增許可權
   * 下列許可權：

      * **工作區的每個人都可以檢視**：這可以讓工作區的每個人<!-- is this OK to say "workspace? should it be "record"??-->都可以檢視記錄
      * **只有受邀者才能存取**：這是預設選取的選項，允許限制特定人員存取記錄。

* 您可以授予記錄的下列許可權層級：

   * 檢視
   * 管理

* 當您與使用者共用記錄時，預設會以與記錄型別相同的許可權新增使用者。

  例如：

   * 如果他們擁有記錄型別的檢視許可權，他們將獲得記錄的檢視許可權
   * 如果他們擁有記錄型別的「貢獻」或「管理」許可權，他們將獲得記錄的「管理」許可權

* 身為工作區管理員，您可以與非工作區一部分的使用者共用記錄。 在這種情況下，新增的實體旁邊會出現警告，通知他們無權存取工作區。 您可以繼續將使用者新增至記錄，這也會將使用者新增至工作區，或停止將使用者新增至記錄，這也不會將使用者新增至工作區。

* 當您與具有工作區管理許可權的使用者共用記錄時，他們也會依預設取得該記錄的管理許可權。 檢視許可權會變暗。

* 如果您沒有將人員新增至工作區的許可權，您將只會看到並新增已新增至工作區的使用者、團隊、群組、角色和公司。 您無法新增任何尚未成為工作區一部分的實體。

* 您可以停用單一記錄的繼承許可權，在這種情況下，您可以授予他們個別記錄的許可權，或者如果他們屬於&#x200B;**工作區中的每個人都可以檢視**&#x200B;選項，則他們可以取得許可權。<!-- is this OK to say "workspace? should it be "record"??-->

* 如果同一個使用者套用多個共用許可權，這些使用者會獲得這些許可權的最高許可權。

  例如，如果記錄與具有檢視許可權的使用者共用，並且其群組具有管理存取權，則他們可獲得該記錄的管理許可權。

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* 如果所連線記錄的公式欄位或查閱欄位是以您沒有許可權的記錄欄位為基礎的，您將看到正確的計算，其中哪些是您無法以其他方式存取的記錄因素。

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## 共用記錄許可權

如果您有工作區的管理許可權，您可以調整個別記錄的許可權。

{{step1-to-planning}}

1. 開啟您要共用其記錄的工作區。
1. 按一下您要共用其記錄的記錄型別。

1. 執行下列其中一項：

   * 在資料表檢視中，暫留在記錄名稱上，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**共用**。
   * 從任何檢視中，按一下記錄名稱，然後按一下記錄詳細資訊頁面右上角的&#x200B;**共用**。

   **共用**&#x200B;方塊開啟。

   ![具有繼承許可權的記錄在](assets/permissions-for-records-with-inherited-permissions-on.png)上的許可權

1. （選擇性）在&#x200B;**擁有存取權**&#x200B;區域中，預設會選取&#x200B;**工作區中的每個人都可以檢視**&#x200B;選項。  所有對工作區和記錄型別具有檢視或更高許可權的使用者都可以檢視記錄。

1. （選擇性）按一下&#x200B;**繼承的許可權**&#x200B;選項下的使用者人數，以檢視從工作區繼承許可權的使用者、團隊、群組、公司或工作角色。

   >[!TIP]
   >
   >您無法從繼承的許可權清單中移除個別實體。

1. （選擇性和條件性）如果您想要與特定實體共用記錄型別，並授予他們不同於工作區現有的記錄型別存取權，請執行以下操作：

   1. 從&#x200B;**繼承許可權**&#x200B;下拉式功能表中選取&#x200B;**停用**。

   >[!TIP]
   >
   >Workspace管理員繼續擁有記錄型別和記錄的管理許可權。

   1. （選擇性）選取&#x200B;**只有受邀者才能從**&#x200B;誰有存取權&#x200B;**區域存取**。

   1. 在&#x200B;**授與此記錄型別**&#x200B;的存取權欄位中，新增您要授與不同於工作區或記錄型別之許可權等級的使用者、團隊、群組、公司或工作角色。
   1. 選擇下列其中一個許可權層級：

      * 檢視
      * 管理

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* 除了團隊、群組、公司和職務角色之外，您只能與已新增至Adobe Admin Console的使用者共用。 您無法新增僅限Workfront的使用者。 如需詳細資訊，請參閱[在Adobe Admin Console中管理使用者](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。
   >* 如果使用者擁有工作區和記錄型別的「貢獻」或「管理」許可權，他們將保留記錄的「管理」許可權。 檢視許可權會變暗
   >* 如果使用者擁有Contribute或以上版本，則您無法授予他們較低許可權存取記錄。
   > 如需詳細資訊，請參閱[在Adobe Workfront Planning中共用許可權的總覽](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

1. 若要為沒有工作區存取許可權的使用者提供檢視記錄的存取許可權，請在&#x200B;**授予此檢視的存取許可權**&#x200B;欄位中，開始輸入使用者、群組、團隊、公司或工作角色的名稱，然後當它顯示在清單中時按一下它。

   您選取的實體已新增至記錄和工作區，並具有&#x200B;**檢視**&#x200B;許可權。

   系統管理員一律會收到與其共用之記錄的管理許可權，並會顯示使用者是系統管理員。

1. （選擇性）按一下&#x200B;**複製連結**&#x200B;以將記錄的連結複製到剪貼簿，並與他人共用。 該連結將開啟記錄的詳細資訊頁面。
1. 按一下「**儲存**」。

   記錄現在已與其他使用者共用。
   <!--Checking with Lilit on this: The users you shared the record with receive both an in-app and email notification about having given permissions to the following entities:

   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them. -->

1. 與他人共用複製的連結。 收到連結的使用者必須是作用中使用者，並登入Workfront，才能存取記錄型別頁面並在選取的檢視中顯示該頁面。 使用者必須具有記錄型別的許可權才能檢視該記錄型別。 如需詳細資訊，另請參閱[使用連結](/help/quicksilver/planning/records/share-records.md)共用記錄。

## 移除記錄的許可權(**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;***&#x200B;這是從記錄型別複製而來，需要針對記錄進行編輯，但等待LILIT的SLACK回應&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**)

您可以從記錄中移除使用者的許可權。 但是，他們至少會保留記錄工作區的檢視許可權，這也會給予他們記錄型別的至少檢視許可權。 如果您希望他們沒有工作區中記錄型別的許可權，則必須從工作區中移除他們的存取權。

{{step1-to-planning}}

1. 開啟您要停止共用其記錄型別的工作區，然後按一下記錄型別卡片。 這會開啟記錄型別頁面。

1. 從任何檢視的索引標籤，按一下記錄型別右上角的&#x200B;**共用**。
1. 按一下&#x200B;**共用記錄型別**。

   **共用**&#x200B;方塊開啟。
1. 尋找您要移除其許可權的使用者、群組、團隊、公司或工作角色，展開其名稱右側的許可權下拉式功能表，然後按一下&#x200B;**移除**。<!--check the screen shot below - the UI text for View might not be accurate-->

   ![移除記錄型別共用下拉式清單上的選項](assets/remove-option-on-record-type-sharing-drop-down.png)

1. 按一下「**儲存**」。

   人員不再具有記錄型別的指定許可權。 但是，他們仍擁有工作區的許可權，除非您也將他們從工作區許可權中移除。

   對於已從存取檢視中移除的使用者，不會通知他們不再擁有此存取權。
