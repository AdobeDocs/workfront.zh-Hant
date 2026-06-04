---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: 使用者名稱已經有人使用
description: 當您收到使用者名稱已被使用的錯誤時，請閱讀這些提示。
author: Becky
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
TQID: https://experienceleague.adobe.com/uGrOaZZzbE6CkodhE1TlCtW4rRJkfqljWGJbNSzxODc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 300
ht-degree: 8%

---

# 使用者名稱已經有人使用

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td><p>系統管理員</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 問題

建立新使用者時，會顯示[!UICONTROL 糟糕]錯誤，指出使用者名稱已被使用。 在系統中沒有此電子郵件的其他例項。 為何顯示此訊息？

## 解決方案

這可能是因為使用者名稱或電子郵件地址在目前的[!DNL Adobe Workfront]執行個體中不是唯一的。 使用者在不同的執行個體中可以使用相同的使用者名稱或電子郵件地址。 例如，使用者A可能擁有下列與[!DNL Workfront]帳戶關聯的電子郵件地址：usera@company1.com和usera@company2.com。

>[!NOTE]
>
>如果主要[!DNL Workfront]管理員位在相同叢集上的不同Workfront執行個體中，則不能有相同的使用者名稱或電子郵件地址。
>
>如果執行個體位於不同的叢集，主要管理員可以有相同的使用者名稱或電子郵件地址。 您可以在[!UICONTROL 設定] > [!UICONTROL 系統] > [!UICONTROL 客戶資訊]下檢視執行個體所在的叢集。

### 檢查您的使用者名稱在執行個體中是否唯一

確認使用者名稱和電子郵件地址在目前的[!DNL Workfront]執行個體中是唯一的：

{{step-1-to-users}}

1. 在人員清單中，檢視&#x200B;**[!UICONTROL 電子郵件]**&#x200B;欄，確保沒有重複的電子郵件。
1. 在檢視中新增使用者名稱欄。

   1. 在&#x200B;**[!UICONTROL 檢視]**&#x200B;下拉式功能表中，按一下&#x200B;**[!UICONTROL 自訂檢視]**。
   1. 按一下「**[!UICONTROL 新增欄]**」。
   1. 在搜尋欄位中，輸入&#x200B;*[!UICONTROL 使用者名稱]*。
   1. 選取&#x200B;**[!UICONTROL 使用者]** > **[!UICONTROL 使用者名稱]**。
   1. 儲存檢視。\
      這會導致檢視顯示使用者名稱，您可以在其中尋找重複專案。

1. 在人員清單中，檢視&#x200B;**[!UICONTROL 使用者名稱]**&#x200B;欄，確保沒有重複的使用者名稱。
