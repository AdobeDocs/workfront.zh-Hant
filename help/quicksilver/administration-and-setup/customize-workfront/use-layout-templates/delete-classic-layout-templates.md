---
title: 刪除傳統版面範本
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 傳統Workfront體驗中的版面配置範本在Workfront介面中不再提供，但仍可能影響Workfront資料。 這可能會導致報表或儀表板上受版面配置範本影響的欄位不一致（例如「共用對象」）。
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c68b63230b07ea8c8475b710e256b5e0f049b1eb
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# 授予配置範本的管理存取權

傳統Workfront體驗中的版面配置範本在Workfront介面中不再提供，但仍可能影響Workfront資料。 這可能會導致報表或儀表板上受版面配置範本影響的欄位不一致（例如「共用對象」）。

您可以刪除傳統版面配置範本，以解決這些不一致問題。 由於無法在Workfront介面中使用，因此使用必須使用Workfront API來刪除這些專案。

## 存取需求

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
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用API呼叫刪除傳統版面配置範本

您可以在瀏覽器的URL列中輸入API呼叫，然後按Enter鍵。 API回應會顯示在瀏覽器中。

>[!NOTE]
>
>無法刪除全域和系統配置範本。

1. 登入Workfront。
1. 使用下列API呼叫，找出您要刪除的版面配置範本：
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. 記下要刪除的版面配置範本識別碼。
1. 使用下列API呼叫找出您的工作階段ID：
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >切勿與任何人共用您的工作階段ID。

1. 將版面配置範本ID和工作階段ID插入以下API呼叫：
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. 將步驟4的API呼叫貼到瀏覽器的URL列中，然後按Enter鍵。

   這將刪除版面配置範本。



