---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: 用戶名已在使用中
description: 收到使用者名稱已被擷取的錯誤時，請閱讀這些提示。
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 用戶名已在使用中

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權</strong></td> 
   <td> <p>[!UICONTROL計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置</strong></td> 
   <td> <p>[!UICONTROL系統管理員]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

建立新使用者時， [!UICONTROL 哇] 系統會顯示錯誤，指出已使用使用者名稱。 系統中沒有發生此電子郵件的其他事件。 為何顯示？

## 解決方案

這可能發生，因為目前的使用者名稱或電子郵件地址不唯一 [!DNL Adobe Workfront] 例項。 使用者可在不同例項中擁有相同的使用者名稱或電子郵件地址。 例如，使用者A可能有下列與 [!DNL Workfront] 帳戶：usera@company1.com和usera@company2.com。

>[!NOTE]
>
>主要 [!DNL Workfront] 如果管理員位於相同叢集上的個別Workfront執行個體中，則無法擁有相同的使用者名稱或電子郵件地址。
>
>如果執行個體位於不同叢集，則主要管理員可以有相同的使用者名稱或電子郵件地址。 您可以在下查看您的實例所在的群集 [!UICONTROL 設定] > [!UICONTROL 系統] > [!UICONTROL 客戶資訊].

### 檢查您的使用者名稱在您的執行個體中是否唯一

請確定使用者名稱和電子郵件地址在目前的 [!DNL Workfront] 例項：

1. 作為 [!DNL Workfront] 管理員，按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 使用者]**.
1. 在人員清單中，查看 **[!UICONTROL 電子郵件]** 欄，確保電子郵件不重複。
1. 將使用者名稱的欄新增至檢視。

   1. 在 **[!UICONTROL 檢視]** 下拉式功能表，按一下 **[!UICONTROL 自訂檢視]**.
   1. 按一下 **[!UICONTROL 添加列]**.
   1. 在搜尋欄位中，輸入 *[!UICONTROL 用戶名]*.
   1. 選擇 **[!UICONTROL 使用者]** > **[!UICONTROL 使用者名稱]**.
   1. 保存視圖。\
      這樣，您就可以檢視，以顯示您可在其中尋找重複項目的使用者名稱。

1. 在人員清單中，查看 **[!UICONTROL 使用者名稱]** 欄以確保沒有重複的使用者名稱。
