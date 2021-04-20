---
unique-page-id: 7514918
description: 登録解除 —Marketoドキュメント — 製品ドキュメントについて
title: 登録解除
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# 登録解除{#understanding-unsubscribe}について

実際にMarketoにはいくつかの種類の組み込み登録解除があります。 名と同じように、すべては人物オブジェクトのフィールドで表されます。

>[!NOTE]
>
>Marketoは、ブラックリストやホワイトリストなどの用語を、当社の製品でブロックリストや許可リストに変更する過程にあります。 この更新中、UIとドキュメントのスクリーンショットには古い用語が表示され、ドキュメントのテキストには新しい用語が表示される場合があります。 ご混乱をおかけして申し訳ございません。

これらのフィールドはすべて、Marketo購読に組み込まれています。 これらはすべてブール型（チェックボックス）です。 これらは、Formsまたは[データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)のフローステップで使用できます。

## 配信停止完了 {#unsubscribed}

これは、標準の登録解除ページで使用されます。 ユーザーがこのボックスをオンにした場合、または電子メール内の登録解除リンクをクリックした場合、マーケティング用の電子メールは受信されなくなります。 ただし、[操作用の電子メール](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)を受け取ります。

## マーケティングを中断したリード {#marketing-suspended}

このフィールドは、ユーザーが一時的な登録解除にユーザーを配置するために設定します。 ユーザーがこのステータスにできるのは、手動で変更した場合、または変更データ値のフロー手順を利用した場合のみです。

## メールの中断 {#email-suspended}

このステータスにより、人が激しいバウンスが発生してから24時間はメールを受けるのを防ぐことができます。 24時間が経つと、再び郵送可能になります。

>[!NOTE]
>
>「停止された電子メール」は、24時間が過ぎてもチェックされたままになるので、過去に停止とマークされた人を参照できます。 その人が郵送可能かどうかを確認するには、電子メールの一時停止の時点から24時間を計算します。

## ブロックリストに加える{#blocklisted}

[これは競合他社などの人に使用します](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md)。電子メールを&#x200B;**受信しない** — 運用、マーケティングなど 何も得られない！

![](assets/image2015-5-18-12-3a6-3a40.png)
