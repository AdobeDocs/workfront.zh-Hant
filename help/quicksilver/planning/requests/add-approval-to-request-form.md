---
title: 在Adobe Workfront Planning中新增核准至請求表單
description: 您可以在Adobe Workfront Planning請求表單中新增核准流程，以便對每個提交的請求啟動核准，然後再建立記錄。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 2ffd06f2f50d14b6d33bc79c92616ebed1d58fed
workflow-type: tm+mt
source-wordcount: '1195'
ht-degree: 1%

---

# 在Adobe Workfront Planning中新增核准至請求表單

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning請求表單中新增核准流程，以便對每個提交的請求啟動核准，然後再建立記錄。

本文說明工作區管理員如何為與記錄型別關聯的請求表單新增核准。

如需有關在Workfront Planning中建立請求表單的資訊，請參閱[在Adobe Workfront Planning中建立和管理請求表單](/help/quicksilver/planning/requests/create-request-form.md)。

如需有關將請求提交至記錄型別以建立記錄的資訊，請參閱[提交Adobe Workfront Planning請求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<p>任何Workfront套件和任何Planning套件</p>
或
<p>任何Workflow套件和任何Planning套件</p>

<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區與記錄型別</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將核准新增至請求表單的考量事項

* 您可以將一個或多個核准者新增至請求表單。 您只能將使用者新增為核准者。
* 您可以在「核准者」與「已核准日期」欄位中提交請求表單，顯示所建立記錄的核准資訊。 如需詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。
* 將多位核准者新增至請求表單時，所有核准者都必須先接受請求，才能在Workfront Planning中建立記錄。
* 如果所有核准者都核准請求，系統將會針對與請求表單相關聯的記錄型別建立記錄。
* 如果至少有一位核准者拒絕請求，而所有其他核准者皆已核准請求，則會在Workfront的「請求」區域中建立請求，但不會針對與請求表單相關聯的記錄型別建立記錄。
* 將核准新增至請求表單為選用。 如果請求表單未與核准相關聯，Workfront Planning會在提交請求時立即建立記錄。

## 在生產環境中新增核准到請求表單

1. 開始建立記錄型別的要求表單，如[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)中所述。
1. 按一下&#x200B;**組態**。

   顯示&#x200B;**組態**&#x200B;區域。

   ![設定索引標籤](assets/configuration-tab.png)
1. 在&#x200B;**核准者**&#x200B;欄位中，開始輸入您要設定為核准者的使用者或團隊名稱，然後在其顯示在清單中時選取它。
1. （選擇性和條件性）如果您已設定多個核准者，且僅需要一個核准者才能做出決定，請啟用&#x200B;**僅需要一個決定**&#x200B;選項。

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* 您可以將一個或多個核准者新增至請求表單。
   >
   >* 如果您新增多個核准者，但未啟用「僅需一個決定」選項，則所有核准者必須在Workfront Planning建立記錄前核准請求。
   >
   >* 如果至少有一位核准者拒絕請求，則請求會遭到拒絕，且不會建立記錄。 此請求會保留在Workfront的請求區域中。
   >
   >* 如果您新增多個核准者，但未啟用「只有一個決定是必要的」選項，則所有核准者必須在核准或拒絕請求之前做出決定。
   >
   >* 如果團隊被設定為核准者，則只需從團隊中做出一個決定。


1. （選擇性）如果您之前從未共用過請求表單，請按一下&#x200B;**發佈**。

   或

   按一下[共用]以共用表單，然後按[複製]連結&#x200B;**。**&#x200B;**&#x200B;**
1. （選用）使用者使用您共用的連結並提交請求後，Workfront Planning會傳送核准應用程式內通知及電子郵件給核准者。

   >[!NOTE]
   >
   >   您組織的Workfront執行個體必須上線至Adobe統一體驗，使用者才能接收電子郵件和應用程式內通知。


   如需核准要求的詳細資訊，請參閱[核准要求](/help/quicksilver/planning/requests/approve-request.md)。

<div class="preview">

## 將核准規則新增至請求表單

>[!NOTE]
>
>此功能僅在預覽環境中可用。

核准規則會根據已提交請求中的欄位值來定義核准流程。

例如，如果請求表單有「Campaign type」欄位，則可建立規則，當欄位值為「Digital」時傳送請求給一個人，當值為「Print」時傳送請求給另一個人。

新增核准規則時，請考量下列事項：

* 您可以將一或多個核准者新增至核准規則。
* 如果至少有一位核准者拒絕請求，則請求會遭到拒絕，且不會建立記錄。 此請求會保留在Workfront的請求區域中。
* 如果您新增多個核准者，但未啟用「只有一個決定是必要的」選項，則所有核准者必須在核准或拒絕請求之前做出決定。
* 如果團隊被設定為核准者，則只需從團隊中做出一個決定。

如需新增核准的詳細資訊，請參閱[新增核准至要求表單](/help/quicksilver/planning/requests/add-approval-to-request-form.md)。

若要設定請求表單的核准規則：

1. 開始建立記錄型別的要求表單，如[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)中所述。
1. 按一下&#x200B;**設定**。

   「設定」標籤隨即顯示。

1. 若要開始設定核准規則，請按一下左側導覽中的核准![核准圖示](assets/approvals-icon-on-form.png)。

1. （選擇性）如果您想要設定預設核准程式，請在[預設核准規則]區域的&#x200B;**核准者**&#x200B;欄位中新增至少一位使用者或團隊，然後按一下&#x200B;**僅需要一個決定**&#x200B;核取方塊（如果您想要在任何一位預設核准者核准記錄後建立記錄）。

   ![預設核准規則區域](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. （選用）請針對每個額外的核准規則，執行下列作業：

   1. 按一下&#x200B;**新增核准規則**
   1. 按一下預留位置標題「未命名的核准規則」，然後輸入核准規則的名稱。
   1. 按一下&#x200B;**選取欄位**&#x200B;並選取啟用規則的欄位。
   1. 選取規則的運運算元。 運運算元會依欄位型別而異。
   1. 如果選取的運運算元需要值，請按一下加號圖示並新增一或多個值。
   1. （選用）按一下「新增條件」 ，並依照步驟C-E設定其他條件，使用AND或OR新增更多條件。
   1. 在核准規則的「動作」區域中，在&#x200B;**核准者**&#x200B;欄位中，新增至少一位當符合條件時要在核准者處設定的使用者或團隊。
   1. &#x200B;
      1. （視條件而定）如果要在任何核准者核准記錄後建立記錄，請核取&#x200B;**僅需要一個決定**&#x200B;核取方塊。

1. 按一下[儲存]儲存核准規則。**&#x200B;**
1. （選擇性）如果您之前從未共用過請求表單，請按一下&#x200B;**發佈**。

</div>
