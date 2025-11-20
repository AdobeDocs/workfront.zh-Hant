---
title: 共用記錄
description: 您可以使用「共用」按鈕共用記錄，以提升Adobe Workfront Planning中的協同合作。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 0964ad24535bf43a23c740cd63abcf8fea705b8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 2%

---


<!--update metadata with real information at release-->

# 共用記錄

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

您可以調整人員對記錄型別中個別記錄的許可權。 O

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


## 存取需求

+++ 展開以查看此文章中功能的存取需求。 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 套件</p></td> 
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

* 身為工作區管理員，您可以與非工作區一部分的使用者共用記錄。 在這種情況下，新增的實體旁邊會出現警告，通知他們無權存取工作區。 您可以接受將使用者新增至記錄和工作區，或拒絕將使用者新增至工作區，這也會將使用者從記錄中移除。

* 當您與具有工作區管理許可權的使用者共用記錄時，他們也會依預設取得該記錄的管理許可權。 檢視許可權會變暗。

* 如果您沒有將人員新增至工作區的許可權，您將只會看到並新增已新增至工作區的使用者、團隊、群組、角色和公司。 您無法新增任何尚未成為工作區一部分的實體。

* 您可以停用單一記錄的繼承許可權，在此情況下，您可以單獨授予他們許可權，或者如果他們屬於「工作區中的每個人」選項，則可獲得許可權。<!-- is this OK to say "workspace? should it be "record"??-->

* 如果同一個使用者套用多個共用許可權，這些使用者會獲得這些許可權的最高許可權。

  例如，如果記錄與具有檢視許可權的使用者共用，並且其群組具有管理存取權，則他們可獲得該記錄的管理許可權。

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* 如果所連線記錄的公式欄位或查閱欄位是以您沒有許可權的記錄欄位為基礎的，您將看到正確的計算，其中哪些是您無法以其他方式存取的記錄因素。

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## 共用記錄許可權

