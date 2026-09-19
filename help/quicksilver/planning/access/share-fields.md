---
title: 共用Workfront規劃欄位
description: 您可以與其他人共用Workfront Planning記錄的欄位，以確保在使用Adobe Workfront Planning時共同作業。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: ac94936cc4dc9dc4f2d56b3f1221f71a405c5c65
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 2%
---

# 共用Workfront規劃欄位

{{planning-important-intro}}

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 在「預覽」版發行後，啟用的客戶每月可在「生產」環境中使用相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


您可以與其他人共用Workfront Planning記錄的欄位，以確保在使用Adobe Workfront Planning時共同作業。

欄位共用可讓工作區管理員控制對個別欄位的存取權。 記錄型別中的每個欄位都有自己的共用對話方塊，其中存取權可以設定為無存取權、檢視欄位值或管理欄位值。

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
<p>具有Planning套件的任何Workfront或工作流程</p> 
或
<p>任何Workfront Planning作為獨立產品套件</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>任何</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe計畫授權</p></td> 
   <td><p>任何</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>擁有Workflow和Planning套件時，您必須將Workflow和Planning授權型別新增到存取層級</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td><p>管理欄位的許可權以變更欄位的值</p>  
   <p>貢獻或更高的記錄型別許可權以繼承欄位的管理許可權</p>  
   </td> 
  </tr>
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共用欄位的相關考量事項

* 您可以與使用者、工作角色、群組、團隊或公司共用欄位。
* 您只能從記錄型別的表格檢視中共用欄位。
* 您無法共用下列型別的欄位：

  * 系統欄位（例如，建立者、記錄ID）
  * 主要欄位
  * 查詢欄位。 使用者一律會繼承其來源物件欄位的許可權。
* 對欄位的存取權來自結合下列設定：

  * **繼承許可權**：依預設，欄位會繼承某人對於記錄型別的相同存取權。 您可以關閉繼承許可權，並給予使用者比記錄型別更低的欄位存取權。
  * 有權存取記錄型別的&#x200B;**每個人都可以檢視**&#x200B;或&#x200B;**只有受邀者才能存取**&#x200B;選取專案。 您可以允許擁有工作區許可權的所有人檢視欄位，或僅將許可權授予個別實體。

  如果同一個人套用多個規則，這些規則會從其中一個規則中取得他們可用的最高許可權。

* 若要讓工作區的每個人都可以檢視欄位，請確定下列設定存在：

  * 關閉繼承的權限
  * 保留&#x200B;**所有可存取記錄型別的人都可以檢視**&#x200B;設定
  * 請勿新增任何個別實體。

* 根據記錄型別許可權，使用者可以收到以下欄位許可權：

  * 檢視記錄型別許可權授予使用者檢視欄位值的許可權
  * Contribute或Manage記錄型別許可權提供使用者管理欄位值的許可權

* 只有工作區擁有者和管理員可以調整欄位許可權。 Workspace管理員一律保留所有欄位的「管理」存取權，且不可降低。
* 欄位共用控制對值的存取，而不是欄位設定。 只有工作區管理員可以變更欄位的設定。
* 將某人新增至欄位的共用清單不會授予他們工作區或記錄型別存取權。 如果他們沒有該存取權，警告圖示會指出該許可權只有在將其新增到記錄型別後才會生效。
* 具有受限制許可權的欄位會在任何顯示欄位的位置強制執行。 這包括所有的檢視、記錄詳細資訊頁面、請求表單、連線和查詢欄位、畫布控制面板、API和MCP工具。
* 任何可以存取公開檢視的使用者都能完全看見這些檢視，且維持唯讀狀態。
  <!--Not sure if this is right - right now, it allows me to duplicate with the values in the new record - checking with Lilit: * When you duplicate a record, the restricted values are not copied to the new records.-->
* 限制的欄位值變更不會記錄在記錄的歷史記錄中。
* 欄位的許可權變更不會觸發通知。
* 對於全域記錄型別，欄位許可權會套用至所有次要工作區，且無法在本機調整。

<!--
From Claude: 
Additional permissions for fields - maybe add this to the Overview article for all of the sharing?? - help/quicksilver/planning/access/sharing-permissions-overview.md 

Here's how record type / workspace access maps to field-level access in the document:

Field permission levels (only two, plus none):

No Access – field is completely hidden
View field values – can see the value, can't edit
Manage field values – can view and edit

Default inheritance from record type role

Record type / workspace access    Default field permission
View    View field values
Contribute    Manage field values
Manage (workspace manager)    Manage field values (locked — cannot be reduced)

So by default, a field simply mirrors whatever role someone has on the record type — Viewers get read-only, Contributors and Managers get edit rights. Workspace managers are a special case: whenever they're added to a field's sharing list, "Manage field values" is pre-selected and the "View field values" option is disabled, since their edit access can never be taken away.

Wildcard (fallback) setting
Separate from inheritance, each field has a wildcard default:

Everyone in the workspace can view (default)
Only invited people can access

How the final permission is calculated

