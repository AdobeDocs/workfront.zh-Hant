---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 建立和修改群組的專案範本
description: 當您檢視您在「群組」區域中管理的群組時，您可以檢視和使用與群組及其任何子群組相關聯的專案範本。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 1%

---

# 建立和修改群組的專案範本

當您檢視您在「群組」區域中管理的群組時，您可以檢視和使用與群組及其任何子群組相關聯的專案範本。

如果您的群組之上有任何群組，其管理員也可以為您的群組執行下列動作。 Workfront管理員也是如此（適用於任何群組）。

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
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr>
  <tr> 
   <td role="rowheader">物件許可權</td>
   <td>檢視您要檢視及使用之範本的存取許可權或以上版本</td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 從群組區域檢視、處理和建立群組的範本

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組](assets/groups-icon.png)。

1. 按一下要為其建立或修改範本的群組名稱。
1. 在左側面板中，按一下&#x200B;**範本**&#x200B;列出與群組及其可能擁有的任何子群組相關聯的範本。

   您必須有範本的檢視存取權才能在此清單中檢視它。 如需關於此存取許可權的資訊，請參閱[授予範本存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)。

1. 執行下列任一項作業：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新增範本</td> 
      <td> <p>按一下「<strong>新增範本</strong>」，然後使用可用的選項進行設定。 如需這些選項的相關資訊，請參閱<a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">建立專案範本</a>。</p> <p>範本會自動與群組建立關聯。</p> <p>如需關於如何將群組偏好設定套用至新範本的資訊，請參閱本文中的<a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">如何將偏好設定套用至範本和範本工作</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">編輯一或多個範本</td> 
      <td> <p>請至少選取一個範本，按一下「編輯」圖示<img src="assets/edit-icon.png">，然後使用任何可用選項來設定它。 如需這些選項的相關資訊，請參閱<a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">編輯專案範本</a>。</p> <p>只有當您擁有所有選取範本的「編輯」存取權時，才能使用「編輯」圖示。 如需關於此存取許可權的資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予範本存取許可權</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除一或多個範本</td> 
      <td> <p>請至少選取一個範本，然後按一下「刪除」圖示<img src="assets/delete.png">。</p> <p>此圖示僅在您擁有所有選取範本的「編輯」存取權時可用。 如需關於此存取許可權的資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予範本存取許可權</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">共用一或多個範本</td> 
      <td> <p>請至少選取一個範本，按一下「共用」圖示<img src="assets/share-icon.png">，然後在下拉式功能表中按一下下列其中一個選項：</p> 
       <ul> 
        <li> <p><strong>範本</strong>：在顯示的<strong>範本存取</strong>方塊中，新增名稱以指定您想要存取範本本身的人員。</p> <p>如需詳細資訊，請參閱文章<a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">共用專案範本</a>中的<a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">共用範本</a>一節。</p> </li> 
        <li><strong>專案</strong>：在顯示的<strong>專案存取權</strong>方塊中，新增名稱以指定您希望誰能存取使用範本建立的專案</li> 
       </ul> <p>「共用」圖示僅在您擁有所有所選範本的「共用」存取權時可用。 如需關於此存取許可權的資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">授予範本存取許可權</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">匯出範本清單</td> 
      <td>按一下<strong>匯出</strong> <img src="assets/export.png">，然後選取您要用於匯出清單的檔案格式。</td> 
     </tr> 
    </tbody> 
   </table>

## 偏好設定如何套用至範本和範本任務 {#how-preferences-apply-to-templates-and-template-tasks}

當您建立專案範本時，下清單格中所列的設定會由相關的專案或任務偏好設定自動設定。

