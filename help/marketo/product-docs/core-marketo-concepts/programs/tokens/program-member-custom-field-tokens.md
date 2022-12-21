---
unique-page-id: 1147114
description: プログラムメンバーカスタムフィールドトークン - Marketo ドキュメント - 製品ドキュメント
title: プログラムメンバーカスタムフィールドトークン
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
source-git-commit: 30f56d93dfd5a600ef3ea75d352ede12c6104940
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 97%

---

# プログラムメンバーカスタムフィールドトークン {#program-member-custom-field-tokens}

## プログラムメンバーカスタムフィールドのトークンサポート {#token-support-for-program-member-custom-fields}

プログラムメンバーカスタムフィールド機能の背後で、トークンフレームワークのプログラムメンバーカスタムフィールドに対するサポートが拡張されています。

PMCF トークンは、トークンファミリーのメンバードメインでサポートされます。

メンバートークンは、プログラムメンバーの範囲のフィールドに使用されます。現状では、メンバートークンは、統合サービスパートナーから一意の値を挿入するためにも使用されます。`{{member.webinar url}}` トークンは、サービスプロバイダーによって生成されたユーザーの一意の確認 URL を自動的に解決します。{{member.registration code}} は、サービスプロバイダーから提供された登録コードに解決されます。

>[!NOTE]
>
>* プログラムメンバーカスタムフィールドは、プログラムのコンテキストでのみ使用できます。
>* プログラムメンバーカスタムフィールドトークンは、メールのプリヘッダー、待機ステップの日付トークン、スニペットでは使用できません。
>* メンバートークンでは、プログラムメンバーステータスはサポートされていません。


## アセットでのプログラムメンバーカスタムフィールドトークンの使用 {#using-program-member-custom-field-tokens-in-assets}

プログラムメンバーカスタムフィールドトークンは、電子メール、ランディングページ、SMS メッセージ、プッシュ通知、web フックに挿入できます。

**メール**

1. 目的のメールを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-1.png)

1. 「トークンを挿入」アイコンをクリックします。

   ![](assets/program-member-custom-field-tokens-2.png)

1. 目的のプログラムメンバーカスタムフィールドトークンを検索して選択し、デフォルト値を入力して、「**挿入**」をクリックします。

   ![](assets/program-member-custom-field-tokens-3.png)

1. 「**保存**」をクリックします。

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>忘れずにメールを承認してください。

**ランディングページ**

1. ランディングページを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >ランディングページデザイナーが新しいウィンドウで開きます。

1. トークンを追加するリッチテキストボックスをダブルクリックします。

   ![](assets/program-member-custom-field-tokens-6.png)

1. トークンを挿入する場所をクリックし、「トークンを挿入」アイコンをクリックします。

   ![](assets/program-member-custom-field-tokens-7.png)

1. 目的のトークンを見つけて選択します。

   ![](assets/program-member-custom-field-tokens-8.png)

1. デフォルト値を入力し、「**挿入**」をクリックします。

   ![](assets/program-member-custom-field-tokens-9.png)

1. 「**保存**」をクリックします。

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. 目的の SMS を選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-11.png)

1. 「**`{{ Token`**」ボタンをクリックします。

   ![](assets/program-member-custom-field-tokens-12.png)

1. 目的のプログラムメンバーカスタムフィールドトークンを検索して選択します。デフォルト値を入力し、「挿入」をクリックします。

   ![](assets/program-member-custom-field-tokens-13.png)

1. 「SMS アクション」ドロップダウンをクリックし、「**承認して閉じる**」を選択します。

   ![](assets/program-member-custom-field-tokens-14.png)

**プッシュ通知**

1. 目的のプッシュ通知を選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-15.png)

1. 「**プッシュ通知**」をクリックします。

   ![](assets/program-member-custom-field-tokens-16.png)

1. エディターでメッセージをクリックし、「`{{`」ボタンをクリックしてトークンセレクターを取得します。

   ![](assets/program-member-custom-field-tokens-17.png)

1. 目的のプログラムメンバーカスタムフィールドトークンを検索して選択します。デフォルト値を入力し、「**挿入**」をクリックします。

   ![](assets/program-member-custom-field-tokens-18.png)

1. 「**完了**」をクリックして、保存して終了します（または「**次へ**」をクリックして最初にレビューします）。

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>プログラムのメンバーのプログラムメンバーカスタムフィールドに値がない場合、トークンはデフォルト値に置き換えられます（指定されている場合）。

## キャンペーンでのプログラムメンバーカスタムフィールドトークンの使用 {#using-program-member-custom-field-tokens-in-campaigns}

プログラムメンバーカスタムフィールドトークンは、次の場所で使用できます。

* タスクの作成
* Microsoft でのタスクの作成
* 注目のアクション
* データ値の変更フローアクション
* Web フック
