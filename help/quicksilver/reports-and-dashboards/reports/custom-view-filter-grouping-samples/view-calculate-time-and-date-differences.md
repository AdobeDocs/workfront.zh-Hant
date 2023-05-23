---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''查看：計算時間和日期差異'
description: 您可以計算以下 — EDIT ME之間的差。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# 視圖：計算時間和日期差異

>[!IMPORTANT]
>
>不能計算同一類型的兩個不同對象在Adobe Workfront的時間和日期差。 例如，您不能計算兩個不同項目、任務或問題上兩個日期之間的時間和日期差。

您可以計算以下兩者之間的差異：

* 同一對象上兩個日期欄位之間的時間和日期差異
* 對象上的欄位與父對象上的另一個欄位之間的時間和日期差異

>[!TIP]
>
>這些計算顯示兩個日期之間的天數。 結果以天為單位顯示。 日期欄位上的時間戳也會被考慮在內，如果時間戳不匹配，則天數後跟小數。 如果任務已延遲完成，則天數將顯示為負值。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>請求修改視圖 </p>
   <p>計畫修改報表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問以修改報表</p> <p>編輯對篩選器、視圖、分組的訪問以修改視圖</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 計算同一對象上兩個日期欄位之間的時間和日期差異

例如，您可以計算任務的計畫完成日期與實際完成日期之間的差值。

![](assets/view-planned-actual-completion-dates-datediff-column-350x92.png)

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，按一下 **新建視圖**。

1. 按一下 **添加列** 並開始在 **在此列中顯示** 欄位，然後在清單中顯示時選擇它。

1. 按一下 **添加列** 並開始在 **在此列中顯示** 欄位，然後在清單中顯示時選擇它。

1. 按一下 **添加列**，然後按一下 **切換到文本模式**。

1. 懸停在文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼替換它：

   ```
   displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML
   ```

1. 按一下 **保存**，則 **保存視圖**。

## 計算對象上的欄位與父對象上的其他欄位之間的時間和日期差異

有關對象及其父項的清單，請參閱中的「瞭解對象的相互依賴關係和層次」部分 [瞭解Adobe Workfront的對象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。\
例如，您可以計算任務的計畫完成日期與其父任務或任務所在項目的計畫完成日期之間的差異。

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-350x184.png)

1. 轉到任務清單。
1. 從 **視圖** 下拉菜單，按一下 **新建視圖**。

1. 按一下 **添加列** 並開始在中鍵入「項目計畫完成日期」或「父項完成日期」 **在此列中顯示** 欄位，然後在清單中顯示時選擇它。

1. 按一下 **添加列** 並開始在 **在此列中顯示** 欄位，然後在清單中顯示時選擇它。

1. 按一下 **添加列**，然後按一下 **切換到文本模式**。

1. 懸停在文本模式區域上，然後按一下 **按一下可編輯文本**。
1. 刪除在中查找的文本 **文本模式** 框，並用以下代碼之一替換它：

   * 要顯示項目的計畫完成日期與任務的計畫完成日期之間的差異，請執行以下操作：

      ```
      displayname=Project Planned Completion - Task Planned Completion (Days)<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>valueformat=HTML
      ```

   * 要顯示父任務的計畫完成日期與任務的計畫完成日期之間的差異，請執行以下操作：

      ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion (Days)
      ```

1. 按一下 **保存**，則 **保存視圖**。
