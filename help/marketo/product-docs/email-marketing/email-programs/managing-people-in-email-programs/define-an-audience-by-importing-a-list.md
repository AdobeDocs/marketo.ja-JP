---
unique-page-id: 1900597
description: リストインポートによる対象ユーザーの定義 - Marketo ドキュメント - 製品ドキュメント
title: リストインポートによる対象ユーザーの定義
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '372'
ht-degree: 100%

---

# リストインポートによる対象ユーザーの定義 {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[メールプログラム向け新規メールの作成](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

メールプログラムを作成したら、メールを送信する相手を指定します。それには、[スマートリストを作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)するか、リストをインポートします。ここでは、リストをインポートする方法を説明します。

>[!NOTE]
>
>対象ユーザーの指定は、メールプログラムが承認されていない状態でのみ機能します。
>
>インポートされる日付／時間フィールドはすべて、アメリカの中央時間帯として処理されます。日付／時間フィールドが異なるタイムゾーンに指定されている場合、Excel の関数を用いて中央時間帯（アメリカ／シカゴ）に変換することができます。

1. 「**マーケティングアクティビティ**」に移動します。

   ![](assets/login-marketing-activities-1.png)

1. メールプログラムを選択し、「オーディエンス」タイルの下部にある「リストをインポート」をクリックします。

   ![](assets/importlist.png)

1. リストをインポートウィンドウが開いたら、「**参照**」をクリックして、インポートするファイルを選択します。リードのリストを選択したら、「**次へ**」をクリックします。

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >リストが UTF-8、UTF-16、Shift-JIS、EUC-JP のいずれかでエンコードされていて、ファイルサイズが 50MB を超えていないことを確認します。

1. ファイル内のフィールドが正しくマッピングされていることを確認し、「**次へ**」をクリックします。

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo は、それ以降のインポートで使用できるように、このマッピングを記憶します。

1. リストの「**名前**」を入力し、「**インポート**」をクリックします。

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. インポートが完了したら、メインのプログラムタブに戻ります。ここで、条件を満たすリードの数を確認します。

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**定義**
>
>「ブロック済み」の数に気づきましたか？この数は、条件を満たすリードのうち、以下の理由によりメールを送信できないサブセットを表します。
>
>* 登録解除
>* マーケティングを中断したリード
>* ブロックリスト掲載
>* メール無効
>* 空のメール

>
>数字をクリックすると、このメール配信からブロックされた対象ユーザーの詳細なリストが表示されます。
>
>**オーディエンス**&#x200B;タイルの「![--](assets/image2014-10-23-16-3a32-3a36-1.png)」ボタンを使用して、スマートリストの条件に基づいて、メールの受信に適合する人数を確認します。このリード数からブロック済みリード数を差し引いて、メールを受信するリード総数を算出します。

>[!TIP]
>
>リストのインポートが完了するまで待つ必要はありません。必要であれば、別の作業を続けることができます。

簡単ですね。次に、これらのリードに送信するために、既存のメールを選択するか、新規メールを作成するかを選択します。

>[!MORELIKETHIS]
>
>* [既存のメールの選択](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [メールプログラム向け新規メールの作成](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

