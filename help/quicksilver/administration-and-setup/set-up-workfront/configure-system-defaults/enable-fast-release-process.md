---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 啟用或停用組織的快速發行
description: 您可以選取想要每月或每季接收新的Workfront功能。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 71ef7a50-7a9f-43c4-b67c-8d9fc722569f
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 1%

---

# 啟用或停用組織的快速發行

Adobe Workfront有兩種發佈新功能和更新的模型。 您可以選擇每季接收新功能，還是以更快的發行時間表接收。

這兩種模型提供相同的功能和更新。 唯一的差異在於時間。

範例：

* 公司X已啟用快速發行程式。 他們在8月獲得功能A，在9月獲得功能B，並在10月獲得功能C。
* Y公司已停用快速發行程式。 他們在10月的季度發行中會收到功能A、B和C。

>[!NOTE]
>
>* 在23.3版（2023年7月）之後購買Workfront的客戶預設會啟用快速發行程式，並且可以選擇退出。
>* 在23.3版之前購買Workfront的客戶，其快速發行程式預設為停用，並可選擇加入。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>標準</p> <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是Workfront管理員。 </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 啟用或停用快速發行程式時的注意事項

啟用或停用快速發行程式時，請考量下列事項：

* **啟用**&#x200B;在季度中啟用快速發行程式，讓您的組織能夠存取已發行到快速發行的功能。

  例如，如果功能A在8月發行，而功能B在9月發行，則任何在9月啟用快速發行程式的組織都可以立即存取功能A和B。

* **正在停用**&#x200B;快速發行程式要等到下一次每季發行才會生效。

  例如，如果已啟用快速發行的組織在8月將其停用，則他們仍會在9月收到快速發行功能，因為他們要到10月進行下一個季度發行時才會移至季度發行。

## 啟用或停用組織的快速發行程式

若要啟用或停用快速核發處理，請執行下列步驟：

{{step-1-to-setup}}

1. 展開左側導覽中的&#x200B;**系統**，然後按一下&#x200B;**偏好設定**。
1. 若要啟用快速發行，請核取&#x200B;**允許快速發行程式**&#x200B;核取方塊。

   或

   若要停用快速發行並移至每季發行週期，請取消勾選&#x200B;**允許快速發行程式**&#x200B;核取方塊。

1. 在快顯視窗中確認您的選擇。
1. 按一下「**儲存**」。
