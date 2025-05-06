---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 管理小時型別
description: 您可以將時數型別與時數專案建立關聯。 小時型別是您用來定義小時專案的標籤。
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 1%

---

# 管理時數類型

<!--Audited: 05/2025-->

<!--Audited: 07/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

小時型別是您用來定義小時專案的標籤。 您可以將時數型別與時數專案建立關聯。

時數型別有兩組：

* 特定專案小時型別：這是專案、任務和問題的記錄時間。 特定專案小時型別可以與[!DNL Adobe Workfront]中的任何時間專案相關聯，您可在此記錄專案、任務和問題的時間。

  在[!DNL Workfront]中記錄時間時，可用的專案特定小時型別取決於在系統、專案和使用者層級設定的組態選項。

  以下專案專屬預設小時型別一律可用：

   * 專案時間
   * 任務時間
   * 問題時間

  [!DNL Workfront]管理員會決定哪些專案特定時數型別可供使用，如[定義時數型別和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)中所述。

  >[!NOTE]
  >
  >如果您在[!DNL Workfront]系統中啟用任何特定專案小時型別，則必須在系統中的每個專案上啟用至少一個特定專案小時型別。 您無法在系統層級啟用特定專案小時型別，且在專案層級沒有可用的特定專案小時型別。

* 一般時數型別：一般時數無法與專案、任務或問題建立關聯，而是會直接記錄到時程表中。

如需有關記錄時數並將其與時數型別關聯的資訊，請參閱[記錄時間](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md)。

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
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>系統管理員</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 內建時數型別

Workfront隨附一組內建時數型別。 這些小時型別無法編輯或隱藏。

[!DNL Workfront]隨附的時數型別為：

* **[!UICONTROL 病假時間]**：無法與專案、任務或問題的小時專案關聯的一般小時型別。 病假時數不得計算為收入。
* **[!UICONTROL 休假時間]**：無法與專案、任務或問題的小時專案關聯的一般小時型別。 休假時間不能計為收入。
* **[!UICONTROL 一般管理費用]**：無法與專案、任務或問題的時數專案產生關聯的一般時數型別。 這可在您的專案計畫程式中計為收入。
* **[!UICONTROL 專案時間]**：一般時數型別，只能與專案上的時數專案相關聯。
* **[!UICONTROL 任務時間]**：一般時數型別，只能與任務上的時數專案相關聯。
* **[!UICONTROL 問題時間]**：一般時數型別，只能與問題的時數專案相關聯。

## 建立小時型別

作為[!DNL Workfront]管理員，您可以在系統和專案級別上為您的組織建立新的小時型別。 之後，使用者可以定義哪些時數型別可供特定專案和使用者使用。 如需詳細資訊，請參閱[定義小時型別和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

若要建立新的小時型別：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**時程表和時數**，然後按一下&#x200B;**時數型別**。

1. 在&#x200B;**小時型別**&#x200B;區段中，按一下&#x200B;**+新小時型別**。
1. 在&#x200B;**新小時型別**&#x200B;對話方塊中，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL名稱]</td> 
      <td>輸入在系統中可輕鬆識別的小時型別名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL說明]</td> 
      <td>新增小時型別的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL範圍]</td> 
      <td> <p>在<strong>範圍</strong>下拉式功能表中，選取時數型別是一般或專案特定的時數型別。</p> <p>一般小時型別僅在時程表中可見，並且不能與專案、任務或問題相關聯。</p> <p><b>重要</b>：如果您有特定於[！UICONTROL專案的自訂時數型別，並且您將其變更為[！UICONTROL一般]，則所有現有的任務、問題和專案時數都會設定為其系統預設型別。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL計入收入]</td> 
      <td><p>如果您希望與此時數型別相關的時數條目影響您的收入計算，請選取此選項。</p>
      <p>病假和休假時間不計算為收入。</p>
      <p><b>附註</b></p>
      <p>當一般時數型別計入收入時，與記錄時間之使用者的設定檔相關聯的成本費率會與時數成本相關聯。  
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 建立小時型別].**

## 停用小時型別

如果您不再希望使用者將自己的時數與其建立關聯，您可以停用時數型別。 停用時數型別會從[!DNL Workfront]中顯示時數型別的任何位置隱藏它們。

若要停用小時型別：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 時程表和時數]**，然後按一下&#x200B;**[!UICONTROL 時數型別]**。

1. 選取要停用的時數型別。

1. 按一下&#x200B;**[!UICONTROL 停用]**。

   ![停用按鈕](assets/deactivate-button.png)
