---
unique-page-id: 7514918
description: 登録解除 — Marketto Docs — 製品ドキュメントについて
title: 登録解除
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# 登録解除 {#understanding-unsubscribe}

Marketoには様々な種類の組み込み登録解除があります。 名と同じように、すべては人物オブジェクトのフィールドで表されます。

>[!NOTE]
>
>マーケティング担当者は、ブラックリストやホワイトリストなどの用語を、当社の製品のブロックリスト許可リストやに変更する過程にあります。 この更新中、UIとドキュメントのスクリーンショットには古い用語が表示され、ドキュメントのテキストには新しい用語が表示される場合があります。 ご混乱をおかけして申し訳ございません。

これらのフィールドはすべて、マーケティング購読に組み込まれています。 これらはすべてブール型（チェックボックス）です。 これらは、Formsまたは [Change Data Value](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) （データ値を変更）フローステップで使用できます。

## 登録解除 {#unsubscribed}

これは、標準の登録解除ページで使用されます。 ユーザーがこのボックスをオンにした場合、または電子メール内の登録解除リンクをクリックした場合、マーケティング用の電子メールは受信されなくなります。 ただし、 [操作用の電子メールを受け取ります](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)。

## マーケティングの中断 {#marketing-suspended}

このフィールドは、ユーザーが一時的な登録解除にユーザーを配置するために設定します。 ユーザーがこのステータスにできるのは、手動で変更した場合、または変更データ値のフロー手順を利用した場合のみです。

## 電子メールの一時停止 {#email-suspended}

このステータスにより、人が激しいバウンスが発生してから24時間はメールを受けるのを防ぐことができます。 24時間が経つと、再び郵送可能になります。

>[!NOTE]
>
>「停止された電子メール」は、24時間が過ぎてもチェックされたままになるので、過去に停止とマークされた人を参照できます。 その人が郵送可能かどうかを確認するには、電子メールの一時停止の時点から24時間を計算します。

## ブロックリストに加える {#blocklisted}

[これは競合他社などの人に使用します](http://docs.marketo.com/x/uwOQ)。 電子メール **を受け取りたくない人** （運用、マーケティングなど） 何も得られない！

![](assets/image2015-5-18-12-3a6-3a40.png)

