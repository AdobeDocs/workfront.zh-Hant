---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 刪除職位角色
description: 您可以刪除組織不再使用的工作角色。 若職務角色過去曾與工作專案相關聯，建議您不要刪除。 若要保留您關於工作指派的所有歷史資訊，我們建議您停用角色，而不是在角色過時時將其刪除。 如需有關停用角色的資訊，請參閱停用工作角色。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# 刪除職位角色

您可以刪除組織不再使用的工作角色。 若職務角色過去曾與工作專案相關聯，建議您不要刪除。

若要保留您關於工作指派的所有歷史資訊，我們建議您停用角色，而不是在角色過時時將其刪除。 如需有關停用角色的資訊，請參閱[停用工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>職位角色的管理存取權</p> <p><b>注意</b>：如果您仍然沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 刪除工作角色

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**[!UICONTROL 工作角色].**
1. 選取您要刪除的工作角色，然後按一下&#x200B;**[!UICONTROL 刪除]。**
1. 如果有任何指派給工作角色的物件（使用者、任務、問題），請執行下列任一項作業：

   * **以不同的工作角色取代工作角色：**&#x200B;從下拉式清單中選取新的工作角色。

     與已刪除工作角色相關聯的任何目前和過去資源配置都會轉移到您選取的工作角色。

     只指派了一個工作角色的使用者會被重新指派給您選取的工作角色；指派了輔助工作角色的使用者不會重新指派給您選取的工作角色。

   * **刪除工作角色及其資源配置：**&#x200B;從下拉式清單中選取&#x200B;**[!UICONTROL 無]**。

     >[!IMPORTANT]
     >
     >刪除工作角色會刪除所有專案中與該工作角色相關的所有目前和過去資源配置。

     例&#x200B;如，如果任務或問題僅指派給該工作角色，則任務或問題會在工作角色刪除後取消指派。

1. 按一下&#x200B;**[!UICONTROL 是，刪除]**。
