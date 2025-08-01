---
unique-page-id: 15695924
description: アカウントプロファイリングのランキングと調整 - Marketo ドキュメント - 製品ドキュメント
title: アカウントのプロファイリングのランキングと調整
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 73%

---

# アカウントのプロファイリングのランキングと調整 {#account-profiling-ranking-and-tuning}

アカウント・プロファイリングでは、理想的な顧客プロファイル（ICP）を識別し、ICP に基づいてデータベース内の企業をランク付けし、ICP インディケータ・データを [!UICONTROL &#x200B; 指定勘定科目 &#x200B;] として昇格された勘定科目に追加します。

>[!IMPORTANT]
>
>2025 年をもって、新規ユーザはアカウントプロファイリングを使用できなくなります。既存のユーザに対しては引き続き機能します。

## モデル結果 {#model-results}

成績別に分類された既知のアカウントがすべて表示されます。A は最も高いグレード、D は最も低いグレードです。

![](assets/results.png)

オプションではありますが、「自動的に昇格」チェックボックスはオンにすることをお勧めします。これにより、時間を大幅に節約できます。ただし、各アカウントを調べて[手動で追加する](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts)場合は、このチェックボックスをオフのままにしておきます。

<table>
 <tbody>
  <tr>
   <td><strong><span class="uicontrol">ランク</span></strong></td>
   <td>
    <div>
      理想的な顧客プロファイルに基づくアカウントランク。A は最適で、D は最も適していません。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">傾向</span></strong></td>
   <td>
    <div>
      非 ICP に基づいて選択したアカウントと比較した、コンバージョン率の推定増加。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">アカウント（%）</span></strong></td>
   <td>
    <div>
      このランクを持つモデル入力のアカウントの割合。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">モデル基準の割合</span></strong></td>
   <td>
    <div>
      このランクを持つモデル基準のアカウントの割合。
    </div></td>
  </tr>
 </tbody>
</table>

## モデルの調整 {#model-tuning}

「モデル」タブで、「**[!UICONTROL モデルを調整]**」ボタンをクリックします。

![](assets/two.png)

いくつかのタブから選択でき、詳細なカスタマイズが可能です。

![](assets/tuning-page.png)

**指標カテゴリ**

<table>
 <tbody>
  <tr>
   <td><strong><span class="uicontrol">コンプライアンス</span></strong></td>
   <td>
    <div>
      認定、コンプライアンス関連の職階／雇用。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">運用</span></strong></td>
   <td>
    <div>
      業務関連の職階／雇用。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">人事</span></strong></td>
   <td>
    <div>
      人事または給与計算ソフトウェア、人事関連の職階／雇用。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">エンジニアリング</span></strong></td>
   <td>
    <div>
      テクノロジー、フレームワーク、エンジニアリング関連の職階／雇用。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">セールス</span></strong></td>
   <td>
    <div>
      セールス向けソリューションとソフトウェア、セールス関連の職階／雇用。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">目的</span></strong></td>
   <td>
    <div>
      目的指標。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">IT</span></strong></td>
   <td>
    <div>
      ハードウェアおよびソフトウェアのソリューション、テクノロジー、IT 関連の職階／雇用。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">財務</span></strong></td>
   <td>
    <div>
      財務ソフトウェア、財務関連の職階／雇用。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">マーケティング</span></strong></td>
   <td>
    <div>
      マーケティング技術およびソフトウェア、マーケティング関連の職階／雇用。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">ビジネス</span></strong></td>
   <td>
    <div>
      Forbes リストや上場企業またはビジネスパートナーシップ。
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">カスタマーエクスペリエンスとリレーション</span></strong></td>
   <td>
    <div>
      カスタマーサクセスおよびカスタマーリレーション関連の職階／雇用。
    </div></td>
  </tr>
 </tbody>
</table>

各列の説明を表示するには、ツールヒントの上にカーソルを置きます。

![](assets/tool-tip.png)

[!UICONTROL ICP インジケータの追加 &#x200B;] ドロップダウンをクリックして、モデルにインジケータを追加します。

![](assets/add-icp.png)

「[!UICONTROL &#x200B; エクスポート &#x200B;]」ボックスをチェックすると、[!UICONTROL &#x200B; 指定勘定科目 &#x200B;] 詳細ページに ICP インディケータを表示でき、選択した ICP インディケータを [ 指定勘定科目フィルタ ](/help/marketo/product-docs/target-account-management/engage/account-filters.md) の制約として使用できます。

![](assets/export.png)

>[!NOTE]
>
>ICP 指標は、**[!UICONTROL 重点顧客のメンバー]**&#x200B;フィルターとトリガーに制約として含まれます。

[!UICONTROL &#x200B; インジケーターの重み付け &#x200B;] は、各インジケーターがモデルで受け取る重要度を制御するものです。

![](assets/weightage.png)

**[!UICONTROL モデルを更新]** をクリックして、これらの変更を有効にします。

![](assets/refresh-button.png)

（更新後に）モデルの調整が完了したら、「モデル結果」タブに戻り、「**[!UICONTROL 保存してランクを適用]**」をクリックします。

![](assets/ranks.png)
