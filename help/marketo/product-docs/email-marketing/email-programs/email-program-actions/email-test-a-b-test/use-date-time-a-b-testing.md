---
unique-page-id: 2359520
description: 「日時」A/B テストの使用 - Marketo ドキュメント - 製品ドキュメント
title: 「日付／時間」A/B テストの使用
exl-id: ee686d46-9427-4f8b-a16f-858c5109cabd
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '260'
ht-degree: 100%

---

# 「日付／時間」A/B テストの使用 {#use-date-time-a-b-testing}

メールの A/B テストはとても簡単に実施できます。1 つは&#x200B;**日時**&#x200B;テストです。このテストでは、メールの送信に最適な時間帯または曜日をテストします。その設定方法を説明しましょう。

>[!PREREQUISITES]
>
>[A/B テストの追加](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

1. **メール**&#x200B;タイルの下で、「**A/B テストを追加**」をクリックします。

   ![](assets/image2014-9-12-15-3a41-3a3.png)

1. 新しいウィンドウが開きます。「**テストタイプ**」で「**日時**」を選択します。

   ![](assets/image2014-9-12-15-3a41-3a12.png)

1. 既存のテスト情報（件名テストなど）がある場合は、「**テストのリセット**」をクリックします。

   ![](assets/image2014-9-12-15-3a41-3a19.png)

1. 最初の日時の日付を選択します。

   ![](assets/image2014-9-12-15-3a41-3a26.png)

1. 最初の日時の時刻を選択します。

   ![](assets/image2014-9-12-15-3a41-3a33.png)

1. 2 回目の日時にも同じ操作をおこないます。

   ![](assets/image2014-9-12-15-3a41-3a40.png)

1. A/B テストを送信したいオーディエンスの割合をスライダーで選択して、「**次へ**」をクリックします。

   ![](assets/image2014-9-12-15-3a41-3a53.png)

   >[!NOTE]
   >
   >それぞれのバリエーションの割合は、選択された「テストサンプルサイズ」を等分したものとなります。

   >[!CAUTION]
   >
   >**サンプルサイズを 100% に設定しないことをお勧めします**。静的リストを使用している場合、サンプルサイズを 100% に設定すると、オーディエンスの全員にメールが送信され、だれも勝者になりません。**スマート**&#x200B;リストを使用している場合、サンプルサイズを 100% に設定すると、_その時点で_&#x200B;オーディエンスの全員にメールが送信されます。メールプログラムが後日再実行されると、スマートリストに振り分けられた新しいリードも、オーディエンスに含まれるようになっているのでメールを受け取ります。

   ここまで来れば、あと一歩です。続いて、[A/B テストの勝者の条件を定義](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/define-the-a-b-test-winner-criteria.md)する必要があります。
