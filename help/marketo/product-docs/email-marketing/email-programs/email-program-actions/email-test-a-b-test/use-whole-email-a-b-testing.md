---
unique-page-id: 2359502
description: 「メール全体」A/B テストを使用する — Marketo ドキュメント — 製品ドキュメント
title: 「メール全体」A/B テストを使用する
exl-id: 28e5f0e0-702d-4e1d-add8-6bf61752ca5b
feature: Email Programs, A/B Testing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: ht
source-wordcount: '272'
ht-degree: 100%

---

# 「メール全体」A/B テストを使用する {#use-whole-email-a-b-testing}

メールの A/B テストはとても簡単に実施できます。なかでも便利なのが、**メール全体**&#x200B;テストです。その設定方法を説明しましょう。

>[!PREREQUISITES]
>
>[A/B テストの追加](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. 「メール」タイルで、目的のメールを選択して「**[!UICONTROL A/B テストの追加]**」をクリックします。

![](assets/image2014-9-12-15-3a22-3a12.png)

1. 新しいウィンドウが開きます。**[!UICONTROL テストタイプ]**&#x200B;ドロップダウンをクリックし、「**[!UICONTROL メール全体]**」を選択します。

   ![](assets/image2014-9-12-15-3a22-3a27.png)

1. 既存のテスト情報（件名テストなど）がある場合は、「**[!UICONTROL テストのリセット]**」をクリックします。

   ![](assets/image2014-9-12-15-3a22-3a40.png)

1. 1 つ目のメールを選択します。

   ![](assets/image2014-9-12-15-3a22-3a52.png)

1. 「**[!UICONTROL 追加]**」をクリックしてメールを適用します。

   ![](assets/image2014-9-12-15-3a23-3a20.png)

   >[!TIP]
   >
   >複数のメールを追加できます。ただし、追加する数が多すぎると、テストプロセスの速度が低下する可能性があります。

1. 2 つ目のメールを選択します。

   [](assets/image2014-9-12-15-3a23-3a49.png)

1. 「**[!UICONTROL 追加]**」をクリックして 2 つ目のメールを適用します。A/B テストを送信するオーディエンスの割合をスライダーで選択して、「**[!UICONTROL 次へ]**」をクリックします。

   [](assets/image2014-9-12-15-3a24-3a1.png)

   >[!NOTE]
   >
   >それぞれのバリエーションの割合は、選択された「**テストサンプルサイズ**」を等分したものとなります。

   >[!CAUTION]
   >
   >**サンプルサイズを 100% に設定しないことをお勧めします**。静的リストを使用している場合、サンプルサイズを 100% に設定すると、オーディエンスの全員にメールが送信され、だれも勝者になりません。**スマート**&#x200B;リストを使用している場合、サンプルサイズを 100% に設定すると、_その時点で_&#x200B;オーディエンスの全員にメールが送信されます。メールプログラムが後日再実行されると、スマートリストに振り分けられた新しいリードも、オーディエンスに含まれるようになっているのでメールを受け取ります。

   ここまで来れば、あと一歩です。続いて、[A/B テストの勝者の条件を定義](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md)する必要があります。
