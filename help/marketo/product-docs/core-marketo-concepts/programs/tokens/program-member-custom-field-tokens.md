---
unique-page-id: 1147114
description: プログラムメンバーのカスタムフィールドトークン — Marketto Docs — 製品ドキュメント
title: プログラムメンバのカスタムフィールドトークン
translation-type: tm+mt
source-git-commit: 35e8b41574ebf8aafa27a59440c8ea9cb6413d50
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---


# プログラムメンバのカスタムフィールドトークン{#program-member-custom-field-tokens}

## プログラムメンバーのカスタムフィールドのトークンサポート{#token-support-for-program-member-custom-fields}

プログラムメンバーカスタムフィールド機能の背面では、トークンフレームワークのプログラムメンバーカスタムフィールドに対するサポートが拡張されています。

PMCFトークンは、トークン・ファミリのメンバ・ドメインでサポートされます。

メンバートークンは、プログラムメンバーの範囲内のフィールドに使用されます。 現在の状態では、メンバートークンは、統合サービスパートナーから一意の値を挿入するためにも使用されます。 `{{member.webinar url}}` トークンは、サービスプロバイダーが生成した個人の固有の確認URLを自動的に解決します。{{member.registration code}}は、サービスプロバイダーが提供する登録コードに解決されます。

>[!NOTE]
>
>* プログラムメンバのカスタムフィールドは、プログラムのコンテキストでのみ使用できます。
>* プログラムメンバカスタムフィールドトークンは次の場所では使用できません：電子メールスクリプト、電子メールプリヘッダー、待機手順の日付トークンまたはスニペット。
>* プログラムメンバーの状態は、メンバートークンではサポートされていません。


## アセット{#using-program-member-custom-field-tokens-in-assets}でのプログラムメンバーのカスタムフィールドトークンの使用

プログラムメンバのカスタムフィールドトークンは、電子メール、ランディングページ、SMS、プッシュ通知、Webフックに挿入できます。

**電子メール**

1. 目的の電子メールを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-1.png)

1. 「Insert Token」アイコンをクリックします。

   ![](assets/program-member-custom-field-tokens-2.png)

1. 目的のプログラムメンバーカスタムフィールドトークンを検索して選択し、デフォルト値を入力して、**挿入**&#x200B;をクリックします。

   ![](assets/program-member-custom-field-tokens-3.png)

1. 「**保存**」をクリックします。

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>電子メールの承認を忘れないでください。

**ランディングページ**

1. ランディングページを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >ランディングページデザイナーが新しいウィンドウで開きます。

1. トークンを追加するリッチテキストボックスを重複クリックします。

   ![](assets/program-member-custom-field-tokens-6.png)

1. トークンの挿入先をクリックし、「トークンの挿入」アイコンをクリックします。

   ![](assets/program-member-custom-field-tokens-7.png)

1. 目的のトークンを探して選択します。

   ![](assets/program-member-custom-field-tokens-8.png)

1. デフォルト値を入力し、「**挿入**」をクリックします。

   ![](assets/program-member-custom-field-tokens-9.png)

1. 「**保存**」をクリックします。

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. 目的のSMSを選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-11.png)

1. **`{{ Token`**&#x200B;ボタンをクリックします。

   ![](assets/program-member-custom-field-tokens-12.png)

1. 目的のプログラムメンバーカスタムフィールドトークンを検索して選択します。 デフォルト値を入力し、「挿入」をクリックします。

   ![](assets/program-member-custom-field-tokens-13.png)

1. SMSアクションドロップダウンをクリックし、**承認して閉じる**&#x200B;を選択します。

   ![](assets/program-member-custom-field-tokens-14.png)

**プッシュ通知**

1. 目的のプッシュ通知を選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/program-member-custom-field-tokens-15.png)

1. 「**プッシュ通知**」をクリックします。

   ![](assets/program-member-custom-field-tokens-16.png)

1. エディターでメッセージをクリックし、「`{{`」ボタンをクリックしてトークンセレクターを取得します。

   ![](assets/program-member-custom-field-tokens-17.png)

1. 目的のプログラムメンバーカスタムフィールドトークンを検索して選択します。 デフォルト値を入力し、「**挿入**」をクリックします。

   ![](assets/program-member-custom-field-tokens-18.png)

1. 「**完了**」をクリックして保存し、終了します（最初に確認する場合は「**次へ**」）。

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>プログラムのメンバーのプログラムメンバーカスタムフィールドに値がない場合、トークンはデフォルト値に置き換えられます（指定されている場合）。

## キャンペーン{#using-program-member-custom-field-tokens-in-campaigns}でのプログラムメンバのカスタムフィールドトークンの使用

プログラムメンバのカスタムフィールドトークンは、次の場所で使用できます。

* タスクの作成
* Microsoftでタスクを作成する
* 興味深い瞬間
* データ値フローのアクションの変更
* Webhooks
