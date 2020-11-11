---
title: 目標追跡と予測登録の理解
description: 目標追跡と予測登録について
translation-type: tm+mt
source-git-commit: 1231bc32a3abdf66c10864d6605234763618dbe0
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---


# 目標追跡と予測登録について

<br> 

イベントの目標 [を設定し](/help/sky/setting-event-goals.md)、 [スマートなキャンペーンを通じて招待を送信した後で](/help/sky/create-a-smart-campaign.md)、目標の進行状況を追跡し、マーケティング担当者の予測を理解する方法を以下に示します。

>[!NOTE]
>
>Marketo Classicのエクスペリエンスでイベントプログラムを作成すると、イベント開始日は現在、イベント作成日がデフォルトになります。 登録予測では、イベントの開始日までの時間が考慮されるので、開始日と作成日が同じ場合は（意図的に設定しない限り）、これらの数字は正確ではない場合があります。

## 目標追跡と登録の予測

1. 目標追跡の詳細は、イベントプログラムの「 [!UICONTROL **レポート**] 」タブで確認できます。 この例では、現在のところ、200(75%)という目標に対して150人の会員が登録されています。

   ![イメージ1](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-1.png)

また、 [!UICONTROL **予測登録も表示されます**] 。 情報アイコンの上にカーソルを置くと、尤度セグメントによるこの数の分類が表示されます。

![イメージ2](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>「有効」および「超過」のグラフは、イベントの日まで空のままです。

1. 「グラフ」トグルをクリックして、登録の確率に基づくメンバーの分類に切り替えます。 各セグメントの現在の登録率が、過去のプログラムでのそのセグメントの平均割合に比べて表示されます。

   ![イメージ3](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-3.png)

すべての会員（登録済みで未登録）は、その会員の登録確率に基づいて分類されます。 情報アイコンの上にマウスポインターを置くと、これらの尤度カテゴリの定義方法が表示されます。

![画像4](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>予測数は、イベントの日まで、24時間ごとに更新されます。 「_処理_」としてリストされるメンバーは、次の計算サイクルに含まれます。

## 類似プログラム

過去にどの程度類似したプログラムが行われたかを見ると、現在のイベントをいくつか把握できます。 このセクションには、過去6か月間で最大5人の類似プログラムと、_登録されたメンバーの数/割合_ 以上が表示されます。

同様のプログラムを計算する際、以下の要因を含めます。

* プログラム型
* プログラムチャネル
* オーディエンスサイズ
* プログラムタグ
* イベントの作成からイベントの開始までの時間
* イベント時間

   ![画像5](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-5.png)

## Recommendations

レポートページの上部では、進行状況に基づいたAI/ML主導のレコメンデーションを見つけることができます。 定期的に戻って役立つヒントとインサイトを確認してください。

![画像6](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-6.png)

## 人間レベルの予測

「[!UICONTROL **メンバー**] 」タブをクリックして、すべてのプログラムメンバーを表示します。 「 [!UICONTROL **登録の確率**] 」または「 [!UICONTROL **出席の確率**] 」のバーにマウスポインターを置くと、正確な割合と分類が表示されます。 その後、特定のカテゴリのメンバー(「可能性が低い」メンバー全員がカテゴリを登録する)に対して行動を起こし、特に登録番号を増やす可能性を高めるようにターゲットできます。

![画像7](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>個別の可能性は、プロファイル属性、個人アクティビティ、過去の招待/登録/参加アクティビティなど、40人以上の個人要因を考慮に入れます。

## FAQ

**Q:セグメントとは何ですか。**

A:登録できる値は0 ～ 100です。 イベントプログラムのメンバーである人は全員、0 ～ 100の確率値を受け取ります。

尤度の値を次の3つのセグメントに分けます。

* 50%を超える登録の可能性=高い可能性の高いセグメント
* 登録する可能性が25%を超えて50%未満=可能性の高いセグメント
* 25%未満登録する可能性=可能性の低いセグメント

登録する可能性がある場合、予測は次のセグメントの1つに分類されます(プログラムのメンバーであるすべての人がその1つに分類されます)。 例えば、イベントプログラムの尤度予測に基づいて1000人のメンバーがいる場合、その1000人は _高度_、 _高度_、 _低確度_ 、または低い確率のセグメントに配分されます。

したがって、「高可能性」セグメントに入る訪問者は、イベントに登録する可能性が高くなります。

登録へのコンバージョン=セグメントに登録された人数をセグメントに含まれる人数で割った値(例えば、100人が「高い確率」セグメントに含まれ、60人が登録された場合、コンバージョン率は60%になります)。

登録するコンバージョン率は次のパターンに従います。可能性が高い>可能性が低い>可能性が低い。

**Q:インサイトの使用方法**

A:ベストプラクティスには、次の事項が含まれます。

i.プログラムを作成した後、スマートキャンペーンで「Xより大きい」を含む予測フィルターを使用すると、一定の人数（例えば1000）のが発生し、キャンペーンを実行できます。

2. 24時間後に、「 [!UICONTROL レポート] 」タブで、現在招待されているすべての訪問者の値を登録する可能性に基づいて計算された、予測登録を確認できます。

iii. 予測される登録数が目標より少ない場合は、より多くの人を招待する必要があります。 この時点で、過去のプログラムでのしきい値の効果を示すインサイトを確認できます。

![画像8](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-8.png)

iv. そのしきい値を持つ新しいスマートキャンペーンを作成して、より多くの人を招待できます。

v.予測される数が表示される理由を把握したい場合は、セグメント間のオーディエンスの分布、過去のコンバージョン率を切り替えて、これらのコンバージョン率を現在のオーディエンスに適用できます（下のスクリーンショットを参照）。

**Q:登録別セグメントグラフとは**

A:3つのバー。それぞれがセグメントを表します（「高い確率」、「高い確率」、「低い確率」）。

**紫の点線：** 過去の類似プログラムに基づく、そのセグメント内の登録に対する平均会話率。

**青いバー：** そのセグメント内のすべての訪問者の登録率。

![画像9](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-9.png)

例えば、100人が登録した100人のうち50%を超え60人が登録する可能性があるとします。 コンバージョン率は60%である可能性が高い。 そのため、プログラムに追加されたすべてのメンバーは値を登録する可能性が得られ、セグメントに入れられ、各セグメントコンバージョン率に登録された人数に応じて計算されます。

**Q:「登録済み」と「上位」とは何を意味するか**

A:登録者として記載されている者その他のステップ番号が等しい者

イベントプログラムの新しい進行状況のステータスを作成できますが、これらのステータスを標準のステータスに対応付けています。 訪問者を招待からアニメーションに移すケースを考えてみましょう。これは登録よりも高いステップです。 この人物は、登録済みと見なされ、目標追跡に表示されます。

![画像10](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-10.png)

**Q:予測登録はどのように計算されますか？**

A:以下を参照。

![イメージイレブン](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-11.png)
