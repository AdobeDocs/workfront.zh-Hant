---
product-area: documents
navigation-topic: approvals
title: 檔案決定狀態概觀
description: 列出並解釋檔案決策狀態
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 30a10ed9-ae11-4ff1-a66c-58ea94fe9959
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/VESaWT8Xq7iU85LiRJCAL-tldNpXtdLqlTFxSqpK3Ok
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 6%

---

# 檔案決定狀態概觀

您可以直接在檔案清單中檢視檔案的狀態：

![檔案清單](assets/status-in-doc-list.png)中的狀態


可使用下列狀態：

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                 <tr>
                    <td>
                        待審閱</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                已通知檢閱者和核准者，但尚未開啟資產。
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        審閱中</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>至少有一個檢閱者已檢視該資產</p>
                            </li>
                            <li>
                                <p>至少有一個檢閱者尚未完成其檢閱</p>
                            </li>
                            <li>
                                <p>沒有指派給此資產的核准者</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        已審閱</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>所有稽核者已完成稽核</p>
                            </li>
                            <li>
                                <p>沒有指派給此資產的核准者</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>需要工作</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>所有核准和審查均已完成</p>
                            </li>
                            <li>
                                <p>至少有一位核准者已決定「需要工作」</p>
                                <p>其他核准者可能已作出「已核准變更」或「已核准」的決定
                            </li>
                        </ul>
                    </td>
                </tr>
                  <tr>
                    <td>已核准 (附帶變更)</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>所有核准和審查均已完成</p>
                            </li>
                            <li>
                                <p>至少有一位核准者已決定「已核准變更」</p>
                                <p>其他核准者可能已提供「已核准」的決定
                            </li>
                            <p>注意：如果您使用Frame.io整合進行檢閱和核准，則此選項無法使用。</p>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>已核准</p>
                    </td>
                    <td>
                        <ul>
                           <!--
                           <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            -->
                            <li>
                                <p>所有核准者可能已提供「已核准」的決定
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>



<!--



<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                 <tr>
                    <td>
                        Pending review</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                Reviewers and approvers have been notified, but have not yet opened the asset.
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        In review</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>At least one reviewer or approver has viewed the asset</p>
                            </li>
                            <li>
                                <p>At least one reviewer has not completed their review</p><p>Or</p>
                                <p>At least one approver has not made an approval decision</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        Reviewed</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                All reviews are complete
                            </li>
                            <li>
                                There are no approvers
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>Needs work</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>At least one approver has made a decision of "Needs work"</p>
                                <p>Other approvers may have given decisions of "Approved with changes" or "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
                  <tr>
                    <td>Approved with changes</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>At least one approver has made a decision of "Approved with changes"</p>
                                <p>Other approvers may have given decisions of "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>Approved</p>
                    </td>
                    <td>
                        <ul>
                            <li>
                                <p>All approvals and reviews are complete</p>
                            </li>
                            <li>
                                <p>All approvers may have given decisions of "Approved"
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>


-->
