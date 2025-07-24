---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 管理小時型別
description: 您可以將時數型別與時數專案建立關聯。 小時型別是您用來定義小時專案的標籤。 小時型別可以是一般時間或專案特定時間。
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 1%

---

# 管理時數類型

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

<div class="preview">

本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 在預覽版發佈一週後，生產環境中也將提供相同功能給所有客戶。

如需詳細資訊，請參閱[介面現代化](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)。

</div>

小時型別是您用來定義小時專案的標籤。 您可以將時數型別與時數專案建立關聯。

時數型別有兩種類別：

* **特定專案小時型別**：這是登入專案、任務和問題的時間。 特定專案小時型別可以與[!DNL Adobe Workfront]中的任何時間專案相關聯，您可在此記錄專案、任務和問題的時間。

  在[!DNL Workfront]中記錄時間時，可用的專案特定小時型別取決於在系統、專案和使用者層級設定的組態選項。

  以下專案專屬預設小時型別一律可用：

   * 專案時間
   * 任務時間
   * 問題時間

  [!DNL Workfront]管理員會決定哪些專案特定時數型別可供使用，如[定義時數型別和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)中所述。

  >[!NOTE]
  >
  >如果您在[!DNL Workfront]系統中啟用任何特定專案小時型別，則必須在系統中的每個專案上啟用至少一個特定專案小時型別。 您無法在系統層級啟用特定專案小時型別，且在專案層級沒有可用的特定專案小時型別。

* **一般時數型別**：一般時數無法與專案、任務或問題建立關聯，且會直接記錄到時程表中。

如需有關記錄時數並將其與時數型別關聯的資訊，請參閱[記錄時間](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md)。

## 存取需求

+++ 展開以檢視存取需求。

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
   <td> <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級</td> 
   <td>系統管理員</td>
  </tr> 
 </tbody> 
</table>

*如需此表格中資訊的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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

作為[!DNL Workfront]管理員，您可以在系統和專案層級為貴組織建立時數型別。

在系統層級定義小時型別後，使用者可以定義哪些小時型別可用於特定專案或特定使用者。

如需詳細資訊，請參閱[定義小時型別和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

若要建立小時型別：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**時程表和時數**，然後按一下&#x200B;**時數型別**。

1. 在&#x200B;**小時型別**&#x200B;區段中，按一下&#x200B;**新增小時型別**。
1. 在&#x200B;**新小時型別**&#x200B;對話方塊中，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名稱]</td> 
      <td>輸入在系統中可輕鬆識別的小時型別名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 說明]</td> 
      <td>新增小時型別的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 範圍]</td> 
      <td> <p>在<strong>範圍</strong>下拉式功能表中，選取時數型別是一般或專案特定的時數型別。</p> <p>一般小時型別僅在時程表中可見，並且不能與專案、任務或問題相關聯。</p> <p><b>重要</b></p><p> 如果您有特定於&lbrack;！UICONTROL專案的自訂時數型別，並且您將其變更為[!UICONTROL 一般]，則所有現有的任務、問題和專案時數都會設定為其系統預設型別。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="preview">[!UICONTROL 計入收入]</span></td> 
      <td><p>如果您希望與此時數型別相關的時數條目影響您的收入計算，請選取此選項。</p>
      <p>病假和休假時間不計算為收入。</p>
      <p><b>附註</b></p>
      <p>當一般時數型別計入收入時，與記錄時間之使用者的設定檔相關聯的成本費率會與時數成本相關聯。  
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 建立小時型別]** <span class="preview">或&#x200B;**儲存**。</span>

   時數型別會新增至您的Workfront系統，並依預設啟用。

## 編輯小時型別

作為[!DNL Workfront]管理員，您可以在系統和專案層級編輯組織的小時型別。

>[!NOTE]
>
>* 您無法編輯內建時數型別。
>* 您無法大量編輯時數型別。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**時程表和時數**，然後按一下&#x200B;**時數型別**。

1. 按一下小時型別名稱或選取小時型別，然後按一下清單頂端的&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。
1. 在&#x200B;**編輯時數型別**&#x200B;對話方塊中，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名稱]</td> 
      <td>輸入在系統中可輕鬆識別的小時型別名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 說明]</td> 
      <td>新增小時型別的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 範圍]</td> 
      <td> <p>在<strong>範圍</strong>下拉式功能表中，選取時數型別是一般或專案特定的時數型別。</p> <p>一般小時型別僅在時程表中可見，並且不能與專案、任務或問題相關聯。</p> <p><b>重要</b></p> <p>如果您有特定於&lbrack;！UICONTROL專案的自訂時數型別，並且您將其變更為[!UICONTROL 一般]，則所有現有的任務、問題和專案時數都會設定為其系統預設型別。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="preview">[!UICONTROL 計入收入]</span></td> 
      <td><p>如果您希望與此時數型別相關的時數條目影響您的收入計算，請選取此選項。</p>
      <p>病假和休假時間不計算為收入。</p>
      <p><b>附註</b></p>
      <p>當一般時數型別計入收入時，與記錄時間之使用者的設定檔相關聯的成本費率會與時數成本相關聯。  
      </td> 
     </tr> 
    </tbody> 
   </table>


1. 按一下&#x200B;**[!UICONTROL 儲存變更]** <span class="preview">或&#x200B;**儲存**。</span>

   您的變更會儲存並編輯時數型別。

## 停用小時型別

如果您不再希望使用者將自己的時數與其建立關聯，您可以停用時數型別。 停用時數型別會從[!DNL Workfront]中顯示時數型別的任何位置隱藏它們。

>[!NOTE]
>
>* 您無法停用內建時數型別。
>* 您可以大量停用時數型別。
>* 停用特定專案時數型別時，該型別的所有記錄時間會自動預設為內建特定專案時數型別。 例如，專案記錄的時間預設為專案時間小時型別；任務記錄的時間預設為任務時間小時型別。
>* 停用一般時數型別時，記錄時間會保留在時程表中，但使用者未來無法再為該時數型別記錄時間。



若要停用小時型別：

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 時程表和時數]**，然後按一下&#x200B;**[!UICONTROL 時數型別]**。

1. 選取要停用的時數型別。 您可以選取多個小時型別。

1. 按一下&#x200B;**更多**，然後按&#x200B;**停用**。

   ![啟用和停用時數型別連結](assets/activate-and-deactivate-hour-type-links.png)

   時數型別已停用，使用者在記錄時數時數時已無法找到該型別。

1. （選擇性）若要重新啟用小時型別，請在&#x200B;**小時型別**&#x200B;清單中選取該型別，然後按一下&#x200B;**更多** > **啟用**。

