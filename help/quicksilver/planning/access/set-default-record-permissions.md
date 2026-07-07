---
title: 設定記錄的預設許可權
description: 修改記錄型別或工作區設定時，您可以設定記錄的預設許可權。 您可以將開啟或限制的許可權授與將針對記錄型別新增的所有記錄。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: a76a39fde984bece43cda9812c436d81f41eb989
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 3%

---


# 設定記錄的預設許可權

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 在「預覽」版發行後，啟用的客戶每月可在「生產」環境中使用相同的功能。</span>\
<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}


修改記錄型別或工作區設定時，您可以設定記錄的預設許可權。

您可以將開啟或限制的許可權授與將針對記錄型別新增的所有記錄。


## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

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

</tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>任何</p> 
   <p><b>附註</b></p>
   <p>只有具有Standard授權的使用者才能被授與記錄的「管理」許可權。 所有其他授權只能具有「檢視」許可權，而且這些授權的「管理」選項會變暗。</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>  <p>管理工作區和記錄型別的許可權</p>  
   <p><b>重要</b></p>
   <p>只有對工作區具有管理許可權的使用者才能共用記錄</p></td> 
  </tr>
</tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定預設記錄許可權的考量事項

設定預設記錄許可權時，請考慮下列事項：

* 每個記錄型別一次只能有一個預設許可權規則為作用中。
* 變更規則只會影響變更後建立的記錄。 現有記錄會保留其目前的許可權。
* 無論規則為何，系統管理員與工作區管理員一律保留管理每個記錄的存取權。
* 建立記錄後，即可在共用對話方塊中獨立變更其許可權，而不會影響預設規則。
* 對於全域記錄型別，每個工作區（主要和次要）都可以設定自己的預設規則，而新記錄會採用建立它們的工作區規則。

## 設定工作區的預設記錄許可權

1. 前往工作區> **更多**&#x200B;功能表![更多功能表](assets/more-menu.png) > **設定** > **記錄型別**。

   ![Workspace記錄型別設定區域](assets/workspace-record-types-settings-area.png)

1. （選擇性）在&#x200B;**記錄型別**&#x200B;的儲存格內按一下，以編輯記錄型別名稱。

1. 在&#x200B;**新記錄許可權預設值**&#x200B;欄中，按一下您要更新其許可權的記錄型別儲存格。

1. 從下列選項中選擇:

   * **開啟**：所有工作區參與者都可以管理新建立的記錄。 這是所有現有及新記錄型別的目前預設行為。
   * **已限制**：只有記錄建立者和您明確新增的任何人都可以編輯新建立的記錄。 其他所有人都取得僅限檢視的存取權。

1. （視條件而定）如果您要將預設許可權從&#x200B;**受限制的**&#x200B;變更為&#x200B;**開啟**，請按一下&#x200B;**切換至開啟**&#x200B;方塊中的&#x200B;**切換**&#x200B;以確認您的選擇。
1. （視條件而定）如果您選取&#x200B;**受限制的**，請在&#x200B;**誰可以編輯記錄**&#x200B;欄中新增其他編輯器。 您可以新增使用者、群組、團隊、角色或公司。

   >[!NOTE]
   >
   >* 記錄建立者永遠包括在內，且無法移除。
   >* 您只能選取已有該記錄型別的「貢獻」或「管理」許可權的實體。

   變更會自動儲存。 儲存後，規則會立即生效，並自動套用至針對該記錄型別建立的所有記錄。

## 設定記錄型別的預設記錄許可權

1. 移至記錄型別> **更多**&#x200B;功能表![更多功能表](assets/more-menu.png) > **設定** > **記錄設定**。

   ![記錄型別設定區域中的[記錄設定]索引標籤](assets/record-settings-tab-in-record-type-settings-area.png)

1. 在&#x200B;**記錄許可權型別**&#x200B;欄位中，按一下下列其中一個選項：

   * **開啟**：所有工作區參與者都可以管理新建立的記錄。 這是所有現有及新記錄型別的目前預設行為。
   * **已限制**：只有記錄建立者和您明確新增的任何人都可以編輯新建立的記錄。 其他所有人都取得僅限檢視的存取權。
1. （視條件而定）如果您要將預設許可權從&#x200B;**受限制的**&#x200B;變更為&#x200B;**開啟**，請按一下&#x200B;**切換至開啟**&#x200B;方塊中的&#x200B;**切換**&#x200B;以確認您的選擇。
1. （視條件而定）如果您選取&#x200B;**受限制的**，請在&#x200B;**誰可以編輯記錄**&#x200B;欄位中新增其他編輯器。 您可以新增使用者、群組、團隊、角色或公司。

   >[!NOTE]
   >
   >* 記錄建立者永遠包括在內，且無法移除。
   >* 您只能選取已有該記錄型別的「貢獻」或「管理」許可權的實體。

   變更會自動儲存。 儲存後，規則會立即生效，並自動套用至針對該記錄型別建立的所有記錄。