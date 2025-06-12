---
title: 要求檢視或Workspace的許可權
description: 當有人與您無權存取的檢視或工作區共用連結時，您可以要求開啟該連結的許可權。 本文說明當您遇到無法開啟的共用連結時，請求存取檢視或工作區的步驟。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 94dfa36a-801a-4eef-bcf5-4a3fecc5a3d0
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%

---

# 要求檢視或工作區的許可權

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

>[!IMPORTANT]
>
>本文所述的功能僅在您的組織已上線到Adobe Unified Experience時可用。
>
>如需詳細資訊，請參閱[適用於Workfront的Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。


當有人與您共用您無權存取之檢視或工作區的連結時，您可以要求檢視或工作區的許可權。

向檢視要求許可權與向工作區要求許可權類似。

本文介紹當有人與您共用連結而您無法存取共用頁面時，如何要求存取檢視或工作區。

如需授予檢視和工作區許可權的相關資訊，請參閱下列文章：

* [共用檢視](/help/quicksilver/planning/access/share-views.md)
* [共用工作區](/help/quicksilver/planning/access/share-workspaces.md)


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
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p> 
<p><b>重要</b></p>
<p>只有當您的組織加入Adobe統一體驗時，您組織中的使用者才能請求檢視和工作區的許可權。 </p>
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準、光源或貢獻者</p>
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
   <td>  <p>您的許可權要求取得授權後，您就可以取得下列許可權：</p>
   <ul><li><p>檢視或管理檢視</p></li>
   <li><p>檢視、貢獻或管理工作區</p></li></ul>  
   <p>只有對工作區和檢視具有管理許可權的使用者才能公開共用檢視。</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> 
   <p>在「生產」環境中，所有使用者（包括系統管理員）都必須指派給包含Planning區域的版面配置範本。</p>
   <div class="preview">
<p> 在「預覽」環境中，必須為具有「輕度」或「貢獻者」授權的使用者指派一個版面配置範本，該範本包含以下區域的Planning選項：</p>
   <ul><li>主要功能表</li>
   <li>專案、投資組合和方案的左側面板</li>
   </ul>
   <p>如需詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">建立及管理配置範本</a>。</p>
   <p>標準使用者和系統管理員預設會啟用Planning區域。</p></div>
   </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 要求檢視或工作區的許可權

向檢視要求許可權與向工作區要求許可權類似。

當有人與您共用一個連結至工作區或一個您沒有存取權的檢視時：

1. 按一下與您共用的連結，以檢視或工作區。

   顯示&#x200B;**您沒有存取權**&#x200B;頁面，通知您您沒有檢視或工作區的存取權。

   ![要求檢視的存取權](assets/request-access-to-view.png)

1. （視條件而定）如果共用的連結是針對您有存取權的工作區的檢視，請按一下&#x200B;**以現有檢視開啟**。 如果您有存取工作區的許可權，記錄型別頁面會在預設檢視中開啟。

1. （選擇性和條件性）如果您沒有檢視工作區的許可權，請在可用的方塊中新增個人化訊息，然後按一下&#x200B;**要求存取**。

   所有具有檢視或工作區管理許可權的使用者都會收到下列存取請求通知：
   * 應用程式內通知
     ![存取要求的應用程式內通知](assets/in-app-notification-for-access-request.png)
   * 電子郵件通知
     ![存取要求的電子郵件通知](assets/email-notification-for-access-request.png)

1. （視條件而定）當檢視或工作區管理員授予您檢視或工作區的許可權時，您會收到電子郵件通知和應用程式內通知，其中包含已授予許可權的確認。<!--check this - I was not able to test this, but Isk confirmed.-->
