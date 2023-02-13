---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: 更新單一登入的使用者
description: 您可以更新Workfront中單一登入的使用者。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# 更新單一登入的使用者

{{important-admin-console-onboard}}

在Adobe Workfront執行個體中啟用單一登入(SSO)時，您可以使用SSO憑證登入Workfront。

如果現有系統已填入與SSO憑證相關聯的使用者，您可以將逗號分隔值(CSV)檔案匯入Workfront，將使用者的ID匯入Workfront。

如需將Workfront與SSO系統整合的詳細資訊，請參閱 [Adobe Workfront中的單一登入概觀](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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

## SSO用戶名

根據您使用的SSO解決方案，您的SSO環境中的使用者名稱可以稱為下列任一名稱：

* SSO 使用者名稱
* 同盟 ID
* 聯合用戶名

在Workfront中，所有這些名稱都儲存在使用者物件的SSO使用者名稱欄位中。

為了讓您的使用者能夠使用其SSO憑證登入Workfront，您必須更新其設定檔，以在其Workfront使用者名稱之外，加入其SSO使用者名稱。

身為Workfront管理員，您可以使用使用者名稱清單並在Workfront中匯入，大量更新Workfront使用者的SSO使用者名稱欄位。 此清單必須包含Workfront使用者ID(GUID)以及每個使用者的對應SSO使用者名稱，且必須儲存為CSV或TSV檔案。 此程式會更新Workfront中現有的SSO使用者名稱，或新增新的SSO使用者名稱（如果使用者缺少使用者名稱）。

## 準備匯入檔案 {#prepare-the-import-file}

您可以建立Workfront中所有使用者的報表，並更新其SSO使用者名稱欄位，以開始準備匯入檔案。

1. 在Workfront中建立使用者報表。

   如需在Workfront中建立使用者報表的指示，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 在報表中選取下列欄位：

   | 名稱 | Workfront使用者的完整名稱。 |
   |---|---|
   | ID | ID是Workfront英數字GUID。 |
   | SSO 使用者名稱 | 選取「SSO使用者名稱」欄位，以確保您匯入時不會覆寫任何使用者名稱。 如果您的使用者尚未針對SSO更新，則所有使用者都應將此欄位留空。 |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. 儲存報表。
1. 按一下 **匯出** 將報表匯出為Excel。
1. 開啟匯出的Excel檔案，然後開始在「SSO使用者名稱」欄的報表中新增每位使用者的SSO使用者名稱。

   >[!IMPORTANT]
   >
   >SSO使用者名稱會區分大小寫。

1. 消除Excel檔案中的所有列， **ID** 和 **SSO用戶名** 欄。

1. 消除欄標題，並確保報表頂端沒有空白列。

   您使用SSO使用者名稱來更新Workfront使用者的檔案，必須依順序僅包含2欄：

   * 第一欄應顯示Workfront使用者ID(Workfront中的使用者GUID)。
   * 第二欄應包含SSO使用者名稱，如您的SSO系統中所示。
   * 欄應沒有標題，且名稱清單頂端不應有任何空白列。

      ![](assets/update-users-for-sso-csv-file-for-import.png)

1. 將報表儲存為電腦上的CSV或TSV檔案。

## 更新SSO的用戶 {#update-your-users-for-sso}

為SSO更新使用者的程式會在沒有SSO使用者名稱欄位時，將SSO使用者名稱欄位新增至您的Workfront使用者，或是在有與使用者相關聯的值時，更新該欄位中的值。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **系統** then **更新SSO的用戶**.

1. 按一下 **選擇檔案** 瀏覽您準備的檔案。

   如需有關如何準備此檔案的詳細資訊，請參閱 [準備匯入檔案](#prepare-the-import-file).

1. 選取儲存在電腦上的檔案，然後按一下 **開啟**.

   這可讓所有使用者使用其SSO憑證登入Workfront。

   此 **僅允許 `<SSO Configuration>` 驗證** 會為CSV中包含的所有使用者啟用「 」設定。

## 驗證使用者的Workfront使用者名稱的SSO

有關構建包含SSO用戶名資訊的用戶報表的說明，請參閱 [準備匯入檔案](#prepare-the-import-file).

1. 執行包含SSO使用者名稱資訊的使用者報表。

   請注意，系統會為每個使用者填入SSO使用者名稱欄。

1. 確保SSO用戶名列的值與SSO伺服器上的SSO用戶名匹配。
1. 如果「SSO使用者名稱」欄空白，請更新使用者的SSO使用者名稱。

   ![](assets/users-with-sso-field-updated.png)

   有關為SSO更新用戶的說明，請參閱 [更新SSO的用戶](#update-your-users-for-sso).
