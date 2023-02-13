---
product-area: projects
navigation-topic: convert-issues
title: 將問題與其解決對象取消連結
description: 將問題轉換為項目或任務以建立項目或任務時，您可以選擇保留原始問題。 您的Adobe Workfront管理員必須啟用此偏好設定，才能在問題轉換期間使用此選項。 如需將問題轉換為專案和工作的詳細資訊，請參閱在Adobe Workfront中轉換問題的概觀。
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 將問題與其解決對象取消連結

將問題轉換為項目或任務以建立項目或任務時，您可以選擇保留原始問題。 您的Adobe Workfront管理員必須啟用此偏好設定，才能在問題轉換期間使用此選項。\
如需將問題轉換為專案和工作的詳細資訊，請參閱 [轉換Adobe Workfront問題概觀](../../../manage-work/issues/convert-issues/convert-issues.md).

當您決定保留已轉換為專案或任務的問題時，問題的解決會系結至專案或任務。 此問題成為項目或任務的可解析對象。 項目或任務是問題的解決對象。

您也可以手動將問題連結至其他問題。 第二個問題會成為第一個問題的「解決物件」(Resoling Object)，在本例中為。\
有關解析對象的詳細資訊，請參閱 [解析和可解析對象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>無法更改問題狀態，因為問題狀態會隨「解決對象」的狀態自動更改。

通過從問題中刪除項目、任務或問題，可以將問題的解決與項目、任務或問題的解決取消連結。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯問題的存取權</p> <p>查看對任務和項目的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理問題的權限</p> <p>查看任務或項目的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 將問題與項目、任務或問題取消連結

1. 轉到連結到項目、任務或問題的問題。
1. 按一下 **問題詳細資訊** 區段。
1. 前往 **概述** 區域 **問題詳細資訊** 區段。
1. 在 **解析者** 欄位，移除可解析的對象類型。\
   問題可由專案、任務或問題解決。

   這會從問題中移除解決物件。

1. 按一下 **儲存** **變更**.\
   問題不再連結至專案、任務或問題，您現在可以獨立解決問題。
