---
description: Stream Designer - Marketoドキュメント — 製品ドキュメント
title: ストリームデザイナー
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
source-git-commit: 38e65efc50f7f5e7a2a3dbe91035327007475721
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 86%

---

# ストリームデザイナー {#stream-designer}

_多数の_&#x200B;ストリームの組み合わせを作成できます。この記事には、マーケターがサイト訪問者に製品に関する質問をする例が含まれています。 「はい」の場合、訪問者は予定をスケジュールできます。「いいえ」の場合、訪問者には、今後の通信用にメーリングリストに参加するオプションが与えられます。目標は、予定をスケジュールするか、訪問者のメールを収集することです。

## ストリームデザイナーカード {#stream-designer-cards}

ストリームデザイナーには、チャット会話を形成するために追加できる複数のカードが含まれています。

<table>
 <tr>
  <td><strong>メッセージ</strong></td>
  <td>応答を必要としない文を作成する場合に使用します（例：「こんにちは。コード「SAVE25」を使用すると、今日は全品が 25% オフです）。
</td>
 </tr>
 <tr>
  <td><strong>質問</strong></td>
  <td>複数選択の質問に対して、利用可能な回答を提供する場合に使用します（例：どのような車に興味がありますか？応答 = SUV、コンパクト、トラックなど）。</td>
 </tr>
 <tr>
  <td><strong>情報取得</strong></td>
  <td>情報を収集する場合に使用します。選択できる 3 つのフィールドは、「電子メールアドレス」、「電話番号」、「テキスト」（訪問者が独自のメッセージを書き込むことができる）です。</td>
 </tr>
 <tr>
  <td><strong>予定スケジューラー</strong></td>
  <td>訪問者に、フォローアップをスケジュールするために使用可能な日付のカレンダーを提供します。カレンダーの可用性は<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">次のエージェント</a>を反映します。</td>
 </tr>
 <tr>
  <td><strong>ゴール</strong></td>
  <td>訪問者に表示されないカードはこれだけです。特定のチャット内で目標を達成した時点を決定する必要があります（例：訪問者のメールを収集することが目標の場合は、ストリームの情報キャプチャの直後に目標カードを配置します）。</td>
 </tr>
</table>

## ストリームの作成 {#create-a-stream}

1. 以下を実行した後： [ダイアログを作成しました](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md)、 **ストリームデザイナー** タブをクリックします。

   ![](assets/create-a-stream-1.png)

1. 質問カードをドラッグ＆ドロップします。

   ![](assets/create-a-stream-2.png)

1. 「チャットボットの回答」で、質問を入力します。

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >「Poke」はデフォルトでオンに設定されており、訪問者がチャットアイコンをクリックしなくてもチャットアイコンの横に開始の質問が表示されます。

1. ユーザーの回答を入力し、「**保存**」をクリックします。

   ![](assets/create-a-stream-4.png)

1. 「はい」の場合は、予定をスケジュールしたいので、下のオプションの予定スケジューラーカードにドラッグします。

   ![](assets/create-a-stream-5.png)

1. 右側の列で、「**保存**」をクリックします。

   ![](assets/create-a-stream-6.png)

1. これは目標なので、予定スケジューラーの下にある目標カードをドラッグします。

   ![](assets/create-a-stream-7.png)

1. 目標に名前を付け（または既存のものを選択）、「**保存**」をクリックします。

   ![](assets/create-a-stream-8.png)

1. 「いいえ」の場合は、ユーザーがメーリングリストに登録するかどうかを確認したいので、その下に、別の質問カードをドラッグします。

   ![](assets/create-a-stream-9.png)

1. 回答を入力し、訪問者の回答を追加します。終了したら「**保存**」をクリックします。

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >「**回答を追加**」をクリックすると、更に回答を追加できます。

1. 「はい」の回答の下で、情報キャプチャカードをドラッグして、訪問者のメールを収集できます。

   ![](assets/create-a-stream-11.png)

1. **タイプ**&#x200B;ドロップダウンをクリックして、「**メール**」を選択します。

   ![](assets/create-a-stream-12.png)

1. チャットボットのメッセージとプレースホルダーを入力します。属性が Marketo の適切なフィールドにマッピングされていることを確認し、「**保存**」をクリックします。

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>タイプ</strong></td>
     <td>取得する情報のタイプ（電話、テキスト、メール）</td>
    </tr>
    <tr>
     <td><strong>チャットボットメッセージ</strong></td>
     <td>情報の提供を促すメッセージが訪問者に表示されます。</td>
    </tr>
    <tr>
     <td><strong>プレースホルダー</strong></td>
     <td>訪問者が何を入力するかを確認するのに役立つサンプルテキスト。</td>
    </tr>
    <tr>
     <td><strong>回答を属性にマッピング</strong></td>
     <td>訪問者の回答を、Marketo サブスクリプション内のユーザーレコードの対応するフィールドに同期できます。</td>
    </tr>
   </table>

1. メールの収集が目標なので、情報キャプチャの下にゴールカードをドラッグします。

   ![](assets/create-a-stream-14.png)

1. 目標に名前を付け（または既存のものを選択）、「**保存**」をクリックします。

   ![](assets/create-a-stream-15.png)

1. 「いいえ」の場合は、必ず回答を追加してください。メッセージカードをそのオプションの下にドラッグします。

   ![](assets/create-a-stream-16.png)

1. メッセージを入力して「**保存**」をクリックします。

   ![](assets/create-a-stream-17.png)

1. を選択します。 **プレビュー** を切り替えて、ダイアログをプレビューします。

   ![](assets/create-a-stream-18.png)

1. ダイアログをアクティブにする準備が整ったら、 **公開**.

   ![](assets/create-a-stream-19.png)

>[!NOTE]
>
>「公開」をクリックする前に、必ず[ターゲット URL](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#target) を入力したことを確認してください。

>[!MORELIKETHIS]
>
>* [ダイアログの作成](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [オーディエンス条件](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target=&quot;_blank&quot;}
>* [レポート](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

