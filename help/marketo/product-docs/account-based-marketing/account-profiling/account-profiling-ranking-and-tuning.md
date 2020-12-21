---
unique-page-id: 15695924
description: アカウントプロファイリングのランキングと調整 — Marketto Docs — 製品ドキュメント
title: アカウントプロファイリングのランク付けと調整
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---


# アカウントプロファイルのランク付けとチューニング{#account-profiling-ranking-and-tuning}

勘定科目プロファイリングは、理想的な顧客プロファイル(ICP)を識別し、ICPに基づいてデータベース内の会社をランク付けし、ICPインジケータ・データを名前付き勘定科目として昇格させる勘定科目に追加します。

## モデル結果{#model-results}

結果により、等級別に分類された既知の勘定科目がすべて表示されます。 Aは最も高い等級、Dは最も低い等級です。

![](assets/results.png)

オプションですが、[自動的にプロモート]チェックボックスをオンにすることをお勧めします。これにより、時間を節約できます。 ただし、各アカウントを調べて[手動で](/help/marketo/product-docs/account-based-marketing/target/named-accounts/discover-accounts.md#discover-crm-accounts)追加したい場合は、チェックボックスをオフにしておいてください。

<table> 
 <tbody> 
  <tr> 
   <td><strong>ランク</strong></td> 
   <td> 
    <div>
      理想的な顧客プロファイルに基づくアカウントランク。 Aは最適フィット、Dは最も適合しない。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>傾向</strong></td> 
   <td> 
    <div>
      非ICPベースの勘定科目の選択と比較したコンバージョン率の増加予測。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>アカウント(%)</strong></td> 
   <td> 
    <div>
      このランクを持つモデル入力の勘定の割合。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>モデル基準の%</strong></td> 
   <td> 
    <div>
      このランクを持つモデルベースの勘定の割合。 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## モデルのチューニング{#model-tuning}

「モデル」(Model)タブで、「モデルを調整」(Tune Model)ボタンをクリックします。

![](assets/two.png)

いくつかのタブから選択でき、詳細なカスタマイズが可能です。

![](assets/tuning-page.png)

**インジケーターカテゴリ**

<table> 
 <tbody> 
  <tr> 
   <td><strong>準拠</strong></td> 
   <td> 
    <div>
      認定、コンプライアンス関連の職階/採用 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>操作</strong></td> 
   <td> 
    <div>
      業務関連の職階/採用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>人事</strong></td> 
   <td> 
    <div>
      人事または給与ソフトウェア、人事関連の職階/雇用。
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>エンジニアリング</strong></td> 
   <td> 
    <div>
      テクノロジー、フレームワーク、エンジニアリング関連の職階/採用 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>売上高</strong></td> 
   <td> 
    <div>
      販売、販売関連の職階/雇用に関するソリューションとソフトウェア 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>意図</strong></td> 
   <td> 
    <div>
      インテントインジケーター。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      ハードウェア/ソフトウェア・ソリューション、テクノロジー、IT関連の位置づけ/採用
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>金融</strong></td> 
   <td> 
    <div>
      金融ソフト、財務関連の職階/雇用。 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>マーケティング</strong></td> 
   <td> 
    <div>
      マーケティングテクノロジーとソフトウェア、マーケティング関連の職位/雇用 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>ビジネス</strong></td> 
   <td> 
    <div>
      フォーブス又は株式会社の上場又は事業提携 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>顧客体験と関係</strong></td> 
   <td> 
    <div>
      顧客の成功と顧客関係の位置/雇用。
    </div></td> 
  </tr> 
 </tbody> 
</table>

各列の説明を表示するには、ツールヒントの上にカーソルを置きます。

![](assets/tool-tip.png)

「追加ICPインジケータ」ドロップダウンをクリックして、追加のインジケータをモデルに挿入します。

![](assets/add-icp.png)

「エクスポート」ボックスを選択すると、「名前付き勘定科目の詳細」ページにICPインジケータが表示され、選択したICPインジケータを[名前付き勘定科目フィルター](/help/marketo/product-docs/account-based-marketing/engage/account-filters.md)の制約として使用できます。

![](assets/export.png)

>[!NOTE]
>
>ICPインジケータは、**名前付きアカウント**&#x200B;のフィルターおよびトリガーのメンバーに制約として含まれます。

インジケーターの重み付けは、モデルで各インジケーターが受け取る重要度のレベルを制御します。

![](assets/weightage.png)

変更を有効にするには、「モデルを更新」をクリックします。

![](assets/refresh-button.png)

モデルの調整が完了したら（更新後）、「モデル結果」タブに戻り、**ランクの保存と適用**&#x200B;をクリックします。

![](assets/ranks.png)
