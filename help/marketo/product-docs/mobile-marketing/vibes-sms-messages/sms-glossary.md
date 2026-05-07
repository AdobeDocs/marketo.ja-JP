---
description: Marketo Engageで使用されるVibes SMSの一般的な用語について説明します。 この用語集は、顧客獲得や購読リスト、ショートコードなどに使用できます。
title: SMS 用語集
feature: Mobile Marketing
exl-id: 0c23ca9f-f994-42ae-bd72-7d37289b7a94
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 1%

---

# SMS 用語集 {#sms-glossary}

以下は、Vibes SMS メッセージをMarketo Engageで使用する際に発生する一般的な用語です。

<table>
<thead>
  <tr>
    <th>用語</th>
    <th>定義</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>獲得キャンペーン</td>
    <td>購読リストの新規登録者を獲得するために作成されたキャンペーン。 Marketoのweb フォームやキーワードを通じて、オーディエンスを獲得キャンペーンに追加できます。</td>
  </tr>
  <tr>
    <td>Campaign Manager</td>
    <td>Vibes プラットフォームのCampaign Managerでは、購読リストと獲得キャンペーンを設定できます。 Vibesのプラットフォームライセンスを完全に保有しているユーザーは、他の種類のキャンペーンにもアクセスできます。</td>
  </tr>
  <tr>
    <td>企業キー</td>
    <td>company_keyは、プラットフォームアカウントの一意の英数字IDです。 Vibes プラットフォームに複数の会社アカウント（子アカウントなど）がある場合は、複数のcompany_keysがある可能性があります。 Marketo Engageの各インスタンスは、1つのVibes company_keyにのみマッピングできます。</td>
  </tr>
  <tr>
    <td>CTA（call to action）</td>
    <td>定期的なテキストメッセージプログラムや購読リストに加入者を獲得するためのデジタルまたは物理的なサイネージまたは口頭スクリプト。 オンライン、ソーシャルメディア、電子メール、印刷物などに配置できます。</td>
  </tr>
  <tr>
    <td>カスタムショートドメイン</td>
    <td>Vibes リンク短縮サービスを使用している場合、短縮URLはデフォルトでVibes短いURL https://vbs.cm/xxxxxxの下に表示されます。 カスタムショートドメインとは、自社ブランドに固有のドメインのことです。 <a href="https://developer-platform.vibes.com/docs/creating-a-custom-short-domain"> カスタムショートドメインの詳細</a>。<p>
    これは、Vibes プラットフォームから送信されるメッセージ、特に獲得キャンペーンメッセージとショートコードのデフォルトメッセージにのみ適用されます。<p>
    Marketo プログラムにクリックデータを含めるには、Marketo URL短縮サービスをお勧めします。</td>
  </tr>
  <tr>
    <td>デフォルトメッセージ</td>
    <td>HELP、STOP、および認識されないメッセージリクエストに返信するための短いコードの必須メッセージ。</td>
  </tr>
  <tr>
    <td>接続解除</td>
    <td>切断は、携帯電話番号が通信事業者ネットワークから削除されることでオプトアウトの一形態です。 アカウントが完全に閉鎖された、前払いのアカウントが資金を使い果たした、またはその他の不明な理由で番号がキャリア ネットワークから削除された、などの理由があります。 切断され、別の携帯電話会社にポートされていない携帯電話番号は、Vibes プラットフォームのすべての購読リストから登録解除されます。</td>
  </tr>
  <tr>
    <td>ダブルオプトイン</td>
    <td>潜在的な購読者が、「Y」などの応答コマンドを使用して購読リストに追加することへの同意を確認する必要がある取得方法または郵便番号。 ダブルオプトインプロンプトを使用すると、州および連邦のテキストメッセージのガイドラインに準拠できます。</td>
  </tr>
  <tr>
    <td>イベント</td>
    <td>イベントは、Vibes プラットフォームに送信でき、メッセージ送信を含むAPI トリガーのアクションをトリガーするために使用される定義済みのオカレンスです。 各イベントには、イベントに固有のデータが含まれます。これには、event_typeが含まれ、対応するAPI トリガーのメッセージキャンペーンを判断するために使用されます。 Event APIは、Marketo EngageのWebhookを介してトリガーできます。 詳しくは、<a href="https://developer-platform.vibes.com/reference/event-api"> イベント API リファレンス </a>を参照してください。</td>
  </tr>
  <tr>
    <td>キーワード</td>
    <td>モバイルエクスペリエンスを開始するために、消費者が短いコードに送信した短い単語または英数字の文字列。</td>
  </tr>
  <tr>
    <td>ロングコード（10DLC）</td>
    <td>ブランドと消費者の間で双方向メッセージを送信する送信者ID。 米国の長いコードは10桁の数字です。</td>
  </tr>
  <tr>
    <td>MDN</td>
    <td>モバイルディレクトリ番号、またはユーザーの電話番号。 Marketoでは、MDNと携帯電話の番号は一意の識別子ではありません。</td>
  </tr>
  <tr>
    <td>Mobile Database</td>
    <td>Mobile Databaseは、Vibesが加入者データを保存するデータベースです。 各購読者には、携帯電話番号と関連するカスタムフィールドが入力される一意の「個人レコード」があります。</td>
  </tr>
  <tr>
    <td>参加者</td>
    <td>モバイルプログラムで1つ以上のモバイルインタラクション（テキストメッセージの送信など）を持っているが、サブスクリプションリストを購読していない人物。</td>
  </tr>
  <tr>
    <td>顧客レコード</td>
    <td>個人レコードとは、特定の携帯電話番号のデータを集めたものです。 各人物レコードには、識別用に一意のperson_keyも割り当てられます。 Marketo IDは、external_person_id フィールドを使用してVibesにリンクされます。 個人レコードについて詳しくは、<a href="https://developer-platform.vibes.com/reference/person-api">Vibes Person API ドキュメント </a>を参照してください。</td>
  </tr>
  <tr>
    <td>ショートコード</td>
    <td>ブランドと消費者の間で双方向メッセージを送信する送信者ID。 米国のショートコードは5 ～ 6桁の数字です。 カナダのショートコードは4～6桁の数字です。 Marketo LaunchPointとVibesの連携では、1つのインスタンスにつき1つのショートコードがサポートされます。</td>
  </tr>
  <tr>
    <td>SMS</td>
    <td>ショートメッセージサービス： これはテキストのみを含むメッセージです。</td>
  </tr>
  <tr>
    <td>購読リスト</td>
    <td>プログラムから定期的なメッセージを受け取ることに同意したモバイル番号（および対応する個人レコード）のリスト。</td>
  </tr>
  <tr>
    <td>購読者</td>
    <td>購読リストに登録されている携帯電話番号。</td>
  </tr>
  <tr>
    <td>Vibes Platform</td>
    <td>キャンペーンを管理するためにログインするweb サイト。 <a href="https://nexus.us.vibes.com/">https://nexus.us.vibes.com/</a>に移動して、Vibes プラットフォームにアクセスします。</td>
  </tr>
</tbody>
</table>
