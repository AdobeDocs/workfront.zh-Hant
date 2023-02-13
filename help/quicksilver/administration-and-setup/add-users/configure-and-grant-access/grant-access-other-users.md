---
title: 授予使用者存取權
description: 身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中其他使用者的存取權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: d1fe7165932fb6f2aff3c8488bdb8e1dfae3b6d3
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# 授予使用者存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中其他使用者的存取，如 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置對用戶的訪問

您可以使用您建立的預設存取層級或自訂存取層級，管理使用者可為其他使用者檢視和編輯的資訊。 具有預設計畫和工作許可證的用戶可以查看其他用戶的聯繫資訊。 下列任何使用者都可以建立和編輯其他使用者：

* Workfront管理員。

   如需詳細資訊，請參閱 [授予使用者完整的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* 具有預設計畫許可的用戶，也具有對用戶的訪問權限，如本文所述。

   僅限查看其公司或主要公司使用者的使用者，只能編輯其可看見的使用者。 如需詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 具有預設計畫許可證的用戶，該用戶還被指定為其他用戶的經理。

   在其存取層級中授予使用者編輯存取權的使用者，可以管理向其報告的使用者。 如需管理使用者的相關資訊，請參閱 [檢視組織圖表](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* 具有預設計畫許可證的用戶可以停用、刪除或編輯其建立的用戶。 如需建立新使用者的相關資訊，請參閱 [新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 使用自訂存取層級設定使用者的存取權以編輯使用者

1. 開始建立或編輯存取層級，如 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 要更改具有計畫或工作許可證的用戶查看其他用戶的配置檔案的能力，請執行以下操作：

   1. 按一下齒輪圖示 ![](assets/gear-icon-settings.png) 在 **檢視** 按鈕 **使用者**.

   1. 停用 **查看聯繫資訊**，然後按一下X以關閉 **微調您的設定** 框。

1. 要修改具有計畫許可證訪問權限的用戶編輯其他用戶的能力，請按一下齒輪表徵圖 ![](assets/gear-icon-settings.png) 在 **編輯** 按鈕 **使用者**，然後選取您要授與的功能：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>建立</strong> </td> 
      <td> <p>可讓使用者建立使用者。<br>預設會啟用此選項。</p> 
      &lt;!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">請務必先進行此變更，再取消這2個備注。 請求檔案說，3/29取決於調查結果。</p>

       &lt;p>&lt;b>注意&lt;/b>:如果您的組織已上線至Adobe Admin Console，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。&lt;/p>
       —>  &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>刪除</strong> </td> 
      <td> <p> 允許用戶刪除自己建立的用戶。<br>預設會啟用此選項。</p> <p><b>注意</b>:如果您的組織已上線至Adobe Admin Console，則無法使用此功能。 如需詳細資訊，請洽詢您的網路或IT管理員。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>使用者管理 (所有使用者)</strong> </td> 
      <td> <p>可讓使用者針對Workfront中的任何使用者執行下列作業：</p> 
       <ul> 
        <li>編輯、刪除或停用使用者</li> 
        <li>以使用者身分登入</li> 
        <li>重設用戶密碼</li> 
       </ul> <p>預設會停用此選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>管理使用者 (所有使用者)</strong> </td> 
      <td> <p>允許使用者對所管理之群組中的任何使用者執行下列動作： 
        <ul>
         <li><p>編輯、刪除或停用使用者</p></li>
         <li>以使用者身分登入</li>
         <li><p>重設用戶密碼</p><p><b>注意</b>:群組管理員無法以登入身分登入，或重設Workfront管理員的密碼。</p></li>
        </ul><p>預設會停用此選項。</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >如果您不想授予群組管理員對其所管理群組之所有成員的存取權，請停用上述兩個「使用者管理」選項。 群組管理員仍可存取新增至Workfront的群組成員，或在Workfront中向他們報告的群組成員。

1. （可選）要配置您正在處理的訪問級別中其他對象和區域的訪問設定，請繼續以下文章之一列出： [設定Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成後，按一下 **儲存**.

## 按許可類型訪問用戶

如需每個存取層級的使用者可搭配使用者執行之動作的相關資訊，請參閱區段 [使用者](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) 在文章中 [每種物件類型皆可使用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
