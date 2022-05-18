---
unique-page-id: 7514918
description: 登録解除について - Marketo ドキュメント - 製品ドキュメント
title: 登録解除について
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '265'
ht-degree: 100%

---

# 登録解除について {#understanding-unsubscribe}

Marketo には、実際にはいくつかの異なるタイプの組み込みの登録解除があります。これらはすべて、名と同様に、ユーザーオブジェクトのフィールドで表されます。

>[!NOTE]
>
>Marketo では、製品内のブラックリストやホワイトリストなどの用語をブロックリストや許可リストに変更する作業を進めています。更新中は、UI およびドキュメントのスクリーンショットに古い用語が表示されたり、ドキュメントのテキストに新しい用語が表示されたりする場合があります。混乱を招いてしまったことをお詫びいたします。

これらのフィールドはすべて、Marketo での登録に組み込まれています。これらはすべてブール型（チェックボックス）です。これらは Forms または[データ値を変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)フローステップで使用できます。

## 登録解除済み {#unsubscribed}

これは、標準の登録解除ページで使用されます。ユーザーがこのボックスをオンにした場合、または電子メールの登録解除リンクをクリックした場合、そのユーザーはマーケティング電子メールを受け取らなくなります。ただし、[オペレーショナルメール](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)は受け取ります。

## マーケティングを中断したリード {#marketing-suspended}

このフィールドは、ユーザーが一時的な登録解除にリードを配置するために設定します。リードは、手動で変更した場合、またはデータ値の変更フローステップを利用した場合にのみ、このステータスを達成できます。

## メールの中断 {#email-suspended}

このステータスは、ハードバウンスが発生してから 24 時間、リードへのメール送信をブロックします。24 時間後、その人物は再びメールを利用できるようになります。

>[!NOTE]
>
>メールの中断は、24 時間が過ぎてもチェックされたままになるので、過去にそのようにマークされた人を指すことができます。その人が送信可能かどうかを確認するには、電子メールの停止の瞬間から 24 時間後がいつになるかを単に計算します。

## ブロックリスト登録済み {#blocklisted}

[競合他社などの人物に使用](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md)。（オペレーショナル、マーケティングなど）メールを&#x200B;**受けとらない**&#x200B;人これらの人は何も受け取りません。

![](assets/image2015-5-18-12-3a6-3a40.png)
