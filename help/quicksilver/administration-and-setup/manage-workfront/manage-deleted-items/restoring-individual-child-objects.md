---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 還原個別子物件
description: 本文說明如何取得協助，以復原在少於30天前從Adobe Workfront生產或預覽環境刪除的個別子物件。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# 還原個別子物件

本文說明如何取得協助，以復原在少於30天前從Adobe Workfront生產或預覽環境刪除的個別子物件。

Workfront管理員可以還原每個Workfront執行個體中的專案、工作、問題和檔案，如[還原已刪除的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)中所述。 但只有Workfront資料庫團隊可以恢復物件，例如任務、問題、檔案、自訂表單、時數和附註，而不受其父物件的影響。

即時環境中的資料可在「預覽沙箱」中使用長達7天。 這表示您可以使用下列方法，從預覽Sandbox環境匯出獨立資料：

* Kick-Start
* 建立報告並匯出結果

如需有關從Workfront匯出資料的詳細資訊，請參閱[匯出資料](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

匯出的資料可透過下列方式匯入：

* 手動（如果您使用匯出的報告）
* 如果您使用Kick-Start，則可大量使用

  如需使用Kick-Start將資料匯入Workfront的詳細資訊，請參閱[使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。

在週末的維護期間，會重新整理預覽沙箱環境。

如需有關預覽沙箱環境維護期間的詳細資訊，請參閱[Adobe狀態網站](https://status.adobe.com)。

>[!IMPORTANT]
>
>檔案是這些還原方法的例外情況。 您可以從預覽環境中手動下載，然後重新上傳至生產環境。 如果您想要大量下載和上傳檔案，必須向Workfront請求資料還原。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 資料還原所需的資訊

一旦您確定已刪除的物件需要由我們的資料庫團隊還原，請收集您掌握的所有相關資訊。 資料庫管理員需要下列資訊來尋找物件並啟動還原：

* 物件名稱
* 物件型別（任務、問題、專案等）
* 預估刪除日期和時間
* 物件GUID （如果可能）

  找到物件的GUID時，請參閱下列資訊：

   * 可透過參考與物件互動時所觸發的電子郵件通知（指派、評論等）來找到GUID
   * 在URL結尾找到的GUID範例： `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

收集這些資訊後，或需要協助時，請致電我們的客戶支援團隊：844-306-HELP(4357)，或線上提交票證。

## 資料還原程式

1. 我們的客戶支援團隊收到您的資訊後，會將其呈報給我們的客戶支援團隊。
1. 我們的客戶支援團隊將會連絡我們的資料庫團隊。
1. 資料庫團隊有機會檢閱正在還原的資料後，即可提供更準確的ETA估計值。 還原通常需要三天的時間，但視要還原的資料型別和數量而定，可能需要更長的時間。
1. 資料庫團隊會將這些資訊還原到您的預覽沙箱環境，您將在其中檢閱已還原的資料。 我們的客戶支援團隊會在預覽沙箱中找到資料時通知您。
1. 在您滿意沙箱中的還原後，請告知我們的客戶支援團隊，他們將會聯絡我們的資料庫團隊，通知他們可以將資料還原到您的生產環境。
1. 在請求關閉之前，您將有機會檢閱已還原的資料。
