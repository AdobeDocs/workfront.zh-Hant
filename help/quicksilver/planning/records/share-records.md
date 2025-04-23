---
title: 共用記錄
description: 您可以與其他人共用記錄以增加共同作業。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# 共用記錄

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

若要與其他使用者共同作業，您可以與其他使用者共用記錄。

您可以透過下列方式共用Adobe Workfront Planning記錄：

* 當頁面開啟時，從瀏覽器複製記錄頁面的連結。

* 在記錄型別的表格檢視中檢視記錄時，複製指向記錄頁面的連結。

* 您可以共用工作區<span class="preview">和記錄型別，藉此與其他使用者共用工作區中的所有記錄。</span>

  如需詳細資訊，請參閱下列文章：

   * [共用工作區](/help/quicksilver/planning/access/share-workspaces.md)

  <div class="preview">

   * [共用記錄型別](/help/quicksilver/planning/access/share-record-types.md)

  </div>

本文說明如何從記錄型別的表格檢視複製記錄頁面的連結。

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
   <td><p> 投稿人或更高授權 </p>
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
   <td>  <p>檢視工作區<span class="preview">和記錄型別</span>的更高許可權以進行共用   使用連結的記錄 </p>
   <p>管理工作區<span class="preview">和記錄型別</span>的許可權，以共用工作區中的記錄 </p>
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--replace the layout template info in the table with this at release: 

<div class="preview">
<p> Users with a Light or Contributor license must be assigned a layout template that includes the Planning option  in the following areas:</p>
   <ul><li>Main Menu</li>
   <li>Left panel of projects, portfolios, and programs</li>
   <li>Landing page</li>
   <li>Pins</li></ul>
   <p>For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Create and manage layout templates</a>.</p>
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div>
   <p><b>NOTE</b></p>
   <p>In the Production environment, all users including the System administrators must be assigned to a layout template that includes the Planning areas.</p>

-->

## 從記錄型別表格檢視共用記錄連結

{{step1-to-planning}}

您上次存取的工作區會開啟。
1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。
1. （視條件而定）從表格右上角的&#x200B;**檢視**&#x200B;下拉式功能表中，選取表格檢視。 這應為預設檢視，除非您上次存取時間軸檢視時已檢視該記錄型別。

   與所選記錄型別相關聯的記錄會顯示在表格檢視中。
1. 以滑鼠右鍵按一下記錄列

   或

   將游標停留在記錄名稱上，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**複製連結**。

   ![記錄列](assets/contextual-menu-for-record-row.png)的內容相關功能表

   連結已複製到您的剪貼簿。

1. 將連結貼到電子郵件或聊天視窗中，以便與其他使用者共用。 使用者收到連結時，會開啟記錄頁面。

   >[!TIP]
   >
   >記錄頁面中的欄位與記錄的「表格」檢視中可用的欄位相同。


   <!--add there when it will be available: if they have access to this record-->

## 透過共用工作區來共用工作區中的所有記錄

當您與其他人共用工作區時，可以共用工作區中的所有記錄。

只有具有工作區管理許可權的使用者才能與其他人共用。

如需詳細資訊，請參閱[共用工作區](/help/quicksilver/planning/access/share-workspaces.md)。


<div class="preview">

## 透過共用記錄型別來共用記錄型別中的所有記錄

在生產環境中，記錄會繼承工作區的許可權。

在預覽環境中，記錄會繼承記錄型別的許可權。

依預設，記錄型別會繼承工作區的許可權。

不過，您可以執行下列任一作業：

* 停用從記錄型別的工作區繼承的許可權。 這樣會移除記錄的較高許可權，但會保留對工作區、記錄型別和記錄的檢視許可權。
* 手動授予記錄型別的使用者許可權，即使他們無權使用工作區。 這會自動授予他們工作區的「檢視」許可權。 這會授予記錄的使用者許可權。

只有具有工作區管理許可權的使用者才能與其他人共用其記錄型別和記錄。

如需詳細資訊，請參閱[共用記錄型別](/help/quicksilver/planning/access/share-record-types.md)。

</div>
