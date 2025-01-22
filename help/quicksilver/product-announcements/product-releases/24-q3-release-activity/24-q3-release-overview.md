---
title: 2024年第三季度版本總覽
description: 本頁提供2024年第三季度版本中包含的功能相關資訊。 這些增強功能預計會在整個季度內於生產環境中提供。
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: 552e97c427e618f299b55a2eab5868c7b90a4156
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 0%

---

# 2024年第三季度版本總覽

本頁提供2024年第三季度版本中包含的功能相關資訊。 這些增強功能預計會在整個季度內於生產環境中提供。

即時24.7發行網路研討會已取消，但您仍可以[在這裡](https://video.tv.adobe.com/v/3430532/%20)觀看24.7功能的影片示範。

<span class="preview">週期外功能（在2024年第三季度發行日期之前發佈到生產環境的功能）會以黃色標示。</span>

>[!IMPORTANT]
>
>23.3版本包含將您的組織移至每月版本的選項。 因此，Workfront已變更版本的編號方案，以說明每月和每季的發行追蹤。 第一個數字代表年份，第二個數字代表發行月份。 範例： 2024年4月版本的讀取為24.4。
>
>除非另有指定，否則每月和每季發行計畫於每月第二整週的星期四提供。
>
>| 每月發行 | 每季發行 |
>|----|----|
>| <ul><li>24.5 （2024年5月16日）</li><li>24.6 （2024年6月13日）</li><li>24.7 （2024年7月18日）</li></ul> | <ul><li>24.7 （2024年7月18日）</li></ul> |
>
>如需快速發行程式的詳細資訊，請參閱[啟用或停用快速發行程式](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。

## Adobe Workfront增強功能

* [管理員增強功能](#administrator-enhancements)
* [Financial Management增強功能](#financial-management-enhancements)
* [整合增強功能](#integration-enhancements)
* [專案增強功能](#project-enhancements)
* [校訂增強功能](#proofing-enhancements)
* [資源管理增強功能](#resource-management-enhancements)
* [其他增強功能](#other-enhancements)

### 管理員增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">發行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">商業規則現已可用</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>管理員現在可以在Workfront的設定區域中新增商業規則。</p>
                        <p>商業規則可讓您套用驗證至Workfront物件，並防止使用者在滿足某些條件時建立、編輯或刪除物件。 規則是使用與自訂表單中計算欄位類似的公式來建置。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年7月4日</p>
                            </li>
                            <li>
                                <p>適用於所有客戶的生產版本：搭配24.7版（2024年7月18日）</p>
                            </li>
                        </ul>
                        <p><i>僅適用於新Ultimate計畫中的組織。</i></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">自訂表單設計工具通常可在Adobe Workfront中使用</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>在24.7版中，表單設計人員將可正式使用，並成為在Adobe Workfront中建立和編輯自訂表單的預設體驗。 當您建立新的自訂表單或開啟現有的表單時，您將會看到表單設計工具的畫布樣式工作區。</p>
                        <p>此版本後，您將無法再選擇回覆至舊版表單產生器。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年6月19日</p>
                            </li>
                            <li>
                                <p>適用於所有客戶的生產版本：搭配24.7版（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">在具有環境升級的Workfront環境之間移動物件</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>環境升級可讓您將物件從一個Workfront環境移動到另一個環境，例如從沙箱環境移動到生產環境。 您可以設定及測試物件，而不會對貴組織的資料和記錄造成任何風險。 然後，您就可以將這些物件移至生產環境，而無需重新設定，從而節省時間和精力。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>適用於所有客戶的生產版本：搭配24.6版（2024年6月13日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">在自訂表單設計工具中共用自訂表單和自訂欄位</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>您現在可以在新的表單設計工具中共用自訂表單和自訂欄位。 這可讓自訂表單的使用者之間有更多共同作業。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年6月6日</p>
                            </li>
                            <li>
                                <p><span class="preview">所有客戶的生產版本： 6月13日</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">從欄位區域新增自訂欄位</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>您現在可以直接從Workfront中的欄位區域新增自訂欄位或Widget，而無需開啟自訂表單來建立欄位。 這可讓您快速建立可重複使用的自訂欄位。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年6月6日</p>
                            </li>
                            <li>
                                <p>適用於所有客戶的生產版本：搭配24.7版（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">表單設計工具上可用的多重選取下拉式欄位型別</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>為協助您更輕鬆地定義下拉式欄位，我們已將多選下拉式欄位新增到自訂表單設計工具。 此欄位型別可讓使用者從下拉式清單中選擇多個選項。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年6月4日</p>
                            </li>
                            <li>
                                <p><span class="preview">適用於所有客戶的生產： 2024年6月4日</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### Financial Management增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">發行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">專案與任務可用的可記帳與不可記帳費用欄位</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>為了幫助您更輕鬆地檢視費用型別，在專案和工作中，費用被分成可記帳和不可記帳費用。 下列欄位可供您新增至檢視和報表：</p>
                        <ul>
                            <li><p>規劃可計費費用成本</p></li>
                            <li><p>計畫非可開立帳單費用成本</p></li>
                            <li><p>實際不可開立帳單的費用成本</p></li>
                            <li><p>實際不可開立帳單的費用成本</p></li>
                        </ul>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年5月10日</p>
                            </li>
                            <li>
                                <p><span class="preview">適用於所有客戶的生產： 2024年5月10日</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### 整合增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">發行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        適用於Experience Manager Assets和Assets Essentials的<a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront改善</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>我們已針對Experience Manager Assets與Assets Essentials整合的Workfront進行下列改善：</p>
                        <ul>
                            <li><p>整合現在支援GCP作為雲端服務提供者。 先前已支援AWS和Azure。</p></li>
                            <li><p>透過整合傳送至Experience Manager的檔案大小限制已提高至30 GB。 先前的限製為5 GB。</p></li>
                        </ul>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年6月27日</p>
                            </li>
                            <li>
                                <p>適用於所有客戶的生產：24.7版（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### 專案增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">發行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">從標題或詳細資訊區段編輯任務和問題認可日期和條件</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>為了讓您更輕鬆地更新任務和問題，我們現在新增了提交日期和條件欄位，作為選項以新增到任務和問題標題和版面配置範本中的詳細資訊區段。 當使用者被指派給修改的版面配置範本時，他們現在可以從頁面的標題或詳細資訊區段更新這些欄位。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年5月30日</p>
                            </li>
                            <li>
                                <p>快速發行生產：24.6版（2024年6月13日）</p>
                            </li>
                            <li>
                                <p>適用於所有客戶的生產版本：搭配24.7版（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">更多相關指派已新增至新任務工作流程</a></p>
                        [！BADGE In Production for Fast Release ]{type=Positive}
                        <p>將任務新增至專案和專案任務清單時，我們已將相同功能新增至「新增任務」方塊的「工作總攬」欄位，以提供更相關的智慧指派。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年2月13日</p>
                            </li>
                            <li>
                                <p>快速發行生產：第24.5發行版本（2024年5月16日）</p>
                            </li>
                        </ul>
                    <p><i>此功能已從「預覽」和「快速發行產品」中移除。</i></p>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">更多相關的智慧指派</a></p>
                        [！BADGE In Production for Fast Release ]{type=Positive}
                        <p>我們已變更Workfront用來計算及建議智慧型任務指派的演演算法。 新演演算法適用於Workfront中指派任務的以下區域：任務清單、任務標題中的「工作」區域、「首頁」和「摘要」面板。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年12月21日</p>
                            </li>
                            <li>
                                <p>快速發行生產：第24.5發行版本（2024年5月16日）</p>
                            </li>
                        </ul>
                    <p><i>此功能已從「預覽」和「快速發行產品」中移除。</i></p>
                    </td>
                 </tr>
           </tbody>
        </table>

### 校訂增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">發行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">案頭校訂檢視器的安全性更新</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>Workfront Proof Desktop Proofing Viewer 2.1.35安全性更新針對舊版中已發現的弱點提供安全性錯誤修正。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年7月4日</p>
                            </li>
                            <li>
                                <p><span class="preview">適用於所有客戶的生產： 2024年7月4日</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### 資源管理增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">發行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">休假現在反映在工作負載平衡器</a>中</p>
                        [！BADGE In Production ]{type=Informative}
                        <p>為了在任務的主要受指派人排程休假時順暢地調整工作，現在重新計算專案時間表時，工作負載平衡器會重新分配時數給主要和次要使用者。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年6月6日</p>
                            </li>
                            <li>
                                <p>適用於所有客戶的生產版本：搭配24.7版（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### 其他增強功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">發行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">產品內指南的後端變更</a></p>
                        <p>我們將在未來幾週針對產品內指南實施技術變更。 雖然我們已嘗試將此轉換的影響降至最低，但有些使用者可能會遇到先前看過的指南。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>適用於所有客戶的生產：逐步推進至2024年8月中旬</p>
                            </li>
                         </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">現在更多Workfront組織可使用Adobe統一體驗</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>為了讓組織能夠存取Adobe統一體驗的各項優點，我們已經開始為現有的Workfront客戶提供這項功能。 </p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年6月20日</p>
                            </li>
                            <li>
                                <p>指定客戶的生產：搭配24.7版（2024年7月18日）</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">AdobeUnified Shell正在分階段推出。 其他組織將加入AdobeUnified Shell 24.10和25.1版本。 </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">說明按鈕已從主要導覽列移除</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>為了統一不在Unified Shell上的使用者體驗，已移除主要導覽列上的「說明」按鈕。 此按鈕未提供給Unified Shell的使用者，已連結至Workfront檔案，並且備有提供給主功能表中所有使用者使用的類似「說明」按鈕。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年6月6日</p>
                            </li>
                            <li>
                                <p>適用於所有客戶的生產版本：搭配24.7版（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">改善物件存取受限使用者的UI體驗</a></p>
                        [！BADGE In Production ]{type=Informative}
                        <p>當使用者無權存取物件時，使用者將在Workfront中顯示物件名稱的任何位置看到「無權存取」。 此改善的體驗也適用於Workfront API。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2024年3月27日</p>
                            </li>
                            <li>
                                <p>快速發行生產：第24.5發行版本（2024年5月16日）</p>
                            </li>
                            <li>
                                <p>每季發行生產：24.7版（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        在2024年第三季時間範圍內<a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">外觀和感覺更新</a></p>
                        <p>在2024年第三季時間範圍內，對Adobe Workfront應用程式的各個區域外觀和感覺進行了小幅更新。 檢閱特定發行日期的個別發行說明。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本：在整個2024年第三季度版本時間範圍內</p>
                            </li>
                            <li>
                                <p><span class="preview">生產版本：檢閱特定日期的發行說明</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>

## 公告

### Workfront Fusion增強功能

Workfront Fusion中的新功能可在2024年第三季度發行排程之外的步調中用於「生產」環境。 如需最新功能的詳細資訊，請參閱[Adobe Workfront Fusion發行活動](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)。

### Workfront Scenario Planner增強功能

此版本中目前沒有Scenario Planner更新。 在有更新可用時，此區域將會更新。

### Workfront Proof增強功能

此版本目前沒有Workfront Proof更新。 在有更新可用時，此區域將會更新。

### Workfront目標增強功能

此版本中目前沒有Workfront目標更新。 在有更新可用時，此區域將會更新。

### API 18版

針對API版本18，我們已修改一些資源和端點。 有些變更支援新功能，有些則讓您更輕鬆地透過API使用可用資訊。

如需新增和更新的詳細資訊，請參閱[ API 18](/help/quicksilver/wf-api/api/new-api-version-18.md)版的新增功能。

如需API版本的資訊，請參閱[API版本設定與支援排程](/help/quicksilver/wf-api/api/api-version-support-schedule.md)。

### Workfront 維護更新

如需2024年第三季期間所進行維護更新的相關資訊，請參閱[Workfront維護更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)。

### 訓練更新

探索每個Adobe Workfront產品版本的學習計畫、學習路徑、影片和指南的最新更新。 如需詳細資訊，請參閱[WorkfrontTutorials頁面](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html)的「新增功能」一節。
