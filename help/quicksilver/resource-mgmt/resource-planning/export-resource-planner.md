---
product-area: resource-management
navigation-topic: resource-planning
title: 從資源規劃工具匯出資訊
description: 您可以從資源規劃工具的任何檢視中，將資訊匯出至儲存在電腦上的Excel (.xlsx)檔案。
author: Lisa
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 4%

---

# 從資源規劃工具匯出資訊

您可以從資源規劃工具的任何檢視中，將資訊匯出至儲存在電腦上的Excel (.xlsx)檔案。

>[!IMPORTANT]
>
>顯示的資訊以及您可以從資源規劃工具匯出的資訊皆有限制。 如需這些限制的詳細資訊，請參閱[資源規劃工具顯示限制](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td><p>新增：任何</p>
       <p>或</p>
       <p>目前：Pro或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：淺色或更高</p>
       <p>或</p>
       <p>目前：檢閱或以上</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>檢視專案、使用者和資源管理的存取權或以上許可權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案的許可權或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從資源規劃工具匯出資訊

{{step1-to-resourcing}}

依預設會顯示&#x200B;**規劃師**。

1. 選取供需規劃員的檢視。 您可以選取下列其中一個選項：

   * 依使用者檢視
   * 依專案檢視
   * 依角色檢視

1. 按一下&#x200B;**匯出**。

   「匯出選項」對話方塊隨即顯示。

   ![匯出選項](assets/rp-export-options-box-350x421.png)

1. 指定下列資訊：\
   **開始日期**：您匯出的開始日期。 匯出的檔案包含從一週的第一天開始的配置和可用性資訊，其中包含您在此指定的日期。\
   **週期數**：您要包含在檔案中的週期數。 預設值為4個期間。\
   **型別**：您要在匯出檔案中顯示資訊的時間週期型別（周、月或季）。\
   以下是您可以匯出的最長時段：

   * 52 週
   * 36 個月
   * 12季

   **選取以匯出**：視您選取的檢視而定，您可以選取匯出畫面中列出的所有物件或特定物件的使用狀態和預算資訊。
您可以選取匯出下列資訊：

   * 在「專案檢視」中，選取以匯出：

      * 專案
      * 專案和角色
      * 全部（這是預設選項）

   * 在「使用者檢視」中，選取以匯出：

      * 使用者
      * 使用者和專案
      * 全部（這是預設選項）

   * 在「角色檢視」中，選取以匯出：

      * 角色
      * 角色和專案
      * 全部（這是預設選項）

   **資料格式**：根據您希望Excel檔案的顯示方式，選取下列選項：

   * **原始**：選取此選項可顯示可用性與配置資訊，此資訊已按照Excel檔案中物件所屬的群組取消分組。 （這是預設選項）
   * **已群組**：選取以顯示依其所屬物件分組的使用狀態和配置資訊。 這樣就會在熒幕上顯示匯出的資訊。

   「匯出選項」對話方塊中會顯示匯出檔案中資訊外觀的範例。

1. 按一下&#x200B;**匯出**&#x200B;以從資源規劃工具匯出資訊。\
   只會匯出您儲存的資訊。

1. （視條件而定）如果您在角色或專案檢視中有未儲存的預算時數，請按一下&#x200B;**儲存並繼續。**
Excel (.xlsx)檔案會下載至您的電腦。\
   當檔案準備下載時，無法從資源規劃工具匯出。\
   （視條件而定）如果您匯出大量資料，您會收到一封電子郵件，其中包含您可下載檔案的連結。\
   ![RP_eamil_with_exported_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. （視條件而定）當您收到含有匯出檔案的電子郵件時，請按一下[下載] **&#x200B;**&#x200B;下載檔案。\
   這會帶您返回Workfront以下載檔案。\
   您必須登入Workfront才能完成下載。\
   如果您在傳送檔案時未下載檔案，下載連結會在您啟動匯出後的7天內保持作用中。
