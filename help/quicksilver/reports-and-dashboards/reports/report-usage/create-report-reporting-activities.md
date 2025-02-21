---
product-area: reporting
keywords: 變更，擁有者，已共用，報表，共用，執行，使用者，存取權，已進入，上次，已檢視，日期，報告，活動
navigation-topic: report-usage
title: 建立報告活動的報告
description: 建立報表相關報表時，您可以識別特定的報表資訊，這些資訊可包括：報表是否已指派給已停用的使用者、報表是否設定為透過已停用使用者的存取許可權執行、使用者是否存取您計畫刪除的報表等。
author: Nolan
feature: Reports and Dashboards
exl-id: 3861ac81-d2e4-4dec-b9cd-96eee0b66a38
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# 建立報告活動的報告

建立報表相關報表時，您可以識別特定的報表資訊，這些資訊可包括：報表是否已指派給已停用的使用者、報表是否設定為透過已停用使用者的存取許可權執行、使用者是否存取您計畫刪除的報表等。

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
   <td> <p>規劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 建立現有報表的相關報表 {#create-the-report-about-existing-reports}

1. 按一下Adobe Workfront右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)。
1. 按一下&#x200B;**報表**，然後按一下&#x200B;**新報表**。
1. 在&#x200B;**新報告**&#x200B;下拉式清單中，選取&#x200B;**報告**&#x200B;以建立現有報告的報告。

1. 在&#x200B;**欄（檢視）**&#x200B;索引標籤中，新增您想要在報表中的欄。\
   下列部分欄位可能會很實用：

   | 欄位 | 說明 |
   |---|---|
   | **以使用者身分執行：名稱** | 這是在&#x200B;**執行此報告時指定的使用者，報告的存取許可權為：**&#x200B;欄位。 如果停用此使用者，則不會為該報告共用對象顯示報告。 |
   | **與**&#x200B;共用 | 這些是與報表共用的所有實體。 |
   | **輸入者** | 這是報表的擁有者。 |
   | **上次檢視日期** | 這是使用者上次檢視報表的日期和時間。 |

   {style="table-layout:auto"}

1. （選用）若要將報表清單限製為特定已停用使用者：

   1. 選取&#x200B;**篩選器**&#x200B;標籤，然後按一下&#x200B;**新增篩選器規則**。

   1. 新增篩選器&#x200B;**以使用者ID** > **Equal**&#x200B;執行。

   1. 輸入您要新增至篩選的已停用使用者名稱，然後在其顯示在清單中時按一下名稱。
   1. 重複步驟C，直到選取要納入報表的所有已停用使用者為止。

1. （可選）若要將報表清單限製為排程報表：

   1. 選取&#x200B;**篩選器**&#x200B;標籤，然後按一下&#x200B;**新增篩選器規則**。

   1. 新增篩選器&#x200B;**排程報告識別碼** > **不是空白的**。

1. 按一下&#x200B;**儲存+關閉**，然後輸入報告的名稱，再按一下&#x200B;**儲存報告**。

   您的報告資訊隨即顯示。

1. （選用）將此報表匯出至Excel並儲存在電腦上。\
   如需匯出報告的資訊，請參閱[匯出資料](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

## 更新報表的相關資訊

建立報表後，您可以視需要更新報表。

1. 前往您要更新的報告。
1. 請根據您要採取的動作，執行下列任一項動作：

   * 將&#x200B;**以：**&#x200B;的存取許可權執行此報告給作用中的使用者：如需詳細資訊，請參閱[以其他使用者的存取許可權執行並傳遞報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md)。

   * 建立報告副本：如需詳細資訊，請參閱[建立報告副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。
   * 刪除報告：如需詳細資訊，請參閱文章[建立報告復本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)的[建立報告復本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md#update2)區段。

   * 共用報告：如需詳細資訊，請參閱[在Adobe Workfront中共用報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)。

1. （視條件而定）如果您複製原始報告，請使用您在[中建立的報告資訊建立現有報告的相關報告](#create-the-report-about-existing-reports)，以與原始報告相同的實體共用新副本。
