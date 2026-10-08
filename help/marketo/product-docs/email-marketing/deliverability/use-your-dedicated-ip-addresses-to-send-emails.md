---
unique-page-id: 1900587
description: Marketoでメール送信に専用IP アドレスを使用する方法について説明します。 配信品質コンサルタントが、IP ウォームアップとDNS設定に関するコーチングを提供します。
title: 専用 IP アドレスを使用したメール送信
exl-id: cc83cf43-8b6d-4869-9c4f-7f3d2cd82dfa
feature: Deliverability
TQID: 'https://experienceleague.adobe.com/eZdDKPbVZJ5CCk9J73Wn934Bachb-y-rzyKBCznhlPw'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: be80ef53-082b-4612-a88f-dfce57d36b02
    internal-label: Deliverability
topic_v2:
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 78%
---
# 専用 IP アドレスを使用したメール送信 {#use-your-dedicated-ip-addresses-to-send-emails}

1 つ以上の専用 IP から送信することで、送信レピュテーションを完全に制御できます

>[!AVAILABILITY]
>
>専用 IP はアドオン製品です。 すべてのユーザーが専用 IP をプログラムに追加する資格を持つわけではありません。 専用 IP を維持するには、月に 100,000 件を超えるメールを送信し、キャンペーンの安定したケイデンスを維持する必要があります。 専用 IP を Marketo プログラムに追加する方法の詳細については、アカウントチームにお問い合わせください。
>
>月に送信するメールが 100,000 件未満で、キャンペーンの量が変化する場合、または季節に応じてメールを送信する場合は、専用 IP を維持できません。 Marketo は、厳格なベストプラクティスに従う顧客向けに、個別の信頼できる IP 共有プールを維持しています。 Marketoの信頼済みIP プログラムに申し込むには、[このアンケート ](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html)に入力してください。

すべての Marketo アカウントは共有 IP から使用開始し、すぐにメールを送信できます。 専用IPを追加する場合は、配信品質コンサルタントと協力してIPのプロビジョニングをスケジュールします。

配信品質専任のコンサルタントは、次の内容を提供します。

* IP ウォームアップに関するコーチングとコンサルティング
* 新しい専用 IP をブランディングするために必要な DNS エントリ
* 専用 IP の設定とアクティベーション
* ウォームアップフェーズ中のチェックインで成功をサポート

## 専用 IP の立ち上げ {#dedicated-ip-ramp-up}

長期にわたる配信品質を最大化するために、配信品質コンサルタントは、専用 IP 上でのメールキャンペーンの配信量を徐々に増やすためのカスタマイズされたレコメンデーションを提供します。 このプロセスは「IPのウォーミングアップ」と呼ばれます。 最初は、コールド（まっさら）な状態から始めて、メールの送信によってウォームアップします。 コールドな IP から大量のメールを送信すると、送信速度が制限されることが多く、通常はスパムとして分類されます。

**重要**：1 か月あたり最低 50,000 通のメールを維持します。 これにより、レピュテーションと配信品質について一貫したパターンが確立されます。 「ウォーム」IP 上でも、メールの量が大幅に増減すると、メールがメールプロバイダーに疑わしいものと見なされる可能性があります。

>[!TIP]
>
>データベースをクリーンな状態に保つことで、高い配信品質を維持できます。 [Adobe では](https://www.adobe.com/jp/legal/terms/aup.html)、メールの受信をオプトイン／リクエストした人にのみマーケティングコミュニケーションを送信する必要があります。 未承諾の電子メールは送信しないでください。

>[!CAUTION]
>
>バウンス件数が多い場合や、その他の問題がある場合は、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。 クリーンなデータベースの管理と、プログラムへのエンゲージメントの向上に関する詳細なサポートについては、Marketoのメール配信品質コンサルタントがカスタムサービスパッケージを利用できます。
