---
description: ランディングページへの SSL の追加 — Marketo ドキュメント — 製品ドキュメント
title: ランディングページへの SSL の追加
hide: true
hidefromtoc: true
feature: Landing Pages
exl-id: 00ec2d91-3d4f-4671-af9d-9750c1642d40
source-git-commit: c7bf6c7ffca16e95f13a7009897bce6fc39a9ffd
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 44%

---

# ランディングページへの SSL の追加 {#add-ssl-to-your-landing-pages}

SSL（Secure Socket Layer）暗号化を使用すると、Marketo Engage インスタンスのすべてのランディングページをセキュリティで保護できます。

Web フォームに入力する場合、または Marketo Engage がホストするランディングページに訪問する場合、デフォルトでは、情報はセキュリティで保護されていないプロトコル（HTTP）を使用して送信されます。会社のポリシーによっては、Marketo に送信される情報を（HTTPS）を使用して保護する必要が生じる場合があります。例えば、`http://info.mydomain.com/` へのアクセスは `https://info.mydomain.com/` になります。

Marketo Engage では、デフォルトで、セキュリティで保護されていない HTTP プロトコルを使用して「訪問した web ページ」と「Web ページのリンクをクリック」を追跡します。独自の証明書でトラッキングリンクを保護したい場合、Marketo に共有されていない別のサーバーを作成させて有効にする必要があります。取引先責任者とのやり取りのあらゆる側面を保護するということは、通常は、ランディングページとトラッキングリンクの両方を保護することを意味します。

## SSL 証明書を有効にする {#enable-ssl-certification}

ランディングページのルールの一部として作成したすべてのドメインエイリアスに SSL を自動的に追加します。

1. 「**管理者**」領域に移動します。

   ![](assets/add-ssl-to-your-landing-pages-1.png)

1. ツリーから **ランディングページ** を選択します。 「**ルール**」タブで「**新規**」ドロップダウンをクリックし、「**新しいドメインエイリアス**」を選択します。

   ![](assets/add-ssl-to-your-landing-pages-2.png)

1. _ドメインエイリアス_ と _デフォルトページ_ を入力します。 「**SSL 証明書を生成**」チェックボックスを選択します。 完了したら「**作成**」をクリックします。

   ![](assets/add-ssl-to-your-landing-pages-3.png)

このドメインの SSL 証明書が自動的に追加されます。

## デフォルトドメインの SSL の有効化 {#enable-ssl-default-domain}

デフォルトドメインの SSL を有効にするには、次の手順に従います。

1. 「**管理者**」セクションで、「**ランディングページ**」を選択します。 _設定_ の横のオレンジ色の **編集** ボタンをクリックします。

   ![](assets/add-ssl-to-your-landing-pages-4.png)

   >[!NOTE]
   >
   >ここでドメイン名を変更することもできます（有効なドメインが必要です）。

1. 「SSL 証明書を生成」チェックボックスを選択し、「保存」をクリックします。

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>* リストの「SSL 証明書」列には、この機能がリリース（DATE）された後に作成されたすべてのドメインエイリアスの証明書ステータスが表示されます。 Marketo サポートを通じてドメインに対して SSL を有効にした場合、証明書は引き続き存在しますが、表には表示されません。 この表は、この記事の手順を使用して追加されたドメインの SSL 証明書のみを反映しています。
>
>* SSL が準備完了状態になるまで、最大 3 分かかる場合があります。 変更を表示するには、ページを更新する必要があります。
