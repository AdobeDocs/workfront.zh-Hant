---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 刪除職位角色
description: 您可以刪除組織不再使用的工作角色。 若職務角色過去曾與工作專案相關聯，建議您不要刪除。 若要保留您關於工作指派的所有歷史資訊，我們建議您停用角色，而不是在角色過時時將其刪除。 如需有關停用角色的資訊，請參閱停用工作角色。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# 刪除職位角色

您可以刪除組織不再使用的工作角色。 若職務角色過去曾與工作專案相關聯，建議您不要刪除。

若要保留您關於工作指派的所有歷史資訊，我們建議您停用角色，而不是在角色過時時將其刪除。 如需有關停用角色的資訊，請參閱[停用工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)。

## 存取需求

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[！UICONTROL標準]</p>
       <p>[！UICONTROL計畫]</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>工作角色的管理存取權</td>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 刪除工作角色

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

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
