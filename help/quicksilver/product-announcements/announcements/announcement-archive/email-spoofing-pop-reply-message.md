---
content-type: reference
navigation-topic: announcements
title: 刪除電子郵件欺騙和POP回復
description: 我們在20.3版（目標為2020年8月）中，對Adobe Workfront傳送和接收電子郵件的方式進行了兩項變更。
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# 電子郵件欺騙和POP回復

我們在20.3版（目標為2020年8月）中，對Adobe Workfront傳送和接收電子郵件的方式進行了兩項變更。

## 來自Workfront的傳出電子郵件

為了增加電子郵件的成功傳送，我們將消除電子郵件的欺騙行為，這些電子郵件通常被標籤為垃圾郵件（請參閱電子郵件欺騙）。 來自Workfront的所有電子郵件都將從notifications@my.workfront.com傳送，包括自動警報和使用者與使用者的通訊。 來自Joan Harris的範例電子郵件在您電子郵件的發件者區域中如下所示：

![](assets/noreply.png)

*強烈建議您與IT團隊聯絡* 以確保不會因傳入電子郵件而封鎖來自notifications@my.workfront.com的電子郵件至您的系統。 您也可以參考 [配置防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) 以取得流量和電子郵件來源的IP位址詳細資訊。

## 傳入電子郵件對通知的回覆（POP回覆）

某些電子郵件通知可讓使用者透過電子郵件回覆，並將回覆複製至Workfront，作為Workfront系統中的留言回覆。 Workfront的系統管理員傳統上可以選擇提供自己的POP電子郵件伺服器來接收這些回覆，或使用內建的Workfront回覆系統。 自訂POP電子郵件伺服器選項在20.3版中正在移除。 所有設定為使用自訂伺服器的帳戶會自動轉換為使用原生Workfront電子郵件回覆系統。 系統管理員或其他Workfront使用者不需要執行任何動作。

直接從Workfront校樣系統傳送的電子郵件將不會變更。 您會繼續收到過去所收到的電子郵件。

若您有任何其他問題或疑慮，請聯絡 [Workfront支援團隊](https://one.workfront.com/s/support?language=en_US).
