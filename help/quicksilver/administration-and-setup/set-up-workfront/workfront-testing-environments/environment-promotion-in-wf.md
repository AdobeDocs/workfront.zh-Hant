---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 在Workfront中將物件從一個環境移動到另一個環境
description: 「環境升級」功能的目的是提供與組態相關的物件從一個環境移動到另一個環境的功能。 不支援移動異動物件的功能（只有少數例外）。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: 0cc1ab3a7412b7200ddab1a789ef5e9d86c3949f
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 2%

---

# 在Workfront環境之間移動物件的概觀（環境升級）

環境推進功能可讓您將物件從一個Workfront環境移動到另一個環境。 例如，您可以建立範本並在沙箱環境中進行設定，因為您知道進行的任何測試都不會影響組織的實際資料。 設定並測試範本後，您可以將其移至生產環境以準備使用。

此程式稱為「環境升級」。

您可以在Workfront中執行此程式，方法是建立要移動的物件套件，然後在新環境中安裝該套件。

* 如需在Workfront中執行此程式的特定指示，請參閱：

   * [建立或編輯環境升級套件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [安裝環境升級套件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* 如需透過Workfront API執行此程式的指示，請參閱[使用 [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md)在 [!DNL Workfront] 環境之間移動物件。

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3429735/){target=_blank}

## 環境推進的支援物件

環境推進功能的用意是提供與組態相關的物件從一個環境移動到另一個環境的功能。 這些是可設定的物件，例如專案、團隊或自訂表單。

由於環境推進會處理物件組態，因此不會包含異動物件（經常變更或高度依賴使用案例的物件）。 異動物件的範例包括檔案、問題、請求、更新和校訂決定。

* [工作物件](#work-objects)
* [報表物件](#reporting-objects)
* [自訂資料物件](#custom-data-objects)
* [組織物件](#organization-objects)
* [其他組態物件](#other-configuration-objects)


### 工作物件

| 可升級的物件 | 包含的可升級連結物件 |
| --- | --- |
| 專案（專案） | 專案<br>任務<br>指派<br>前置任務<br>公司<br>覆寫率<br>群組<br>角色<br>團隊<br>核准程式<br>核准路徑<br>核准步驟<br>步驟核准者<br>排程<br>非工作日<br>佇列定義<br>佇列主題群組<br>佇列主題<br>路由規則<br>里程碑路徑<br>里程碑<br>小時型別<br>資源池<br>類別<br>類別引數<br>引數<br>參陣列<br>引數選項<br>類別顯示邏輯 |
| 範本(TMPL) | 範本<br>範本任務<br>範本任務指派<br>範本任務前置任務<br>公司<br>覆寫率<br>群組<br>角色<br>團隊<br>核准程式<br>核准路徑<br>核准步驟<br>步驟核准者<br>排程<br>非工作日<br>佇列定義<br>佇列主題群組<br>佇列主題<br>路由規則<br>里程碑路徑<br>里程碑<br>小時型別<br>資源池<br>類別<br>類別引數<br>引數<br>參陣列<br>引數選項<br>類別顯示邏輯 |

### 報表物件

| 可升級的物件 | 包含的可升級連結物件 |
| --- | --- |
| 版面配置範本(UITMPL) | 配置範本<br>儀表板<br>行事曆<br>行事曆區段<br>外部頁面<br>報表<br>篩選器<br>群組<br>檢視<br>引數<br>群組 |
| 控制面板(PTLTAB) | 儀表板<br>行事曆<br>行事曆區段<br>外部頁面<br>報表<br>篩選器<br>群組<br>檢視<br>引數 |
| 行事曆(CALEND) | 行事曆<br>行事曆區段 |
| 外部頁面(EXTSEC) | 外部頁面 |
| 報告(PTLSEC) | 報表<br>篩選器<br>群組<br>檢視<br>引數 |
| 篩選器(UIFT) | 篩選器<br>引數 |
| 分組(UIGB) | 群組<br>引數 |
| 檢視(UIVW) | 檢視<br>引數 |

### 自訂資料物件

| 可升級的物件 | 包含的可升級連結物件 |
| --- | --- |
| 類別(CTGY) | 類別<br>類別引數<br>引數<br>引數群組<br>引數選項<br>類別顯示邏輯<br>群組 |
| 引數（引數） | 引數<br>引數選項 |
| 引數群組(PGRP) | 參數群組 |

### 組織物件

| 可升級的物件 | 包含的可升級連結物件 |
| --- | --- |
| 群組（群組） | 群組<br>子群組（最多5個層級） *<br>類別<br>類別引數<br>引數<br>引數群組<br>引數選項<br>類別顯示邏輯 |
| 角色(ROLE) | 角色 |
| 團隊（團隊） | 團隊<br>群組 |
| 公司(CMPY) | 公司<br>覆寫率<br>類別<br>類別引數<br>引數<br>引數群組<br>引數<br>類別顯示邏輯<br>群組 |
| Portfolio （連線埠） | Portfolio<br>程式<br>群組<br>類別<br>類別引數<br>引數<br>引數群組<br>引數選項<br>類別顯示邏輯 |
| 方案(PRGM) | 程式<br>Portfolio<br>群組<br>類別<br>類別引數<br>引數<br>引數群組<br>引數選項<br>類別顯示邏輯 |

### 其他組態物件

| 可升級的物件 | 包含的可升級連結物件 |
| --- | --- |
| 核准程式(ARVPRC) | 核准程式<br>核准路徑<br>核准步驟<br>步驟核准者<br>角色<br>團隊<br>群組 |
| 時程表(SCHED) | 排程<br>非工作日<br>群組 |
| 里程碑路徑(MPATH) | 里程碑路徑<br>里程碑 |
| 週期性時程表(TSPRO) | 週期性時程表<br>小時型別 |
| 小時型別（小時） | 時數類型 |
| 費用型別(EXPTYP) | 費用類型 |
| 風險型別(RSKTYP) | 風險類型 |
| 資源集區(RSPL) | 資源集區 |
| 存取層級(ACSLVL) | 存取層級 |
| 費率卡(RTCRD) | 費率卡 |
| 位置/分類器(CLSF) | 位置/分類器 |
| 商業規則(BSNRUL) | 業務規則 |

\*目前無法使用

<!--

>[!NOTE]
>
>Actions (ignore, select existing, and create new) are available on the following objects:
>
>* Role
>* Team
>* Company
>* Group

-->

## 環境升級狀態

環境升級套件在建立時和準備在環境之間移動時會在多個狀態下進行。 您可以在Workfront內的套件清單或API回應(如果您使用Workfront API)中檢視這些狀態。

這些狀態包括：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>未組裝</td> 
   <td><p>此狀態會自動指派，代表已儲存但尚未組裝的封裝。 </p><p>使用者無法直接設定此狀態。</p></td> 
  </tr> 
  <tr> 
   <td>組裝</td> 
   <td><p>組裝物件時，會自動指定此狀態。 </p><p>組合是指識別要包含在封裝中的物件和子物件，並將這些物件及其資料加入封裝的自動化程式。</p><p>使用者無法直接設定此狀態。</p></td> 
  </tr> 
  <tr> 
   <td>草稿</td> 
   <td><p>此狀態會在元件流程結束時或建立空推進封裝時指派。</p><p>使用者可以將促銷活動套件移回此狀態。</p><p>處於此狀態時，升級套件無法安裝在任何環境中。</p></td> 
  </tr> 
  <tr> 
   <td>測試</td> 
   <td><p>此狀態可讓促銷活動套件安裝在任何預覽或自訂重新整理沙箱中。 處於此狀態時，無法在生產環境中安裝套件。</p></td> 
  </tr> 
  <tr> 
   <td>作用中</td> 
   <td><p>此狀態可讓促銷活動套件安裝在任何環境中，包括生產環境。</p><p>當封裝狀態設定為ACTIVE時，<code>publishedAt</code>日期會自動設定為要求目前的時間戳記。</p></td> 
  </tr> 
  <tr> 
   <td>已停用</td> 
   <td><p>此狀態用於隱藏先前使用的促銷活動套件，這些套件未來不會安裝至任何環境。</p><p>當套件處於此狀態時，無法將其安裝在任何環境中。</p><p>當封裝狀態設定為DISABLED時，<code>retiredAt</code>日期會自動設定為要求目前的時間戳記。</p><p>建議您不要使用<code>DELETE /package</code>端點來使用此狀態，因為此狀態是可擷取的，而且使用此封裝進行的任何部署都會保留安裝歷史記錄。</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLY_FAILED</td> 
   <td><p>如果ASSEMBLY階段失敗，則推進封裝會自動處於此狀態。</p><p>若要將封裝返回ASSEMBLING階段，您必須再次觸發組裝過程。</p><p>如需組裝套件的詳細資訊，請參閱文章建立或編輯環境升級套件中的<a href="https://experienceleague.adobe.com/zh-hant/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package">編輯或組裝現有套件</a>小節。</td> 
  </tr> 
  </tbody> 
</table>

## 資源

* 如需有關環境升級的常見問題集，請參閱[環境升級常見問題集](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-faq.md)
* 如需疑難排解建議，請參閱[環境升級疑難排解](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-troubleshooting.md)


