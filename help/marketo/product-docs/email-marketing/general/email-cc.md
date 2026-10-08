---
unique-page-id: 17727995
description: Marketoの電子メール CC オプションについて説明します。 コンプライアンスや可視性のために必要に応じて、CC受信者をメールに追加しましょう。
title: メール CC
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
feature: Email Editor
TQID: 'https://experienceleague.adobe.com/gshenY7XsQYoWMkkrHQROoSu6uqtxUFxSsKSOLPPCAU'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: eeae636f-f283-4051-94f0-4d74945464fb
    internal-label: Email Editor
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 75%
---
# メール CC {#email-cc}

メール CC を使用すると、Marketo を通じて送信される特定のメールに CC 受信者を含めることができます。

この機能は、メールの送信方法（バッチまたはトリガーキャンペーン）に関係なく、すべての Marketo メールアセットで使用できます。 CC の受信者は、選択された Marketo の人物に送信されたメールの正確なコピーを受け取ります。 エンゲージメントアクティビティ（開封数、クリック数など） メールの「宛先」行にMarketo ユーザーのアクティビティログが記録されます。 ただし、配信アクティビティ（送信、配信、ハードバウンスなど） 「ソフトバウンス」 _以外の_&#x200B;は、**not**&#x200B;登録します。これは、MarketoがMarketo ユーザーの配信イベントとCC受信者を区別できないためです。 Marketo で一度に CC できるのは最大 10 万人までです。 スマートリストが100kを超え、すべてのユーザーにCCを付与することが不可欠な場合は、リストを分割することをお勧めします。

>[!NOTE]
>
>メール CC は A/B テストで使用するようには設計されていません。 いずれにしても、必要に応じて使用できますが、技術的にサポートされていないため、Marketo サポートではトラブルシューティングを支援できません。

## メール CC の設定 {#set-up-email-cc}

1. マイ Marketo で、「**[!UICONTROL 管理]**」をクリックします。

   ![](assets/one.png)

1. ツリーで、「**[!UICONTROL メール]**」を選択します。

   ![](assets/two.png)

1. 「**[!UICONTROL メール CC 設定を編集]**」をクリックします。

   ![](assets/three.png)

1. 最大 25 個の Marketo リードまたは会社フィールド（「メール」タイプ）を選択して、メール内で CC アドレスとして使用できるようにします。 終了したら「**保存**」をクリックします。

   ![](assets/four.png)

## メール CC の使用 {#using-email-cc}

1. メールを選択して、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/five.png)

1. 「**[!UICONTROL メール設定]**」をクリックします。

   ![](assets/six.png)

1. CC に使用するフィールドを選択します。 _メール 1 通につき 5 つまでの制限があります_。 この例では、リード所有者CCにのみ。 終了したら「**保存**」をクリックします。

   ![](assets/seven.png)

   それくらい簡単です！ 上記の例では、メールを送信する際に、選択した受信者のリード所有者が CC されます。

   >[!NOTE]
   >
   >「CC」フィールドに無効なメールアドレスが入力されている場合は、そのメールアドレスはスキップされます。

   素早く識別できるように、メールの概要ビューには、どのメール CC フィールドが選択されているかが表示されます。

   ![](assets/eight.png)

   メールが承認されたが、Marketo 管理者がメールの送信前に 1 つ以上の CC フィールドを無効にした場合、**これらのユーザーはメールを受信しません**。 このシナリオでは、メールの概要ビューで、承認後から送信前の間に無効にされたフィールドがグレー表示されます。

   ![](assets/removal.png)

   >[!NOTE]
   >
   >また、上記のエラーは、メールのドラフトのメール設定セクションにも表示されます。

## 送信後 {#after-the-send}

* CC の受信者がメール内のトラッキングされたリンクをクリックすると、（他のすべてのエンゲージメントアクティビティと同様に）クリックアクティビティがメールのメイン受信者に関連付けられます。 また、クリックスルーして Marketo の web トラッキングコード（munchkin.js）を含むページに移動すると、メイン受信者として Cookie に紐付けられる場合があります。

>[!TIP]
>
>メールで[一部またはすべてのトラッキングリンクを無効にする](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md)オプションがあります。

* メールキャンペーンの実行後、「メールを送信」アクティビティには、メールの各受信者に含まれるすべての CC アドレスのリストが含まれます。 購読解除により CC アドレスがスキップされた場合は、その旨がアクティビティにも記録されます。
* 購読解除リンクと購読解除ページは、CC されたメールでも通常どおり機能します。 これにより、CC の受信者は、希望すれば（スパム対策規制に準拠して）問題なく購読解除でき、この操作の記録が Marketo データベースに保存されます。
* Marketo データベースで登録解除済みとしてリストされているユーザーは、CC 経由でメールを受信&#x200B;**しません**。
