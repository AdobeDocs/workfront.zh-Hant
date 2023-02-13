---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ADFS登出URL無法運作
description: 本頁所述的程式僅適用於尚未上架到Adobe Admin Console的組織。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# ADFS登出URL無法運作

>[!IMPORTANT]
>
>本頁面所述的程式僅適用於尚未上架到 [!UICONTROL Adobe Admin Console].
>
>如果您的組織已上線至 [!UICONTROL Adobe Admin Console]，請參閱 [平台管理差異([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## 問題

使用ADFS登出URL(https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0)時，您會收到訊息頁面，並出現錯誤：「訪問站點時出現問題。 嘗試再次瀏覽到該站點。」

如果問題仍然存在，請與此站點的管理員聯繫，並提供以下參考編號以識別問題： **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

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
   <td role="rowheader">Adobe [!DNL Workfront] 授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解決方案

1. 在ADFS管理器伺服器中，轉至 **[!UICONTROL 信任關係]** > **[!UICONTROL 信賴方信託]** > `<your party trust>` 屬性。

1. 在 **[!UICONTROL 端點]** 按一下 **[!UICONTROL 新增]**.

1. **[!UICONTROL 端點類型]** = SAML登出， Binding =POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   如果您想要將回應URL重新導向至其他頁面，可以設定回應URL。 但我們建議使用ADFS網站，因為它會警告您已登出，但您仍應關閉瀏覽器。
