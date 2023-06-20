---
description: Salesforce での一括送信セールスメールの使用 — Marketoドキュメント — 製品ドキュメント
title: Salesforce でのセールスメールの一括送信の使用
source-git-commit: 4d88547ecdc25a2a1e0de49fab1493bbefd6800b
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Salesforce でのセールスメールの一括送信の使用 {#using-bulk-send-sales-email-in-salesforce}

セールスアクションを使用してアウトバウンド通信を拡大・縮小するために、Salesforce で一括メールを送信する方法を説明します。

>[!NOTE]
>
>Salesforce では、一度に 200 件のレコードを選択できる制限が適用されています。

>[!PREREQUISITES]
>
>をインストール済みであることを確認します。 [最新の Sales Insight パッケージ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} to your Salesforce instance and have configured the [Action buttons](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"} を Salesforce の連絡先およびリードリスト表示に追加しました。

## Salesforce Lightning での一括メールの送信 {#sending-bulk-email-in-salesforce-lightning}

1. Salesforce で、 **リード/連絡先** タブをクリックします。

   ![](assets/using-bulk-send-sales-email-in-salesforce-1.png)

1. 「表示」ドロップダウンで、電子メールで送信するリード/連絡先の表示を選択します。

   >[!TIP]
   >
   >新しいビューを作成するには、右側のコグアイコンをクリックし、「 **新規**. ビューに新しい名前を付けて保存したら、右側のフィルターアイコンをクリックして、電子メールで送信するリード/連絡先を絞り込むことができます。

1. 目的のリードまたは連絡先のリストを選択し、 **セールスメールの送信** 」ボタンをクリックします。

   ![](assets/using-bulk-send-sales-email-in-salesforce-2.png)

1. アクション作成ウィンドウに移動し、選択したユーザーが追加されます。

1. アクション作成ウィンドウエディターに挿入するテンプレートを選択するか、カスタムメールを作成します。

   >[!TIP]
   >
   >用途 [ピンされたカテゴリ](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} お気に入りの電子メールテンプレートに容易にアクセスできるようにします。

   **オプションの手順**:動的フィールドのパーソナライゼーションをプレビューするには、 **ダイナミックフィールドをプレビュー** 」ボタンをクリックします。

   >[!TIP]
   >
   >すべての受信者用にテンプレートをカスタマイズする場合は、一括作成サイドバーの「すべての受信者」オプションをクリックすると、すべての受信者の E メールを同時に編集できます。 特定の E メールを変更する場合は、一括作成サイドバーで受信者の名前または E メールをクリックします。 個々の E メールに変更を加え、「すべての受信者」を選択して変更を加えると、「すべての受信者」に加えた変更は、個々の E メールに加えた変更を上書きします。

1. 選択 **送信** E メールを即座に送信する場合、または **スケジュールを設定** ：電子メールを送信する日時を設定します。

   ![](assets/using-bulk-send-sales-email-in-salesforce-3.png)

## Salesforce Classic での一括メールの送信 {#sending-bulk-email-in-salesforce-classic}

1. Salesforce で、 **リード/連絡先** タブをクリックします。

1. 「表示」ドロップダウンで、電子メールを送信するリード/連絡先の目的のビューを選択し、「 」をクリックします **移動**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-4.png)

   >[!TIP]
   >
   >新しいビューを作成するには、「新しいビューを作成」をクリックし、セールスキャンペーンに追加するユーザーのリストを絞り込むために使用可能なフィルターを設定します。

1. 目的のリードまたは連絡先のリストを選択し、 **セールスメールの送信** 」ボタンをクリックします。

1. アクションの作成ウィンドウに移動し、作成ウィンドウで選択した受信者が表示されます。

1. アクション作成ウィンドウエディターに挿入するテンプレートを選択するか、カスタムメールを作成します。

   ![](assets/using-bulk-send-sales-email-in-salesforce-6.png)

   >[!TIP]
   >
   >用途 [ピンされたカテゴリ](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} お気に入りの電子メールテンプレートに容易にアクセスできるようにします。

   **オプションの手順**:動的フィールドのパーソナライゼーションをプレビューするには、 **ダイナミックフィールドをプレビュー** 」ボタンをクリックします。

   >[!TIP]
   >
   >すべての受信者用にテンプレートをカスタマイズする場合は、一括作成サイドバーの「すべての受信者」オプションをクリックすると、すべての受信者の E メールを同時に編集できます。 特定の E メールを変更する場合は、一括作成サイドバーで受信者の名前または E メールをクリックします。 個々の E メールに変更を加え、「すべての受信者」を選択して変更を加えると、「すべての受信者」に加えた変更は、個々の E メールに加えた変更を上書きします。

1. 選択 **送信** E メールを即座に送信する場合、または **スケジュールを設定** ：電子メールを送信する日時を設定します。
