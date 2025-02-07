---
title: 使用版面配置範本自訂使用者介面術語
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 身為Adobe Workfront管理員，您可以使用版面配置範本來變更某些物件的標籤，這些標籤會顯示在Workfront中，以符合組織中使用的辭彙。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 2%

---

# 使用版面配置範本自訂使用者介面術語

身為Adobe Workfront管理員，您可以使用版面配置範本來變更某些物件的標籤，這些標籤會顯示在Workfront中，以符合組織中使用的辭彙。

當您儲存變更術語的版面配置範本，然後登出Workfront並再次登入後，您變更的標籤會顯示在Workfront大多數區域中預設標籤的位置：

* 主要功能表
* 從主要功能表存取的所有區域
* 所有標籤
* 所有功能表
* Report Builder和報告元素（檢視、篩選器和群組）
* 儲存按鈕
* 匯出的檔案
* 電子郵件
* 行動應用程式

>[!NOTE]
>
>* Outlook增益集區域未顯示自訂標籤。
>* 當您自訂標籤時，可能會遇到文法和其他問題。 例如，如果您將「問題」變更為「請求」，UI中可能會出現您看到片語「請求」的位置。 如需詳細資訊，請參閱文章[瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的[自訂物件名稱的影響](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names)
>

如需配置範本的詳細資訊，請參閱[建立和管理配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

如需有關群組配置範本的資訊，請參閱[建立和修改群組的配置範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置版面範本後，您必須將其指派給使用者，才能讓其他人看到您所做的變更。 如需將配置範本指派給使用者的詳細資訊，請參閱[將使用者指派給配置範本](../use-layout-templates/assign-users-to-layout-template.md)。

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
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td><p>新增：標準</p>
  <p> 目前：計畫</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>若要在系統層級執行這些步驟，您需要系統管理員存取層級。
若要為群組執行這些動作，您必須是該群組的管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自訂使用者介面術語

1. 開始使用版面配置範本，如[建立和管理版面配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 按一下頁面右上角附近的&#x200B;**設定術語**。
1. 執行下列任一項作業：

   * 若要使用Workfront提供的替代詞語，請按一下標籤旁的向下箭頭![向下箭頭](assets/dropdown-arrow.png)，然後在下拉式清單中按一下您想要的替代標籤。

     >[!NOTE]
     >
     >非英文本地化的Workfront版本支援下拉式清單中提供的替代標籤。

   * 若要針對物件顯示的標籤提供您自己的自訂替代方案，請按一下標籤右側的&#x200B;**設定自訂名稱**，然後輸入自訂字詞的&#x200B;**單數**&#x200B;和&#x200B;**Plural**&#x200B;形式。 如果您改變心意，可以按一下&#x200B;**重設**。

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
        <td><p>如需這些物件的詳細資訊，請參閱<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">瞭解Adobe Workfront中的物件</a>。</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Workfront目標物件</p></td>
        <td>
         <ul>
          <p>目標</p>
          <p>結果</p>
          <p>活動</p>
         </ul></td>
        <td><p>這些物件需要額外的授權。 如需詳細資訊，請參閱<a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront目標總覽</a>。</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront情境規劃工具物件</p></td>
        <td>
         <ul>
          <p>行動方案</p>
          <p>情境</p>
          <p>規劃 </p>
         </ul></td>
        <td><p>這些物件需要額外的授權。 如需詳細資訊，請參閱<a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">開始使用Scenario Planner</a>。</p></td>
       </tr>
      </tbody>
     </table>

1. 完成時，按一下&#x200B;**完成**。

   >[!TIP]
   >
   >在您按一下「完成」（甚至在儲存版面配置範本後）後，您隨時可以返回「設定術語」設定，然後按一下任何自訂術語旁的「重設」(Reset)，以將其恢復為預設狀態。

1. 繼續自訂版面範本。

   或

   如果您已完成自訂，請按一下&#x200B;**儲存**。

1. 若要檢視術語變更：

   1. 登出並重新登入Workfront。
   1. 關閉您已為Workfront環境開啟的所有瀏覽器標籤。

   >[!IMPORTANT]
   >
   >在您變更術語之前，使用版面配置範本的任何人也需要此專案。

如需配置範本的詳細資訊，請參閱[建立和管理配置範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。
