---
description: Dynamic Chatに関する FAQ - Marketo ドキュメント – 製品ドキュメント
title: Dynamic Chatに関するよくある質問
feature: Dynamic Chat
exl-id: 7b31afc3-77f4-46fb-9f0e-8cb9d60f3ffb
source-git-commit: 941fdf08b580bab80c456e3956e965c9e2fa6942
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 5%

---

# Dynamic Chatに関するよくある質問 {#dynamic-chat-faq}

Dynamic Chatに関するよくある質問への回答については、以下を参照してください。

**私はDynamic Chatへのアクセス権がないようです。 どうすれば手に入りますか。**

Marketo Engage管理者に連絡し、Adobe Admin Consoleで [ ユーザーとして追加 ](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} されたことを確認してください。

**Dynamic Chatは、会社の web サイトの任意の場所にインストールできますか。それとも、Marketo ランディングページでのみ機能しますか？**

このDynamic ChatJavaScript スニペットは、任意の web サイトとMarketo ランディングページにインストールできます。

**レポート用のデータはどのくらいの期間保存されますか？**

90 日間。 制限/パラメーターの完全なリストについては、Marketo Engage[Product Description page](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage-product-description.html){target="_blank"} を参照してください。

**Dynamic Chat は英語以外の言語をサポートしていますか？**

あります。Dynamic Chatがサポートする言語は、フランス語、スペイン語、ドイツ語、日本語、オランダ語、イタリア語、ポルトガル語（ブラジル）、韓国語、中国語（簡体字）および中国語（繁体字）です。 詳しくは、[ 言語の変更 ](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#changing-the-language){target="_blank"} を参照してください。

**AI／NLP 機能はサポートしていますか？**

AI／NLP 機能はサポートしていません。

**匿名ユーザーをターゲットにするには、どうすればよいですか？**

ダイアログで、_Person Email is Empty_ 属性を使用します。

**エンゲージメントの高い会話と言えるものは何ですか？**

エンゲージメントのある会話は、訪問者がダイアログまたは会話フローでボットに応答するとすぐに発生します。 訪問者がチャットボットを開いてもボットに応答しない場合（応答の選択や情報の送信など）、エンゲージメントとしてはカウントされません。

**月間エンゲージメント済み会話数の上限に達した場合はどうなりますか？**

1 か月のエンゲージメント済み会話制限に達すると、すべての公開済みダイアログと会話フローは、制限を増やすか、翌月の初めに制限がリセットされるまでトリガーを停止します。

**エンゲージメントされている会話の制限に近づいているときにを把握するにはどうすればよいですか？**

エンゲージメントされた会話の上限である 90% に達すると、Dynamic Chat管理者にメール通知が届き、すべてのユーザーにDynamic Chatでバナー通知が表示されます。

**訪問者がダイアログにエンゲージメントした後にライブエージェントに接続した場合、そのエンゲージメントは 1 つまたは 2 つに数えられますか？**

Select パッケージを使用するお客様の場合、これは 2 つの個別のエンゲージメントとしてカウントされます。1 つは Dialog エンゲージメント用、もう 1 つはライブチャットエンゲージメント用です。 Prime パッケージを使用しているお客様の場合、ライブチャットのエンゲージメントは個別にカウントされないので、1 つのエンゲージメントとしてのみカウントされます。

**エンゲージメントされた会話の制限がリセットされる頻度はどれくらいですか？**

エンゲージメントされた会話の制限は、毎月 1 日にリセットされます。

**会話が終わった後、チャットボットが戻ってきませんか？**

ダイアログは、訪問者に 1 回だけ表示されるように設計されています。 したがって、訪問者がダイアログ内の特定のブランチの終わりに到達するとすぐに、そのダイアログは完了と見なされ、その訪問者に二度と表示されなくなります。

**MarketoのDynamic ChatタイルをクリックしてAdobe Experience Cloudにログインすると、次のメッセージが表示されるのはなぜですか？ 「_Adobe IDはAdobe Experience Cloud ソリューションアカウントとリンクされていないようです_。」**

これは、Adobe Admin ConsoleでDynamic Chatユーザーとして追加されていないことを示している可能性があります。 Dynamic Chatへのアクセスをリクエストするには、Adobe組織のシステム管理者またはDynamic Chatの製品管理者にお問い合わせください。

**エンゲージメントのある会話のトランスクリプトにアクセスするにはどうすればよいですか？**

Dynamic Chatトランスクリプトには、Marketo Engageの「対話に関与」アクティビティを通じて、Dynamic Chatの対話に関与した既知のリードについてアクセスできます。

**訪問者がダイアログに参加すると、会話を再開したり、前の質問に戻ったりできますか？**

現在、会話を再開したり、以前の時点に戻したりする体系的な方法はありませんが、これはDynamic Chatロードマップに記載されています。

**Dynamic Chatは Salesforce と統合されますか？**

Dynamic Chatは、Marketo Engage Salesforce 統合を介して Salesforce と統合されます。

**カレンダーはDynamic Chatに接続されており、自分はルーティングルールに含まれているので、ミーティングが行われないのはなぜですか？**

これは、カレンダー接続の再認証が必要であることを示している可能性が高くなります。 この問題は、予定表プロバイダのパスワードを変更したときに、Dynamic Chatが接続を失ったときに最もよく発生します。 Dynamic Chatの [Agent Settings] ページに移動して、[Reauthenticate calendar] をクリックするだけです。

**対話と会話フローの違いは何ですか？**

ダイアログは、定義された一連のターゲティング条件を満たす web 訪問者に自動的に表示される会話です。 会話フローは、ボタンを押すなど、web 上で特定のアクションを実行した訪問者にのみ表示されます。

**Dynamic Chatでメールから直接会議を予約する方法はありますか？**

はい。[ 詳細を表示する ](https://nation.marketo.com/t5/product-blogs/using-dynamic-chat-conversational-flows-for-meeting-booking/ba-p/340936){target="_blank"}。

**「エンゲージメント」や「獲得した人物」などの用語は正確にはどのような意味ですか？**

Dynamic Chatで使用される用語は複数あります。 それらの多くの定義は、それぞれの領域のヘルプ記事で確認できます。

* 「People Acquired」などの Analytics 用語 [ こちらを参照 ](/help/marketo/product-docs/demand-generation/dynamic-chat/analytics.md#definitions){target="_blank"}。
* スマートリストのトリガーとフィルターの定義 [ こちらを参照 ](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities.md#definitions){target="_blank"}。
* 様々なストリームDesignerカードの説明 [ こちらを参照 ](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-cards){target="_blank"}。

**Marketo EngageなしでDynamic Chatを使用できますか？**

いいえ。Dynamic ChatはMarketo Engageとは別の用途ですが、この 2 つは密接に関連しています。
