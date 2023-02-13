---
title: 建立或編輯狀態
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: 身為Adobe Workfront管理員，您可以為專案、工作和問題建立自訂狀態。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: f3785c66b979cc95bf1d2d2ccacbdeefe0ef0967
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 2%

---

# 建立或編輯狀態

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

身為Adobe Workfront管理員，您可以為專案、工作和問題建立自訂狀態。 這可適用於整個Workfront系統的使用者，或特定群組或子群組。 如需狀態的詳細資訊，請參閱 [狀態概觀](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>群組管理員也可以建立自己的群組狀態，僅供群組使用。 如需詳細資訊，請參閱 [建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

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
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 建立或編輯自訂狀態

您可以新增自訂狀態，供整個組織或單一群組使用。

當您為整個組織建立自訂狀態時，可以進行設定，讓系統中的所有群組都能使用它，而不需要編輯。 或者，您也可以進行設定，讓群組管理員可以修改其群組，如 [建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **專案偏好設定** > **狀態**.

1. （條件性）如果要建立或編輯狀態以供系統範圍使用，請確保 **系統狀態** 中，將選定「URL」。

   ![](assets/system-statuses-in-upper-rt-corner.jpg)

   或

   如果狀態是組或子組，請開始在右上角鍵入組的名稱，然後在出現時選擇它。

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. 選擇對象類型的頁簽(**專案**, **工作**，或 **問題**)，以便與狀態建立關聯。

1. 如果要建立新狀態，請按一下 **新增狀態**.

   或

   如果您正在編輯現有狀態，請將滑鼠指標暫留在該狀態上，然後按一下 **編輯** 圖示顯示。

   ![](assets/custom-status-edit.png)

1. 使用下列選項設定狀態：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">狀態名稱</td> 
      <td> <p>輸入狀態的名稱。 這是必填欄位。</p> <p>建立狀態名稱時，請注意系統中的其他人可以建立具有相同名稱的狀態。 建議您使用唯一名稱，以避免在Workfront中選取狀態時產生混淆。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>（選用）輸入狀態說明。 這就向使用它的人傳達了它的目的。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">顏色</td> 
      <td> <p>按一下顏色欄位並從色票面板中選取顏色，自訂狀態的顏色。 您也可以在欄位中輸入十六進位數字。</p> <p>使用者檢視物件時，狀態顏色會顯示在Workfront的右上角。</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">視為</td> 
      <td> <p>從清單中選取最能說明狀態函式的選項之一。 例如，如果狀態名稱為Done，則其相等的選項應為Complete。</p> <p>每個狀態都必須等同於其中一個選項，因為這會決定狀態的運作方式。</p> <p>建立狀態後，無法修改此選項。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">密鑰</td> 
      <td> <p>如果要建立新狀態，請鍵入狀態的代碼或縮寫，或使用為您生成的代碼或縮寫。 此金鑰在Workfront中必須是唯一的，因為可用於報表用途。 如果嘗試指定已在系統中使用的鍵，則欄位將變為紅色。</p> <p>使用縮寫，讓將使用縮寫的人看得懂，或許會很實用。</p> <p>建立狀態後，無法修改此選項。</p> <p>您不能更改「計畫」、「當前」和「完成」狀態的關鍵代碼。 如果您要以文字模式建立報表，這很重要。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">隱藏狀態</td> 
      <td> <p>（僅限項目和任務狀態）</p> <p>如果要向用戶隱藏狀態，請啟用此選項。 禁用時（預設設定），系統中的所有用戶都可以使用狀態。</p> <p>您可以停用所有4種問題類型（「錯誤報告」、「更改順序」、「問題」、「請求」），以隱藏「問題」狀態。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">鎖定所有群組</td> 
      <td>
       <p>鎖定狀態時，系統中的使用者可以查看及使用狀態，而群組管理員無法針對其群組自訂狀態。</p> 
       <p>狀態解除鎖定時，群組管理員可針對個別群組自訂狀態。</p>

   <div>
       <p>您可以在系統批准過程中使用鎖定狀態和解鎖狀態。 如果您建立具有未鎖定系統狀態的系統批准進程，則系統中的用戶可以將批准進程附加到系統中的任何項目、任務或問題。</p>
       <p> 在下列情況下，會顯示警告訊息，協助您和您的使用者了解解除狀態鎖定的結果：</p>
       <ul>
       <li>管理員解除鎖定在批准過程中使用的系統級狀態。 系統會發出警告，指出可能會刪除其群組的解除鎖定狀態，這會使群組成員無法針對指派給其群組的物件正確使用該核准程式。</li>
       <li>用戶開始編輯使用解鎖狀態的批准進程。 訊息會提醒使用者解除鎖定狀態，讓他們評估重新鎖定或更換是否是個好主意。</li>
       <li>對象上附加了具有未鎖定狀態的系統級批准進程，並且為分配給該對象的組刪除了該狀態。 當組成員進入對象的「批准」部分時，消息將說明無法為對象啟動批准進程。</li>
       </ul>
       <p>有關鎖定狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">鎖定和解除鎖定系統級狀態</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。

   有關將此狀態設為預設狀態的說明，請參閱 [使用自訂狀態作為預設狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

有關重新排序組狀態的資訊，請參閱 [重新排序系統級和組狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
