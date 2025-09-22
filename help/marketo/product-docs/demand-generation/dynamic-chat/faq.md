---
description: Dynamic Chat に関するよくある質問 - Marketo ドキュメント - 製品ドキュメント
title: Dynamic Chat に関するよくある質問
feature: Dynamic Chat
exl-id: 7b31afc3-77f4-46fb-9f0e-8cb9d60f3ffb
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 98%

---

# Dynamic Chat に関するよくある質問 {#dynamic-chat-faq}

Dynamic Chat に関するよくある質問への回答について詳しくは、以下を参照してください。

**Dynamic Chat へのアクセス権が付与されていないようです。アクセス権を取得するには、どうすればいいですか？**

Marketo Engage 管理者に問い合わせて、Adobe Admin Console に[ユーザとして追加](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"}されていることを確認してください。

**Dynamic Chat は、会社の web サイトの任意の場所にインストールできますか？それとも、Marketo のランディングページでのみ機能しますか？**

Dynamic Chat の JavaScript スニペットは、任意の web サイトおよび Marketo のランディングページにインストールできます。

**レポート用のデータはどのくらいの期間保存されますか？**

90 日です。制限/パラメーターの完全なリストについては、Marketo Engage[Product Description page](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage-product-description.html){target="_blank"} を参照してください。

**Dynamic Chat は英語以外の言語をサポートしていますか？**

はい。Dynamic Chat は、フランス語、スペイン語、ドイツ語、日本語、オランダ語、イタリア語、ポルトガル語（ブラジル）、韓国語、簡体字中国語、繁体字中国語をサポートしています。詳しくは、[言語の変更](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#changing-the-language){target="_blank"}を参照してください。

**AI／NLP 機能はサポートしていますか？**

AI／NLP 機能はサポートしていません。

**匿名ユーザーをターゲットにするには、どうすればよいですか？**

ダイアログで、_Person Email is Empty_ 属性を使用します。

**エンゲージ済み対話には、何が該当しますか？**

エンゲージ済み対話は、訪問者がダイアログまたは対話型フローでボットに応答するとすぐに発生します。訪問者がチャットボットを開いてもボットに応答しない場合（応答の選択や情報の送信などを行わない場合）は、エンゲージメントとしてカウントされません。

**月別エンゲージ済み対話数の上限に達した場合はどうなりますか？**

月別エンゲージ済み対話数の上限に達すると、上限を増やすか、翌月の初めに制限がリセットされるまで、すべての公開済みダイアログと対話型フローのトリガーが停止します。

**エンゲージ済み対話数の上限に近づいていることを把握するにはどうすればよいですか？**

エンゲージ済み対話数の上限の 90％に達すると、Dynamic Chat 管理者にメール通知が届き、すべてのユーザに Dynamic Chat でバナー通知が表示されます。

**訪問者がダイアログにエンゲージした後でライブエージェントに接続した場合、エンゲージメントは 1 回と 2 回のどちらとしてカウントされますか？**

Select パッケージのお客様の場合、これは 2 回の個別のエンゲージメント (ダイアログエンゲージメントが 1 回、ライブチャットエンゲージメント が 1 回) としてカウントされます。Prime パッケージのお客様の場合、ライブチャットエンゲージメントは個別にカウントされないので、エンゲージメントが 1 回のみカウントされます。

**エンゲージ済み対話数の上限はどのくらいの頻度でリセットされますか？**

エンゲージ済み対話数の上限は、各カレンダー月の初日にリセットされます。

**対話の終了後、チャットボットが表示されないのはなぜですか？**

ダイアログは、訪問者に 1 回のみ表示されるように設計されています。したがって、訪問者がダイアログ内の特定の分岐の最後に到達すると、そのダイアログは完了と見なされ、その訪問者に対しては再度表示されません。

**My Marketo の Dynamic Chat タイルをクリックして Adobe Experience Cloud にログインすると、次のメッセージが表示されるのはなぜですか？「_Adobe ID が Adobe Experience Cloud ソリューションアカウントにリンクされていないようです。_」**

Adobe Admin Console で Dynamic Chat ユーザとして追加されていない可能性があります。Dynamic Chat へのアクセスをリクエストするには、アドビ組織のシステム管理者または Dynamic Chat の製品管理者にお問い合わせください。

**エンゲージ済み対話数の上限のトランスクリプトにアクセスするにはどうすればよいですか？**

Dynamic Chat のトランスクリプトでは、Marketo Engage の「ダイアログでエンゲージ済み」アクティビティを通じて Dynamic Chat ダイアログにエンゲージし、対話ステータスが「完了」または「ドロップ」になっている既知のリードについてアクセスできます。

**訪問者はダイアログにエンゲージした後で、対話を再開したり、前の質問に戻ったりできますか？**

現在、対話を再開したり、前の時点に戻ったりする体系的な方法はありませんが、Dynamic Chat のロードマップにはこの方法が含まれています。

**Dynamic Chat は Salesforce と統合されますか？**

Dynamic Chat は、Marketo Engage Salesforce 統合を通じて Salesforce と統合されます。

**カレンダーは Dynamic Chat に接続されており、私はルーティングルールにも含まれていますが、ミーティングが表示されません。なぜでしょうか？**

カレンダー接続の再認証が必要な可能性があります。この問題は、カレンダープロバイダーのパスワードを変更し、Dynamic Chat の接続が失われた場合に頻繁に発生します。Dynamic Chat のエージェント設定ページに移動し、「カレンダーを再認証」をクリックするだけです。

**ダイアログと対話型フローの違いは何ですか？**

ダイアログは、定義済みの一連のターゲティング条件を満たす web 訪問者に自動的に表示される対話です。対話型フローは、ボタンを押すなど、web 上で特定のアクションを実行する訪問者にのみ表示されます。

**Dynamic Chat を使用してメールから直接ミーティングを予約する方法はありますか？**

はい、あります。[方法についてはこちらを参照してください](https://nation.marketo.com/t5/product-blogs/using-dynamic-chat-conversational-flows-for-meeting-booking/ba-p/340936){target="_blank"}。

**「エンゲージ済み」や「獲得済み人物」などの用語は、正確にはどのような意味ですか？**

Dynamic Chat で使用される用語は複数あります。それらの多くの定義は、各領域のヘルプ記事で確認できます。

* 「獲得済み人物」などの Analytics の用語について詳しくは、[こちらを参照してください](/help/marketo/product-docs/demand-generation/dynamic-chat/analytics.md#definitions){target="_blank"}。
* スマートリストのトリガー／フィルターの定義について詳しくは、[こちらを参照してください](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities.md#definitions){target="_blank"}。
* 様々なストリームデザイナーのカードについて詳しくは、[こちらを参照してください](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-cards){target="_blank"}。

**Marketo Engage なしで Dynamic Chat を使用できますか？**

いいえ、できません。Dynamic Chat は Marketo Engage とは別のアプリケーションですが、この 2 つは密接に関連しています。
