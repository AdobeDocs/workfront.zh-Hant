---
title: 授予團隊存取權
description: 作為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中團隊的存取權
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: 09bb41e16da89edd2c2cbfb5a85213045e52394d
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 5%

---

# 授予團隊存取權

身為Adobe Workfront管理員，您可以使用存取層級來定義使用者對Workfront中團隊的存取權，如[存取層級概觀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td>規劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 設定使用者的存取權，以使用自訂存取層級編輯使用者

1. 開始建立或編輯存取層級，如[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 按一下Teams右側![](assets/gear-icon-settings.png)檢視&#x200B;**或**&#x200B;編輯&#x200B;**按鈕上的齒輪圖示**，然後在&#x200B;**微調您的設定**&#x200B;下選取您要授與的功能。

   ![微調小組](assets/fine-tune-teams.png)

   * **檢視**：如果您正在設定擁有任何授權的使用者檢視團隊的方式，請變更下列任一選項：

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">檢視與我的群組相關聯的團隊</td>
         <td>
          <p><b>已啟用</b>：當使用者在團隊預先輸入欄位中尋找團隊時，使用者可以看到與其群組相關聯的團隊，無論他們是否為團隊成員。 </p>
          <p><b>已停用</b>：當使用者在團隊預先輸入欄位中尋找團隊時，使用者只能看見與其群組相關聯的團隊，只要他們是團隊成員即可</p><p>此選項預設為啟用。</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">檢視所有團隊</td>
         <td><p>當啟用此選項且使用者在團隊預先輸入欄位中尋找團隊時，使用者可以檢視和選取任何團隊。</p><p>此選項預設為啟用。 </p></td>
        </tr>
       </tbody>
      </table>

   * **編輯**：如果您正在設定擁有「計畫」授權與「工作」授權的使用者如何管理團隊，請變更下列任一選項：

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">建立</td>
         <td><p>允許擁有計畫授權或工作授權的使用者建立團隊。</p><p>此選項預設為啟用。</p></td>
        </tr>
        <tr>
         <td role="rowheader">刪除</td>
         <td><p> 允許擁有計畫授權的使用者刪除他們有權編輯的團隊（不適用於擁有工作授權的使用者）。</p><p>此選項預設為啟用。</p></td>
        </tr>
        <tr>
         <td role="rowheader">在我管理的群組中編輯團隊 (僅限群組管理員)</td>
         <td><p>允許指定為群組管理員的計畫授權使用者編輯與其所管理群組相關聯的團隊。</p><p>此選項預設為啟用。</p></td>
        </tr>
        <tr>
         <td role="rowheader">編輯我所在的團隊</td>
         <td><p>允許使用者計畫授權或工作授權編輯他們所屬的團隊。</p><p>此選項預設為停用。</p></td>
        </tr>
        <tr>
         <td role="rowheader">檢視與我的群組相關聯的團隊</td>
         <td>
         <p><b>已啟用</b>當使用者在團隊預先輸入欄位中尋找團隊時，使用者可以看到與其群組相關聯的團隊，無論他們是否為團隊成員。 </p>
         <p><b>已停用</b>：當使用者在團隊預先輸入欄位中尋找團隊時，使用者只能看見與其群組相關聯的團隊，只要他們是團隊成員即可</p><p>此選項預設為啟用。</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">檢視所有團隊</td>
         <td><p>當啟用此選項且使用者在團隊預先輸入欄位中尋找團隊時，使用者可以檢視和選取任何團隊。</p><p>此選項預設為啟用。 </p></td>
        </tr>
       </tbody>
      </table>



1. 按一下X以關閉&#x200B;**微調您的設定**&#x200B;方塊。
1. （選擇性）若要針對您正在處理的存取層級中的其他物件與區域設定存取設定，請繼續使用[設定對Adobe Workfront的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中所列的文章之一，例如[授與對工作的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授與對財務資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成時，按一下&#x200B;**儲存**。

>[!NOTE]
>
>* 無論存取層級設定為何，以下皆為true：
>
>   * 團隊擁有者隨時都可以檢視和編輯其團隊
>   * 使用者一律擁有檢視其所在團隊的許可權
>
>* 如果您決定在存取層級中選取「檢視」而非「編輯」或「檢視」，而是選取「檢視」，則會保留「檢視」和「編輯」（例如「與我的群組相關聯的檢視專案團隊」）可用的任何選項設定。
>

## 依授權型別存取團隊

如需有關每個存取層級中的使用者可以對問題執行的資訊，請參閱文章[每個物件型別可用的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams)中的[團隊](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)小節。
