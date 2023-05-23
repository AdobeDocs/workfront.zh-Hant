---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：永久編輯列的寬度'
description: 可以通過拖放列邊距來臨時修改列寬，以匹配所需寬度。 有關詳細資訊，請參閱修改列寬和順序。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# 視圖：永久編輯列的寬度

可以通過拖放列邊距來臨時修改列寬，以匹配所需寬度。 有關詳細資訊，請參見 [修改列寬和順序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)。

在編輯視圖時，可以使用列中的文本模式永久更改任何視圖的任意列的寬度。

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

## 永久編輯列的寬度

>[!IMPORTANT]
>
>如果手動修改列的寬度，如文章「臨時修改列的寬度和順序」一節所述 [修改列寬和順序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) 永久修改列寬後，將根據手動調整大小保留列寬，並覆蓋根據以下步驟更新的列寬。 清除快取或從其他瀏覽器登錄後，可以根據以下步驟中定義的寬度查看列。

1. 轉到對象清單。
1. 從 **視圖** 下拉菜單，按一下 **新建視圖**。

1. 按一下 **添加列** 的子菜單。

   或

   按一下任何現有列的列標題。

1. 按一下 **切換到文本模式**。
1. 懸停在文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 將以下代碼添加到列的文本模式：

   ```
   width=200
   usewidths=true
   ```

   對於 **寬度** 行，指定表示希望列在視圖中顯示的寬度的任意數字（以像素為單位）。

1. 按一下 **保存**，則 **保存視圖**。
