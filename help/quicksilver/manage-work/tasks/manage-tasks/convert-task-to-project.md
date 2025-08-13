---
product-area: projects
navigation-topic: manage-tasks
title: 將任務轉換為專案
description: 當專案中的任務需要比您原本計畫更大的工作量完成時，您可以將其轉換為專案。
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: 55c714436fe59c84251c7f4e2a46614feae92cd6
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 2%

---

# 將任務轉換為專案

當專案中的任務需要比您原本計畫更大的工作量完成時，您可以將其轉換為專案。

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
   <td> <p>編輯任務與專案的存取權</p> <p>使用範本轉換為專案時，檢視或更高的範本存取許可權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務的許可權</p> <p>如果使用範本轉換為專案，檢視範本的許可權</p> <p>建立專案後，您即擁有專案的管理許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 將任務轉換為專案的考量事項

* 您可以將任務轉換為空白專案或使用範本轉換為專案。
* 已刪除原始任務。
* 所有子任務、問題和附註都會彙總至新專案。
* 檔案、檔案版本和校樣會移至新專案。
* 將任務轉換為專案時有5分鐘的處理限制。 如果任務附加了大量檔案且無法轉換，您可能需要移除部分檔案，然後再試一次。
* 所有子任務和問題的狀態和完成百分比會保留。
* 任務受指派人和將任務轉換為專案的使用者成為專案上的共用使用者。
* 專案開始日期設定為任務的開始日期。
* 下表列出專案資訊，以及專案資訊是從範本還是從作業轉移：

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>說明</td> 
    <td> <p>任務的「描述」轉移到新專案。 </p> <p> 如果作業沒有描述，則範本中的「描述」會轉移到專案。 </p> <p>如果任務和範本的「說明」欄位都為空，則專案上的欄位為空。 </p> </td> 
    </tr> 
    <tr> 
    <td>狀態</td> 
    <td> 為範本上的群組選取的預設狀態。 如果範本未與群組相關聯，則專案狀態會設為Workfront管理員在設定的專案偏好設定區域中設定的預設狀態。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">設定全系統的專案偏好設定</a>

  在更新專案狀態時存在下列情況：
  <ul>
    <li> 如果任務狀態為「新增」，則專案狀態會設為「計畫」。</li>
    <li> 如果任務狀態為「進行中」，則專案狀態會設為「目前」。</li>
    <li> 如果任務狀態為「完成」，則專案狀態會設為「完成」。</li></ul>

  </td> 
    </tr> 
    <tr> 
    <td>優先順序</td> 
    <td>從作業移轉至專案，或者從範本移轉（如果您在轉換中使用範本）。 </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>任務的URL會轉移至新專案。 </p> <p> 如果任務未指定URL，則範本中的URL會傳輸到專案。 </p> <p>如果問題和範本的URL欄位都為空，則專案上的欄位為空白。 </p> </td> 
    </tr> 
    <tr> 
    <td>專案狀態型別</td> 
    <td>從範本傳輸。</td> 
    </tr> 
    <tr> 
    <td>專案狀況</td> 
    <td>符合由Workfront管理員在設定區域中決定的系統層級預設偏好設定。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md">將自訂條件設為專案的預設值</a>
    </td> 
    </tr> 
    <tr> 
    <td>排程開始時間</td> 
    <td>從範本傳輸。</td> 
    </tr> 
    <tr> 
    <td>專案日期</td> 
    <td> 
      <ul> 
      <li> <p><b>計劃開始日期</b>：應根據範本排程的時區，預先選取根據範本排程的工作時間最接近的工作時間。 如果「排程開始日期」欄位設為「完成日期」，則會停用此欄位。 </p> </li> 
      <li> <p><b>計畫完成日期</b>：應根據範本排程的時區，預先選取根據範本排程的工作時間最接近的工作時間。 如果[排程開始日期]欄位設為[開始日期]，則會停用此欄位。 </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td>專案組合</td> 
    <td>從範本傳輸。 否則，此欄位為空白。</td> 
    </tr> 
    <tr> 
    <td>方案</td> 
    <td>從範本傳輸。 否則，此欄位為空白。</td> 
    </tr> 
    <tr> 
    <td>群組</td> 
    <td><p> 存在下列情況：</p>
      <ul><li>如果在轉換期間指定了群組，則該群組會成為專案的群組</li>
      <li>如果您使用範本轉換為專案，且範本上有一個群組，且在轉換過程中您未指定群組，則範本群組會變成新專案的群組</li>
      <li> 如果範本上沒有群組，且您在轉換期間未指定群組，則原始問題專案的群組將變成新專案的群組</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>公司</td>    
    <td>  從範本傳輸。 否則，此欄位為空白。</td>

  </tr> 
    <tr> 
    <td>專案所有者</td> 
    <td>從範本的「範本所有者」欄位轉移。 否則，會設定為執行轉換的登入使用者。 </td> 
    </tr> 
    <tr> 
    <td>專案贊助者</td> 
    <td>從範本上的範本贊助者欄位轉移。 否則，此欄位為空白。</td> 
    </tr> 
    <tr> 
    <td>資源管理員</td> 
    <td>從範本傳輸。 否則，此欄位為空白。</td> 
    </tr> 
    <tr> 
    <td>任務設定</td> 
    <td>從範本轉移。</td> 
    </tr> 
    <tr> 
    <td>問題設定</td> 
    <td>從範本轉移。 </td> 
    </tr> 
    <tr> 
    <td>存取</td> 
    <td> <p>從範本的「存取」區段轉移。 </p> </td> 
    </tr> 
    <tr> 
    <td>核准</td> 
    <td>從範本轉移。 與任務相關的核准會在轉換期間移除。 </td> 
    </tr> 
  </tbody> 
  </table>


## 將任務轉換為專案

1. 移至您要轉換為專案的工作。
1. 按一下&#x200B;**更多**&#x200B;圖示![](assets/more-icon.png)，然後按一下&#x200B;**轉換為專案**。
1. 選擇下列任一選項：

   * **新專案**
   * **從範本中選取**&#x200B;區段中的範本

     ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. 在出現的通知上按一下&#x200B;**繼續**。
1. 在&#x200B;**轉換成專案**&#x200B;方塊中，指定下列專案：

   * **名稱**：為專案命名。 預設名稱是任務的名稱。
   * （選用） **描述**：說明此專案的用途。
   * （選擇性和條件性）如果您已選取從範本建立專案，請更新&#x200B;**轉換為專案**&#x200B;對話方塊中的可用欄位。

     如需有關編輯專案欄位的詳細資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

     >[!TIP]
     >
     >若要更新「轉換為專案」方塊中「財務」區段中的欄位，您必須擁有存取層級中「財務」資料的「編輯」存取權。 如果您在存取層級中擁有財務資料的檢視存取權，則範本中的所有財務資訊都會傳輸至新專案，而在您轉換問題時，無法編輯它。 如需詳細資訊，請參閱[授予財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)和[共用範本](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)。

   * （選用）新增&#x200B;**自訂Forms**&#x200B;至新專案。

     >[!TIP]
     >
     >如果將附加到任務的多物件自訂表單設定為與任務和專案一起使用，則當您進行轉換時，會保留表單中儲存的所有資訊。
     >
     >
     >如果您使用範本進行轉換，並且附加到範本的自訂表單包含附加到任務的自訂表單中也找到的自訂欄位，則任務的欄位值將用於新專案。 但是，如果任務上的自訂欄位為空白，則會使用範本的值。

1. 按一下「**儲存變更**」。
