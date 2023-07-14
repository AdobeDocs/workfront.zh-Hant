---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：永久編輯欄寬」
description: 您可以拖放欄的邊界以符合所需的寬度，藉此暫時修改欄的寬度。 如需詳細資訊，請參閱修改欄寬和順序。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 檢視：永久編輯欄寬

您可以拖放欄的邊界以符合所需的寬度，藉此暫時修改欄的寬度。 如需詳細資訊，請參閱 [修改欄寬和順序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

編輯檢視時，您可以使用欄中的文字模式，永久變更任何檢視的任何欄寬。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>請求修改檢視 </p>
   <p>計畫修改報告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 永久編輯欄寬

>[!IMPORTANT]
>
>如果您手動修改欄的寬度，如文章中「暫時修改欄的寬度和順序」一節中所述 [修改欄寬和順序](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) 永久修改欄的寬度後，會根據手動調整大小來保留欄的寬度，而且會覆寫根據以下步驟更新的欄寬度。 清除快取或從其他瀏覽器登入後，您可以根據下列步驟中定義的寬度來檢視欄。
>
>如需在使用「文字模式」介面時自訂欄寬的其他資訊，請參閱 [Adobe Workfront術語表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. 前往物件清單。
1. 從 **檢視** 下拉式功能表，按一下 **新增檢視**.

1. 按一下 **新增欄** 以新增欄。

   或

   按一下任何現有欄的欄標題。

1. 按一下 **切換至文字模式**.
1. 暫留在文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 將下列程式碼新增至欄的文字模式：

   ```
   width=200
   usewidths=true
   ```

   對於 **寬度** 行，指定代表您希望欄在檢視中顯示之寬度的任何數字（以畫素為單位）。

1. 按一下 **儲存**，則 **儲存檢視**.


