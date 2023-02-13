---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront Proof Manager權限疑難排解
description: 以下是 [!DNL Adobe] Workfront（校對用戶） — 編輯我。
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: ecb6928c946203b03a93cf5687fd53abf8e6a8f3
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] 校樣管理員] 權限疑難排解

以下是 [!DNL Adobe Workfront] 對於校對用戶：

* [!UICONTROL 管理員]
* [!UICONTROL 主管]
* [!UICONTROL 經理]

<!--For detailed information about these options and how to configure them, see .-->

授與使用者時 [!UICONTROL 管理員] 權限，則可使用下列疑難排解資訊：

* **問題：** 具有 [!UICONTROL 管理員] 權限無法檢視其他使用者建立的校樣。 相反地，他們會看到 [!UICONTROL 拒絕訪問] 螢幕。

   ![](assets/access-denied-350x161.png)

   **解決方案：** 具有 [!UICONTROL 管理員] 權限必須明確新增至校樣。 校樣應一律透過 [!UICONTROL 進階校對選項] 視窗和使用者，則一律應透過此選項新增。

* **問題：** 具有 [!UICONTROL 管理員] 權限無法將校樣版本添加到其他用戶建立的校樣中（他們可能會在文檔集中提交校樣，但版本不會連接到其他用戶建立的原始集）。\
   **解決方案：** 具有 [!UICONTROL 管理員] 只有具有 [!UICONTROL 管理員] 權限：

   * 明確新增至校樣
   * 設為 [!UICONTROL 作者] （證明角色）

* **問題：** 具有 [!UICONTROL 管理員] 權限無法編輯其他使用者未擁有或未建立的校樣的意見。\
   **解決方案：** 如果使用 [!UICONTROL 管理員] 校樣不屬於權限，但是校樣應該能夠編輯留言，並將留言新增為 [!UICONTROL 作者] (或 [!UICONTROL 協調者])。\
   這三種權限類型可在 [!DNL Workfront] for [!UICONTROL 計畫員], [!UICONTROL 工作人員], [!UICONTROL 請求者], [!UICONTROL 審核者] 鍵入許可證。 中的系統管理員或使用者管理員 [!DNL Workfront] 可以編輯使用者的設定檔並調整 [!DNL Workfront Proof] 權限。
