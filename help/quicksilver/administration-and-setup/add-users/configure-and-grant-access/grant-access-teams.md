---
title: 授予團隊的存取權
description: 身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中團隊的存取權
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 4%

---

# 授予團隊的存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中團隊的存取，如 [存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## 使用自訂存取層級設定使用者的存取權以編輯使用者

1. 開始建立或編輯存取層級，如 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 按一下齒輪圖示 ![](assets/gear-icon-settings.png) 在 **檢視** 或 **編輯** 按鈕，然後選擇要授予的功能 **微調您的設定**.

   * **檢視**:如果您要設定擁有任何授權的使用者如何檢視團隊，請變更下列任一選項：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">檢視與我的群組相關聯的團隊</td>
         <td>
          <p><b>已啟用</b>:當用戶在「團隊預先類型」欄位中查找團隊時，無論他們是否為團隊成員，用戶都可以查看與其組關聯的團隊。 </p>
          <p><b>已停用</b>:當用戶在「團隊預先類型」欄位中查找團隊時，用戶只能在團隊成員所在的位置查看與其組關聯的團隊</p><p>預設會啟用此選項。</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">檢視所有團隊</td>
         <td><p>當啟用此選項，且使用者在「團隊預先類型」欄位中尋找團隊時，使用者可以看見並選取任何團隊。</p><p>預設會啟用此選項。 </p></td>
        </tr>
       </tbody>
      </table>

   * **編輯**:如果您正在配置具有計畫許可證和工作許可證的用戶如何管理團隊，請更改以下任一選項：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">建立</td>
         <td><p>允許具有計畫許可證或工作許可證的用戶建立團隊。</p><p>預設會啟用此選項。</p></td>
        </tr>
        <tr>
         <td role="rowheader">刪除</td>
         <td><p> 允許具有計畫許可證的用戶刪除他們有權編輯的團隊（具有工作許可證的用戶無法使用）。</p><p>預設會啟用此選項。</p></td>
        </tr>
        <tr>
         <td role="rowheader">在我管理的群組中編輯團隊 (僅限群組管理員)</td>
         <td><p>允許指定為組管理員的計畫許可證用戶編輯與他們管理的組關聯的團隊。</p><p>預設會啟用此選項。</p></td>
        </tr>
        <tr>
         <td role="rowheader">編輯我所在的團隊</td>
         <td><p>允許用戶在其所屬的團隊中編輯計畫許可證或工作許可證。</p><p>預設會停用此選項。</p></td>
        </tr>
        <tr>
         <td role="rowheader">檢視與我的群組相關聯的團隊</td>
         <td>
         <p><b>已啟用</b> 當用戶在「團隊預先類型」欄位中查找團隊時，無論他們是否為團隊成員，用戶都可以查看與其組關聯的團隊。 </p>
         <p><b>已停用</b>:當用戶在「團隊預先類型」欄位中查找團隊時，用戶只能在團隊成員所在的位置查看與其組關聯的團隊</p><p>預設會啟用此選項。</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">檢視所有團隊</td>
         <td><p>當啟用此選項，且使用者在「團隊預先類型」欄位中尋找團隊時，使用者可以看見並選取任何團隊。</p><p>預設會啟用此選項。 </p></td>
        </tr>
       </tbody>
      </table>

1. 按一下X以關閉 **微調您的設定** 框。
1. （可選）要配置您正在處理的訪問級別中其他對象和區域的訪問設定，請繼續以下文章之一列出： [設定Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予任務的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成後，按一下 **儲存**.

>[!NOTE]
>
>* 無論存取層級設定為何，下列皆為true:
   >
   >   * 團隊擁有者可隨時檢視和編輯其團隊
   >   * 使用者隨時都可檢視其所在的團隊
>
* 如果您決定在存取層級中選取「檢視」而非「編輯」或「編輯」，而非「檢視」，則會保留「檢視」和「編輯」可用的任何選項的設定（例如「檢視與我的群組相關聯的團隊」）。
>


## 依授權類型存取團隊

如需每個存取層級的使用者可針對問題執行哪些動作的相關資訊，請參閱區段 [團隊](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) 在文章中 [每種物件類型皆可使用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
