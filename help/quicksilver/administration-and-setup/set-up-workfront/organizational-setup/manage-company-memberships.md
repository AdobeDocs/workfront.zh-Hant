---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 管理公司成員資格
description: 在[設定]的[!UICONTROL 公司]區域中，您可以新增及移除公司成員。 您也可以編輯他們的使用者設定檔，提醒他們在 [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] 系統中註冊。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: 705fc990f2d90ff2102233fc68947fdbe1eb6946
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 1%

---

# 管理公司成員資格

在[!UICONTROL 設定]的[!UICONTROL 公司]區域中，您可以新增和移除公司成員。 您也可以編輯其使用者設定檔、提醒他們在[!DNL Workfront]中註冊、在[!DNL Workfront]中停用它們，以及從[!DNL Workfront]系統中移除它們。

如需有關建立新公司的資訊，請參閱[建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] 計劃</p> </td> 
   <td><p>目前： [！UICONTROL Team]或更高版本</p>
   <p>或</p>
   <p>新增：任何</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 授權</p> </td> 
   <td><p>目前： [！UICONTROL計畫]</p>
   <p>或</p>
   <p>新增：[！UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>存取層級設定</strong> </td> 
   <td> <p>下列其中一項：</p> 
    <ul> 
     <li> <p>[！UICONTROL系統管理員]存取層級，可讓您編輯系統中的任何公司。</p> </li> 
     <li> <p>管理公司的管理存取權，可讓您編輯系統中的任何公司。</p> </li> 
    </ul> <p><b>附註</b>：  
     <ul> 
      <li> <p>您也可以管理與您被指派為群組管理員的任何群組相關聯的公司。</p> </li> 
      <li> <p>若要在[!DNL Workfront]系統中新增和移除使用者，您必須具備下列其中一項：</p> 
       <ul> 
        <li> <p>[！UICONTROL系統管理員]存取層級。</p> </li> 
        <li> <p>在您的存取層級中，必須為[！UICONTROL使用者]設定選取[！UICONTROL編輯] 。 此外，針對[！UICONTROL使用者]設定，在[！UICONTROL微調您的設定] <img src="assets/gear-icon-in-access-levels.png">下，必須啟用[！UICONTROL建立]選項以及兩個[！UICONTROL使用者管理]選項中的至少一個。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>如果您使用[！UICONTROL使用者管理員（群組使用者）]選項，您必須是使用者所屬群組的群組管理員。</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 管理公司成員資格

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 公司]**。
1. 按一下公司名稱。
1. 按一下左側面板中的&#x200B;**[!UICONTROL 公司成員]**。
1. 執行下列任一項作業：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">新增成員</td> 
      <td> <p>按一下<b>[！UICONTROL新增成員]</b>，然後在顯示的下拉式功能表中選取下列其中一個選項：</p> 
       <ul> 
        <li> <p><b>[！UICONTROL新使用者]</b>：新增尚未新增至[!DNL Workfront]的使用者。</p> <p>如需新增使用者至[!DNL Workfront]的相關資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">新增使用者</a>和<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>。</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>：新增您擁有編輯許可權的使用者（位於系統中）。</p> <p><b>重要</b>：如果使用者已是其他公司的成員，則新指派會覆寫舊指派。 使用者會失去與先前公司共用專案的存取權，並取得與此公司共用專案的存取權。</p> </li> 
        <li> <p><b>[！UICONTROL匯入使用者]</b>：上傳試算表匯入檔案來匯入使用者。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">匯入使用者</a>。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">編輯成員</td> 
      <td> 
       <ol> 
        <li value="1"> <p>請至少選取一位使用者，然後按一下工具列中的[！UICONTROL編輯]圖示<img src="assets/edit-icon.png">。</p> </li> 
        <li value="2"> <p>在顯示的<b>[！UICONTROL編輯使用者]</b>方塊中設定選項。</p> <p>如需這些選項的相關資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">複製成員</td> 
      <td> <p>您可以複製現有公司成員來建立公司成員。 </p> <p><b>附註</b>：  <p>當您以這種方式建立使用者時，所有資訊都會從原始使用者複製到新建立的使用者，以下資訊除外：</p> 
        <ul> 
         <li>[！UICONTROL個人資訊]區段中的資訊。</li> 
         <li>[！UICONTROL當我登入時，顯示]：在此方塊中會選取存取層級的預設登陸標籤。</li> 
         <li>[！UICONTROL直接下屬]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>選取使用者，然後按一下[！UICONTROL複製]圖示<img src="assets/copy-icon.png">。 </p> </li> 
        <li value="2"> <p>在顯示的<b>[！UICONTROL新使用者]</b>方塊中，編輯新使用者可用的欄位。</p> <p>如需與使用者相關聯之所有欄位的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">編輯使用者的設定檔</a>。</p> </li> 
        <li value="3"> <p>按一下<strong>[！UICONTROL新增此使用者]</strong>。</p> <p>或</p> <p>按一下<strong>[！UICONTROL新增人員使用者並開始另一個]</strong>以儲存新使用者並新增另一個使用者。</p> </li> 
       </ol> <p>這會在[!DNL Workfront]中為使用者建立新帳戶。</p> <p>如果您選取傳送邀請給使用者的選項，使用者應會收到電子郵件，在電子郵件中他們可以依照連結建立其[!DNL Workfront]密碼。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">移除使用者</td> 
      <td> 
       <div> 
        <p>請至少選取一個使用者，按一下<b>[！UICONTROL移除使用者]</b>，然後在顯示的下拉式功能表中選取下列其中一個選項：</p> 
        <ul> 
         <li> <p><b>[！UICONTROL從公司移除]</b>：從公司移除一個或多個使用者。</p> </li> 
         <li> <p><b>[！UICONTROL Delete]</b>：從[!DNL Workfront]系統刪除一個或多個使用者。</p> <p><b>重要</b>：從系統刪除使用者時，也會刪除您可能想要保留之使用者的相關資訊。 建議您停用使用者，而非刪除使用者。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">傳送註解給使用者及他們的[！UICONTROL更新]區域</td> 
      <td> 
       <ol> 
        <li value="1"> <p>請至少選取一位使用者，然後按一下工具列中的<b>[傳送更新給使用者]</b>。</p> </li> 
        <li value="2"> <p>輸入您要傳送給使用者及其使用者設定檔之[！UICONTROL更新]區域的註解。</p>
         <p>如需詳細資訊，請參閱<a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">傳送直接訊息給其他使用者</a>。</p></li> 
       </ol>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">匯出公司成員清單</td> 
      <td> <p>按一下工具列中的[！UICONTROL匯出]圖示<img src="assets/export.png">，然後選取您要用於匯出檔案的格式。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">停用系統中的成員</td> 
      <td> <p>請至少選取一個使用者，按一下工具列中的[！UICONTROL更多]圖示<img src="assets/more-icon.png">，然後選取<b>[！UICONTROL停用]</b>。</p> <p>如需詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">停用或重新啟用使用者</a>。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">提醒使用者在系統中註冊</td> 
      <td> <p> 在<b>[！UICONTROL名稱]</b>欄中，<b>[！UICONTROL已取消註冊]</b>會顯示在每個已取消註冊使用者的名稱旁。 若要提醒這些使用者在系統中註冊，請選取使用者，按一下工具列中的[！UICONTROL更多]圖示<img src="assets/more-icon.png">，然後選取<b>[！UICONTROL提醒使用者註冊]</b>。</p> </td> 
     </tr> 
    </tbody> 
   </table>
