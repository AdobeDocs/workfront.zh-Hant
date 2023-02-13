---
title: 刪除使用者
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 當使用者離開您的組織時，可從Workfront中移除該使用者，不過我們建議停用使用者，而非將其刪除。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# 刪除使用者

當使用者離開您的組織時，您可以從Adobe Workfront中移除該使用者。

>[!IMPORTANT]
>
>* 從系統中刪除用戶也會刪除與您可能希望保留的用戶相關聯的資訊。 我們建議停用使用者，而非將其刪除。 如需詳細資訊，請參閱 [停用或重新啟用使用者](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* 本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>從 [!DNL Adobe Admin Console] 停用 [!DNL Workfront]，但不會從 [!DNL Workfront].
>
>  如需在Adobe Admin Console中刪除使用者的指示，請參閱文章中的「永久刪除使用者」一節 [個別管理使用者](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 或聯絡您的Adobe Admin Console管理員。
>
>  如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員訪問級別。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>. </p> </li> 
     <li> <p><b>使用者</b> 在您的存取層級中設定 <b>編輯</b> 存取，使用 <b>建立</b> 和兩者中的至少一個 <b>使用者管理</b> 選項 <b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>在這兩個選項中，如果用戶 <b>管理員（群組使用者）</b> 啟用時，您必須是使用者所屬群組的群組管理員。</p> <p>如需 <b>使用者</b> 在存取層級中設定，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 刪除與停用使用者

停用使用者會導致下列情況發生：

* 如果Workfront校樣元件與您的Workfront帳戶相關聯，則同時移除使用者的Workfront和Workfront Proof授權。 如需Workfront Proof的詳細資訊，請參閱 [Workfront校樣](../../../workfront-proof/workfront-proof.md).
* 無法再為用戶分配工作。
* 無法再將使用者新增至更新。
* 無法再將使用者新增至團隊或群組。
* 對象不再能與用戶共用。
* 它們與以下對象的關聯保持不變：

   * 任務，問題，項目，產品組合
   * 儀表板

      >[!NOTE]
      >
      >如果您停用使用者，但無法再檢視與使用者相關聯的報表或控制面板，則可能需要更新 **以下列權限運行此報告：** 欄位。\
      >若要進一步了解，請參閱 [為何無法存取已停用使用者擁有的報表？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) 區段 [報表常見問題集](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 文章。

   * 文件
   * 更新
   * 時數

* 如果用戶已簽出文檔，則當您停用這些文檔時，文檔將保持簽出狀態。 只有Workfront管理員可以重新登入。 有關簽出文檔的詳細資訊，請參閱 [簽出文檔](../../../documents/managing-documents/check-out-documents.md).

刪除使用者會導致下列情況發生：

* 如果Workfront校樣元件與您的Workfront帳戶相關聯，請同時移除使用者的Workfront和Workfront Proof授權。 如需Workfront Proof的詳細資訊，請參閱 [Workfront校樣](../../../workfront-proof/workfront-proof.md).
* 無法再為用戶分配工作。
* 無法再將使用者新增至更新。
* 無法再將使用者新增至團隊或群組。
* 對象不再能與用戶共用。
* 刪除該用戶與以下對象的關聯：

   * 任務，問題，項目，產品組合
   * 儀表板

      >[!NOTE]
      >
      >您也會失去對包含與已刪除使用者相關聯的控制面板之自訂區段的存取權。\
      >若要進一步了解，請參閱 [如何存取包含已刪除使用者所擁有報表的控制面板？](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) 區段 [報表常見問題集](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) 文章。

   * 更新
   * 時數

      >[!NOTE]
      >
      >這些物件仍保留在Workfront中，但物件的擁有者現在空白。

* 如果用戶在全局導航欄的「文檔」區域下上傳了任何文檔，則文檔也會被刪除。
* 如果用戶已簽出他們擁有的文檔，並且這些文檔在主「文檔」區域（從主菜單訪問）中上載，則文檔將隨用戶一起刪除。 有關簽出文檔的詳細資訊，請參閱 [簽出文檔](../../../documents/managing-documents/check-out-documents.md).

如需停用使用者的詳細資訊，請參閱 [停用或重新啟用使用者](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

您可以一次永久刪除一個使用者，也可以同時永久刪除多個使用者。 刪除個別使用者時，必須先等待刪除程式完成，才能繼續執行Workfront中的其他活動。 同時刪除多個使用者的程式會在背景執行，因此您可以在刪除使用者時繼續使用Workfront。

## 刪除一或多個使用者

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **使用者**.
1. 選擇至少一個要刪除的用戶，按一下「更多」菜單 ![](assets/more-icon.png)，然後按一下 **刪除**.
1. 在出現的方塊中，按一下 **刪除** 以確認刪除。

   刪除使用者的程式會在背景執行，因此您可以在刪除使用者或使用者時繼續使用Workfront。

   視您刪除的使用者人數而定，程式可能需要幾分鐘甚至數小時。

   在Workfront中收到刪除使用者的確認函後，您可能會繼續在系統中看到這些使用者，直到刪除程式在背景完成為止。

   稍後，如果您發現一個或多個用戶未成功刪除，請嘗試一次刪除一個用戶。
