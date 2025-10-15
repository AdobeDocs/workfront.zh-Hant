---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: 共用畫布控制面板
description: 您可以與其他Adobe Workfront使用者共用畫布控制面板，讓使用者可以檢視或編輯。
author: Jenny
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
source-git-commit: 1059950dd3b20e0959c626e580f958bed5076541
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

# 共用畫布控制面板

>[!IMPORTANT]
>
>畫布儀表板功能目前僅適用於參與Beta階段的使用者。 在此階段中，部分功能可能無法完成或如預期般運作。 請依照「畫布控制面板」測試版概觀文章中[提供意見回饋](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)一節的指示，提交有關您體驗的任何意見回饋。<br>
>>如果您對可能的錯誤或技術問題有回饋，請向Workfront支援提交票證。 如需詳細資訊，請參閱[聯絡客戶支援](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>>請注意，以下雲端服務供應商未提供此測試版：
>
>* 自備Amazon Web Services金鑰
>* Azure
>* Google Cloud Platform

您可以與其他Adobe Workfront使用者共用畫布控制面板，讓他們可以檢視或編輯。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<p>任何 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td> 
<p>標準 </p> 
<p>規劃</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td><p>檢視對報告、儀表板和行事曆的存取權</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td><p>檢視儀表板的許可權以共用儀表板</p>
   <p>管理儀表板的許可權以指派儀表板許可權</p>
  </td> 
  </tr>
</tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 關於共用控制面板的考量事項

* 控制面板可以與使用者、團隊、群組、工作角色或公司資源共用。

* 依預設，控制面板的建立者擁有控制面板的管理許可權。

* 系統管理員和具有「管理」許可權的使用者可以授與儀表板的檢視或管理存取權。

* 擁有控制面板檢視許可權的使用者可以授予控制面板的檢視存取權。

* 共用控制面板時，與其共用的資源會繼承控制面板上所顯示報告的許可權。

* 當控制面板透過版面配置範本分配時，控制面板（及其報表）的自動檢視許可權會授予指派給版面配置範本的所有資源。


## 共用畫布控制面板


{{step1-to-dashboards}}

1. 在左側面板中，按一下&#x200B;**畫布控制面板**。

1. 在「**畫布控制面板**」頁面上，選取您要共用的控制面板。

1. 在頁面的右上角，按一下&#x200B;**共用**&#x200B;按鈕。 **儀表板共用**&#x200B;對話方塊就會顯示。

1. 在&#x200B;**授與**&#x200B;存取權的欄位中，開始輸入您要共用畫布控制面板的特定使用者、團隊、角色、群組或公司的名稱，然後在其出現在下拉式清單中時選取它。

1. （選擇性）若要編輯資源對儀表板的存取權，請按一下其名稱旁的&#x200B;**檢視**，然後在出現的下拉式清單中選取&#x200B;**管理**。

   >[!NOTE]
   >
   > 當使用者沒有透過其存取層級指派的儀表板編輯許可權時，無法將管理許可權指派給儀表板。

1. 針對您想要與其共用控制面板的每個資源，重複步驟5至6。

1. 按一下&#x200B;**共用**&#x200B;按鈕。 收件者會收到電子郵件通知，告知他們該儀表板已與他們共用，他們現在可以在&#x200B;**儀表板** > **畫布儀表板** > **共用儀表板**&#x200B;存取該儀表板。

   >[!NOTE]
   >
   > 可能會套用電子郵件通知的個別使用者偏好設定和系統排除。<br>
   > 僅當直接與使用者共用時才會傳送通知。 與群組、角色、公司和團隊共用不會產生電子郵件通知。<br>
   > 從版面配置範本繼承的許可權將不會產生有關儀表板存取權的電子郵件通知。
