---
unique-page-id: 15695924
description: アカウントプロファイリングのランキングと調整 - Marketo ドキュメント - 製品ドキュメント
title: アカウントのプロファイリングのランキングと調整
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '381'
ht-degree: 100%

---

# アカウントのプロファイリングのランキングと調整 {#account-profiling-ranking-and-tuning}

アカウントプロファイリングは、理想的な顧客プロファイル（ICP）を特定し、ICP に基づきデータベース内の企業をランク付けし、ICP 指標データを重点顧客として昇格されたアカウントに追加します。

## モデル結果 {#model-results}

成績別に分類された既知のアカウントがすべて表示されます。A は最も高いグレード、D は最も低いグレードです。

![](assets/results.png)

オプションではありますが、「自動的に昇格」チェックボックスはオンにすることをお勧めします。これにより、時間を大幅に節約できます。ただし、各アカウントを調べて[手動で追加する](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts)場合は、このチェックボックスをオフのままにしておきます。

<table> 
 <tbody> 
  <tr> 
   <td><strong>ランク</strong></td> 
   <td> 
    <div>
      理想的な顧客プロファイルに基づくアカウントランク。A は最適で、D は最も適していません。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>傾向</strong></td> 
   <td> 
    <div>
      非 ICP に基づいて選択したアカウントと比較した、コンバージョン率の推定増加。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>アカウント（%）</strong></td> 
   <td> 
    <div>
      このランクを持つモデル入力のアカウントの割合。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>モデル基準の割合</strong></td> 
   <td> 
    <div>
      このランクを持つモデル基準のアカウントの割合。 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## モデルの調整 {#model-tuning}

「モデル」タブで、「モデルを調整」ボタンをクリックします。

![](assets/two.png)

いくつかのタブから選択でき、詳細なカスタマイズが可能です。

![](assets/tuning-page.png)

**指標カテゴリ**

<table> 
 <tbody> 
  <tr> 
   <td><strong>コンプライアンス</strong></td> 
   <td> 
    <div>
      認定、コンプライアンス関連の職階／雇用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>運用</strong></td> 
   <td> 
    <div>
      業務関連の職階／雇用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>人事</strong></td> 
   <td> 
    <div>
      人事または給与計算ソフトウェア、人事関連の職階／雇用。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>エンジニアリング</strong></td> 
   <td> 
    <div>
      テクノロジー、フレームワーク、エンジニアリング関連の職階／雇用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>セールス</strong></td> 
   <td> 
    <div>
      セールス向けソリューションとソフトウェア、セールス関連の職階／雇用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>目的</strong></td> 
   <td> 
    <div>
      目的指標。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      ハードウェアおよびソフトウェアのソリューション、テクノロジー、IT 関連の職階／雇用。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>財務</strong></td> 
   <td> 
    <div>
      財務ソフトウェア、財務関連の職階／雇用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>マーケティング</strong></td> 
   <td> 
    <div>
      マーケティング技術およびソフトウェア、マーケティング関連の職階／雇用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>ビジネス</strong></td> 
   <td> 
    <div>
      Forbes リストや上場企業またはビジネスパートナーシップ。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>カスタマーエクスペリエンスとリレーション</strong></td> 
   <td> 
    <div>
      カスタマーサクセスおよびカスタマーリレーション関連の職階／雇用。
    </div></td> 
  </tr> 
 </tbody> 
</table>

各列の説明を表示するには、ツールヒントの上にカーソルを置きます。

![](assets/tool-tip.png)

「ICP 指標の追加」ドロップダウンをクリックして、モデルに追加の指標を挿入します。

![](assets/add-icp.png)

「エクスポート」チェックボックスをオンにすると、重点顧客の詳細ページで ICP 指標を表示でき、選択した ICP 指標を[重点顧客フィルター](/help/marketo/product-docs/target-account-management/engage/account-filters.md)の制約として使用できます。

![](assets/export.png)

>[!NOTE]
>
>ICP 指標は、**重点顧客のメンバー**&#x200B;フィルターとトリガーに制約として含まれます。

指標の重み付けは、モデル内で各指標が受け取る重要度のレベルを制御します。

![](assets/weightage.png)

変更を有効にするには、「モデルを更新」をクリックします。

![](assets/refresh-button.png)

（更新後に）モデルの調整が完了したら、「モデル結果」タブに戻り、「**保存してランクを適用**」をクリックします。

![](assets/ranks.png)
