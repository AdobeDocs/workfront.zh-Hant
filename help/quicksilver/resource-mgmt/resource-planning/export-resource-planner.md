---
product-area: resource-management
navigation-topic: resource-planning
title: 從資源計畫員導出資訊
description: 您可以將資訊從資源規劃器的任何檢視匯出至儲存在電腦上的Excel(.xlsx)檔案。
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 3%

---

# 從資源計畫員導出資訊

您可以將資訊從資源規劃器的任何檢視匯出至儲存在電腦上的Excel(.xlsx)檔案。

>[!IMPORTANT]
>
>顯示的資訊以及可以從資源計畫器導出的資訊有限。 如需這些限制的詳細資訊，請參閱 [資源計畫器顯示限制](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>審核或更高版本 <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看或更高權限訪問項目、用戶和資源管理</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案的權限或更高版本</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 從資源計畫員導出資訊

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **資源**. 此 **計畫員** 預設顯示。

1. 選擇計畫員視圖。 您可以選取下列其中一個選項：

   * 依使用者檢視
   * 依專案檢視
   * 依角色檢視

1. 按一下 **匯出**.

   「導出選項」對話框隨即顯示。

   ![](assets/rp-export-options-box-350x421.png)

1. 指定下列資訊：\
   **開始日期**:匯出的開始日期。 匯出的檔案包含從一週的第一天開始的分配和可用性資訊，當中包含您在此指定的天。\
   **期間數**:您要納入檔案的時段數。 預設為4個句號。\
   **類型**:要在導出檔案（周、月或季）中顯示資訊的時段類型。\
   以下是您可匯出的最大時段：

   * 52 週
   * 36 個月
   * 12個季度

   **選擇以導出**:您可以根據所選的視圖選擇導出螢幕上列出的所有對象或特定對象的可用性和預算資訊。
您可以選取匯出下列資訊：

   * 在「項目視圖」中，選擇以導出：

      * 專案
      * 專案和角色
      * 所有項目（此為預設選項）
   * 在「用戶視圖」中，選擇以導出：

      * 使用者
      * 使用者和專案
      * 所有項目（此為預設選項）
   * 在「角色視圖」中，選擇以導出：

      * 角色
      * 角色和專案
      * 所有項目（此為預設選項）

   **資料格式**:視您希望Excel檔案的顯示方式而定，選取下列選項：

   * **原始**:選取「 」，在Excel檔案中顯示依其所屬物件取消分組的可用性和配置資訊。 （這是預設選項）
   * **分組**:選擇以顯示按其所屬對象分組的可用性和分配資訊。 這會顯示匯出的資訊，如同它顯示在畫面上一樣。

   「導出選項」對話框中顯示了導出檔案中資訊外觀的示例。

1. 按一下 **匯出** 要從資源計畫器導出資訊，請執行以下操作：\
   僅導出您保存的資訊。

1. （條件性）如果「角色」或「專案」檢視中有未儲存的「預算小時數」，請按一下 **保存並繼續。**
Excel(.xlsx)檔案已下載至您的電腦。
\
   當檔案準備下載時，從資源規劃器導出不可用。\
   （條件性）如果您匯出大量資料，您會收到一封電子郵件，內含您可下載檔案的連結。\
   ![RP_eamil_with_exported_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. （條件性）收到含有匯出檔案的電子郵件時，請按一下 **下載** 下載檔案。\
   這會帶您回到Workfront，以便下載檔案。\
   您必須登入Workfront才能完成下載。\
   如果您在傳送檔案時未下載該檔案，則下載連結在您開始匯出後的7天內會保持作用中狀態。
