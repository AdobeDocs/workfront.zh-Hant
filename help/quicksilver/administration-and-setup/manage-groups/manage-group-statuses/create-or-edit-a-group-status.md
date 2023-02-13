---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 建立或編輯群組狀態
description: 身為群組管理員，您可以為您管理的群組建立自訂狀態。 這有助於消除數十種公司範圍自訂狀態的需求，並讓您在群組階層中擁有更多自主權。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: 027d636e8256c6a12d552af736884f6f27886114
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 1%

---

# 建立或編輯群組狀態

身為群組管理員，您可以為您管理的群組建立自訂狀態。 這有助於消除數十種公司範圍自訂狀態的需求，並讓您在群組階層中擁有更多自主權。

如果Workfront管理員已解除鎖定狀態，您也可以編輯所管理群組的系統層級狀態。 如需詳細資訊，請參閱 [鎖定和解除鎖定系統級狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

如果群組上有任何群組，其管理員也可以為群組執行這些動作。 Workfront管理員（適用於任何群組）也是如此。

>[!NOTE]
>
>以敏捷檢視檢視專案時，無法在專案上顯示自訂群組狀態。 在敏捷檢視中檢視專案時，只會顯示預設和自訂鎖定狀態。 如需自訂專案敏捷檢視的相關資訊，請參閱區段 [建立或自訂敏捷檢視](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) 在文章中 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

如需狀態的一般資訊，請參閱 [狀態概觀](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

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
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 建立或編輯群組的狀態

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 按一下您要建立或自訂狀態的群組名稱。
1. 在左側面板中，按一下 **狀態**.

   如果您檢視的群組是頂層群組，則顯示的清單包括：

   * 系統級鎖定狀態。
   * 已為群組建立自訂狀態。

   此外，如果您正在查看的組是子組，則清單還包括：

   * 屬於子組上方組的鎖定狀態。
   * 建立子組時屬於子組上方組的解除鎖定狀態。

      建立子組後，在其上方的組中建立的未鎖定狀態不會包含在子組的狀態清單中。 但是，如果某人稍後鎖定其中一個，則會將其包含在子組的狀態清單中。 如需詳細資訊，請參閱 [組如何繼承狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).


1. 選擇對象類型的頁簽(**專案**, **工作**，或 **問題**)，以便與狀態建立關聯。

1. （條件性）如果狀態為問題狀態，請確定 **主清單** 中所有規則的URL。

   ![](assets/master-list.png)

   如需自訂其他問題類型（錯誤報告、變更順序、問題、請求）的相關資訊，請參閱 [自訂預設問題類型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. （條件性）若要建立新狀態，請按一下 **新增狀態**.

   或

   若要編輯現有狀態，請將滑鼠移至您要編輯的狀態上，然後按一下 **編輯** 選項。

   ![](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >只有符合以下條件時，您才可以編輯群組的狀態：
   >      
   >* 您可以管理為其建立狀態的群組
   >* Workfront管理員解除了系統級別的狀態
   >* 組上方組的組管理員解除了狀態鎖定

   >      
   >      
   >編輯現有狀態時，您只能更改其名稱、說明和顏色。
   >
   >編輯鎖定狀態時，您所做的更改將影響從組繼承狀態的所有子組。
   >   
   >相反，編輯解鎖狀態不會影響從組繼承狀態的子組。

1. 指定下列資訊。

   如果您正在編輯狀態，則只能變更前3個設定。

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
      <td> <p>按一下顏色欄位並從色票面板中選取顏色，自訂狀態的顏色。 您也可以在欄位中輸入十六進位數字。</p> <p>使用者檢視物件時，狀態顏色會顯示在Workfront的右上角。</p> <p> <img src="assets/status-color.png"> </p> </td> 
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
      <td> <p>（僅限項目和任務狀態）</p> <p>如果要向用戶隱藏狀態，請啟用此選項。 禁用後（預設設定），組下的所有子組都可以使用狀態。</p> <p>提示：您可以停用所有4種問題類型（「錯誤報告」、「更改順序」、「問題」、「請求」），以隱藏「問題」狀態。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">鎖定所有群組</td> 
      <td> 
       <p>如果保留此選項為啟用狀態，則組及其子組中的用戶可以查看和使用狀態，並且組管理員不能為較低的子組自定義該狀態。</p> 
       <p>禁用此選項後，組管理員可以自定義較低子組的狀態。</p> 
       <p><b>注意</b>:您可以在群組核准程式中使用鎖定和解除鎖定的狀態。 如果您建立了組批准進程，且組狀態處於未鎖定狀態，則用戶可以將批准進程附加到與該組關聯的任何項目、任務或問題。</p> 
       <p>有關鎖定狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">鎖定和解除鎖定的群組狀態</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。

   現在，與您的群組或子群組相關聯的所有專案都可以使用狀態。 如果已鎖定，則任何較低的子組都可以使用它。

   您可以將狀態設定為群組的預設狀態。 如需詳細資訊，請參閱 [使用自訂狀態作為群組的預設狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## 為多個群組建立自訂狀態

如果您是Workfront管理員，您可以建立系統範圍狀態，然後將該狀態隱藏於不需要的任何群組，借此建立多個群組的自訂狀態。

如果您是群組管理員(或Workfront管理員)，您可以為管理的群組階層中的多個子群組建立自訂狀態，方法是為較高層級的群組建立狀態，然後將該狀態隱藏於不需要的較低子群組中。

1. 如果您是Workfront管理員，請建立系統範圍的解鎖狀態，如 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. 在右上角的方塊中，刪除 **系統狀態**，開始輸入您要隱藏狀態之群組的名稱，然後在出現時按一下名稱。
1. 將滑鼠指標暫留在您要在群組中隱藏的狀態上，然後按一下 **編輯** 時顯示。

   ![](assets/hover-click-edit.jpg)

1. 啟用 **隱藏狀態** 選項。

   ![](assets/hide-group-status.png)

1. 按一下&#x200B;**儲存**。

   狀態會呈現暗灰色，該群組中的所有使用者都看不到。

1. 重複步驟3到5以隱藏自訂狀態，使其不讓任何其他不需要的群組使用。
