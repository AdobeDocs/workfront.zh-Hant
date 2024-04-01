---
title: 使用版面配置範本自訂新首頁
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 您可以使用版面配置範本來設定使用者在開啟新首頁時看到的內容。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 9de4a3729abe0ea2ee89df0be2974b714e65332a
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 1%

---

# 使用版面配置範本自訂新首頁

您可以使用版面配置範本來設定使用者在開啟新首頁時看到的內容。

您可以設定：

* 預設工作區中顯示哪些Widget，及其在頁面上的版面
* 選取哪個背景
* 特定Widget設定，包括哪些篩選器和群組可用於「我的專案」、「我的任務」和「我的問題」Widget，以及其預設值

>[!IMPORTANT]
>
>本頁所述的管理員配置範本選擇會覆寫個別使用者的自訂選擇。
>
>儲存對版面配置範本的變更後，該版面配置範本的使用者將會變更其新首頁以符合版面配置範本，而其現有的Widget選取專案將會推送至頁面底部。 雖然管理員選取的Widget可由使用者重新定位及調整大小，但無法移除。

如需有關新首頁的資訊，請參閱 [開始使用新首頁](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

如需有關建立版面配置範本的資訊，請參閱 [建立及管理版面範本](../use-layout-templates/create-and-manage-layout-templates.md).

如需有關群組版面配置範本的資訊，請參閱 [建立和修改群組的版面配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

配置版面範本後，您必須將其指派給使用者，才能讓其他人看到您所做的變更。 如需有關指派配置範本給使用者的資訊，請參閱 [將使用者指派至版面配置範本](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。
若要為群組執行這些動作，您必須是該群組的管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用版面配置範本自訂新首頁

1. 開始使用版面範本，如所述 [建立及管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. 按一下向下箭頭 ![](assets/dropdown-arrow.png) 在 **自訂使用者看到的內容**，然後按一下 **首頁工作區**.

1. 在右側顯示的標籤中，按一下 **設計與配置** 選擇並排列Widget與背景，或 **Widget設定** 管理個別Widget的設定，例如可用的篩選器和群組。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">設計與配置</td> 
      <td>
      <p>選取使用者工作區中將會出現的Widget、其位置，然後選擇背景。 請注意，雖然使用者無法移除選取的Widget，但他們可以自由移動及調整大小，以及新增其他Widget。</p>
      <p>此索引標籤的作用基本上是作為小型的新Home工作區；因此，可以根據中所述的步驟來自訂它 <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">新增、編輯或移除新首頁中的Widget</a>. 選取Widget，並依照您想要為使用者顯示的工作區來安排工作區。</p>
      <p>若要變更背景，請遵循底下的步驟 <b>背景自訂</b> 在 <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">開始使用新首頁</a>.</p>
      <p>

>[!NOTE]
>
>只有在配置範本中移動或調整Widget大小時，不會觸發使用者的新首頁更新其配置。 不過，新增或移除Widget將會觸發使用者頁面的更新。

</p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Widget 設定</td> 
      <td>
      <p>變更個別Widget設定。 目前僅支援三個Widget：</p>
      <ul>
        <li>我的專案</li>
        <li>我的任務</li>
        <li>我的問題</li>
      </ul>
      <p>選取您要編輯的Widget後，可用選項將顯示在右側。 這些選項包括 <b>篩選器</b>， <b>欄</b>、和 <b>群組</b>. 您可以：</p>
      <ul>
      <li><p><b>選取並排序使用者可用的篩選器、欄或群組：</b></p>
      <p>勾選清單中所有選項旁的方塊，讓使用者能夠使用。 使用者看不到未核取的選項。 拖放清單中的選項以設定順序。</li></p>
      <p>

>[!IMPORTANT]
>
>使用者必須至少具有對檢視的建立存取權，管理員資料行設定才能正確套用至他們的新首頁。

</p>
      <li><p><b>設定Widget的預設篩選或群組：</b></p>
      <p>將滑鼠停留在選項上，會出現一個按鈕，可讓您將該選項設定為使用者的預設值。 目前預設的右側會有藍色的「預設」徽章。</li></p>
      <li><p><b>將現有的篩選器、欄或群組新增至可用選項清單：</b></p>
      <p>按一下每個清單底部的加號按鈕，將選項新增至該清單。 請注意，只有現有的篩選器、欄位（用於欄）或群組可以這種方式新增。</p></li>
      </ul>
      <p>

>[!NOTE]
>
>如果您使用版面配置範本為特定Widget設定預設篩選或群組，則由於現有使用者偏好設定，該選項可能不會立即生效。 若要立即套用新篩選器或群組，您或使用者可能需要將「/resetUser」附加至其URL結尾以重設其使用者偏好設定。

</p>
  </td> 
  </tr>
  </tbody> 
  </table>

1. 繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下 **儲存** 左下角。
