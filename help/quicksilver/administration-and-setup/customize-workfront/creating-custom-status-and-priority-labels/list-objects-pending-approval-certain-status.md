---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 使用特定狀態列出具有未決核准流程的物件
description: 如果您嘗試刪除狀態，則錯誤訊息可能會告訴您無法刪除該狀態，因為該狀態正用於系統中物件的未決核准流程。 如果您想要尋找並檢閱這些物件以決定您需要做什麼，您可以執行列出這些物件的報告。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# 使用特定狀態列出具有未決核准流程的物件

如果您嘗試刪除狀態，則錯誤訊息可能會告訴您無法刪除該狀態，因為該狀態在您的系統中至少有一個未決核准流程。 您可以執行報告，列出物件在擱置核准程式中的位置，然後決定您需要為每個物件做什麼。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>
     <p>標準</p>
     <p>規劃</p>
   </td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td><p>編輯報告、儀表板、行事曆的存取權</p><p>編輯對篩選器、檢視、群組的存取權</p></td>
  </tr>
  <tr> 
   <td>物件許可權</td> 
   <td>您可取得所建立報告的「管理」許可權。</td>
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在標準模式中

{{step1-to-reports}}

1. 按一下&#x200B;**新報告**，然後選取&#x200B;**專案報告**、**任務報告**&#x200B;或&#x200B;**問題報告**。
1. 開啟&#x200B;**篩選器**&#x200B;索引標籤。
1. 按一下&#x200B;**新增篩選規則**，然後執行下列動作以設定規則：
   1. 開始輸入`status`，然後在顯示時選取&#x200B;**狀態**。
   1. 在第二個欄位中保留&#x200B;**等於**。
   1. 在第三個欄位中選取狀態名稱。
1. 再按一下&#x200B;**新增篩選器規則**，然後執行下列動作以設定規則
   1. 開始輸入`pending status`，然後在該專案顯示於您正在檢視的物件型別下方時選取該專案（**專案**、**任務**&#x200B;或&#x200B;**問題**）。
   1. 在第二個欄位中保留&#x200B;**等於**。
   1. 在第三個欄位中輸入`in`。
1. 再按一下&#x200B;**新增篩選器規則**，然後執行下列動作以設定規則
   1. 開始輸入核准程式，然後在&#x200B;**核准程式**&#x200B;下顯示&#x200B;**群組識別碼**&#x200B;時選取該識別碼。
   1. 在第二個欄位中選取&#x200B;**為空白**。
1. 按一下&#x200B;**儲存+關閉**&#x200B;以執行報告，並根據您指定的狀態（**專案**、**任務**&#x200B;或&#x200B;**問題**），列出處於擱置狀態的核准程式所指定型別的所有物件。
1. 重複這些步驟，尋找其他兩種物件型別的相同資訊。


## 在文字模式中

{{step1-to-reports}}

1. 按一下&#x200B;**新報告**，然後選取&#x200B;**專案報告**、**任務報告**&#x200B;或&#x200B;**問題報告**。
1. 開啟&#x200B;**篩選器**&#x200B;索引標籤。
1. 選取&#x200B;**切換到文字模式**。
1. 將下列內容複製並貼到編輯視窗中，將XXX取代為3個字母的狀態鍵：

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   您可以檢視狀態清單中的索引鍵，如下列文章所示：
   * [存取系統專案狀態清單](project-statuses.md)
   * [存取系統工作狀態清單](task-statuses.md)
   * [存取系統問題狀態清單](issue-statuses.md)

1. 按一下&#x200B;**儲存+關閉**&#x200B;以執行報告，並根據您指定的狀態（**專案**、**任務**&#x200B;或&#x200B;**問題**），列出處於擱置狀態的核准程式所指定型別的所有物件。
1. 重複這些步驟，尋找其他兩種物件型別的相同資訊。
