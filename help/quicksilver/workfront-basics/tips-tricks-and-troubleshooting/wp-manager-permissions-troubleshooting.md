---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Workfront校樣管理器權限疑難解答
description: 在中可用的權限配置檔案 [!DNL Adobe] Workfront的校對用戶包括管理員、主管和經理。
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] 校樣管理器] 權限疑難解答

以下是中提供的權限配置檔案 [!DNL Adobe Workfront] 對於校對用戶：

* [!UICONTROL 管理員]
* [!UICONTROL 主管]
* [!UICONTROL 經理]

<!--For detailed information about these options and how to configure them, see .-->

授予用戶時 [!UICONTROL 經理] 權限，以下疑難解答資訊可用：

* **問題：** 具有 [!UICONTROL 經理] 權限無法查看其他用戶建立的校樣。 相反，他們看到 [!UICONTROL 拒絕訪問] 的上界。

   ![](assets/access-denied-350x161.png)

   **解決方案：** 具有 [!UICONTROL 經理] 必須將權限顯式添加到校樣中。 應始終通過 [!UICONTROL 高級校對選項] 窗口，應始終通過此選項添加用戶。

* **問題：** 具有 [!UICONTROL 經理] 權限不能向其他用戶建立的校樣添加校樣版本（他們可能會在文檔集中提交校樣，但版本不會連接到其他用戶建立的原始集）。\
   **解決方案：** 具有 [!UICONTROL 經理] 權限僅在具有 [!UICONTROL 經理] 權限：

   * 顯式添加到校樣
   * 設定為 [!UICONTROL 作者] （證明角色）

* **問題：** 具有 [!UICONTROL 經理] 權限無法編輯其他用戶對其不擁有或未建立的證據的評論。\
   **解決方案：** 如果用戶 [!UICONTROL 經理] 權限不擁有校樣，但它們應能夠編輯注釋，並將其添加為 [!UICONTROL 作者] 或 [!UICONTROL 版主])。\
   以下三種權限類型可在 [!DNL Workfront] 為 [!UICONTROL 計畫員]。 [!UICONTROL 工作人員]。 [!UICONTROL 請求者]。 [!UICONTROL 審閱者] 鍵入licenses。 系統管理員或用戶管理員 [!DNL Workfront] 可以編輯用戶的配置檔案並調整 [!DNL Workfront Proof] 權限。
