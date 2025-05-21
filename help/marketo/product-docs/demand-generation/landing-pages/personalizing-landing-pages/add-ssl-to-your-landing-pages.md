---
unique-page-id: 2359828
description: ランディングページへの SSL の追加 — Marketo ドキュメント — 製品ドキュメント
title: ランディングページへの SSL の追加
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: fddc2f24d9a66146f567c762305ab2825c2f29ae
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 44%

---

# ランディングページへの SSL の追加 {#add-ssl-to-your-landing-pages}

SSL（Secure Socket Layer）暗号化を使用すると、Marketo Engage インスタンスのすべてのランディングページをセキュリティで保護できます。

Web フォームに入力する場合、または Marketo Engage がホストするランディングページを訪問する場合、デフォルトでは、情報はセキュリティで保護されていないプロトコル（HTTP）を使用して送信されます。会社のポリシーによっては、Marketo に送信される情報を（HTTPS）を使用して保護する必要が生じる場合があります。例えば、`http://info.mydomain.com/` へのアクセスは `https://info.mydomain.com/` になります。

Marketo Engage では、デフォルトで、セキュリティで保護されていない HTTP プロトコルを使用して「訪問した web ページ」と「Web ページのリンクをクリック」を追跡します。独自の証明書でトラッキングリンクを保護したい場合、Marketo に共有されていない別のサーバーを作成させて有効にする必要があります。取引先責任者とのやり取りのあらゆる側面を保護するということは、通常は、ランディングページとトラッキングリンクの両方を保護することを意味します。

## SSL 証明書を有効にする {#enable-ssl-certification}

ランディングページのルールの一部として作成したすべてのドメインエイリアスに SSL を自動的に追加します。

1. 「**管理者**」領域に移動します。

   ![](assets/add-ssl-to-your-landing-pages-1.png)

1. ツリーから&#x200B;**ランディングページ**&#x200B;を選択します。「**ルール**」タブで、「**新規**」ドロップダウンをクリックし、「**新規ドメインエイリアス**」を選択します。

   ![](assets/add-ssl-to-your-landing-pages-2.png)

1. _ドメインエイリアス_&#x200B;と&#x200B;_デフォルトページ_&#x200B;を入力します。「**SSL 証明書を生成**」チェックボックスを選択します。完了したら「**作成**」をクリックします。

   ![](assets/add-ssl-to-your-landing-pages-3.png)

このドメインの SSL 証明書が自動的に追加されます。

## デフォルトドメインの SSL の有効化 {#enable-ssl-default-domain}

デフォルトドメインの SSL を有効にするには、次の手順に従います。

1. 「**管理**」セクションで、「**ランディングページ**」を選択します。「_設定_」の横のオレンジ色の「**編集**」ボタンをクリックします。

   ![](assets/add-ssl-to-your-landing-pages-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >必要に応じて、ここでドメイン名を変更することもできます（有効なドメインが必要です）。

1. 「SSL 証明書を生成」チェックボックスを選択し、「保存」をクリックします。

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>* リスト内の SSL 証明書列には、この機能がリリースされた（2025 年 4 月 25 日（PT））後に作成されたすべてのドメインエイリアスの証明書ステータスが表示されます。 Marketo サポートを通じてドメインに対して SSL を有効にした場合、証明書は引き続き存在しますが、表には表示されません。この表は、この記事の手順を使用して追加されたドメインの SSL 証明書のみを反映しています。
>
>* SSL が準備完了状態になるまで、最長 3 分かかる場合があります。変更を表示するには、ページを更新する必要があります。

## エラー メッセージ {#error-messages}

以下に、エラーメッセージとその定義を示します。

<table><thead>
  <tr>
    <th>エラー</th>
    <th>詳細</th>
  </tr></thead>
<tbody>
  <tr>
    <td><i>ドメインの作成中に予期しないエラーが発生しました。 サポートが必要な場合は、サポートにお問い合わせください。</i></td>
    <td>予期しないエラーが発生しました。 ログとエラーの詳細を収集し、問題をサポートにエスカレーションしてください。</td>
  </tr>
  <tr>
    <td><i>既定のドメインが見つかりませんでした。 サポートが必要な場合は、サポートにお問い合わせください。</i></td>
    <td>デフォルトドメインの検索中に問題が発生しました。 サポートに問い合わせて、調査を依頼してください。</td>
  </tr>
  <tr>
    <td><i>SSL 証明書は既に発行されています。</i></td>
    <td>このカスタムドメインには SSL 証明書が既に存在します。 証明書の有効期限が切れているか、証明書を再発行する必要がない限り、これ以上の操作は必要ありません。</td>
  </tr>
  <tr>
    <td><i>ドメインは、デフォルトドメインにマッピングされません。</i></td>
    <td>カスタムドメインがデフォルトドメインに正しくマッピングされていない。 ドメインマッピング設定を確認し、DNS 設定が正しいデフォルトドメインを指していることを確認してください。</td>
  </tr>
  <tr>
    <td><i>ドメインは既に存在します。</i></td>
    <td>同じ名前のドメインが既に存在します。</td>
  </tr>
  <tr>
    <td><i>ドメインを追加するには、1 回限りの IP 設定が必要です。 セットアップを完了して別のドメインを追加するには、サポートにお問い合わせください。</i></td>
    <td>デフォルトドメインの後の最初のカスタムドメインは、1 回限りの設定を開始する必要があります。 サポートチケットを発行して設定を完了し、完了したらドメインを追加してください。</td>
  </tr>
</tbody></table>

## 注意事項 {#things-to-note}

* **ドメインをMarketo Engageに DNS マッピング**:UI でドメインを追加する前に、[CNAME をMarketo提供のドメインにマッピング ](https://experienceleague.adobe.com/ja/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"} する必要があります。

* **カスタム SSL**：カスタム SSL が必要な場合は、[ サポートチケット ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} を送信してください。 SSL 作成にセルフサービスチェックボックスを使用しないでください。

* **既存の SSL**：ドメインの追加中に、システムは既存の SSL をチェックします。これは、以前に手動で作成された SSL の可能性があります。 この検証が発生した場合は、SSL 作成を選択せずにドメインを作成すると、接続されます。 [ サポートにお問い合わせください ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} 詳細/オプション。

* **初回のトラッキングドメイン**：メールトラッキングリンクドメインを初めて作成する場合は、[Marketo サポート ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} による手動操作が必要です。 同じドメイン内でそれ以降にサブドメインを作成することは、UI で許可されます。

* **Marketo オンプレミスのみ**：現在、この機能はオンプレミスでのみ使用できます。 Marketo Engage on Cloud Services では、[Marketo サポート ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} に連絡して、SSL を設定する必要があります。

* **既存のドメインへの証明書の追加**：既存のドメインへの証明書の追加は、現時点ではサポートされていません。 既存のドメインの場合、または SSL 証明書ボックスを確認しなかった場合、証明書を追加するには、[Marketo サポート ](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} に連絡する必要があります。

* **ドメインの削除**：現時点では、ドメインを削除しても SSL 証明書は自動的には削除されません。 これは、今後のリリースで対処される予定です。
