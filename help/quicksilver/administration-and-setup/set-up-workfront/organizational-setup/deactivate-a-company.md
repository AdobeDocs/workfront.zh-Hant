---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 停用或重新啟用公司
description: 您可以停用不再使用的公司，同時保留其所有相關歷史資料。 如果您將系統中某處已在使用的公司停用，該公司的運作方式會一如既往。 系統不會移除或封鎖該檔案。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: 30b61b32add4c6d062b5b524773d309008c9563d
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 1%

---

# 停用或重新啟用公司

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

您可以停用不再使用的公司，同時保留其所有相關歷史資料。 如果您將系統中某處已在使用的公司停用，該公司的運作方式會一如既往。 系統不會移除或封鎖該檔案。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] 封裝</p> </td> 
   <td><p>任何</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權</p> </td> 
   <td><p>[!UICONTROL 計畫]</p>
   <p>[!UICONTROL 標準]</p>
   </td> 
  </tr>
  <tr> 
   <td>存取層級設定</td> 
  <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>[!UICONTROL 系統管理員]存取層級，可讓您編輯系統中的任何公司。</p> </li> 
     <li> <p>管理公司的管理存取權，可讓您編輯系統中的任何公司。</p> </li> 
    </ul> <p><b>附註</b>：  
     <ul> 
      <li> <p>您也可以管理與您被指派為群組管理員的任何群組相關聯的公司。</p> </li> 
      <li> <p>若要從[!DNL Workfront]系統中新增和移除使用者，您必須具備下列其中一項：</p> 
       <ul> 
        <li> <p>[!UICONTROL 系統管理員]存取層級。 </p> </li> 
        <li> <p>您的存取層級中的<b>[!UICONTROL Users]</b>設定已設定為<b>[!UICONTROL Edit]</b>存取，且<b>[!UICONTROL Create]</b>以及在<b>[!UICONTROL Fine-tune your settings]</b> <b>下啟用的兩個</b>[!UICONTROL User Admin]<img src="assets/gear-icon-in-access-levels.png">選項中的至少一個選項。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>在這兩個選項中，如果已啟用<b>[!UICONTROL User Admin (Group Users)]</b>，您必須是使用者所屬群組的群組管理員。</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 停用或重新啟用公司

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 公司]** ![公司圖示](assets/companies-icon-left-panel.png)。

1. 選取一或多個要停用或重新啟用的公司。
1. 按一下&#x200B;**[!UICONTROL 編輯]**.<!--MAKE THIS A SEPARATE NUMBERED LINE<span class="preview">In the Preview environment, disable the **[!UICONTROL Is Active]** option to deactivate it, or enable the option to activate it.</span>-->
1. &#x200B;<!--In the Production environment, -->針對單一公司，請停用&#x200B;**[!UICONTROL 作用中]**&#x200B;選項以停用它，或啟用啟用啟用它的選項。

   或

   若為多家公司，請從&#x200B;**[!UICONTROL Is Active]**&#x200B;下拉式功能表中選取&#x200B;**[!UICONTROL No]**&#x200B;以停用公司，或選取&#x200B;**[!UICONTROL Yes]**&#x200B;以啟用公司。

1. 按一下「**[!UICONTROL 儲存變更]**」。
