---
unique-page-id: 2359476
description: メールプログラムダッシュボードの使用 - Marketo ドキュメント - 製品ドキュメント
title: メールプログラムダッシュボードの使用
exl-id: 47c1925a-144b-4277-a08d-1af660ed3d50
feature: Email Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 100%

---

# メールプログラムダッシュボードの使用 {#use-the-email-program-dashboard}

このダッシュボード表示でメールプログラムの実行状況を確認します。

>[!CAUTION]
>
>正確なレポートを作成するのに、スマートキャンペーンでメールを参照したり、起動したメールプログラムから新しいメールプログラムにアセットを移動したりして、メールプログラムからメールを&#x200B;_再利用_&#x200B;しないでください。再利用すると、そのメールに添付されたすべてのレポートダッシュボードのすべてのデータが集計されます。メールを再利用する必要がある場合は、代わりに[クローンを作成](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-an-asset-in-a-program.md){target="_blank"}してください。これにより、メールがコピーされますが、新しいメール ID で新しいメールが作成されます。

>[!NOTE]
>
>プログラムに A/B テストがある場合は、[メールプログラムダッシュボード：A/B テスト表示](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}を参照してください。

![](assets/image2014-9-12-14-3a12-3a56.png)

>[!NOTE]
>
>この表示のすべてのデータは集計です（A/B テストと最終的なメール送信を含む）。

## メール送信 {#email-send}

ここでは、送信、バウンス、配信されたメールの数を確認できます。

![](assets/image2014-9-12-14-3a13-3a3.png)

>[!NOTE]
>
>メール配信品質の基準が Marketo の管理下にないので、バウンス統計と配信統計は正確ではなく概算的なものになります。

## 開封／クリック数 {#opens-clicks}

このグラフは、メールプログラムが実行された後の特定の期間に開封／クリックされたメールの数を示します。

![](assets/image2014-9-12-14-3a13-3a7.png)

>[!TIP]
>
>時間が経過するにつれて開封数／クリック数がどのように減少しているかに注意してください。

## 概要 - エンゲージメント {#summary-engagement}

全体的な[エンゲージメントスコア](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}を示します。

![](assets/image2014-9-12-14-3a13-3a11.png)

## 概要 - その他 {#summary-rest}

その他のデータには、「開封数」、「クリック数」、「クリック／開封率」、「登録解除数」が表示されます。

![](assets/image2014-9-12-14-3a13-3a15.png)

>[!TIP]
>
>上記の例では、**登録解除**&#x200B;率が非常に小さいのでズームインして見やすくしました。バー内の 2 番目の数字は、表示用の目盛りとして追加されています。

>[!NOTE]
>
>**定義**
>
>**[!UICONTROL 開封数]**&#x200B;は、メール受信者が Marketo が挿入したトラッキングピクセルを含むメールの画像をダウンロードした際にカウントされます。受信者がメールを閲覧したがその画像をダウンロードしなかった場合は、開封とは見なされません。受信者のプレビューパネルに画像が読み込まれた場合は、通常は開封としてカウントされますが、メールクライアントによって異なります。
>
>**[!UICONTROL クリックして開く]**&#x200B;は、開かれてメール内のリンクがクリックされたメールの割合を測定します。ユニーククリック数をユニーク開封数で割ってから 100 を掛けて、割合で表示します。

## ダッシュボードの更新 {#refresh-dashboard}

最新のデータを表示するには、ダッシュボードを更新アイコンをクリックします。

![](assets/refreshicon.png)

>[!MORELIKETHIS]
>
>[メールプログラムのダッシュボードを使用する：A/B テスト表示](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}
