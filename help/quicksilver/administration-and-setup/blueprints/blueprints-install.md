---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 安裝Blueprint
description: 您可以在生產環境或沙箱環境中安裝Blueprint。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 安裝Blueprint

您可以在生產環境或沙箱環境中安裝Blueprint。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃</strong></td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 授權</strong></td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置</strong></td> 
   <td> <p>[!UICONTROL系統管理員]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 應在何處安裝Blueprint? {#where-should-i-install-a-blueprint}

您可以在下列任何環境中安裝您的套件：

<table style="table-layout:auto">
        <tr>
        <td><strong>生產</strong></td>
        <td>生產是您的即時環境。</td>
    </tr>
    <tr>
        <td><strong>Sandbox 預覽</strong></td>
        <td>沙箱預覽是測試環境，可作為即時環境的復本，並由Workfront每週末重新整理。 所有支援套件都可存取沙箱預覽。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">此 [!DNL Adobe Workfront] 預覽沙箱環境</a>.</td>
    </tr>
    <tr>
        <td><strong>沙箱1和2</strong></td>
        <td>「自訂重新整理沙箱」是個別的測試環境，由您手動重新整理。 取得自訂重新整理沙箱需額外付費。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">此 [!DNL Adobe Workfront] 自訂重新整理沙箱環境</a>.</td>
    </tr>
</table>

>[!TIP]
>
>建議您先在沙箱環境中安裝Blueprint。 如此一來，您便可以測試Blueprint的內容，確保內容非常適合您的組織，而無須變更即時資料。

>[!NOTE]
>
>某些藍圖僅可用於在預覽環境中安裝，以用於測試。 如果您在生產環境、沙箱1或沙箱2中存取僅限預覽的內容，安裝按鈕不會作用中，您可能會看到警告訊息。\
>此外，即使您在預覽環境中，存取僅限預覽的內容時，環境切換功能也會受到限制。

## 安裝Blueprint

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 藍圖]**.
1. 找到您要安裝的藍圖。 您可以依使用案例、成熟度層級、安裝狀態，以及右側的類型進行篩選。
1. （選用）按一下 **[!UICONTROL 詳細資料]** 來了解Blueprint的運作方式。
1. 按一下 **[!UICONTROL 安裝]**.
1. 選擇在生產環境或沙箱環境上安裝。\
   如需詳細資訊，請參閱 [應在何處安裝Blueprint?](#where-should-i-install-a-blueprint) 一節。
1. 在 [!UICONTROL 設定] 頁面中，您可以選擇執行下列任一操作：

   * 照原樣安裝Blueprint。 對於不需要任何設定的Blueprint類型，此為唯一選項。 對於需要配置的Blueprint類型，您可以選擇立即安裝Blueprint並稍後進行配置。 按一下 **[!UICONTROL 按原樣安裝]**.
   * 在安裝前配置Blueprint，以了解需要配置的Blueprint。 進行配置選擇，然後按一下 **[!UICONTROL 安裝Blueprint]**.\

      如需詳細資訊，請參閱 [設定Blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
安裝完成後，消息將顯示已成功與Blueprint一起安裝的特定對象（如角色、團隊或組）的清單以及任何無法安裝的對象。

安裝Blueprint後，可能需要執行一些其他操作才能完全部署它。 如需詳細資訊，請參閱 [安裝Blueprint後要採取的動作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
