---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 建立個人任務
description: 個人任務是指您傳送給使用者、自己或您在「首頁」區域中為自己建立的待辦事項的臨時工作請求。 Workfront會儲存隨選工作請求以及將專案作為個人任務來執行。
author: Becky
feature: Get Started with Workfront
exl-id: b40d6b10-19c7-4e11-a74f-a8af3ebafb65
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# 建立個人任務

<!--Audited: 10/2024-->

個人任務是指您傳送給使用者或自己傳送或新增的臨時工作請求。

Adobe Workfront會儲存臨時工作請求，以及將專案當做個人任務在Wprfront自動為每個使用者建立的使用者個人專案上。

以下是使用者個人專案的特徵：

* Workfront中的所有使用者都有名為「&lt;使用者全名>的任務」的個人專案。 例如，「John Smith的任務」。
* 每個使用者的個人專案不會顯示在搜尋中，且會隱藏。
* 無法刪除個人專案，即使使用者已停用。
* 個人專案的狀態一律為最新。 無法完成或取消個人專案。
* 所有個人任務都儲存在使用者的個人專案中。
* 如有需要，您可以將個人任務移至另一個專案。

您可以透過下列方式建立個人工作：

* 在您的首頁區域中建立待辦事項

  如需詳細資訊，請參閱[從首頁區域建立工作專案和專案](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)。

* 從使用者設定檔頁面建立個人工作請求並傳送給另一個使用者
* 從您的使用者設定檔頁面建立並傳送個人工作請求給您自己

本文說明如何從使用者設定檔頁面為使用者或您自己建立個人工作請求。

無論您如何新增個人任務，都可以在Workfront的相同區域中找到。 如需詳細資訊，請參閱本文中的[尋找個人工作](#locate-personal-tasks)一節。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront套件</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權</strong></td> 
   <td> 
   <p>標準<p>
   <p>規劃</p>
   <p>這是傳送請求給其他使用者所需的授權。 所有使用者都可以為自己建立工作請求。</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>編輯使用者的存取權以為其建立工作請求。 檢視存取權以建立自己的個人工作請求。 </p>
   </td> 
  </tr>

</tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> 
   <p>New: Standard to send requests to other users. All users can create a work request for themselves.</p> 
   <p>Current: Plan to send requests to other users. All users can create a work request for themselves.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>Edit access to Users to create a work request for them. View access to create a personal work request for yourself. </p>
   </td> 
  </tr> 
 
 </tbody> 
</table>-->


## 建立個人工作請求

1. 移至您使用者的設定檔頁面，或移至您有權檢視的其他使用者的設定檔頁面。

   >[!TIP]
   >
   >當某些使用者設定您的存取層級時，您的Workfront管理員可能會阻止您檢視這些使用者。

1. 按一下標題中使用者名稱右側的&#x200B;**更多功能表** ![](assets/more-menu.png)。
1. 按一下&#x200B;**傳送工作要求**。
顯示&#x200B;**傳送工作要求**&#x200B;方塊。

   ![](assets/personal-task-box.png)
1. 更新下列資訊：

   * **工作名稱**：這是臨時工作要求或個人工作的名稱。
   * **描述**：新增任務的描述。
   * **指派給**：預設會顯示您選取的使用者名稱。 您可以新增更多使用者或團隊。
   * **到期日**：這是您想要完成此工作的日期。 依預設，這是今天的日期。 您無法選取過去的日期
   * **時間**：這是您想要完成此工作的時間。 依預設，這是目前的時間。

1. 按一下&#x200B;**傳送要求**&#x200B;以儲存工作要求。

   工作請求會儲存為Workfront中的個人任務，並會新增到使用者首頁區域的待辦事項Widget中。 如果您將工作請求傳送給自己，它會顯示在您首頁的待辦事項Widget中。


## 尋找個人工作

您可以在下列區域找到個人工作：

* 傳送個人請求之使用者的「首頁」區域中的待辦事項Widget。

  如需詳細資訊，請參閱[從首頁區域建立工作專案和專案](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)。

* 個人工作報告或清單。 您可以建立並套用個人任務篩選器至任務報告或清單，以僅顯示個人任務並排除專案任務。

  如需詳細資訊，請參閱[篩選：個人工作](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md)。
