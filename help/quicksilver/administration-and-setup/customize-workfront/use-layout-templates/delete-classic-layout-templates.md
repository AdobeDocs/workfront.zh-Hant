---
title: 刪除傳統版面範本
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 傳統 Workfront 體驗中的版面範本在 Workfront 介面中不再可用，但仍可能影響 Workfront 資料。 這可能會導致報告或儀表板上受版面範本 (例如共用對象) 影響的欄位出現不一致。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 52%

---

# 刪除傳統版面範本

傳統 Workfront 體驗中的版面範本在 Workfront 介面中不再可用，但仍可能影響 Workfront 資料。 這可能會導致報告或儀表板上受版面範本 (例如共用對象) 影響的欄位出現不一致。

您可以刪除傳統版面配置範本，以解決這些不一致問題。 由於無法在Workfront介面中使用，因此使用必須使用Workfront API來刪除這些專案。

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
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td><p>新增：標準</p>
  <p> 目前：計畫</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。
若要為群組執行這些動作，您必須是該群組的管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用API呼叫刪除傳統版面配置範本

您可以在瀏覽器的URL列中輸入API呼叫，然後按Enter鍵。 API回應會顯示在瀏覽器中。

>[!NOTE]
>
>全域和系統版面範本無法刪除。

1. 登入Workfront。
1. 使用以下 API 呼叫找出要刪除的版面範本：
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. 記下要刪除之版面範本的 ID。
1. 使用以下 API 呼叫找出您的工作階段 ID：
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >切勿與任何人共用您的工作階段 ID。

1. 將版面範本 ID 和工作階段 ID 插入以下 API 呼叫中：
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. 將步驟 4 中的 API 呼叫貼入瀏覽器的 URL 列，然後按 Enter 鍵。

   這將刪除版面範本。
