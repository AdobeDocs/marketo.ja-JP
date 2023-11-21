---
description: Dynamic ChatFAQ - Marketoドキュメント — 製品ドキュメント
title: Dynamic Chatの FAQ
feature: Dynamic Chat
exl-id: 7b31afc3-77f4-46fb-9f0e-8cb9d60f3ffb
source-git-commit: a7404dc5c3f2014f53d49fd033f7e4002b9b2203
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 12%

---

# Dynamic Chatの FAQ {#dynamic-chat-faq}

Dynamic Chatに関するよくある質問への回答については、以下を参照してください。

**Dynamic Chat は、会社の web サイトの任意の場所にインストールできますか？それとも、Marketo のランディングページでのみ機能しますか？**

Dynamic Chat の JavaScript スニペットは、任意の web サイトおよび Marketo のランディングページにインストールできます。

**レポート用のデータはどのくらいの期間保存されますか？**

90 日間. 制限/パラメーターの完全なリストについては、Marketo Engage [製品の説明ページ](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage-product-description.html){target="_blank"}.

**Dynamic Chat は英語以外の言語をサポートしていますか？**

あります。Dynamic Chatでは、フランス語、スペイン語、ドイツ語、日本語、オランダ語、イタリア語、ポルトガル語（ブラジル）、韓国語、簡体字中国語、繁体字中国語の各言語をサポートしています。 詳しくは、 [言語の変更](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#changing-the-language){target="_blank"}.

**AI／NLP 機能はサポートしていますか？**

AI／NLP 機能はサポートしていません。

**匿名ユーザーをターゲットにするには、どうすればよいですか？**

ダイアログで、_Person Email is Empty_ 属性を使用します。

**エンゲージメントな会話の資格は何ですか？**

訪問者がダイアログまたは会話フローのボットに応答するとすぐに、関与した会話が発生します。 訪問者がチャットボットを開いたが、ボットに応答しない場合（例：回答または送信情報の選択）、エンゲージメントとしてカウントされません。

**月別関与会話の制限に達した場合はどうなりますか？**

月別関与会話の制限に達すると、すべての公開済みのダイアログと会話のフローがトリガーされ、制限が引き上げられるか、制限が翌月の初めにリセットされます。

**婚約した会話の制限に近づいている時を知るにはどうすればよいですか？**

関与した会話の上限の 90%に達すると、Dynamic Chat管理者に電子メール通知が送信され、すべてのユーザーにDynamic Chatのバナー通知が表示されます。

**訪問者がダイアログを操作し、その後ライブエージェントと接続した場合、それは 1 つまたは 2 つのエンゲージメントとしてカウントされますか？**

選択パッケージのお客様の場合は、2 つの個別のエンゲージメントとしてカウントされます。1 つはダイアログエンゲージメント用、もう 1 つはライブチャットエンゲージメント用です。 Prime パッケージのお客様の場合、ライブチャットのエンゲージメントは個別にカウントされないので、1 つのエンゲージメントとしてのみカウントされます。

**関与した会話の制限がリセットされる頻度はどれくらいですか？**

関与した会話の制限は、各月の最初にリセットされます。

**会話を終えた後、チャットボットが戻ってこないのはなぜですか？**

ダイアログは、1 回だけ訪問者に表示されるように設計されています。 したがって、訪問者がダイアログ内の特定のブランチの終わりに到達すると、そのダイアログは完了したと見なされ、その訪問者には再び表示されなくなります。

**My MarketoのDynamic ChatタイルをクリックしてAdobe Experience Cloudにログインすると、なぜ次のメッセージが表示されるのですか。 &quot;_Adobe IDがAdobe Experience Cloudソリューションアカウントにリンクされていないようです_.&quot;**

これは、Adobe Admin ConsoleでDynamic Chatユーザーとして追加されていない可能性が高いことを示しています。 Dynamic Chatへのアクセス権をリクエストするには、Adobe組織のシステム管理者またはDynamic Chatの製品管理者に問い合わせてください。

**関与した会話のトランスクリプトにアクセスする方法を教えてください。**

Dynamic Chatの記録は、Marketo Engageの「ダイアログとの関与」アクティビティを使用して、Dynamic Chatダイアログと関与した既知のリードに対してアクセスできます。

**訪問者がダイアログに参加した後、会話を再開したり、前の質問に戻ったりできますか。**

現在、会話を再開したり、以前の時点に戻ったりする体系的な方法はありませんが、これはDynamic Chat・ロードマップに記載されています。

**Dynamic Chatは Salesforce と統合されていますか？**

Dynamic Chatは、Salesforce 統合Marketo Engageで Salesforce と統合できます。

**カレンダーがDynamic Chatに接続され、ルーティングルールに含まれているので、会議を受け取らないのはなぜですか？**

これは、カレンダー接続を再認証する必要があることを示している可能性が高いです。 これは、多くの場合、カレンダープロバイダのパスワードを変更し、Dynamic Chatが接続を失った場合に発生します。 エージェントの設定ページに移動して、Dynamic Chatの「カレンダーの再認証」をクリックするだけです。

**対話と対話の流れの違いは何ですか？**

ダイアログとは、定義された一連のターゲット条件を満たす Web 訪問者に対して、自動的に表示される会話です。 対話フローは、ボタンの押しなど、Web 上で特定のアクションを実行する訪問者にのみ表示されます。

**メールから直接会議を予約するDynamic Chatを使用する方法はありますか？**

はい! [方法を表示する](https://nation.marketo.com/t5/product-blogs/using-dynamic-chat-conversational-flows-for-meeting-booking/ba-p/340936){target="_blank"}.

**Marketo EngageなしでDynamic Chatを使用できますか？**

いいえ。Dynamic ChatはMarketo Engageとは別の用途ですが、両者は解き放たれない関係にあります。
