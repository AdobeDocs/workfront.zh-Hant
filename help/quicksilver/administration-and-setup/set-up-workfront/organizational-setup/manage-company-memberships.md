---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 管理公司會籍
description: 在 [!UICONTROL 公司] 區域中，您可以新增和移除公司的成員。 您也可以編輯其使用者設定檔，提醒他們註冊 [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] 系統。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# 管理公司會籍

在 [!UICONTROL 公司] 區域 [!UICONTROL 設定]，您可以新增和移除公司的成員。 您也可以編輯其使用者設定檔，提醒他們註冊 [!DNL Workfront]，在 [!DNL Workfront]，並將其從 [!DNL Workfront] 系統。

如需建立新公司的相關資訊，請參閱 [建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## 存取需求

您必須具備下列條件，才能在 [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] 計劃*</p> </td> 
   <td>[!UICONTROL團隊]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 授權*</p> </td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>訪問級別配置*</strong> </td> 
   <td> <p>下列其中一項：</p> 
    <ul> 
     <li> <p>[!UICONTROL系統管理員]存取級別，允許您編輯系統中的任何公司。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>. </p> </li> 
     <li> <p>對管理公司的管理存取，允許您編輯系統中的任何公司。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </li> 
    </ul> <p><b>附註</b>:  
     <ul> 
      <li> <p>您也可以管理與任何群組相關聯的公司，而您在這些群組中被指派為群組管理員。</p> </li> 
      <li> <p>若要新增至，並從 [!DNL Workfront] 系統，您必須具備下列其中一項：</p> 
       <ul> 
        <li> <p>[!UICONTROL系統管理員]訪問級別。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>. </p> </li> 
        <li> <p>在訪問級別中，必須為[!UICONTROL用戶]設定選擇[!UICONTROL編輯]。 此外，對於[!UICONTROL用戶]設定，在[!UICONTROL微調您的設定]下 <img src="assets/gear-icon-in-access-levels.png"> ，必須啟用[!UICONTROL建立]選項和兩個[!UICONTROL用戶管理]選項中的至少一個。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>如果您使用「[!UICONTROL用戶管理員（組用戶）]」選項，則必須是用戶所屬組的組管理員。</p> </li> 
       </ul> <p>如需存取層級中「使用者」設定的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您擁有的計畫、許可類型或訪問級別配置，請與 [!DNL Workfront] 管理員。

## 管理公司會籍

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 公司]**.
1. 按一下公司名稱。
1. 使用 **[!UICONTROL 公司成員]** ，請執行下列任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">添加成員</td> 
      <td> <p>按一下 <b>[!UICONTROL添加成員]</b>，然後在顯示的下拉式功能表中選取下列其中一個選項：</p> 
       <ul> 
        <li> <p><b>[!UICONTROL新用戶]</b>:新增尚未新增至的使用者 [!DNL Workfront].</p> <p>有關將用戶添加到 [!DNL Workfront]，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">新增使用者</a> 和 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>:新增您已擁有編輯權限的使用者（系統中現有）。</p> <p><b>重要</b>:如果用戶已是另一公司的成員，則新分配將覆蓋舊分配。 使用者無法存取與前一公司共用的項目，而無法存取與此公司共用的項目。</p> </li> 
        <li> <p><b>[!UICONTROL導入用戶]</b>:上傳試算表匯入檔案以匯入使用者。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">匯入使用者</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">編輯成員</td> 
      <td> 
       <ol> 
        <li value="1"> <p>請至少選擇一個用戶，然後按一下[!UICONTROL編輯]表徵圖 <img src="assets/edit-icon.png"> 的下一頁。</p> </li> 
        <li value="2"> <p>在 <b>[!UICONTROL編輯用戶]</b> 框。</p> <p>如需這些選項的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">複製成員</td> 
      <td> <p>您可以複製現有的公司成員來建立公司成員。 </p> <p><b>附註</b>:  <p>以此方式建立用戶時，除以下內容外，所有資訊都會從原始用戶複製到新建立的用戶：</p> 
        <ul> 
         <li>[!UICONTROL個人資訊]部分中的資訊。</li> 
         <li>[!UICONTROL登入時，顯示]:此方塊中會選取存取層級的預設登錄標籤。</li> 
         <li>[!UICONTROL直接報告]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>選取使用者，然後按一下[!UICONTROL複製]圖示 <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>在 <b>[!UICONTROL新用戶]</b> 框中，編輯新用戶可用的欄位。</p> <p>如需與使用者相關聯的所有欄位資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>.</p> </li> 
        <li value="3"> <p>按一下 <strong>[!UICONTROL添加此用戶]</strong>.</p> <p>或</p> <p>按一下 <strong>[!UICONTROL添加人員用戶並啟動其他用戶]</strong> 以保存新用戶並添加另一個用戶。</p> </li> 
       </ol> <p>這會在 [!DNL Workfront] 供使用者使用。</p> <p>如果您選取傳送邀請給使用者的選項，使用者應會收到電子郵件，可在此處追蹤連結以建立其邀請 [!DNL Workfront] 密碼。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">移除使用者</td> 
      <td> 
       <div> 
        <p>至少選擇一個用戶，按一下 <b>[!UICONTROL刪除用戶]</b>，然後在顯示的下拉式功能表中選取下列其中一個選項：</p> 
        <ul> 
         <li> <p><b>[!UICONTROL從公司中刪除]</b>:從公司中移除使用者或使用者。</p> </li> 
         <li> <p><b>[!UICONTROL刪除]</b>:從 [!DNL Workfront] 系統。</p> <p><b>重要</b>:從系統中刪除用戶也會刪除與您可能希望保留的用戶相關聯的資訊。 我們建議停用使用者，而非將其刪除。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">將評論傳送至使用者及其[!UICONTROL更新]區域</td> 
      <td> 
       <ol> 
        <li value="1"> <p>請至少選擇一個用戶，然後按一下[!UICONTROL注釋]表徵圖 <img src="assets/comment-icon.png"> 的下一頁。</p> </li> 
        <li value="2"> <p>輸入要傳送給使用者的註解，並輸入其使用者設定檔的[!UICONTROL更新]區域。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">導出公司成員清單</td> 
      <td> <p>按一下[!UICONTROL導出]表徵圖 <img src="assets/export.png"> 在工具列中，選取要匯出檔案的格式。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">停用系統中的成員</td> 
      <td> <p>請至少選擇一個用戶，按一下[!UICONTROL更多]表徵圖 <img src="assets/more-icon.png"> 在工具列中，然後選取 <b>[!UICONTROL停用]</b>.</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">提醒用戶在系統中註冊</td> 
      <td> <p> 在 <b>[!UICONTROL名稱]</b> 欄， <b>[!UICONTROL未註冊]</b> 顯示在每個未註冊用戶的名稱旁邊。 若要提醒這些使用者在系統中註冊，請選取使用者，按一下[!UICONTROL更多]圖示 <img src="assets/more-icon.png"> 在工具列中，然後選取 <b>[!UICONTROL提醒用戶註冊]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
