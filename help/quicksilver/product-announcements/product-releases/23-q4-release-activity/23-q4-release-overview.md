---
title: 2023年第四季版本總覽
description: 2023年第四季版本總覽
author: Becky
feature: Product Announcements
exl-id: 6c14bd61-60b1-49aa-84bd-d494a226d70e
source-git-commit: 73e6a62e4c4103d0a4dc7e3f58ddd68cbd145b8c
workflow-type: tm+mt
source-wordcount: '2695'
ht-degree: 0%

---

# 2023年第四季版本總覽

此頁面提供2023年第四季版本所含功能的相關資訊。 這些增強功能預計將在2023年10月26日和27日發行的23.10版本中，提供給所有客戶在生產環境中使用。

<!--
These enhancements will be included in the following releases:

>|Monthly release|Quarterly release|
>|----|----|
>|<ul><li>23.8 (August 31, 2023)</li><li>23.9 (September 28, 2023)</li><li>23.10 (October 26, 2023)</li></ul>| <ul><li>23.10 (Week of October 26, 2023)</li></ul>|
-->

23.10版本網路研討會是在2023年10月5日舉行。 您可以 [在此報名參加網路研討會以觀看隨選錄影](https://webinars.on24.com/adobe_workfront/whatsnewin2310?partnerref=releasenotes).

<span class="preview">非週期功能（在2023年第四季發行日期之前發佈到生產環境的功能）以黃色醒目提示。</span>

>[!IMPORTANT]
>
>23.3版本包含將您的組織移至每月版本的選項。 因此，Workfront正在變更版本的編號方案，以兼顧每月和每季的發行追蹤。
>
>* 如果您在 **快速發行（每月）** track，23.3之後的版本為 **23.8**，2023年8月31日。
> * 如果您在 **每季** 版本追蹤，23.3之後的版本為 **23.10**，2023年10月26日當週。
> 
> 每季發行將包含三個月發行的功能。 例如，23.10每季發行將包含23.8、23.9和23.10每月發行版本中的功能。
>
>每月和每季發行計畫於當月最後一個星期四提供。
>
>| 每月發行 | 每季發行 |
>|----|----|
>| <ul><li>23.8 （2023年8月31日）</li><li>23.9 （2023年9月28日）</li><li>23.10 （2023年10月26日）</li></ul> | <ul><li>23.10 （2023年10月26日起一週）</li></ul> |
>| <ul><li>無版本（2023年11月）</li><li>無版本（2023年12月）</li><li>24.1 （2024年1月）</li></ul> | <ul><li>24.1 （2024年1月）</li></ul> |
>
>如需快速發行流程的詳細資訊，請參閱 [啟用或停用快速發行程式](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront增強功能

* [管理員增強功能](#administrator-enhancements)
* [展示板增強功能](#boards-enhancements)
* [Financial Management增強功能](#financial-management-enhancements)
* [首頁增強功能](#home-enhancements)
* [整合增強功能](#integration-enhancements)
* [專案增強功能](#project-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">舊版授權模式客戶可用的校訂和檔案決策</a></p><p>[！BADGE In Production ]{type=Informative}</p>
                        <p>尚未轉換至新Adobe Workfront授權模式的舊版客戶，現在可以在單一報表中檢視每個使用者每月校訂/檔案決策數量的資料。 當您執行使用者決定報表時，即可使用此資料。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年10月12日</p>
                            </li>
                            <li>
                                <p><span class="preview">所有客戶的生產： 2023年10月12日</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>            
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">自訂表單的計算欄位現在可以使用$$USER萬用字元</a></p><p>[！BADGE In Production ]{type=Informative}</p>
                        <p>$$USER萬用字元現在可用於新表單設計工具的計算自訂欄位和外部查閱欄位中。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年10月5日</p>
                            </li>
                            <li>
                                <p>快速發行生產：第23.10發行版本</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">從外部API新增值選項至自訂表單</a></p>
                        <p>[！BADGE In Production ]{type=Informative}</p>
                        <p>新的欄位型別， <strong>外部查詢</strong>，現在可用於自訂表單設計工具。 當資料儲存在外部系統時，此欄位型別可讓您從外部API載入選項，並根據自訂表單中的其他欄位值進行篩選。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年9月14日</p>
                            </li>
                            <li>
                                <p>快速發行生產：23.9版</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### 展示板增強功能

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront展示板上現在提供子任務</a></p><p>[！BADGE In Production ]{type=Informative}</p><p>當您將已連線的卡片新增到Workfront任務的展示板時，任何現有的子任務都會匯入到卡片上。 此外，當您在已連線的卡片上建立子任務時，子任務會新增到Workfront任務中。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年10月12日</p>
                            </li>
                            <li>
                                <p>可提早存取展示板的生產環境：不適用</p>
                            </li>
                            <li>
                                <p>快速發行生產：不適用</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">對展示板和卡片上的使用者指派的增強功能</a></p><p>[！BADGE In Production ]{type=Informative}</p><p>現在提供增強功能，可新增彈性將使用者新增到Adobe Workfront面板中的面板和卡片。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月21日</p>
                            </li>
                            <li>
                                <p><span class="preview">適用於所有客戶的生產： 2023年8月24日</span>
                            </li> 
                       </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">在連線的卡片上新增檔案</a></p><p>[！BADGE In Production ]{type=Informative}</p><p>您現在可以在Adobe Workfront展示板上所連線的卡片上附加檔案。 您新增到卡片上的任何檔案都可在已連線任務或問題的檔案索引標籤上使用，且兩個區域都支援相同的檔案型別。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月21日</p>
                            </li>
                            <li>
                                <p>主機板搶先使用的生產日期： 2023年8月24日</p>
                            </li>
                            <li>
                                <p>快速發行生產：不適用</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">連線卡片上的可用檔案僅供檢視</a></p><p>[！BADGE In Production ]{type=Informative}</p><p>針對Adobe Workfront展示板上已連線的卡片，您現在可以檢視檔案，例如影像和PDF。 您可以在瀏覽器中預覽檔案或下載到您的電腦。 </p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月3日</p>
                            </li>
                            <li>
                                <p>主機板搶先使用的生產日期：2023年8月10日</p>
                            </li>
                            <li>
                                <p>快速發行生產：不適用</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">專案的面板檢視現在可針對問題使用</a></p><p>[！BADGE In Production ]{type=Informative}</p><p>您現在可以存取專案問題清單的展示板檢視。 Kanban展示板可協助您以比在清單中檢視更直觀的方式追蹤問題進度。 </p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月3日</p>
                            </li>
                            <li>
                                <p>可提早存取展示板的生產環境：不適用</p>
                            </li>
                             <li>
                                <p>快速發行生產：不適用</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">日期有效成本與記帳費率</a></p><p>[！BADGE In Production ]{type=Informative}</p>
                        <p>現在可針對Workfront中的公司、使用者和工作角色物件使用日期有效成本和計費率。 將日期有效費率套用至專案且將時數記錄至專案任務時，成本與收入會使用每個時段的指定費率計算。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年6月29日</p>
                            </li>
                            <li>
                                <p>快速發行生產：第23.10發行版本</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### 首頁增強功能

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">專案、任務和問題Widget的委派工作按鈕</a> </p><p>[！BADGE In Production ]{type=Informative}</p>
                        <p>作為舊首頁的常見功能，我們現在已將委派按鈕新增到「我的工作」、「我的任務」和「我的問題」Widget，以便您在外出時可以輕鬆委派工作。 請注意，必須在您的Workfront環境中啟用工作委派，按鈕才會出現。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年10月12日</p>
                            </li>
                            <li>
                                <p>快速發行生產：第23.10發行版本</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新首頁的新面板Widget</a> </p><p>[！BADGE In Production ]{type=Informative}</p>
                        <p>除了新首頁提供的工作管理選項，您現在可以在首頁上顯示展示展示板！</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年10月12日</p>
                            </li>
                            <li>
                                <p>快速發行生產：第23.10發行版本</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新的貢獻者預設登陸頁面：新首頁</a>  </p><p>[！BADGE In Production ]{type=Informative}</p>
                        <p>新首頁現在是貢獻者/請求者帳戶的預設登陸頁面。 這個新的預設首頁包含許多特別選取的Widget，以便最佳地讓貢獻者立即管理其工作。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年10月12日</p>
                            </li>
                            <li>
                                <p>快速發行生產：第23.10發行版本</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新首頁中的工作追蹤的變更 </a> </p>
                        <p>[！BADGE In Production ]{type=Informative}</p>
                        <p>根據使用者回饋，我們已移除頁面範圍時間範圍篩選器和摘要列，用於統計到期和完成的工作。 專案、任務和問題Widget各有內建的篩選功能，可讓您依個人情況自訂其範圍。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年9月13日<br /></p>
                            </li>
                            <li>
                                <p>快速發行生產：23.9版</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">我的工作Widget的新快速動作按鈕</a> </p>
                        <p>[！BADGE In Production ]{type=Informative}</p>
                        <p>「我的工作」小工具中已新增新的快速動作按鈕，進一步擴充了您直接從「新首頁」管理工作的能力。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年9月13日<br /></p>
                            </li>
                            <li>
                                <p>快速發行生產：23.9版</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>                
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新首頁的新篩選器選項</a> </p>
                        <p>[！BADGE In Production ]{type=Informative}</p>
                        <p>「新首頁」中的「我的工作」Widget現在提供新篩選器選項。 選項包括物件型別（任務、問題和請求）和狀態（未就緒、準備開始、處理和完成）的篩選器。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月17日<br /></p>
                            </li>
                            <li>
                                <p>快速發行生產：23.8版</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">新首頁的自訂術語支援</a> </p><p>[！BADGE In Production ]{type=Informative}</p>
                        <p>為了更妥善地滿足組織的獨特需求，「新首頁」現在會針對執行個體版面配置範本中定義的物件，使用自訂術語。 例如，如果您的Workfront執行個體中的「專案」物件已重新標籤為「促銷活動」，則我的專案Widget將會在「新首頁」中顯示為「我的促銷活動」。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月17日<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">適用於所有客戶的生產： 2023年8月31日</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">已針對已停用「新首頁」的帳戶移除「嘗試新首頁」按鈕</a> </p>
                        <p>[！BADGE In Production ]{type=Informative}</p>
                        <p>已停用「新首頁」的帳戶不再顯示「嘗試新首頁」按鈕。 系統管理員必須重新啟用新首頁，個別使用者才能使用按鈕嘗試新首頁。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月17日<br /></p>
                            </li>
                            <li>
                                <p>快速發行生產：23.8版</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-home-enhancements.md" class="MCXref xref" xrefformat="{para}">變更為新首頁預設Widget集</a> </p>
                        <p>[！BADGE In Production ]{type=Informative}</p>
                        <p>待辦事項Widget需要建立任務的許可權，現在僅會出現在為具有標準、計畫或工作授權型別的使用者設定的預設Widget中。 此外，Widget已從所有其他授權型別使用者的首頁自動移除。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月17日<br /></p>
                            </li>
                            <li>
                                <p>快速發行生產： 2023年8月17日</p>
                            </li>
                            <li>
                                <p>每季發行量： 2023年8月17日</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">增強將檔案傳送至SharePoint (GraphAPI)時的體驗</a></p><p>[！BADGE In Production ]{type=Informative}</p><p>我們已進行一些變更，以便在傳送檔案至您的SharePoint (GraphAPI)資料夾時更容易找到資料夾</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月24日<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">適用於所有客戶的生產： 2023年8月31日</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">升級為拖放檔案整合</a></p><p>我們做了一些增強功能，讓檔案拖放至連結資料夾時，能更清晰易懂且移除使用者錯誤。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月24日<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">適用於所有客戶的生產： 23.10版之後</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">新檔案核准</a> </p><p>[！BADGE In Production ]{type=Informative}</p>
                        <p>在這個版本中，除了新功能外，核准流程已經針對建立核准和核准/稽核檔案進行了簡化。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年10月12日<br /></p>
                            </li>
                            <li>
                                <p>快速發行生產：第23.10發行版本</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                        <p><span style="color: #ff0000;">此功能屬於分階段發行，目前僅供特定客戶使用。</span></p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">任務清單即時更新</a> </p>
                        <p>[！BADGE In Production]{type=Informative}</p>
                        <p>工作清單現在會即時更新。 對任務所做的變更會在任務清單中更新，因此檢視任務清單的使用者可以在不重新整理頁面的情況下看到變更。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本：不適用<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">所有客戶的生產：分階段推出，於2023年10月19日完成</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">將新問題新增到專案時更新設計</a> </p>
                        <p>[！BADGE In Production ]{type=Informative}</p>
                        <p>此更新已在23.3版本中公告。</p>
                        <p>我們已更新「新問題」方塊，在向專案提交新問題時會顯示此方塊。 現在，介面符合新請求方塊，在將新請求提交到請求佇列時顯示。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年7月26日<br /></p>
                            </li>
                            <li>
                                <p>快速發行生產：23.8版</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">表單上計算欄位的動態重新計算</a></p>
                        <p>[！BADGE In Production ]{type=Informative}</p>
                        <p>現在當頁面上任何表單的相依值被修改時，附加到物件的表單上的計算欄位會動態地即時重新計算。 這可讓您在不儲存表單的情況下檢視更新後的結果。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月17日<br /></p>
                            </li>
                            <li>
                                <p>快速發行生產：23.8版</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-project-enhancements.md" class="MCXref xref" xrefformat="{para}">在子週期性任務上設定沒有指派的簡單期間型別的計畫時數</a></p>
                        <p>[！BADGE In Production ]{type=Informative}</p>
                        <p>我們對計畫時數分配至無指派和簡單期間型別的週期性任務的方式進行了更改。 現在，當您在具有「簡單期間型別」且沒有指派的新遞回任務上設定計畫時數時，時數也會分配給個別遞回。 在此變更之前，當父任務被取消指派時，不會為個別循環儲存時數。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年8月17日<br /></p>
                            </li>
                            <li>
                                <p>快速發行生產：23.8版</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-other-enhancements.md" class="MCXref xref" xrefformat="{para}">投稿人主要功能表變更</a> </p><p>[！BADGE In Production ]{type=Informative}</p>
                        <p>為了更妥善地通知參與者/請求者有關付費Workfront授權型別的可用功能，他們現在可以看到主選單中的所有可用選項。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本： 2023年10月12日</p>
                            </li>
                            <li>
                                <p>快速發行生產：第23.10發行版本</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版本</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md" class="MCXref xref" xrefformat="{para}">新的評論體驗測試版增強功能</a> </p>
                        <p>[！BADGE In Production ]{type=Informative}</p>
                        <p>「更新」區段的增強功能將在2023年第四季發行時間範圍內提供評論體驗Beta版。 這些增強功能將在2023年第四季度版本（2023年10月）的生產環境中提供給所有客戶。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本：在整個2023年第四季版本時間範圍<br /></p>
                            </li>
                            <li>
                                <p>快速發行生產：從23.8版開始</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版（除非另有指定）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md" class="MCXref xref" xrefformat="{para}">新的畫布控制面板Beta版增強功能</a> </p>
                        <p>[！BADGE In Production ]{type=Informative}</p>
                        <p>畫布控制面板的增強功能將在2023年第四季度發行時間範圍內提供，作為進行中Beta版的一部分。 這些增強功能將在2023年第四季度版本（2023年10月）的生產環境中提供給所有客戶。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本：在整個2023年第四季版本時間範圍<br /></p>
                            </li>
                            <li>
                                <p>快速發行生產：從23.8版開始</p>
                            </li>
                            <li>
                                <p>每季發行生產：23.10版（除非另有指定）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">2023年第四季時間範圍內的外觀和感覺更新</a></p><p>[！BADGE In Production ]{type=Informative}</p><p>在2023年第四季時間範圍內，對Adobe Workfront應用程式的各個區域外觀和感覺進行了小幅更新。 檢閱特定發行日期的個別發行說明。</p>
                    </td>
                    <td><p><b>將於下列日期提供：</b></p>
                        <ul>
                            <li>
                                <p>預覽版本：在整個2023年第四季版本時間範圍</p>
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

Workfront Fusion中的新功能可在2023年第四季發行排程之外的步調中推出。 如需最新功能的詳細資訊，請參閱 [Adobe Workfront Fusion發行活動](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Workfront Scenario Planner增強功能

此版本中目前沒有Scenario Planner更新。 在有更新可用時，此區域將會更新。

### Workfront校訂增強功能

此版本目前沒有Workfront校訂更新。 在有更新可用時，此區域將會更新。

### Workfront目標增強功能

此版本中目前沒有Workfront目標更新。 在有更新可用時，此區域將會更新。

### API 17版

API第17版已於2023年10月12日發行。 針對API版本17，我們已修改一些資源和端點。 有些變更支援新功能，有些則讓您更輕鬆地透過API使用可用資訊。

如需新增功能和更新的詳細資訊，請參閱 [API 17版的新增功能](/help/quicksilver/wf-api/api/new-api-version-17.md).

如需API版本的詳細資訊，請參閱 [API版本設定和支援排程](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront 維護更新

如需22.3版本期間所進行維護更新的相關資訊，請參閱 [Workfront維護更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### 訓練更新

探索每個Adobe Workfront產品版本的學習計畫、學習路徑、影片和指南的最新更新。 如需詳細資訊，請參閱 [WorkfrontTutorials頁面](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).

### 即將從Workfront移除的功能

下列功能即將從Workfront中移除：

#### 使用23.10棄用Proof行動應用程式

我們將在23.10版本中正式淘汰Proof行動應用程式。 一般Workfront行動應用程式已透過新校訂功能增強(如需詳細資訊，請參閱Workfront行動增強功能下的發行說明)，建議使用者儘快開始使用以進行校訂工作。

請注意，Workfront行動應用程式需要Workfront登入。 外部使用者和來賓可以繼續使用校訂應用程式進行校訂工作；但是，它不再受支援，並將在23.10中變得無法使用。

#### 已刪除帳戶不使用的工作流程

對於從未在Adobe Workfront面板中建立工作流程的帳戶，自2023年10月11日起，工作流程區域已從面板控制面板中移除。 有使用工作流程的帳戶仍然可以存取它們。增強的Scrum功能將在未來版本中解決。

<!-- HTML you might need

New table

### add product area name

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="ADD LINK" class="MCXref xref" xrefformat="{para}">Title</a><span style="color: #ff0000;"> New in Preview!</span></p>
                        <p>Body</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release:<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

New row for table 

<tr>
  <td>
    <a href="ADD%20LINK">Title</a> New in Preview!
    <p>Body</p>
  </td>
  <td>
    <p><strong>Available on these dates:</strong></p>
    <ul>
      <li>
        <p>Preview release:</p>
      </li>
      <li>
        <p>Production release:</p>
      </li>
    </ul>
  </td>
</tr>


New in preview, prod, and coming soon text

<span style="color: #ff0000;"> New in Preview!</span>
<span style="color: #ff0000;"> New in Production!</span>
<span style="color: #ff0000;"> Coming soon!</span>

Badge for available in Fast Release

[!BADGE In production for Fast Release ]{type=Positive}
[!BADGE In production ]{type=Informative}



Test for boards early access stuff

Production release for early opt-in: March 2, 2023 This feature is available in Production only through the early feature opt-in for Workfront Boards.

Production release for all customers: With the 23.2 release

-->
