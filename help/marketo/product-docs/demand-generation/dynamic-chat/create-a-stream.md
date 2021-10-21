---
description: Stream Marketo ドキュメントの作成-製品マニュアル
title: ストリームの作成
hide: true
hidefromtoc: true
source-git-commit: 1022d3eaf4ee4a1686c5d8ae3168ee0197776289
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 1%

---

# ストリームの作成 {#create-a-stream}

__ 作成できるストリームの組み合わせは多数あります。次の例では、marketer がユーザーに製品についての質問がある場合に、サイトのビジターに説明します。 「はい」をクリックすると、訪問者は予定を設定することができます。 「いいえ」を選択した場合は、後で通信するためにメーリングリストに参加するかどうかをビジターに通知します。 この目的は、予定を設定するか、またはビジターの電子メールを収集することです。

1. [ダイアログボックスを作成したら、 ](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#create-a-new-dialogue) 「 **ストリーミングデザイナー** 」タブをクリックします。

   ![](assets/create-a-stream-1.png)

1. 質問カードをドラッグ &amp; ドロップします。

   ![](assets/create-a-stream-2.png)

1. 「Chatbot 応答」に、ご質問の内容を入力します。

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >Poke はデフォルトでオンに設定されています。これにより、ビジターは、これをクリックすることなく、チャットアイコンの隣に表示されます。

1. ユーザーによる応答を入力し、「保存」をクリックし **** ます。

   ![](assets/create-a-stream-4.png)

1. 「はい」を選択した場合は予定を設定します。その場合は、このオプションの下に、その予定スケジューラカードをドラッグします。

   ![](assets/create-a-stream-5.png)

1. 右側の列にある「保存」をクリックし **** ます。

   ![](assets/create-a-stream-6.png)

1. このような場合は、目的のカードを予定表の上にドラッグします。

   ![](assets/create-a-stream-7.png)

1. 目的の名前を指定します (または既存の目標を選択して、「保存」をクリックし **** ます)。

   ![](assets/create-a-stream-8.png)

1. 「No」については、宛先リストに参加するかどうかを確認する必要があります。そのオプションの下にある場合は、別の質問カード上をドラッグします。

   ![](assets/create-a-stream-9.png)

1. 応答を入力して、ビジターに応答の選択肢を追加します。 終了したら「**保存**」をクリックします。

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >「応答を追加」ボタンをクリックすると、応答を追加することができ **** ます。

1. 「はい」をクリックすると、情報キャプチャカード上にドラッグして、ビジターの電子メールを集めることができます。

   ![](assets/create-a-stream-11.png)

1. **「タイプ** 」ドロップダウンをクリックして、「電子メール」を選択し **** ます。

   ![](assets/create-a-stream-12.png)

1. Chatbot メッセージとプレースホルダーを入力します。 属性が Marketo の適切なフィールドにマップされていることを確認し、「保存」をクリックし **** ます。

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>タイプ</strong></td>
     <td>キャプチャする情報のタイプ。「電話」、「テキスト」、「電子メール」などの情報を入力します。</td>
    </tr>
    <tr>
     <td><strong>Chatbot メッセージ</strong></td>
     <td>ユーザーが情報を入力するよう求めるメッセージが表示されます。</td>
    </tr>
    <tr>
     <td><strong>プレースホルダー</strong></td>
     <td>入力する情報をユーザーが確認できるようにするためのサンプルテキスト</td>
    </tr>
    <tr>
     <td><strong>応答を属性にマップ</strong></td>
     <td>Vistor の応答と、Marketo サブスクリプションの担当記録の該当するフィールドとの同期を行うことができます。</td>
    </tr>
   </table>

1. お客様の電子メールが収集されてから、下の「情報の取得」にドラッグします。

   ![](assets/create-a-stream-14.png)

1. 目的の名前を指定します (または既存の目標を選択して、「保存」をクリックし **** ます)。

   ![](assets/create-a-stream-15.png)

1. 「いいえ」の場合は、応答を必ず追加してください。 メッセージカードをそのオプションの下にドラッグします。

   ![](assets/create-a-stream-16.png)

1. メッセージを入力し、「保存」をクリックし **** ます。

   ![](assets/create-a-stream-17.png)

1. ダイアログを acivate する場合は、「パブリッシュ」をクリックし **** ます。

   ![](assets/create-a-stream-18.png)

>[!NOTE]
>
>「パブリッシュ」をクリックする前に、既にターゲット URL が入力されているかどうかを確認してください [ ](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#target) 。

>[!MORELIKETHIS]
>
>[「?」](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md)
