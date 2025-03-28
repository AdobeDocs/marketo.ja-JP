---
unique-page-id: 2951220
description: モバイルプラットフォームの列があるリード効果レポートを作成する — Marketo ドキュメント — 製品ドキュメント
title: モバイルプラットフォームの列があるリード効果レポートを作成する
exl-id: 93fb6cb4-a6ca-4b35-b8bf-c6657eb9343b
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 100%

---

# モバイルプラットフォームの列があるリード効果レポートを作成する {#build-a-people-performance-report-with-mobile-platform-columns}

モバイルプラットフォーム（iOS/Android）の列があるリード効果レポートを作成するには、以下の手順を実行します。

## モバイルのスマートリストを作成する {#create-mobile-smart-lists}

1. **マーケティング活動**&#x200B;に移動します。

   ![](assets/ma.png)

1. プログラムを選択します。

   ![](assets/two-1.png)

1. 「**新規作成**」で「**新規ローカルアセット**」を選択します。

   ![](assets/three-1.png)

1. 「**スマートリスト**」をクリックします。

   ![](assets/four-1.png)

1. 名前を入力し、「**作成**」をクリックします。

   ![](assets/five-1.png)

1. 「開封済みメール」フィルターを見つけて、キャンバスまでドラッグします。

   ![](assets/six-1.png)

1. 「メール」を「**いずれかに該当**」に設定します。

   ![](assets/seven.png)

1. 「**制約の追加**」をクリックして「**プラットフォーム**」を選択します。

   ![](assets/eight.png)

   >[!TIP]
   >
   >この例では、「開封済みメール」フィルターを使いました。「プラットフォーム」制約があるので、「クリック済みメール」フィルターを使用することもできます。

1. 「プラットフォーム」を「**iOS**」に設定します。

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Marketo の自動提案で見つけられるには、少なくとも 1 つのリードが、iOS デバイス上でメールの 1 つを開封している必要があります。表示されていない場合は、手動で入力して保存してください。

   次に、Android プラットフォーム用に 2 番目のスマートリストを作成します。それが済んだら、次のセクションに進みます。

## リード効果レポートを作成する {#create-a-people-performance-report}

1. 「マーケティング活動」で、**iOS** と **Android** のスマートリストがあるプログラムを選択します。

   ![](assets/ten.png)

1. 「**新規作成**」で「**新規ローカルアセット**」を選択します。

   ![](assets/eleven.png)

1. 「**レポート**」をクリックします。

   ![](assets/twelve.png)

1. 「タイプ」を「**リード効果**」に設定します。

   ![](assets/thirteen.png)

1. 「**作成**」をクリックします。

   ![](assets/fourteen.png)

   いいですね。次の節に進みます。

## モバイルのスマートリストを列として追加する {#add-mobile-smart-lists-as-columns}

1. 作成したレポートで、「**設定**」をクリックし、「**カスタム列**」をキャンバスにドラッグします。

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >デフォルトでは、リード効果レポートには過去 7 日間が表示されます。タイムフレームはダブルクリックすると変更できます。

1. 作成したスマートリストを探して選択し、「**適用**」をクリックします。

   ![](assets/sixteen.png)

1. 「**レポート**」をクリックしてレポートを実行し、データを確認します。

   ![](assets/seventeen.png)

   素晴らしいですね。うまくいきました。
