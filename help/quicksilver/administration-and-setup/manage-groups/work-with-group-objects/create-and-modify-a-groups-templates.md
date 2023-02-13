---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 建立和修改群組的專案範本
description: 在「組」區域中查看管理的組時，可以查看和使用與組及其任何子組關聯的項目模板。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 1%

---

# 建立和修改群組的專案範本

在「組」區域中查看管理的組時，可以查看和使用與組及其任何子組關聯的項目模板。

如果群組上有任何群組，其管理員也可以為群組執行這些動作。 Workfront管理員（適用於任何群組）也是如此。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>在要查看和使用的模板上查看訪問權限或更高</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 從「組」區域查看、使用和建立組的模板

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 按一下要為其建立或修改範本的群組名稱。
1. 在左側面板中，按一下 **範本** 列出與組以及組可能擁有的任何子組關聯的模板。

   您必須擁有範本的檢視存取權，才能在此清單中查看。 如需此存取的相關資訊，請參閱 [授予範本的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. 執行下列任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新增範本</td> 
      <td> <p>按一下 <strong>新範本</strong>，然後使用可用選項進行設定。 如需這些選項的相關資訊，請參閱 <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">建立專案範本</a>.</p> <p>範本會自動與群組相關聯。</p> <p>如需如何將群組偏好設定套用至新範本的詳細資訊，請參閱 <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">首選項如何應用於模板和模板任務</a> 這篇文章。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">編輯一或多個範本</td> 
      <td> <p>至少選擇一個模板，按一下「編輯」表徵圖 <img src="assets/edit-icon.png">，然後使用任何可用選項進行設定。 如需這些選項的相關資訊，請參閱 <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">編輯專案範本</a>.</p> <p>只有在您擁有所選所有範本的「編輯」存取權時，「編輯」圖示才可使用。 如需此存取的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予範本的存取權</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除一或多個範本</td> 
      <td> <p>請至少選取一個範本，然後按一下「刪除」圖示 <img src="assets/delete.png">.</p> <p>只有在您擁有所選所有範本的「編輯」存取權時，此圖示才可用。 如需此存取的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予範本的存取權</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">共用一或多個範本</td> 
      <td> <p>請至少選取一個範本，按一下「共用」圖示 <img src="assets/share-icon.png">，然後在下拉式功能表中按一下下列其中一個選項：</p> 
       <ul> 
        <li> <p><strong>範本</strong>:在 <strong>範本存取</strong> 框中，添加名稱以指定要訪問模板本身的人員。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">共用範本</a> 在文章中 <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">共用專案範本</a>.</p> </li> 
        <li><strong>專案</strong>:在 <strong>專案存取</strong> 框中，添加名稱以指定您有權訪問從模板建立的項目</li> 
       </ul> <p>只有在您擁有所選所有範本的「共用」存取權時，「共用」圖示才可使用。 如需此存取的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予範本的存取權</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">匯出範本清單</td> 
      <td>按一下 <strong>匯出</strong> <img src="assets/export.png">，然後選取要匯出清單的檔案格式。</td> 
     </tr> 
    </tbody> 
   </table>

## 首選項如何應用於模板和模板任務 {#how-preferences-apply-to-templates-and-template-tasks}

建立項目模板時，下表中列出的設定將通過關聯項目或任務首選項自動配置。

>[!NOTE]
>
>組級或系統級項目或任務首選項會影響項目模板，具體取決於建立模板時是否將該模板與組關聯。
>
>如果您確實將其與組關聯，則組級首選項將生效。 這種情況發生在以下情況：
>
>* 如本文所述，您可從「群組」區域建立範本
>* 使用Kickstart檔案建立模板時，可以指定組
>* 使用API建立範本時，您可以指定群組
>
>如果未將新模板與組關聯，則系統級首選項將生效。 在下列情況下，會發生此情況。 （如果您稍後將組分配給模板或模板任務，組的首選項不會影響它。）
>
>* 從「模板」區域建立模板
>* 使用Kickstart檔案建立模板時，不指定組
>* 使用API建立範本時，您不會指定群組
>


* [由項目和任務首選項配置的項目模板設定](#project-template-settings-configured-by-project-and-task-preferences)
* [由任務首選項配置的模板任務設定](#template-task-settings-configured-by-task-preferences)

### 由項目和任務首選項配置的項目模板設定 {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>績效指數方法</p> </td> 
   <td> <p>如果將新模板與組關聯，則由組級項目首選項「效能索引方法」配置；如果不關聯，則由相同的系統級項目首選項配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>狀態類型</p> </td> 
   <td> <p>如果將新模板與組關聯，則由組級項目首選項「根據進度狀態自動設定項目的條件」配置；如果不關聯，則由相同的系統級項目首選項配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>排程自</p> </td> 
   <td> <p>如果將新模板與組關聯，則由組級項目首選項「計畫自」配置；如果不關聯，則由相同的系統級項目首選項配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>用戶超時</p> </td> 
   <td> <p>如果將新模板與組關聯，則由組級項目首選項「用戶關閉時間」配置；如果不關聯，則由相同的系統級項目首選項配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>更新類型</p> </td> 
   <td> <p>由組級項目首選項配置：如果將新模板與組關聯，則「將自動重新計算項目時間軸」；如果不關聯，則配置相同的系統級項目首選項。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>存取區段設定</p> </td> 
   <td> <p>如果將新模板與組關聯，則由「訪問」部分中的組級任務首選項配置；如果不關聯，則由相同的系統級項目首選項配置。</p> </td> 
  </tr> 
 </tbody> 
</table>

有關此表中列出的項目首選項的資訊，請參見 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

有關任務和問題首選項的資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* 如果您變更與現有專案範本相關聯的群組，範本的設定會維持不變。
>* 如果將現有模板任務移動到另一個模板，則無論與新模板關聯的組為何，模板任務中的以下設定都保持不變：>
   >   * 期間類型
   >   * 收入類型
   >   * 成本類型
>
>  但是，模板任務受新模板上「當某人被指派給某個任務時」設定的影響。 如需詳細資訊，請參閱 [存取](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) 在文章中 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* 管理員將項目另存為模板時，模板的所有設定都繼承自項目，包括組。
>
>  當管理員使用模板將任務或問題轉換為項目時，模板的所有設定都取決於模板上已保存的內容。

### 由任務首選項配置的模板任務設定 {#template-task-settings-configured-by-task-preferences}

建立模板任務時，其某些設定是通過相關任務首選項自動配置的。 下表列出這些設定。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>期間類型 </p> </td> 
   <td> <p>如果將模板與組關聯，則由組級任務首選項「持續時間類型」配置；如果不關聯，則由相同的系統級任務和問題首選項配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>收入類型</p> </td> 
   <td> <p>如果將模板與組關聯，則由組級任務首選項「收入類型」配置；如果不關聯，則由相同的系統級任務和問題首選項配置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>成本類型 </p> </td> 
   <td> <p> 如果將模板與組關聯，則由組層任務首選項「成本類型」配置；如果未將模板與組關聯，則由相同的系統層任務和問題首選項配置。</p> </td> 
  </tr> 
 </tbody> 
</table>

有關此表中列出的任務首選項的資訊，請參見 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
