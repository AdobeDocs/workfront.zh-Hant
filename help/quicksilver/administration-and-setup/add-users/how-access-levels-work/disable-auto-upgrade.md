---
title: 對新許可計畫上的未付費用戶禁用自動升級選項
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 訪問，級別，系統，管理員，標準，燈光，參與者
navigation-topic: access-levels
description: 每個用戶必須具有訪問級別才能登錄並在Workfront工作。 您使用訪問級別來控制用戶可以查看的內容以及對某些Workfront對象和區域執行的操作。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 864906732c80af12db051d1d5e6d9bc4ae125eb8
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 1%

---


# 對新許可計畫上的未付費用戶禁用自動升級選項

對於新計畫的所有未付費的Workfront許可證，證明和檔案決定是有限的。 當用戶達到其分配的決策數時，預設情況下，他們將升級到Light許可證。

可以從設定區域禁用自動升級選項。 要瞭解有關自動升級工作方式的詳細資訊，請參閱 [非付費用戶的有限文檔和證明決策概述](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)。

>[!IMPORTANT]
>
>禁用後，任何超出其分配決策數的未付費用戶都不會自動升級。


## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront牌照</td> 
   <td>當前計畫：標準
   <p>或</p>
   <p>舊計畫：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>你必須是Workfront管理員。</p></td> 
  </tr> 
 </tbody> 
</table>

## 禁用非付費用戶的自動升級

{{step-1-to-setup}}

1. 向下滾動到 [!UICONTROL **首選項**]。
1. 在 [!UICONTROL **常規首選項**] 的 [!UICONTROL **在訪問級別中禁用自動升級**] 框。
1. 按一下&#x200B;[!UICONTROL **儲存**]。
