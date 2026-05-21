---
unique-page-id: 10098134
description: エンゲージメントストリームのネストされたプログラムと、それらを使用するタイミングについて説明します。 サブグループ、マルチタッチ、追加のフローステップ用のプログラムを追加します。
title: エンゲージメントプログラムストリームへのプログラムの追加
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
TQID: https://experienceleague.adobe.com/kI2v6drF78DnJhhEbgeVSi4TYbF5rExY2wgR0aAK-bI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 479
ht-degree: 67%

---

# エンゲージメントプログラムストリームへのプログラムの追加 {#adding-a-program-to-an-engagement-program-stream}

## エンゲージメントプログラムストリームでネストされたプログラムを使用する理由 {#why-use-a-nested-program-in-an-engagement-program-stream}

エンゲージメントプログラムのストリームにメールを追加するのは簡単で、うまくいきます。 ただし、ビジネスニーズがより複雑な場合は、メールをプログラム内に配置すると効果的なことがあります。 例えば、次のような場合です。

* ストリーム内でユーザーのサブグループにメールを送信
* ストリーム内のサブグループに対して&#x200B;*異なる*&#x200B;メールを送信
* ランディングページ、フォーム、またはその他のアセットを育成に含める
* マルチタッチ属性の有効化
* アラートメールなどのフローステップを追加する

## ストリームでプログラムを使用するとどうなりますか？ {#what-happens-when-you-use-a-program-in-a-stream}

ネストされたプログラムを使用する場合、メールを個人に送信するかどうかは、プログラムのメンバーシップとプログラム ID に基づいて決定されます。

* プログラムのメンバーでない場合は、プログラムの一部であるメールを1回受信します
* プログラムのメンバーである場合、メールは届きません
* メンバーではなくなったが、そのプログラムを通じて以前にメールを受け取った場合、メールは届きません

ストリームでプログラムを使用する場合、その特定のメールを以前に受信したことがあるかどうかは関係ありません。 *その特定のプログラムで*&#x200B;以前にメールが送信されなかった場合、再度受け取ることがあります。

エンゲージメントプログラムでメールとプログラムを組み合わせるのが難しい場合があります。 どちらか一方を使用するとよいでしょう。

>[!TIP]
>
>スマートリストで&#x200B;**[!UICONTROL エンゲージメントプログラムのメンバー]** フィルターを使用します。

## スマートリストの条件を満たさない場合、どうなりますか？ {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

ネストされたプログラムのスマートキャンペーンのスマートリストから除外されたユーザーは、現在のキャスト中には次のコンテンツには移動されず、 *次の*&#x200B;キャストのストリーム内の次のコンテンツに移動されます。

## ネストされたプログラムには何が含まれますか？ {#what-does-a-nested-program-contain}

適切に設計されたネストされたプログラムには、メール、レポート、スマートキャンペーンが含まれます。 これらを一緒に保つのは理にかなっています。

使用するメールは、プログラム、別のプログラム、[!UICONTROL デザインスタジオ]でも使用できます。 どこに配置するかは、使い方によって異なります。

メールの場所で変更をレポートします。 例えば、メールが[!UICONTROL デザインスタジオ]にある場合、メールのパフォーマンスレポートでは、すべての指標が 1 行に表示され、異なるキャストが組み合わされます。 ただし、エンゲージメントストリーム効果レポートでは、異なる送信が別々に表示されます。

>[!CAUTION]
>
>何かを再送信したい場合は、新しいプログラムとスマートキャンペーンを作成するのが最も安全です。

>[!MORELIKETHIS]
>
>* [ストリームにコンテンツを追加する](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [プログラムについて](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
