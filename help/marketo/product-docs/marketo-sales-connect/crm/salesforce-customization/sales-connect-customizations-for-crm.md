---
unique-page-id: 14745793
description: CRM 用の Sales Connect のカスタマイズ - Marketo ドキュメント - 製品ドキュメント
title: CRM 用の Sales Connect のカスタマイズ
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: dbf058714f6c4e6003c5a64d1048ac8a47931a0f
workflow-type: ht
source-wordcount: '690'
ht-degree: 100%

---

# CRM 用の Sales Connect のカスタマイズ {#sales-connect-customizations-for-crm}

以下のフィールドとボタンは、Salesforce CRM のメタデータ API によって作成されます。フィールドを作成したら、管理者は、CRM でページのレイアウトを設定して公開する必要があります。手順は[こちら](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)にあります。

## Salesforce でのカスタマイズのインストール方法 {#how-to-install-customizations-in-salesforce}

1. Sales Connect で、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/one.png)

1. 管理設定で、**Salesforce** を選択します。

   ![](assets/two.png)

1. 「**Marketo Sales Connect のカスタマイズ**」をクリックします。

   ![](assets/three.png)

1. 「**Salesforce に接続**」をクリックします。

   ![](assets/four.png)

1. Salesforce にログインします。

   ![](assets/five.png)

## Salesforce カスタマイズのアップデート {#update-salesforce-customization}

Salesforce カスタマイズパッケージのアップデートには、機能強化とバグ修正が含まれます。アップデートが利用可能かどうか、またはアップデートを実行するには、次の手順に従います。

>[!NOTE]
>
>**管理者権限が必要。**

