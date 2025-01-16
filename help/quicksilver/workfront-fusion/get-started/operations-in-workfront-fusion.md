---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion中的作業
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的作業



>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [作業](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/operations-in-workfront-fusion.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

[!DNL Adobe Workfront Fusion]中的作業是由模組執行的作業。 基於追蹤目的，模組所執行的任何成功動作都是作業。

## 計算作業數量時的注意事項

* 一般而言，任何成功的動作步驟執行都會被視為作業。

* 案例中的第一個模組只會執行一次，而且一律會計為一項作業，即使未傳回套件組合亦然。

* 其餘模組執行的次數取決於它們必須處理的組合數量。  一個套件組合的一個模組執行為一項作業。 彙總模組則為例外，其計算為每一組處理中的套件組合進行一次作業。

* 作業在案例執行的[!UICONTROL 最終處理]階段計算。

* 下列&#x200B;**不是**&#x200B;計入為作業：

   * 任何篩選步驟。

   * 任何發生錯誤或中斷的動作。

   * 任何因不符合路由規則而不執行的路由，例如遞補或停用的路由。

   * 未執行的任何動作，可能是因為篩選器不允許資料通過，或因為案例因錯誤而停止。

## 作業限制

貴組織可能有每月營運限制。 這是根據貴組織購買的[!DNL Workfront]計畫。 [!UICONTROL Ultimate] [!DNL Workfront]計畫提供無限制的作業。

如果貴組織設有每月上限，則接近上限時會通知您。 如果您超過限制，[!DNL Workfront]將會連絡您的組織，以確保您的計畫符合您的需求。

## 檢視過去30天內執行的作業數目

您可以看到顯示所執行作業次數的圖形。 這些圖表可在下列位置使用：

* **組織儀表板**：整個組織使用的作業
* **團隊儀表板**：此團隊擁有的案例所使用的作業（僅限[!DNL Adobe Experience Cloud]）
* **案例詳細資訊頁面**：此案例使用的作業（僅限[!DNL Adobe Experience Cloud]）
