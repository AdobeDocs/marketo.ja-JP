---
unique-page-id: 45416698
description: リリースノート - 2020 年 7 月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2020 年 7 月
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 100%

---

# リリースノート：2020 年 7 月 {#release-notes-july}

2020 年 7 月リリースには以下の新機能が含まれています。お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。

>[!AVAILABILITY]
>
>ご契約状況によっては、星印（![（星）](assets/yellow-star.png)）がついている機能は有償オプションの追加契約が必要となる場合があります。詳細は Marketo Engage 担当営業にお問い合わせください。

**_四半期リリース_**&#x200B;以下の機能は **2020 年 7 月 31 日**（PT）にリリースされます。

## 管理 {#administration}

* **[フィールド管理の「使用先のエクスポート」機能追加](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**：管理者は、選択したフィールドが使われている全てのアセットリンクを CSV ファイルにエクスポートできるようになりました。この機能強化は、管理者と非管理者の両方が未使用のフィールドをクリーンアップするのに役立ちます。さらに、リンク先のアセットが新しいブラウザータブもしくはウィンドウで開けるようになりました。

## アカウントベースドマーケティング {#account-based-marketing}

![（星）](assets/yellow-star.png)

* **アカウントプロファイリング UI の刷新**：アカウントプロファイリングでのターゲットアカウントリストの作成を簡素化し、すべてのステップを 1 つの画面で行うことができます。

<br> 

**_四半期を通した段階的リリース_**

以下の機能はリリース後約 1 ～ 2 か月の間に段階的にリリースされます。

* **Forms サービス**：より強力なフォームのフィールド構文検証と、ランディングページ用の新しい Secured Domains の機能で一般的なボットパターンをブロックする機能を導入します。ボットパターンをブロックすることでスパムフォームの送信を減らし、データベースの品質を向上させることができます。

>[!NOTE]
>
>拡張フォームフィールド構文の検証の完全なロールアウトは、2021 年 1 月のリリース後まで延期されました。

* **Asset API URI サイズ上限の引き上げ**：「_method」パラメーターの削除に先立ち、URI のサイズ制限を 8 KB から 65 KB に引き上げます。長いクエリ文字列を実行する際に、このサイズ制限を増やすことでデータの受け渡しがより容易になります。「_method」パラメーターの削除は、今後のセキュリティアップグレードの一環として行われます。

## Sales Insight {#sales-insight}

![（星）](assets/yellow-star.png)

* **[CRM コネクタを使用しない Salesforce CRM 連携での Sales Insight の有効化](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)（クローズドベータ版）**：CRM コネクタを使用しないで Salesforce CRM と連携させている Marketo Engage のお客様も Sales Insight を使用することが可能になります。

## Sales Connect {#sales-connect}

![（星）](assets/yellow-star.png)

* **[販売呼び出しに対する双方の同意の強化：](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)**&#x200B;管理者は、通話録音の設定をより細かく管理できるようになりました。双方の同意に関する法律に準拠していることを確認し、[通話録音を有効](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md)にします。通話が録音中であることを示す通知を自動化し、通話の前に通知内容を再生します。

<br> 

## 告知情報＆廃止予定機能 {#announcements-deprecations}

* **Asset API「_method」パラメーターの削除**：2020 年 9 月以降、Asset API エンドポイントは、URI 長制限を回避するための POST ボディ内のクエリパラメーターを渡す方法として「_method」パラメーターを受け付けなくなります。このパラメーターを必要とするリクエストに対応するため、Asset API の URI 制限が 8 KB から 65 KB に引き上げられます。
* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**：このリリースの Munchkin JavaScript Client のバージョン 159 から、Munchkin Associate Lead メソッドのサポートを廃止し始めます。メソッドを呼び出すと、今後のリリースでメソッドが削除されることを示す警告が表示されます。削除すると、メソッドは機能しなくなり、使用しようとしても失敗します。Marketo Engage のお客様で、最近この方法を利用した場合、利用内容が個別に通知されます。
* **Internet Explorer のサポート**：既にお知らせした通り、Marketo Engage の Internet Explorer 11 のサポートは **2020 年 7 月 31 日**（PT）で終了しました。Google Chrome、Mozilla Firefox、Apple Safari、Microsoft Edge のサポートは今後も継続していきます
* **Sky デフォルト UX オプション**：今回のリリースでは、今後行われるメイン UX のアップデートに備えて、管理者やユーザーが Marketo Sky をデフォルト UX として設定するオプションが削除されます。今年後半に予定されているメイン UX のアップデートの詳細は、7 月以降に公開される予定です。Marketo Sky をデフォルトのエクスペリエンスとして設定したユーザーや、Marketo Sky へのアクセス権を付与されたユーザーは、引き続き、マイ Marketo ホームページのタイルから Marketo Sky にアクセスできます。
* **EdgeHTML（Chromium 以外）Microsoft Edge のサポート**：Marketo Engage は、2020 年末に Microsoft Edge の EdgeHTML バージョンをサポートしなくなります。2021 年 1 月 1 日（PT）からは、Microsoft Edge の Chromium 最新版のみをサポートします。
