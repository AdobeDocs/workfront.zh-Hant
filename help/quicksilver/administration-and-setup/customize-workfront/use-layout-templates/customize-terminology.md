---
title: 使用版面範本自訂使用者介面術語
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 身為Adobe Workfront管理員，您可以使用版面範本來變更整個Workfront中出現之某些物件的標籤，以符合貴組織所使用的辭彙。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 3%

---

# 使用版面範本自訂使用者介面術語

身為Adobe Workfront管理員，您可以使用版面範本來變更整個Workfront中出現之某些物件的標籤，以符合貴組織所使用的辭彙。

在您儲存版面範本，其中變更了術語，然後從Workfront登出再次登入後，您變更的標籤會出現在預設標籤在Workfront大部分區域出現的位置：

* 主要選單
* 從「主菜單」訪問的所有區域
* 所有標籤
* 所有菜單
* Report Builder和報表元素（檢視、篩選和群組）
* 保存按鈕
* 匯出的檔案
* 電子郵件
* 行動應用程式

>[!NOTE]
>
>* Outlook插件區域不顯示自定義標籤。
>* 自訂標籤時，您可能會遇到文法和其他問題。 例如，如果您將「問題」變更為「Request」，UI中可能會有地方顯示片語「An request」。 如需詳細資訊，請參閱 [自定義對象名稱的意義](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) 在文章中 [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>


如需群組版面範本的相關資訊，請參閱 [建立和修改群組的版面範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>要在系統級別執行這些步驟，需要系統管理員訪問級別。
要為組執行這些操作，您必須是該組的經理。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自訂使用者介面術語

1. 開始使用版面範本，如 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 按一下 **設定術語** 靠近頁面的右上角。
1. 執行下列任一操作：

   * 若要使用Workfront提供的替代詞語，請按一下向下箭頭  ![](assets/dropdown-arrow.png) 在標籤旁，按一下下拉式清單中您要的替代標籤。

      >[!NOTE]
      >
      >Workfront本地化為非英文版，支援下拉式清單中提供的替代標籤。

   * 若要針對針對物件顯示的標籤提供您自己的自訂替代方案，請按一下 **設定自訂名稱** 在標籤的右側，然後輸入 **奇異** 和 **複數** 自訂詞語的形式。 您可以按一下 **重設** 如果你改變主意了。

      您可以自訂下列物件名稱：

      <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Workfront物件</p></td>
        <td>
          <p>專案組合</p>
          <p>方案</p>
          <p>專案</p>
          <p>任務</p>
          <p>問題</p>
          <p>目標</p>
          <p>結果</p>
          <p>活動</p>
         </ul></td>
        <td><p>有關這些對象的詳細資訊，請參閱 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解Adobe Workfront中的物件</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Workfront目標物件</p></td>
        <td>
         <ul>
          <p>目標</p>
          <p>結果</p>
          <p>活動</p>
         </ul></td>
        <td><p>這些對象需要附加許可證。 如需詳細資訊，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront目標概覽</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront方案計畫器對象</p></td>
        <td>
         <ul>
          <p>行動方案</p>
          <p>情境</p>
          <p>計劃 </p>
         </ul></td>
        <td><p>這些對象需要附加許可證。 如需詳細資訊，請參閱 <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">開始使用方案規劃器</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. 完成後，按一下 **完成**.

   >[!TIP]
   >
   >按一下「完成」（即使在儲存版面範本後）後，您隨時都可以回到「設定術語」設定，然後按一下任何自訂術語旁的「重設」，將它們傳回預設狀態。

1. 繼續自訂配置範本。

   或

   如果您已完成自訂，請按一下 **儲存**.

1. 若要查看術語變更：

   1. 登出再登入Workfront。
   1. 關閉您為Workfront環境開啟的所有瀏覽器分頁。

   >[!IMPORTANT]
   >
   >在您進行術語更改前，使用版面模板的任何人也必須使用此模板。

如需版面範本的詳細資訊，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
