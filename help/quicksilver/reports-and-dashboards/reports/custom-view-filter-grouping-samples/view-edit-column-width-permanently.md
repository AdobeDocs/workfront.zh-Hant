---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：永久編輯欄寬」
description: 您可以拖放欄的邊界以符合想要的寬度，暫時修改欄的寬度。 如需詳細資訊，請參閱修改欄寬和順序。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 261c1b73d785094de4ee8549c856a091920ba04a
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 檢視：永久編輯欄寬

<!-- Audited: 1/2024 -->

您可以拖放欄的邊界以符合想要的寬度，暫時修改欄的寬度。 如需詳細資訊，請參閱 [修改欄寬和順序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

若要永久變更任何檢視的任何欄寬，編輯檢視時必須在欄中使用文字模式。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：<ul><li>修改檢視的貢獻者</li><li>用於修改報告的標準</li></ul></p><p>或</p>目前：<ul><li>請求修改檢視</li><li>計畫修改報表</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 永久編輯欄寬

>[!IMPORTANT]
>
>如果您依照一節所述手動修改欄寬 [暫時修改欄寬和順序](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) 在文章中 [修改欄寬和順序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) 永久修改欄的寬度之後，會根據手動調整大小來保留欄的寬度。 在此情況下，會覆寫根據下列步驟更新的欄寬。 清除快取或從其他瀏覽器登入後，您可以根據下列步驟中定義的寬度來檢視欄。
>
>如需在使用「文字模式」介面時自訂欄寬的其他資訊，請參閱 [Adobe Workfront術語表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. 移至物件清單。
1. 從 **檢視** 下拉式功能表，按一下 **新檢視**.

1. 按一下 **新增欄** 以新增欄。

   或

   按一下任何現有欄的欄標題。

1. 按一下 **切換到文字模式**.
1. 暫留在文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 將下列程式碼新增至欄的文字模式：

   ```
   width=200
   usewidths=true
   ```

   對於 **寬度** 行，指定代表您希望欄在檢視中顯示之寬度的任何數字（畫素）。

1. 按一下 **儲存**，然後 **儲存檢視**.


