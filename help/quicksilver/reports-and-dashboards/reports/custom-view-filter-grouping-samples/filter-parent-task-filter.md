---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選器：顯示父系任務」
description: 您可以套用以下任務篩選器以顯示工作任務。 工作任務是可以獨立工作的任務，不是其他任務的父級任務。 在一個範例中，篩選器會識別可能是父系本身的子系任務。 在這種情況下，他們無法執行任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# 篩選：顯示父系任務

<!--Audited: 10/2024-->

您可以套用以下任務篩選器以顯示工作任務。 工作任務是可以獨立工作的任務，不是其他任務的父級任務。 在一個範例中，篩選器會識別可能是父系本身的子系任務。 在這種情況下，他們無法執行任務。

>[!TIP]
>
>* 如果您考慮在報表中新增多個篩選器，建議使用Report Builder介面新增所有篩選器，並在新增所有其他篩選器規則後按一下「切換至文字模式」 。 然後，您可以新增父系任務篩選器的程式碼，如上所述。 
>* 我們也建議您為專案名稱新增分組，讓報告更易於閱讀。 如需有關將群組新增至報表的詳細資訊，請參閱文章[ Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。
>

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改篩選器的貢獻者 </p></li>
   <li><p>用於修改報告的標準</p></li> </ul>

<p>目前：</p>
   <ul><li><p>請求修改篩選器 </p></li>
   <li><p>計畫修改報表</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 顯示沒有子系的工作（可能有父系）

您可以將下列篩選器套用至任務報告，以顯示無子系的任務。 他們可以擁有自己的父母，也可以是其他工作的子女。

1. 從右上角的&#x200B;**主功能表** ![](assets/main-menu-icon.png)，或左上角的&#x200B;**主功能表** ![](assets/lines-main-menu.png) （如果可用），按一下&#x200B;**報表**。

1. 按一下&#x200B;**新報告**。
1. 選取&#x200B;**任務報告**。
1. 按一下&#x200B;**篩選器**。
1. 按一下&#x200B;**新增篩選規則**。
1. 在&#x200B;**開始輸入欄位名稱……**&#x200B;行中，開始輸入&#x200B;**子係數目**，然後按一下&#x200B;**工作>>子係數目** （當它顯示在清單中時）。

1. 為您的修飾元選取&#x200B;**等於（區分大小寫）**，然後為子係數目輸入&#x200B;**0**。\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   或

   按一下&#x200B;**切換到文字模式**，然後在文字編輯視窗中複製並貼上下列文字

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. 按一下「**儲存並關閉**」。

   這會為系統中正在執行任務的所有任務提取報告。 其中有些任務可能有父系任務，但它們本身並非父系任務。

## 顯示父系的工作（可能有子系）

您可以將下列篩選器套用至任務報告，以顯示具有父系的任務，亦即它們是子系任務。 但是，這些任務也可能有自己的子項，因為篩選器不排除其子項。 同時為其他任務之父項的子任務不會被視為工作任務。

1. 從右上角的&#x200B;**主功能表** ![](assets/main-menu-icon.png)，或左上角的&#x200B;**主功能表** ![](assets/lines-main-menu.png) （如果可用），按一下&#x200B;**報表**。

1. 按一下&#x200B;**新報告**。
1. 選取&#x200B;**任務報告**。
1. 按一下&#x200B;**篩選器**。
1. 按一下&#x200B;**新增篩選規則**。
1. 在&#x200B;**開始輸入欄位名稱……**&#x200B;行中，開始輸入&#x200B;**父系識別碼**，然後選取&#x200B;**工作>>父系識別碼** （當它顯示在清單中時）。
1. 為您的修飾元選取&#x200B;**不為空白**。

   ![](assets/filter-parent-id-not-blank-350x100.png)

   或

   按一下&#x200B;**切換到文字模式**，然後在文字編輯視窗中複製並貼上下列文字： 

   `parentID_Mod=notblank`

1. 按一下「**儲存並關閉**」。

   這會為系統中具有父系且是這些父系的子系任務的所有任務提取報告。 其中有些工作本身可能是父系工作。

## 顯示沒有子系和父系的工作（獨立工作）

您可以將下列篩選器套用至任務報告，以顯示獨立的工作任務。 這些任務沒有父項，也沒有自己的子項。

1. 從右上角的&#x200B;**主功能表** ![](assets/main-menu-icon.png)，或左上角的&#x200B;**主功能表** ![](assets/lines-main-menu.png) （如果可用），按一下&#x200B;**報表**。

1. 按一下&#x200B;**新報告**。
1. 選取&#x200B;**任務報告**。
1. 按一下&#x200B;**篩選器**。
1. 按一下&#x200B;**新增篩選規則**。
1. 在&#x200B;**開始輸入欄位名稱……**&#x200B;行開始輸入&#x200B;**子係數目**，然後從清單中選取&#x200B;**工作>>子係數目**。
1. 為您的修飾元選取&#x200B;**等於（區分大小寫）**，然後為子係數目輸入&#x200B;**0**。
1. 按一下&#x200B;**新增其他篩選器規則**。
1. 在&#x200B;**開始輸入欄位名稱……**&#x200B;行開始輸入&#x200B;**父系識別碼**，然後從清單中選取&#x200B;**工作>>父系識別碼**。
1. 選取修飾元的&#x200B;**為空白**。

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   或

   按一下&#x200B;**切換至文字模式**，而不是步驟6-10 <!--ensure steps above stay accurate-->，然後在文字編輯視窗中，複製並貼上下列文字：

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. 按一下「**儲存並關閉**」。

   這會為系統中沒有父項或子項的所有任務提取報告。 這些是獨立的工作任務。
