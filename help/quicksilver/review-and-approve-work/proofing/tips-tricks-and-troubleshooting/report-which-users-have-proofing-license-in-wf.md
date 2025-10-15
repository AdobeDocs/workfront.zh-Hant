---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 在Adobe Workfront中列出具有校訂授權的使用者
description: 您可以檢視Adobe Workfront中目前有哪些使用者已啟用「使用者可以產生校樣」選項，方法如下。
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 385f4a6663cacfdcf519bf5699fc1840c2cb2adc
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 1%

---

# 在Adobe Workfront中列出具有校訂授權的使用者

您可以檢視Adobe Workfront中目前有哪些使用者已啟用「使用者可以產生校樣」選項，方法如下。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
   <p>標準</p> 
   <p>規劃</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>編輯下列專案的存取權：</p> 
    <ul> 
     <li> <p>建立報告、儀表板和行事曆</p> </li> 
     <li> <p>建立篩選器、檢視和群組</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立使用者報告

您可以建立使用者報告，以檢視哪些使用者可以產生校樣：

1. 導覽至&#x200B;**報表**&#x200B;區域。
1. 按一下&#x200B;**新增報表**&#x200B;下拉式功能表，然後按一下&#x200B;**使用者報表**。

1. 在&#x200B;**篩選器**&#x200B;索引標籤上，按一下&#x200B;**新增篩選器規則**。

1. 在可用的欄位中，展開&#x200B;**使用者**，然後按一下&#x200B;**擁有校訂授權**。

1. 選取&#x200B;**等於** > **True**。

   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. 按一下&#x200B;**儲存+關閉**。

   報表會顯示在Workfront中指派有校訂授權的所有使用者。

## 更新人員檢視

您可以在「人物」檢視中新增欄，以檢視哪些使用者可以產生校樣：

1. 前往&#x200B;**人員**&#x200B;區域。
1. 按一下「**人員**」標籤。
1. 在&#x200B;**檢視**&#x200B;下拉式功能表中，執行下列任一項作業：

   * 若要將此資訊新增至現有的檢視，請選取您要自訂的檢視，然後按一下[自訂檢視]。****
   * 若要將此資訊新增至新檢視，請按一下[新增檢視]。****

1. 按一下「**新增欄**」。
1. 在可用的欄位中，展開&#x200B;**使用者**，然後按一下&#x200B;**擁有校訂授權**。

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存檢視**&#x200B;或&#x200B;**另存為新檢視**。

   檢視會顯示&#x200B;**True**&#x200B;或&#x200B;**False**，視使用者是否擁有指派給他們的校訂授權而定。
