---
title: 授予財務資料的存取權
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: 身為Adobe Workfront管理員，您可以透過使用者存取層級，定義使用者對Workfront中財務資料的存取權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# 授予財務資料的存取權

{{highlighted-preview}}

身為Adobe Workfront管理員，您可以透過使用者的存取層級定義使用者對下列專案的存取權，如[存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述：

* Workfront中專案的財務資訊
* 資源規劃工具中的資源預算資訊

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
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 授予財務資料存取權的考量事項

授與使用者存取Workfront中財務資料之許可權時，請考量下列事項：

* 存取層級不允許存取財務資料的使用者無法為專案建立風險。 如需詳細資訊，請參閱[建立與編輯專案風險](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)。
* 您也可以使用存取層次來決定使用者可採用哪些「資源管理」活動來編列預算或檢視資源配置。 如需詳細資訊，請參閱[授與資源管理的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)。

## 使用自訂存取層級設定財務資料的使用者存取權

1. 開始建立或編輯存取層級，如[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 按一下財務資料右側&#x200B;**檢視**&#x200B;或&#x200B;**編輯**&#x200B;按鈕上的齒輪圖示![](assets/gear-icon-settings.png)，然後在&#x200B;**微調您的設定**&#x200B;下選取您要授與的功能。

   ![](assets/financial-data-fine-tune-nwe.png)

1. （選擇性）在&#x200B;**允許**&#x200B;的管理存取區域中，選取下列選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">匯率</td> 
      <td> <p>在Workfront中新增貨幣。</p> <p>如果沒有此存取權，使用者只能將現有貨幣新增到他們建立的專案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td> <p>檢視Workfront中物件的所有費用。</p> <p>這不允許使用者建立新的費用型別。</p> <p>若無此存取權，使用者只能檢視下列專案：</p> 
       <ul> 
        <li>專案、任務或問題管理的費用</li> 
        <li>他們自己的費用</li> 
        <li>其下屬的費用</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，例如[授予工作存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)。
1. 完成時，按一下&#x200B;**儲存**。

   建立存取層級後，您可以將其指派給使用者。 如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 存取共用的財務資訊

您可以授予其他使用者專案、任務或問題的財務資訊許可權，讓他們共用專案、任務或問題的財務資訊，如[共用物件的財務許可權](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md)中所述。

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

當您與另一個使用者共用任何物件時，收件者對該物件的權利取決於兩個專案的組合：

* 您授予收件者的物件許可權
* 收件者物件型別的存取層級設定

## 依授權型別存取財務資訊

如需有關每個存取層級中的使用者可以對財務資訊執行哪些操作的資訊，請參閱文章[每個物件型別可用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)中的[財務資料](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia)小節。

## 透過設定存取財務資訊

下列資訊可協助您瞭解如何使用存取層級設定來控制使用者對財務資料的存取。

### 無存取權

無權存取財務資料的使用者無權存取下列專案：

* 專案與任務物件下的財務區段
* 業務案例
* 記帳費率和記帳記錄
* <span class="preview">評等卡</span>
* 使用者偏好設定中的每小時成本和每小時帳單

  您可以使用上述步驟4中「檢視」按鈕上的齒輪圖示![](assets/gear-icon-settings.png)來設定此專案。

* 工作角色的每小時成本和每小時帳單

  您可以使用上述步驟4中「檢視」按鈕上的齒輪圖示![](assets/gear-icon-settings.png)來設定此專案。

### 檢視存取權

對財務資料具有「檢視」存取許可權的使用者可以檢視（而非編輯）以下內容：

* 專案與任務物件下的財務區段
* 業務案例
* 記帳費率和記帳記錄
* 使用者偏好設定中的每小時成本和每小時帳單

  您可以使用上述步驟4中「檢視」按鈕上的齒輪圖示![](assets/gear-icon-settings.png)來設定此專案。

* 工作角色的每小時成本和每小時帳單

  您可以使用上述步驟4中「檢視」按鈕上的齒輪圖示![](assets/gear-icon-settings.png)來設定此專案。

### 編輯存取權

具有財務資料編輯存取許可權的使用者可以檢視及編輯下列專案：

* 專案與任務物件下的財務區段
* 業務案例
* 記帳費率和記帳記錄
* <span class="preview">評等卡</span>
* 使用者偏好設定中的每小時成本和每小時帳單

  您可以使用上述步驟4中「編輯」按鈕上的齒輪圖示![](assets/gear-icon-settings.png)來設定此專案。

* 工作角色的每小時成本和每小時帳單

  您可以使用上述步驟4中「編輯」按鈕上的齒輪圖示![](assets/gear-icon-settings.png)來設定此專案。