>[!NOTE]
>
>群組層級或系統層級專案或任務偏好設定會影響專案範本，這取決於您在建立範本時是否將其與群組相關聯。
>
>如果您確實將其與群組相關聯，則群組層級的偏好設定會生效。 這發生在以下情境中：
>
>* 您可以從群組區域建立範本，如本文所述
>* 使用Kickstart檔案建立範本時，您可以指定群組
>* 使用API建立範本時，您可以指定群組
>
>如果您未將新範本與群組建立關聯，則系統層級的偏好設定會生效。 這種情況會在以下情況下發生。 （如果您稍後將群組指派給範本或範本任務，群組的偏好設定不會影響它。）
>
>* 您可從範本區域建立範本
>* 使用Kickstart檔案建立範本時未指定群組
>* 使用API建立範本時未指定群組
>

* [專案與任務偏好設定所設定的專案範本設定](#project-template-settings-configured-by-project-and-task-preferences)
* [由任務偏好設定設定的範本任務設定](#template-task-settings-configured-by-task-preferences)

### 專案和任務偏好設定所設定的專案範本設定 {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>績效指數方法</p> </td> 
   <td> <p>如果您將新範本與群組建立關聯，則由群組層級專案偏好設定「績效指數方法」設定；如果您未將新範本與群組建立關聯，則由相同的系統層級專案偏好設定設定。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>狀況類型</p> </td> 
   <td> <p>如果您將新範本與群組建立關聯，則由群組層級的專案偏好設定設定「根據進度狀態自動設定專案條件」；如果您未建立關聯，則使用相同的系統層級專案偏好設定。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>排程開始日期</p> </td> 
   <td> <p>如果您將新範本與群組建立關聯，則由群組層級專案偏好設定「排程起始日期」設定；如果您未建立關聯，則由相同的系統層級專案偏好設定設定。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>使用者休假</p> </td> 
   <td> <p>如果您將新範本與群組建立關聯，則由群組層級專案偏好設定「使用者休假」設定；如果您未建立關聯，則由相同的系統層級專案偏好設定設定。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>更新型別</p> </td> 
   <td> <p>如果您將新範本與群組建立關聯，則由群組層級的專案偏好設定設定「專案時間表將自動重新計算」，如果您未建立關聯，則使用相同的系統層級專案偏好設定。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>存取區段設定</p> </td> 
   <td> <p>如果您將新範本與群組建立關聯，則由「存取」區段中的群組層級任務偏好設定設定；如果您未建立關聯，則由相同的系統層級專案偏好設定設定。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需此表格中所列專案偏好設定的相關資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

有關任務和問題偏好設定的資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

>[!NOTE]
>
>* 如果您變更與現有專案範本相關聯的群組，範本的設定會維持不變。
>* 如果您將現有的範本任務移至另一個範本，則無論與新範本相關聯的群組為何，範本任務中的下列設定都會保持不變：>
>   * 期間類型
>   * 收入類型
>   * 成本類型
>
>  但是，新範本上的「將某人指派給任務時」設定會影響範本任務。 如需詳細資訊，請參閱文章[編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)中的[存取](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access)一節。
>
>* 當管理員將專案另存為範本時，範本的所有設定都會繼承自專案，包括群組。
>
>  當管理員使用範本將任務或問題轉換為專案時，範本的所有設定由範本上已儲存的內容決定。
>

### 由任務偏好設定設定的範本任務設定 {#template-task-settings-configured-by-task-preferences}

當您建立範本任務時，其某些設定會透過相關任務偏好設定自動進行設定。 下表列出這些設定。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>期間類型 </p> </td> 
   <td> <p>如果您將範本與群組關聯，則由群組層級任務偏好設定「期間型別」設定；如果您未關聯，則由相同的系統層級任務和問題偏好設定設定。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>收入類型</p> </td> 
   <td> <p>如果您將範本與群組建立關聯，則由群組層級任務偏好設定「收入型別」設定；如果您未建立關聯，則由相同的系統層級任務和問題偏好設定設定。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>成本類型 </p> </td> 
   <td> <p> 如果您將範本與群組關聯，則由群組層級任務偏好設定「成本型別」設定；如果您未關聯，則由相同的系統層級任務和問題偏好設定設定。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需此表格中所列工作偏好設定的相關資訊，請參閱[設定全系統的工作與問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。
