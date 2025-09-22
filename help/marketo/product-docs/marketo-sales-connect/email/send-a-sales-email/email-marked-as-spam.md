---
unique-page-id: 14352525
description: スパムとしてマークされたメール - Marketo ドキュメント - 製品ドキュメント
title: スパムとしてマークされたメール
exl-id: 2cd1ec96-441d-4de7-8709-543d04e20a91
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 100%

---

# スパムとしてマークされたメール {#email-marked-as-spam}

当社は、企業として、配信品質の割合を高く保つために懸命に取り組んでいます。それでも、送信したメールがスパムフォルダーにルーティングされるトリガーとなるユーザの行動や設定がいくつかあります。

**設定を確認しましょう**

* カスタムドメイントラッキング：これにより、すべてのトラッキングリンクが「go.toutapp」の代わりに「go.yourdomain」として表示されます。一部のメールセキュリティでは、メールが「yourdomain」から送信されているが、リンクが go.toutapp にリルーティングされていることがわかります。カスタムドメインリンクトラッキングを実装すると、メールは正当に見え、受信者のインボックスに到達する可能性が高くなります。
* メール配信チャネル：デフォルトでは、メールは ToutApp サーバーを通じて送信されます。独自の Gmail またはカスタム SMTP を設定することで、メールが受信者のインボックスに到達するチャンスが最大になります。必要に応じて適切な配信チャネルを選択する方法について詳しくは、[こちら](https://nation.marketo.com/docs/DOC-5080){target="_blank"}をクリックしてください。

**メールの動作の確認をしましょう**

* メールは短く簡易的な内容に保ち、以前に書いたメールとしてテンプレートを貼り付けます。

* 過剰に書式設定されているメールや、多国籍的な言葉を使用するメッセージは避けてください。

* 住所が記載された完全なメール署名があることを確認します。

* 読み上げて [CAN-SPAM 法](https://www.ftc.gov/business-guidance/resources/can-spam-act-compliance-guide-business){target="_blank"}に準拠していることを確認します。
