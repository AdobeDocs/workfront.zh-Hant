---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 列出在Adobe Workfront中具有校對授權的使用者
description: 您可以檢視哪些Adobe Workfront使用者目前已透過下列其中一種方式啟用「使用者可產生校樣」選項。
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# 列出在Adobe Workfront中具有校對授權的使用者

您可以檢視哪些Adobe Workfront使用者目前已透過下列其中一種方式啟用「使用者可產生校樣」選項。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>舊計畫：Select或Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>編輯對以下項目的訪問：</p> 
    <ul> 
     <li> <p>建立報表、控制面板和日曆</p> </li> 
     <li> <p>建立篩選、檢視和群組</p> </li> 
    </ul> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 建立使用者報表

您可以建立使用者報表來檢視哪些使用者可以產生校樣：

1. 導覽至 **報表** 的上界。
1. 按一下 **新增報表** 下拉式功能表，然後按一下 **使用者報表**.

1. 在 **篩選器** 按一下 **新增篩選規則**.

1. 在可用欄位中，展開 **使用者**，然後按一下 **有證明許可證**.

1. 選擇 **等於** > **True**.

   ![report_proflicenses.png](assets/report-prooflicenses-350x135.png)

1. 按一下 **儲存並關閉**.

   報表會顯示Workfront中所有已指派校對授權的使用者。

## 更新「人員」視圖

您可以在「人員」檢視中新增欄，以檢視哪些使用者可產生校樣：

1. 前往 **人員** 的上界。
1. 按一下 **人員** 標籤。
1. 在 **檢視** 下拉式功能表中，執行下列任一操作：

   * 若要將此資訊新增至現有檢視，請選取您要自訂的檢視，然後按一下 **自訂檢視**.
   * 要將此資訊添加到新視圖，請按一下 **新建視圖**.

1. 按一下 **添加列**.
1. 在可用欄位中，展開 **使用者**，然後按一下 **有證明許可證**.

1. 按一下 **完成**，然後按一下 **保存視圖** 或 **另存為新視圖**.

   視圖隨即顯示 **True** 或 **False** 取決於使用者是否獲派校對授權。
