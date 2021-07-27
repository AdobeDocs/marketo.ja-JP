---
unique-page-id: 1147114
description: プログラムメンバーのカスタムフィールドトークン — Marketoドキュメント — 製品ドキュメント
title: プログラムメンバのカスタムフィールドトークン
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
source-git-commit: 30f56d93dfd5a600ef3ea75d352ede12c6104940
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 3%

---

# プログラムメンバのカスタムフィールドトークン {#program-member-custom-field-tokens}

## プログラムメンバーのカスタムフィールドのトークンのサポート {#token-support-for-program-member-custom-fields}

プログラムメンバーカスタムフィールド機能の背面で、トークンフレームワークのプログラムメンバーカスタムフィールドに対するサポートが拡張されています。

PMCFトークンは、トークン・ファミリのメンバー・ドメインでサポートされます。

「メンバー・トークン」は、「プログラム・メンバー」の範囲のフィールドに使用されます。 現在の状態では、メンバートークンは、統合サービスパートナーから一意の値を挿入するためにも使用されます。 `{{member.webinar url}}` トークンは、サービスプロバイダーによって生成されたユニークな確認URLを自動的に解決します。{{member.registration code}}は、サービスプロバイダーから提供された登録コードに解決されます。

>[!NOTE]
>
>* プログラムメンバのカスタムフィールドは、プログラムのコンテキストでのみ使用できます。
>* プログラムメンバーカスタムフィールドトークンは次の場所では使用できません：電子メールのプリヘッダー、待機ステップの日付トークン、スニペット。
>* メンバートークンでは、プログラムメンバーステータスはサポートされていません。


## アセットでのプログラムメンバーカスタムフィールドトークンの使用 {#using-program-member-custom-field-tokens-in-assets}

プログラムメンバーのカスタムフィールドトークンをEメール、ランディングページ、SMS、プッシュ通知、Webフックに挿入できます。

**メール**

1. 目的の電子メールを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-1.png)

1. 「トークンを挿入」アイコンをクリックします。

   ![](assets/program-member-custom-field-tokens-2.png)

1. 目的のプログラムメンバーカスタムフィールドトークンを探して選択し、デフォルト値を入力して、**挿入**&#x200B;をクリックします。

   ![](assets/program-member-custom-field-tokens-3.png)

1. 「**保存**」をクリックします。

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>忘れずにEメールを承認してください。

**ランディングページ**

1. ランディングページを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >ランディングページデザイナーが新しいウィンドウで開きます。

1. トークンを追加するリッチテキストボックスをダブルクリックします。

   ![](assets/program-member-custom-field-tokens-6.png)

1. トークンを挿入する場所をクリックし、トークンを挿入アイコンをクリックします。

   ![](assets/program-member-custom-field-tokens-7.png)

1. 目的のトークンを見つけて選択します。

   ![](assets/program-member-custom-field-tokens-8.png)

1. デフォルト値を入力し、「**挿入**」をクリックします。

   ![](assets/program-member-custom-field-tokens-9.png)

1. 「**保存**」をクリックします。

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. 目的のSMSを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-11.png)

1. 「**`{{ Token`**」ボタンをクリックします。

   ![](assets/program-member-custom-field-tokens-12.png)

1. 目的のプログラムメンバーカスタムフィールドトークンを探して選択します。 デフォルト値を入力し、「挿入」をクリックします。

   ![](assets/program-member-custom-field-tokens-13.png)

1. SMSのアクションドロップダウンをクリックし、「**承認して閉じる**」を選択します。

   ![](assets/program-member-custom-field-tokens-14.png)

**プッシュ通知**

1. 目的のプッシュ通知を選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-15.png)

1. 「**プッシュ通知**」をクリックします。

   ![](assets/program-member-custom-field-tokens-16.png)

1. エディターでメッセージをクリックし、「`{{`」ボタンをクリックしてトークンセレクターを取得します。

   ![](assets/program-member-custom-field-tokens-17.png)

1. 目的のプログラムメンバーカスタムフィールドトークンを探して選択します。 デフォルト値を入力し、「**挿入**」をクリックします。

   ![](assets/program-member-custom-field-tokens-18.png)

1. 「**完了**」をクリックして保存して終了します（または、最初に確認するには「**次へ**」をクリックします）。

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>プログラムのメンバーのプログラムメンバーカスタムフィールドに値がない場合、トークンはデフォルト値に置き換えられます（指定されている場合）。

## キャンペーンでのプログラムメンバーカスタムフィールドトークンの使用 {#using-program-member-custom-field-tokens-in-campaigns}

プログラムメンバーのカスタムフィールドトークンは、次の場所で使用できます。

* タスクの作成
* Microsoftでのタスクの作成
* 注目のアクション
* データ値フローアクションの変更
* ウェブフック
