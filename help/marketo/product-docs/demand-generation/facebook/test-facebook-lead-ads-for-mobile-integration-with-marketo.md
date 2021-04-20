---
unique-page-id: 10098759
description: facebookのリード広告をテストして、Marketoとのモバイル統合 —Marketoドキュメント — 製品ドキュメント
title: facebookのリード広告をテストして、Marketoとのモバイル統合を実現
exl-id: 0c381c53-f97a-4e1d-b44d-5ee6521ac990
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# facebookのリード広告をMarketoとのモバイル統合のためにテスト{#test-facebook-lead-ads-for-mobile-integration-with-marketo}

リード広告を作成した後、テストする必要があります。

>[!PREREQUISITES]
>
>[Facebookリード広告統合](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)を設定する必要があります。

1. facebookパワーエディタで、キャンペーンと広告を選択し、**編集**&#x200B;をクリックします。

1. 「**リンク**」の下の「**モバイルアプリ**」リンクの表示をクリックします。

   ![](assets/image2016-5-13-15-3a2-3a38.png)

1. 認証されたアカウントでモバイルデバイス上でアクセスできる新しい通知がFacebookアカウントに送信されます。 「**OK**」をクリックします。

   ![](assets/image2016-3-11-8-3a35-3a7.png)

1. モバイルデバイス上で、Facebookモバイルアプリの&#x200B;**通知**&#x200B;をタップします。

   ![](assets/image2016-3-11-8-3a38-3a35.png)

1. 「通知」で、**広告をプレビューする準備ができたことを確認します。**

   ![](assets/image2016-3-11-8-3a41-3a59.png)

1. 誘い文句（CTA：コールトゥアクション）をタップし、作成したフォームに入力して、テスト用リード広告ユニットを送信します。

   ![](assets/image2016-3-11-8-3a52-3a20.png)

   >[!NOTE]
   >
   >これは、「詳細なアクションの呼び物」を使用した一例に過ぎません。 リード広告の単位による誘い文句（CTA：コールトゥアクション）が異なる場合があります。

1. ここが魔法が起こる場所だ！ フォームを送信したら、[Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)に、プログラムの一部として、または&#x200B;**入力済みFacebookリード広告フォーム**&#x200B;フィルタを使用するリードリストを作成します。 先ほど提出したフォームのリード広告フォーム名を挿入します。

   ![](assets/image2016-3-11-8-3a59-3a34.png)

1. 次に、「Leads」タブをクリックして、同期が正しく動作していることを検証します。

   ![](assets/image2016-3-11-15-3a27-3a54.png)

それは涼しいですか？

>[!NOTE]
>
>[facebookリード広告の有効化/無効化](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
