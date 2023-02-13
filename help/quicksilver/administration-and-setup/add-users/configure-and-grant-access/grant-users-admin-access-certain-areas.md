---
title: 授予用戶對特定區域的管理訪問權限
description: 身為Adobe Workfront管理員，您可以使用存取層級來授予具有計畫授權管理存取權的使用者對系統特定區域的存取權。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# 授予用戶對特定區域的管理訪問權限

<!--Linked in several places, do not rename or change URL.-->

身為Adobe Workfront管理員，您可以使用存取層級來授予具有計畫授權管理存取權的使用者對系統特定區域的存取權。

>[!NOTE]
>
>這與讓使用者完全管理存取Workfront不同，相關說明請參閱 [授予使用者完整的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md). &#x200B;

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

## 授予計畫使用者對Workfront特定區域的管理存取權

>[!IMPORTANT]
>
>強烈建議您將內建存取層級維持不變，以便在設定使用者後參照這些層級。 要自定義訪問級別，請複製預設訪問級別並修改副本。 （除了「系統管理員」和「外部用戶」之外，您可以對每個訪問級別執行此操作。）

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **存取層級**.
1. 按一下您要用來授予使用者特定區域之管理存取權之存取層級的名稱。
1. 在 **允許的管理存取** 複選框，以授予必要的管理訪問權限。

   這些選項可讓您授與下列功能：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">核准程序</td> 
      <td><p>建立並管理要在整個系統和特定群組使用的核准程式。</p><p>若沒有此存取權，使用者只能針對有權存取的管理項目建立臨機核准程式。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">公司</td> 
      <td><p>在Workfront中新增及編輯現有公司</p>
      <p>若無此存取權，使用者只能檢視現有公司。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂表單</td> 
      <td><p>建立和編輯（新增、編輯和刪除欄位）其群組中的自訂表單。</p><p>若沒有此存取權，使用者只能將現有表單附加至可存取contribute或管理的物件。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">匯率</td> 
      <td> <p>在Workfront中新增貨幣。</p> <p>若沒有此存取權，使用者只能將現有貨幣新增至所建立的專案。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td><p>查看Workfront中對象的所有費用。</p><p>這不允許用戶建立新的費用類型。</p><p>若沒有此存取權，使用者只能檢視下列項目：</p>
       <ul>
        <li>他們管理的項目、任務或問題的費用</li>
        <li>自費</li>
        <li>下屬的費用</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作角色</td> 
      <td> <p>透過此存取權，使用者可執行下列作業：</p> 
       <ul> 
        <li>查看和編輯現有作業角色</li> 
        <li>添加新作業角色</li> 
        <li>編輯職責開單和成本費率</li> 
       </ul> <p><b>重要</b>:如果您授予計畫員用戶對任務職責的管理訪問權限，則會自動為用戶啟用「編輯職責開單和成本費率」設定。 之後，如果禁用計畫員用戶對任務職責的管理訪問，則用戶仍可看到任務職責，因為「編輯職責開單和成本費率」設定仍處於啟用狀態。 如果發生此情況，並且您需要刪除用戶的查看任務角色的訪問權限，則需要禁用用戶的「編輯角色開單和成本費率」權限設定。 如需指示，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予金融資料的存取權</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">我的群組中的里程碑</td> 
      <td>在「設定」的「里程碑路徑」菜單下查看系統中的所有里程碑路徑。 使用者也可以編輯或刪除屬於其任何群組的任何里程碑路徑。 使用者無法管理（編輯或刪除）未指派給其任何群組的里程碑路徑。<br><p>若沒有此存取權，使用者只能檢視現有的里程碑路徑，並將其套用至其可管理存取權的專案。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>在Workfront中建立和管理提醒通知。<br>若無此存取權，使用者只能接收和檢視通知。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">時間表和時數</td> 
      <td> <p>允許用戶查看Workfront中的所有小時和工時單。</p> <p>當此選項停用時，使用者只能在下列時間檢視數小時：</p> 
       <ul> 
        <li>他們管理的專案、工作或問題</li> 
        <li>他們自己的時間表</li> 
        <li>向其報告的人的時間表</li> 
        <li>他們批准的時間表</li> 
       </ul> <p><b>附註</b>:  <p>無論是否啟用或禁用此選項，組管理員都可以為他們管理的組和子組建立時間表配置檔案，並將它們分配給他們有權編輯的用戶配置檔案的組成員。</p> <p>啟用此選項可能會為某些組管理員提供太多訪問權限，因為他們可以查看系統中所有用戶的時間表配置檔案（和小時數）生成的時間表，而不僅是他們管理的組中的用戶。 如果群組管理員不需要這麼多存取權，您可以停用此選項。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 完成後，按一下 **儲存**.
1. 將新的存取層級指派給使用者，如 [新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >您可以讓使用者擁有使用者的管理存取權。 有關授予用戶管理訪問權限以便管理用戶帳戶的詳細資訊，請參閱 [授予使用者存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
