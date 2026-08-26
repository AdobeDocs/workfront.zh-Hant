---
title: 共用Workfront規劃欄位
description: 您可以與其他人共用Workfront Planning記錄的欄位，以確保在使用Adobe Workfront Planning時共同作業。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 2d26437c69b3c36366938952d426532934f55c52
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 2%

---


# 共用Workfront規劃欄位

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

您可以與其他人共用Workfront Planning記錄的欄位，以確保在使用Adobe Workfront Planning時共同作業。

欄位共用可讓工作區管理員控制對個別欄位的存取權。 記錄型別中的每個欄位都有自己的共用對話方塊，其中存取權可以設定為無存取權、檢視欄位值或管理欄位值。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<p>具有Planning套件的任何Workfront或工作流程</p> 
或
<p>任何Workfront Planning作為獨立產品套件</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>任何</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe計畫授權</p></td> 
   <td><p>任何</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>擁有Workflow和Planning套件時，您必須將Workflow和Planning授權型別新增到存取層級</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td><p>管理欄位的許可權以變更欄位的值</p>  
   <p>貢獻或更高的記錄型別許可權以繼承欄位的管理許可權</p>  
   </td> 
  </tr>
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共用欄位的相關考量事項

* 您可以與使用者、工作角色、群組、團隊或公司共用欄位。
* 對欄位的存取權來自結合下列設定：

  * **繼承許可權**：依預設，欄位繼承某人對於記錄型別的相同存取權（檢視記錄型別許可權授予使用者檢視欄位值的許可權；貢獻或管理記錄型別許可權授予使用者管理欄位值的許可權）。 您可以關閉繼承許可權，並給予使用者比記錄型別更低的欄位存取權。
  * 工作區中的&#x200B;**每個人都可以檢視**&#x200B;或&#x200B;**只有受邀者可以存取**&#x200B;選取專案。 您可以允許擁有工作區許可權的所有人檢視欄位，或僅將許可權授予個別實體。

  如果同一個人套用多個規則，這些規則會從其中一個規則中取得他們可用的最高許可權。

* 只有工作區擁有者和管理員可以調整欄位許可權；工作區管理員一律保留對所有欄位的「管理」存取權，這是無法降低的。
* 欄位共用控制對值的存取，而不是欄位設定。 只有工作區管理員可以變更欄位的設定。
* 將某人新增至欄位的共用清單不會授予他們工作區或記錄型別存取權。 如果他們沒有該存取權，警告圖示會指出該許可權只有在將其新增到記錄型別後才會生效。
* 系統欄位（例如，建立者、記錄ID）和主要欄位不能有受限制的共用。
* 限制欄位會在顯示欄位的所有位置強制執行。 這包括所有的檢視、記錄詳細資訊頁面、請求表單、連線和查詢欄位、畫布控制面板、API和MCP工具。
* 查閱欄位繼承其來源欄位的許可權。
* 任何可以存取公開檢視的使用者都能完全看見這些檢視，且維持唯讀狀態。
* 當您複製記錄時，受限制的值不會複製到新記錄中。
* 限制的欄位值變更不會記錄在記錄的歷史記錄中。
* 欄位的許可權變更不會觸發通知。
* 對於全域記錄型別，欄位許可權會套用至所有次要工作區，且無法在本機調整。


從克勞德：
欄位的其他許可權 — 可將此許可權新增至所有共用的概述文章?? - help/quicksilver/planning/access/sharing-permissions-overview.md

以下說明記錄型別/工作區存取對應至檔案中欄位層級存取的方式：

欄位許可權層級（只有兩個，加上無）：

無存取權 — 欄位完全隱藏
檢視欄位值 — 可檢視值，無法編輯
管理欄位值 — 可以檢視和編輯

從記錄型別角色的預設繼承

記錄型別/工作區存取預設欄位許可權
檢視檢視欄位值
「貢獻管理」欄位值
管理（工作區管理員）管理欄位值（已鎖定 — 無法減少）

因此，依預設，欄位只是鏡射某人擁有的任何記錄型別角色 — 檢視者獲得唯讀許可權，貢獻者和管理者獲得編輯許可權。 Workspace管理員是特殊情況：無論何時將其新增到欄位的共用清單中，都會預先選取「管理欄位值」並停用「檢視欄位值」選項，因為他們的編輯存取權永遠無法移除。

萬用字元（備援）設定
除了繼承以外，每個欄位都有萬用字元預設值：

工作區中的所有人都可以檢視（預設）
只有受邀人員才能存取

最終許可權的計算方式

如果已啟用繼承許可權：人員的存取權= （繼承自記錄型別、萬用字元、個別授予的許可權）中的最高者。
如果繼承的許可權被停用：個人的存取權= （萬用字元，個別授予的許可權）中的最高值 — 記錄型別角色不再受影響。
如果停用繼承，萬用字元為「只有受邀人員才能存取」，且在人員獲得「無存取權」→不會個別新增該人員。

其他許可權附註

單獨授予某人存取權不會授予他們工作區/記錄型別的存取權 — 它只會處於非使用中狀態（具有警告圖示），直到他們單獨新增到工作區為止。
對於全域記錄型別，欄位許可權設定一次，並套用至所有次要工作區；次要/團隊工作區管理員無法在本機覆寫它們。

## 共用欄位

