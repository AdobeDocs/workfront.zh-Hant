---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算已計畫的工作成本(BCWS)
description: 「計畫值」也稱為「已計畫的工作成本」(BCWS)，它是一個項目績效度量，表示在計算此度量時應完成的任務量。
author: Alina
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# 計算已計畫的工作成本(BCWS)

## 已計畫工作成本概覽(BCWS)

「計畫值」也稱為「已計畫的工作成本」(BCWS)，它是一個項目績效度量，表示在計算此度量時應完成的任務量。

Adobe Workfront計算項目和任務的已計畫工作成本(BCWS)。

在查看任務或項目上BCWS的值時，請考慮以下事項：

* Workfront根據您對項目的效能索引方法(PIM)的配置計算任務的BCWS。

   您可以配置項目以使用小時或成本計算PIM，並且BCWS也使用相同的值計算。

   有關配置BCWS的計算方式的資訊，請參見一節 [配置BCWS的計算方式](#configure-how-bcws-is-calculated) 這篇文章。

* Workfront通過添加項目上所有父任務和單個任務的所有BCWS值來計算項目的BCWS。

   子任務的值不會添加到項目的BCWS中。

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案的存取權</p> <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 配置BCWS的計算方式 {#configure-how-bcws-is-calculated}

通過配置項目的效能索引方法(PIM)的計算方式，可以配置BCWS的計算時間（小時）還是成本。

1. 前往專案，然後按一下 **專案詳細資料** 中。
1. 在 **金融** 區域，定位 **效能索引方法** 欄位並連按兩下以編輯。

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. 從下列選項中選取：

   | 選項 | 如何執行計算 |
   |---|---|
   | 基於小時 | Workfront使用任務的「計畫時數」計算BCWS。 |
   | 基於成本 | Workfront使用任務的「計畫成本」計算BCWS。 |


1. 按一下 **儲存變更**.

   項目任務的BCWS使用小時數或成本計算。

## 計算BCWS

Workfront使用以下公式計算任務或項目的已計畫工作成本(BCWS):

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

此計算中使用下列值：

| 使用的值 | 所用值的說明 |
|---|---|
| 計畫完成百分比 | 這是任務完成百分比，通過查看任務開始到今天之間所經過的時間量。 |
| 任務預算 | 這是任務的「計畫小時數」或「計畫成本」的值。 |

例如，如果今天是2月12日，而某個任務排程在2月10日到2月20日之間，則該任務應該在今天完成20%。 如果任務預算（計畫成本）為$10,000，則任務的BCWS為：

```
Task BCWS = 20% x $10,000 = $2,000
```

## 找到項目或任務的BCWS

通過將BCWS列添加到您的視圖中，您可以在報告或清單中查看已計畫的預算工作成本的值。

1. 轉到任務或項目清單。
1. 展開 **檢視** 選取 **新建視圖** 或 **自訂檢視**.

1. 按一下 **添加列**.
1. 在 **顯示於此欄中：** 欄位開始鍵入 **BCWS** 並按一下以在清單中顯示時選取。

   ![](assets/bcws-in-project-view.png)

1. 按一下 **保存視圖**.
1. 此 **BCWS** 欄位。
