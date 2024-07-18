---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選：建立參照相同欄位（'AND'陳述式）的多個篩選規則」
description: 在標準模式介面中，當您嘗試建立參照相同欄位的多個篩選器時（使用AND限定詞），當您儲存報表並退出Report Builder時會刪除其中一個篩選器。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# 篩選：建立參照相同欄位（「AND」陳述式）的多個篩選規則

在標準模式介面中，當您嘗試建立參照相同欄位的多個篩選器時（使用AND限定詞），當您儲存報表並退出Report Builder時會刪除其中一個篩選器。

**範例：**&#x200B;您可能只想檢視名稱中包含「綠色」字樣但不包含「紅色」字樣的工作。 Adobe Workfront不允許您使用標準模式介面儲存下列篩選規則，因為它參考相同的欄位（工作名稱），但使用不同的修飾詞和參考不同的值：

* 工作名稱>包含>綠色
* 任務名稱>不包含>紅色

不過，您可以使用文字模式建立此篩選器。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>請求修改篩選器 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 建立參考相同欄位的多個篩選規則

1. 前往工作清單。
1. 從&#x200B;**篩選器**&#x200B;下拉式功能表中，選取&#x200B;**新增篩選器**。
1. 按一下&#x200B;**切換到文字模式**。
1. 暫留在文字模式區域上，然後按一下&#x200B;**按一下以編輯文字**。
1. 在設定報表的篩選規則區域中，新增下列程式碼：

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >若要建置類似的篩選器，請先建置第一個陳述式。 例如：
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >視需要多次複製並貼上陳述式。 然後，您可以視需要新增陳述式，以參考相同欄位（在此案例中為「名稱」），並對其他陳述式進行下列修改：
   >
   >1. 針對每個新欄位可能的值，在兩個複製行的前面加上&quot;AND:1:&quot;、&quot;AND:2:&quot;、&quot;AND:3:&quot;等。
   >1. 將欄位行替換為新的欄位值（在「=」符號之後）。
   >1. 以新的修正因子取代修正因子明細行(_Mod)。
   >   
   >這些陳述式會區分大小寫。

1. 按一下&#x200B;**完成**，然後按一下&#x200B;**儲存篩選器**。
