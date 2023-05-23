---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：顯示影像，而不是列中的字串'
description: 可以使用文本模式將視圖中對象的名稱替換為影像。 您還可以向影像添加一個連結，以開啟它所替換的對象。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# 視圖：在列中顯示影像而不是字串

可以使用文本模式將視圖中對象的名稱替換為影像。 您還可以向影像添加一個連結，以開啟它所替換的對象。

>[!NOTE]
>
>影像以實際解析度顯示，因此請嘗試使用小影像。

![](assets/replace-project-name-with-image-and-link-350x125.png)

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>請求修改視圖 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改視圖</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 示例：將項目視圖中的項目名稱替換為影像：

1. 將映像上載到Adobe Workfront外部的網站或伺服器。 您必須能夠使用Web瀏覽器訪問映像。

   >[!TIP]
   >
   >* 每種瀏覽器類型都不同，但都能顯示URL。
   >* 避免使用上傳到Workfront的影像。 由於儲存在Workfront的影像不可公開，並且具有在一段時間後過期的訪問密鑰，因此這些影像會隨著時間的推移停止在視圖中顯示。
   >* 保存在電腦上的影像沒有固有的URL。 查找提供映像托管和托管映像的站點。 您的組織可能已經擁有此類站點。


1. 使用Web瀏覽器，轉到您保存的影像。
1. 通過執行以下操作獲取影像的URL:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. 按一下右鍵並選擇 **複製映像位置**&#x200B;或 **獲取連結**，具體取決於您的瀏覽器。 您現在擁有該特定影像的URL，並可以從剪貼簿貼上它。
   1. 確保具有該連結的所有人都有權通過訪問該連結來查看該映像，並且他們不需要登錄即可訪問該映像。

1. 轉到項目，按一下 **更多** 菜單 ![](assets/more-icon-45x33.png) 在項目名稱旁，按一下 **編輯**。

1. 在 **URL** 的子菜單。
1. 導航到清單或報表中的項目視圖並自定義視圖。
1. 按一下列的標題 **項目名稱**，然後按一下 **切換到文本模式**。

1. 將以下代碼添加到現有代碼的列中：

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   您選擇的影像將替換項目視圖中的「項目名稱」，並且該影像是指向項目的連結。

1. 按一下 **保存視圖**。