1. [Web アプリケーション](https://www.toutapp.com)で、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. 管理設定で、**Salesforce** をクリックします。

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. アップデートが利用可能な場合は、Sales Connect カスタマイズカードが表示されます。「**カスタマイズをアップデート**」をクリックします。

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. 「**アップグレード**」をクリックします。

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. アップデートがインストールされるまで待ちます。必要なバージョン番号の数に応じて、インストール時間は異なります。

   ![](assets/sales-connect-customizations-for-crm-10.png)

完了すると、カードに「Sales Connect のカスタマイズは最新です」と表示されます。

![](assets/sales-connect-customizations-for-crm-11.png)

## カスタムアクティビティフィールド {#custom-activity-fields}

Marketo は、新しいフィールドの作成を検出し、1 回限りのデータのバックフィル、再マッピングおよび&#x200B;**新しい**&#x200B;フィールドへの値の継続的な同期を実行します。古いフィールドは更新されません。

<table><thead>
  <tr>
    <th>フィールド名</th>
    <th>説明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE 電話ローカルプレゼンス ID</td>
    <td>ユーザは、MSE 電話から電話をかける際に、「ローカルプレゼンス」をオプションとして選択できます。着信電話は、受信者のローカル番号を表示します。</td>
  </tr>
  <tr>
    <td>MSE 電話録音 URL</td>
    <td>通話は録音され、録音のリンクはここに記録されます。</td>
  </tr>
  <tr>
    <td>MSE キャンペーン</td>
    <td>取引先責任者／リードがメンバーの MSE キャンペーンの名前を記録します。</td>
  </tr>
  <tr>
    <td>MSE キャンペーン URL</td>
    <td>MSE で作成されたキャンペーンの URL を記録します。これをクリックすると、MSE web アプリでキャンペーンが開きます。</td>
  </tr>
  <tr>
    <td>MSE キャンペーンの現在のステップ</td>
    <td>取引先責任者／リードがキャンペーンの一部である場合、このフィールドには、リード／取引先責任者が現在参加しているステップの名前が記録されます。</td>
  </tr>
  <tr>
    <td>MSE メール添付ファイルの閲覧</td>
    <td>ファイルが添付されたメールが送信され、受信者が添付ファイルを閲覧した場合に、データを記録します。</td>
  </tr>
  <tr>
    <td>MSE メールのクリック</td>
    <td>受信者がメール内のリンクをクリックしたときにチェックマークを記録します。</td>
  </tr>
  <tr>
    <td>MSE メールの返信</td>
    <td>受信者がメールに返信したときにチェックマークを記録します。</td>
  </tr>
  <tr>
    <td>MSE メールのステータス</td>
    <td>メールが送信済み／処理中／バウンスされたかどうかを表示します（バウンスメールのトラッキングは、使用する配信チャネルに依存します）。</td>
  </tr>
  <tr>
    <td>MSE メールテンプレート</td>
    <td>リード／取引先責任者に送信されたメールで使用された MSE テンプレートの名前を記録します。</td>
  </tr>
  <tr>
    <td>MSE メールテンプレート URL</td>
    <td>MSE で作成されたテンプレートの URL を記録します。これをクリックすると、MSE web アプリでテンプレートが開きます。</td>
  </tr>
  <tr>
    <td>MSE メール URL</td>
    <td>この URL をクリックすると、MSE でコマンドセンターが開き、「リード詳細表示の履歴」タブが前面表示され、送信されたメールを確認できます。</td>
  </tr>
  <tr>
    <td>MSE メールの表示</td>
    <td>受信者がメールを表示したときにチェックマークを記録します。</td>
  </tr>
</tbody></table>

## ログフィールドのロールアップ {#roll-up-logging-fields}

<table><thead>
  <tr>
    <th>フィールド名</th>
    <th>説明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE - 最終マーケティングエンゲージメント</td>
    <td>マーケティングから最後に入ってきたエンゲージメント。</td>
  </tr>
  <tr>
    <td>MSE - 最終マーケティングエンゲージメント日</td>
    <td>マーケティングからのエンゲージメントのタイムスタンプ。</td>
  </tr>
  <tr>
    <td>MSE - 最終マーケティングエンゲージメントの説明</td>
    <td>エンゲージメントの説明。</td>
  </tr>
  <tr>
    <td>MSE - 最終マーケティングエンゲージメントソース</td>
    <td>マーケティングエンゲージメントのソース。</td>
  </tr>
  <tr>
    <td>MSE - 最終マーケティングエンゲージメントのタイプ</td>
    <td>エンゲージメントのタイプ。</td>
  </tr>
  <tr>
    <td>MSE - セールスによる最終アクティビティ</td>
    <td>セールスチームが最後に実行した外部アクティビティ。</td>
  </tr>
  <tr>
    <td>MSE - 最終返信</td>
    <td>セールスメールに最後に返信したメール。</td>
  </tr>
  <tr>
    <td>MSE - 現在のセールスキャンペーン</td>
    <td>リード／取引先責任者がメンバーの MSE キャンペーンの名前を記録します。</td>
  </tr>
  <tr>
    <td>MSE - 最終セールスエンゲージメント</td>
    <td>セールスから最後に入ってきたエンゲージメント。</td>
  </tr>
  <tr>
    <td>MSE - オプトアウト</td>
    <td>オプトアウトフィールド。</td>
  </tr>
</tbody></table>

## ボタン {#buttons}

<table><thead>
  <tr>
    <th>ボタン名</th>
    <th>説明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE メールを送信</td>
    <td>Salesforce からセールスメールを送信します。</td>
  </tr>
  <tr>
    <td>MSE キャンペーンに追加</td>
    <td>Salesforce から MSE キャンペーンに追加します。</td>
  </tr>
  <tr>
    <td>MSE にプッシュ</td>
    <td>Salesforce から MSE に取引先責任者をプッシュします。</td>
  </tr>
  <tr>
    <td>MSE で電話</td>
    <td>Salesforce からセールス電話をかけます。</td>
  </tr>
</tbody>
</table>

## 一括アクションボタン {#bulk-action-buttons}

<table><thead>
  <tr>
    <th>ボタン名</th>
    <th>説明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE キャンペーンに追加</td>
    <td>Salesforce から MSE キャンペーンに追加します。</td>
  </tr>
  <tr>
    <td>MSE にプッシュ</td>
    <td>Salesforce から MSE に取引先責任者をプッシュします。</td>
  </tr>
</tbody>
</table>

## ユーザガイド {#user-guides}

[Salesforce の MSE カスタムレポート](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/reports-and-dashboards.pdf)

[Salesforce Classic 用の MSE](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)

[Salesforce Lightning 用の MSE](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/sfdc-guide-lightning.pdf)
