---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：永久編輯欄的寬度'
description: 您可以拖放欄邊距，以符合所需寬度，以暫時修改為欄寬。 如需詳細資訊，請參閱修改欄寬和順序。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: bb348deb9841320a367695845efe0ca36a9a9d8b
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# 查看：永久編輯欄的寬度

您可以拖放欄邊距，以符合所需寬度，以暫時修改為欄寬。 如需詳細資訊，請參閱 [修改欄寬和順序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

在編輯視圖時，可以使用列中的文本模式永久更改任何視圖的任何列的寬度。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 永久編輯欄的寬度

>[!IMPORTANT]
>
>如果您手動修改欄的寬度，如文章的「暫時修改欄的寬度和順序」一節所述 [修改欄寬和順序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) 永久修改欄寬後，欄寬會根據手動調整大小來保留，並會覆寫根據下列步驟更新的欄寬。 清除快取或從其他瀏覽器登入後，您可以根據下列步驟定義的寬度來檢視欄。

1. 轉到對象清單。
1. 從 **檢視** 下拉式功能表，按一下 **新建視圖**.

1. 按一下 **添加列** 來新增欄。

   或

   按一下任何現有列的列標題。

1. 按一下 **切換到文本模式**.
1. 將滑鼠指標暫留在文字模式區域上，然後按一下 **按一下「 」以編輯文字**.
1. 將下列程式碼新增至欄的文字模式：

   ```
   width=200
   usewidths=true
   ```

   若 **寬度** 行，指定任何數字（以像素為單位），以表示您希望欄在檢視中顯示的寬度。

1. 按一下 **儲存**，然後 **保存視圖**.
