---
solution: Marketo Engage
product: marketo
title: スパム暗殺者
description: ここにテキストが入ります
level: Beginner, Intermediate
feature: Email Editor
hide: true
hidefromtoc: true
source-git-commit: 0157bc64444151a43bf464158d508e84d75b3427
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 9%

---

# スパム暗殺者 {#spam-assassin}

Marketo Engageで SpamAssassin を使用すると、メールコンテンツをテストし、ISP/メールボックスプロバイダーがスパムとしてマークする可能性を確認できます。

SpamAssassin はコンテンツを分析し、様々な条件に基づいてスコアを割り当てます。 スコアが低いほど、より良い結果が得られます。 高いスコアのメールを送信すると、配信品質全体に悪影響を与える可能性があるので、低いスコアを維持することが重要です。

## スパムレポートへのアクセス {#access-the-spam-report}

1. シミュレート画面で、「**スパムレポート**」ボタンをクリックします。

スクリーンショット

1. スパムレポートが生成されます。

スクリーンショット

1. 各項目のスコアと説明を確認します。

>[!IMPORTANT]
>
>全体のスコアが 5 を超える場合、メールがブロックされたり、配信時にスパムと見なされる可能性があります。

1. スコアが高すぎると思われる場合は、メールDesignerのコンテンツを編集し、スコアが望ましい位置になるまでスパムレポートを再実行します。

スクリーンショット

>[!NOTE]
>
>スパムスコアは SpamAssassin によって得られ、ルールはAdobeによって所有されません。 これらのルールについて詳しくは、[SpamAssassin ドキュメント ](https://spamassassin.apache.org/#_blank) を参照してください。 エラーの完全なリスト [ こちらを参照 ](https://spamassassin.apache.org/old/tests_3_0_x.html?utm_source=chatgpt.com)。
