---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 使用其他使用者的存取權限執行並傳送報表
description: 依預設，使用者只能在報表中看到他們擁有檢視權限的物件。
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: 269340bc6a0c237edf44f5aa325d4ff95b647df8
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# 使用其他使用者的存取權限執行並傳送報表

依預設，使用者只能在報表中看到他們擁有檢視權限的物件。

您可以讓所有使用者在報表中看到與其他使用者相同的結果，無論其存取層級或權限層級是否位於報表內的物件。

如果您執行的報表具有其他擁有較高存取權(例如Adobe Workfront管理員的存取權)的使用者存取權，則所有擁有檢視報表權限的使用者，都可以以報告建立工具中指定之使用者的身分，查看報表中的資訊。 您可以為使用者在Workfront介面中找到的兩種報表，或以電子郵件附件的形式傳送給使用者的報表，設定此選項。

>[!TIP]
>
>您應將 **以下列權限運行此報告：** 欄位，且僅限使用者的存取權限來顯示報表時，才會顯示此欄位。 例如，工作許可證用戶可能沒有查看計畫許可證用戶或系統管理員建立的報表中的所有項目的權限，除非該報表顯示具有計畫員或系統管理員的訪問權限。\
如果報表已與具有與 **以下列權限運行此報告：** 欄位，您可將此欄位留空。

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
   <td> <p>檢視報表的權限（以檢視傳送的報表）</p> <p>管理報表的權限（執行報表）</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 顯示具有其他使用者存取權限的報表

填入 **以下列權限運行此報表：** 欄位可確保報表包含相同的資料，而無論哪個使用者正在存取報表。 報表的顯示方式與指定使用者的相同。

存取報表的使用者必須至少擁有報表的「檢視」權限，才能看到它。 若使用者列於 **以下列權限運行此報表：** 欄位已停用，則共用報表的任何其他使用者將不再顯示報表。

若要執行具有其他使用者存取權限的報表：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **報表**.

1. 選取要以其他使用者的存取權限顯示的報表。
1. 按一下 **報表動作**，然後按一下 **編輯**.

1. 按一下 **報表設定**.

1. 在 **以下列權限運行此報告：** 欄位中，開始輸入您希望報表顯示為的使用者名稱，然後在清單中看到報表時選取該名稱。\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   具有較低存取層級且允許建立報表的使用者，無法為 **以下列權限運行此報表：** 欄位。

1. 按一下 **完成**.
1. 按一下 **儲存+關閉**.\
   現在，所有與共用報表的使用者都會看到報表，就像報表是由 **以下列權限運行此報告：** 欄位。

>[!IMPORTANT]
輸入 **以下列權限運行此報告：** 欄位會影響報表中顯示的資訊，如果報表包含的篩選器會對登入使用者使用萬用字元反向連結。 報表會根據 **以下列權限運行此報告：** 欄位，而非萬用字元篩選器中定義的欄位。
如需使用者欄位萬用字元的詳細資訊，請參閱 [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## 傳送具有其他使用者存取權限的報表

您可以設定要以電子郵件附件形式傳送的報表。 您可以設定這些傳送的報表，以便對具有較高存取層級的使用者顯示，讓所有使用者都能在傳送的報表中看到相同的資訊。 將查看電子郵件中傳送之報表的使用者，必須新增至報表傳送內的收件者清單。 如需設定要傳送之報表的詳細資訊，請參閱文章 [報表傳送概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

若要傳送具有其他使用者存取權限的報表：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **報表**.

1. 選取要以其他使用者的存取權限傳送的報表。
1. 按一下報表的名稱以選取它。
1. 按一下 **報表動作**.
1. 按一下 **傳送報表**.

1. 在 **以下列項目的存取權限傳送此報表：** 欄位中，開始輸入您希望報表在電子郵件中傳送時顯示的使用者名稱，然後在您在清單中看到報表時選取。 預設值為建立報表的使用者名稱。\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   具有較低存取層級且允許建立報表的使用者無法為 **以下列方式提供此報表的存取權限：** 欄位。

1. 選取 **格式** 您希望報表顯示在電子郵件中：

   * HTML
   * PDF
   * MS Excel
   * MS Excel(.xlsx)
   * TSV

1. 按一下 **立即發送** 立即發送。\
   或\
   按一下 **進行重複傳送** 排程報表的循環傳送。\
   如需報表傳送的詳細資訊，請參閱文章 [報表傳送概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).