---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 刪除作業角色
description: 您可以刪除您的組織不再使用的工作角色。 如果您過去曾與工作項目相關聯，建議您不要刪除這些工作角色。 要保留有關工作分配的所有歷史資訊，建議您停用角色，而不是在角色過時時將其刪除。 有關停用角色的資訊，請參閱停用作業角色。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# 刪除作業角色

您可以刪除您的組織不再使用的工作角色。 如果您過去曾與工作項目相關聯，建議您不要刪除這些工作角色。

要保留有關工作分配的所有歷史資訊，建議您停用角色，而不是在角色過時時將其刪除。 有關停用角色的資訊，請參閱 [停用作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>對作業角色的管理訪問</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 刪除作業角色

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 作業角色].**
1. 選擇要刪除的作業角色，然後按一下 **[!UICONTROL 刪除].**
1. 如果有任何對象（用戶、任務、問題）被分配給作業角色，請執行以下操作之一：

   * **將作業角色替換為不同的作業角色：** 從下拉清單中選擇新作業角色。

      與已刪除的作業角色關聯的任何當前和過去的資源分配都將轉移到您選擇的作業角色。

      只為其分配了一個作業角色的用戶被重新分配到您選擇的作業角色；分配了輔助作業角色的用戶不會重新分配到您選擇的作業角色。

   * **刪除作業角色及其資源分配：** 選擇 **[!UICONTROL 無]** 從下拉式清單中。

      >[!IMPORTANT]
      >
      >刪除作業角色會刪除與所有項目的該作業角色相關的所有當前和過去資源分配。

      &#x200B;例如，如果僅將任務或問題分配給該作業角色，則在刪除作業角色後，將取消分配該任務或問題。

1. 按一下  **[!UICONTROL 是，刪除它]**.