If inherited permissions are enabled: a person's access = the highest of (inherited from record type, wildcard, individually granted permission).
If inherited permissions are disabled: a person's access = the highest of (wildcard, individually granted permission) — record type role no longer factors in.
If inheritance is disabled, wildcard is "Only invited people can access," and the person isn't individually added → they get No Access.

Other permission notes

Individually granting access to someone doesn't grant them workspace/record-type access — it just sits inactive (with a warning icon) until they're separately added to the workspace.
For Global Record Types, field permissions are set once and apply to all secondary workspaces; secondary/team workspace managers cannot override them locally.

-->

## 共用欄位

身為工作區管理員，您可以調整個別欄位的許可權。

{{step1-to-planning}}

1. 開啟工作區，然後開啟要共用其欄位的記錄型別。

1. 在表格檢視中，暫留在欄位欄位標題的名稱上，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**共用欄位**。

   **共用**&#x200B;方塊開啟。

1. （選擇性）在&#x200B;**授與存取權**&#x200B;區域中，預設會選取&#x200B;**有權存取記錄型別的所有人都可以檢視**&#x200B;選項。 所有對工作區和記錄型別具有&#x200B;**檢視**&#x200B;或更高許可權的使用者對該欄位具有相同的許可權。

1. （可選）按一下「**繼承自**&#x200B;的許可權」選項下的使用者頭像，以檢視從工作區繼承許可權的使用者、團隊、群組、公司或工作角色。

   當您展開繼承的許可權時，會顯示使用者對記錄型別的許可權。

   >[!TIP]
   >
   >您無法從繼承的許可權清單中移除個別實體。 列出來自團隊、群組、公司或工作角色的使用者，而不是與他們共用工作區和記錄型別時他們關聯的實體。

1. （選擇性和條件性）如果您想要與特定實體共用欄位，並授予他們與記錄型別不同的欄位存取權，請執行以下操作：

   1. 從&#x200B;**繼承許可權**&#x200B;中取消選取&#x200B;**開啟**&#x200B;選項。 預設會選取此選項。

      選項變更為&#x200B;**已關閉**。

      >[!TIP]
      >
      >Workspace管理員繼續擁有記錄型別和欄位的管理許可權。

   1. （選擇性）按一下&#x200B;**每個可存取記錄型別的使用者都可以檢視**&#x200B;下拉式功能表，並選取&#x200B;**只有受邀者才能存取**。

      >[!IMPORTANT]
      >
      >此變更與關閉&#x200B;**繼承的許可權**&#x200B;會移除所有可以檢視記錄型別並僅將存取權授予指定人員之人員的存取權。 Workspace管理員和管理員永遠都可存取所有欄位。


   1. 在&#x200B;**授與存取權**&#x200B;方塊中，新增您要授與不同於工作區或記錄型別之許可權等級的使用者、團隊、群組、公司或工作角色。

      當您和使用者共用欄位時，他們的主要工作角色和電子郵件也會顯示在欄位中。 您必須為存取層級中的Users物件啟用[檢視連絡人資訊]設定，才能檢視使用者的電子郵件。

   1. 選擇下列其中一個許可權層級：

      * 檢視欄位值
      * 管理欄位值

      >[!IMPORTANT]
      >
      ><!-- * If users have Contribute or Manage permissions to the workspace and the record type, you can give them Manage permissions to the field. The View permission is dimmed.-->
      >* 如果使用者擁有記錄型別的Contribute或以上版本，則您無法授予其較少的欄位許可權。
      >
      >* 您無法向不在工作區中的使用者授予許可權。 沒有工作區許可權和記錄型別的使用者無法存取任何欄位。 當他們取得工作區和記錄型別的許可權時，將能夠存取欄位。

1. 按一下「**儲存**」。

   此欄位現在已與其他使用者共用。

   <!--
    Not possible for fields: 
    The users you shared the field with receive both an in-app and email notification about having been given permissions to the field.
    For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md).
    -->

## 移除欄位的許可權

您可以從欄位中移除使用者的許可權。 但是，他們至少會保留工作區的檢視許可權和記錄型別，這也會為他們提供至少欄位的檢視許可權。

如果您希望他們沒有工作區中記錄型別或欄位的許可權，則必須從工作區中移除他們的存取權。

您無法從繼承的許可權中移除使用者。

{{step1-to-planning}}

1. 開啟您要停止共用其欄位的工作區，然後按一下記錄型別卡片。 這會開啟記錄型別頁面。
1. 在表格檢視中，暫留在欄位欄位標題的名稱上，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**共用欄位**。

   **共用**&#x200B;方塊開啟。
1. 尋找您要移除其許可權的使用者、群組、團隊、公司或工作角色，展開其名稱右側的許可權下拉式功能表，然後按一下&#x200B;**移除**。

1. 按一下「**儲存**」。

   人員不再具有此欄位所指示的許可權。 但是，他們仍擁有記錄型別和工作區的許可權，除非您也將他們從這些許可權中移除。

   對於已從存取欄位中移除的使用者，不會通知他們不再擁有這些許可權。
