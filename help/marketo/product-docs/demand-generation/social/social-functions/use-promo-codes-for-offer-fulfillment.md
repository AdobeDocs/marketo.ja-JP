---
unique-page-id: 2359819
description: オファー達成のためのプロモコードの使用 — Marketo ドキュメント — 製品ドキュメント
title: オファー達成のためのプロモコードの使用
exl-id: 71cfc1c5-ecd3-435f-8c8c-1a93478fe80c
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 90%

---

# オファー達成のためのプロモコードの使用 {#use-promo-codes-for-offer-fulfillment}

紹介オファーや懸賞を作成する際に、各勝者にプロモ（クーポン）コードを送信できます。報酬を受け取るには、例えば、サイトでの購入のチェックアウトページでコードを使用します。

>[!IMPORTANT]
>
>2024 年 7 月 31 日に、この機能を廃止するプロセスを開始しました。 新しいアセットは作成できなくなりました。 既存のアセットは、2025 年 1 月 31 日（PT）まで引き続き機能します。 [詳細情報](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## プロモコードのアップロード {#upload-promo-codes}

1. **マーケティング活動**&#x200B;に移動します。

   ![](assets/login-marketing-activities-2.png)

1. 紹介オファーを選択して、「**下書きの編集**」をクリックします。

   ![](assets/image2015-4-22-11-3a16-3a45.png)

1. 紹介オファーエディターで、「**アプリ設定**」、「**オファーの詳細**」の順に移動します。

   ![](assets/image2015-4-22-11-3a23-3a39.png)

1. 「メール」で「**プロモコードを使用**」を選択し、「コードのアップロード」で「**参照**」をクリックして、システムからプロモコードファイルを選択します。

   ![](assets/image2015-4-22-12-3a52-3a43.png)

1. プロモコードファイルは、1 行に 1 つのコードと .txt ファイル名拡張子を持つプレーン ASCII テキストファイルである必要があります。例：

   ![](assets/image2015-4-22-13-3a2-3a23.png)

   >[!CAUTION]
   >
   >プロモコードファイル内の空白は、その行のコードの一部として扱われます。特に、各行の末尾での空白を避けるように注意してください。

1. アップロードが完了すると、アップロードされたコードの合計数が表示されます。

   ![](assets/image2015-4-22-13-3a8-3a31.png)

## 送信済みプロモコードの確認 {#review-sent-promo-codes}

参加者がオファー報酬の獲得を開始すると、どのプロモコードが誰にいつ送信されたかを確認できます。

>[!NOTE]
>
>_受賞にアクセス_&#x200B;権限を持つ Marketo ユーザーのみが、この情報にアクセスできます。[ユーザーのロールと権限の管理](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md)を参照してください。

1. **マーケティング活動**&#x200B;に移動します。

   ![](assets/login-marketing-activities-2.png)

1. 紹介オファーまたは懸賞を選択して、「**参加者**」タブをクリックします。

   ![](assets/image2015-4-22-11-3a36-3a22.png)

1. ここに、いくつかのエントリが表示されます。**プロモコード**&#x200B;列の番号をクリックして、その参加者に送信されたプロモコードと、その日時を確認します。

   ![](assets/image2015-4-22-11-3a36-3a43.png)
