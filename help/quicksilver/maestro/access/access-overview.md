---
title: 存取權總覽
description: 使用Adobe Maestro功能時，有授權和共用許可權限制。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 08a7fa1f3871494c4c6b0c385a98a64735b7f7e4
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->
<!--update the title and the metadata title if Maestro is NOT its own product - because the title is too generic for it being a Workfront capability-->

# 存取權總覽

{{maestro-important-intro}}

使用Adobe Maestro功能時，有授權和共用許可權限制。

## 存取需求

您必須具備下列設定才能使用Adobe大師：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 產品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>貴組織必須註冊AdobeMaestro封閉測試版計畫。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront計畫</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權*</p></td>
   <td>
   <p>任何</p>
   <p>若要建立工作區，您必須擁有下列授權：</p>
   <ul>
   <li>
   新增：標準
   </li>
   <li>
   目前：工作者或以上
   </li>
   </ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Maestro物件沒有存取層級控制項</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>物件許可權</p></td>
   <td>
   <p>貢獻或更高的許可權給您未建立的工作區和檢視，以編輯、刪除和共用它們，以及建立、編輯或刪除記錄型別和記錄。</p>
    <p>系統管理員可以管理他們未建立的工作區和檢視 </p>
   <p>如需有關共用Maestro物件許可權的資訊，請參閱  
   <a href="../access/sharing-permissions-overview.md">在Adobe Maestro中共用許可權概觀</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Maestro區域。 </p> <p>如需詳細資訊，請參閱 <a href="/help/quicksilver/maestro/access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*如需有關Workfront存取需求的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 與其他共用主功能表中的Maestro區域

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

貴組織註冊Maestro測試版計畫後，您可以使用版面配置範本將Maestro區域新增到所有使用者的主功能表中。

1. 登入 **Workfront** Workfront管理員。

1. 新增 **大師** 圖示 ![](assets/maestro-icon.png) 至 **主要功能表** 使用 **版面配置範本**.

   如需詳細資訊，請參閱 [使用版面配置範本自訂主功能表](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. 將版面配置範本指派給您要存取Maestro的使用者。

   如需詳細資訊，請參閱 [將使用者指派至版面配置範本](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   所有指派給範本的使用者現在可以在他們的主功能表中存取Maestro。

   使用者可以開始建立工作區、記錄型別、記錄和欄位。

## 授予存取權

Maestro沒有存取控制。

擁有任何授權型別的使用者都可以存取Maestro。

如需在Workfront中授與存取權的相關資訊，請參閱 [建立和修改自訂存取層級](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## 授予許可權

您必須將您建立的工作區和檢視授予非系統管理員的使用者許可權，他們才能存取這些工作區與檢視。

如需詳細資訊，請參閱 [在Adobe Maestro中共用許可權概觀](/help/quicksilver/maestro/access/sharing-permissions-overview.md).

您的Adobe Workfront授權型別會與您的Maestro許可權搭配使用，讓您能夠檢視、貢獻或管理Maestro物件。

如需有關授權型別如何影響Maestro物件許可權等級的資訊，請參閱 [Adobe Maestro中的授權型別概觀](/help/quicksilver/maestro/access/license-type-overview.md).


