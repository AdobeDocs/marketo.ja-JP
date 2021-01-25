---
unique-page-id: 9438139
description: 追加担当者ブロックリスト対- Marketto Docs — 製品ドキュメント
title: 追加ブロックリスト対象
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# 追加ブロックリスト{#add-person-to-blocklist}

ユーザーをブロックリストに追加すると、そのユーザーは通信を受信できなくなります。

>[!NOTE]
>
>マーケティング担当者は、ブラックリストやホワイトリストなどの用語を、当社の製品のブロックリスト許可リストやに変更する過程にあります。 この更新中、UIとドキュメントのスクリーンショットには古い用語が表示され、ドキュメントのテキストには新しい用語が表示される場合があります。 ご混乱をおかけして申し訳ございません。

1. [新しいデフォルト](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md)  ****&#x200B;プログラムを作成し、それに追加ブロックリストという名前を付けます。

1. 「**新規**」をクリックし、「**新規ローカルアセット**」を選択します。

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. リストに名前を付け、「**作成**」をクリックします。

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. 追加&#x200B;**スマートリスト**&#x200B;に追加するすべてのユーザーブロックリストをに追加します。

   >[!NOTE]
   >
   >お使いのブロックリストのユーザーは、操作用の電子メールを受信しません。

   ![](assets/three-6.png)

1. 「**新規**」をクリックし、「**新しいスマートキャンペーン**」を選択します。

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. **新しいスマートキャンペーン**&#x200B;に名前を付けます。 「**作成**」をクリックします。

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. **スマートリストのメンバ**&#x200B;をドラッグ&amp;ドロップします。

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. 作成したスマートリストを選択します。

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. **データ値を変更**&#x200B;をドラッグ&amp;ドロップします。

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. **フロー**&#x200B;に対して、**属性**&#x200B;に&#x200B;**リストされたブロック**&#x200B;を入力し、**新しい値**&#x200B;を&#x200B;**true**&#x200B;に設定します。

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. 「**スケジュール**」タブで、「**1回実行**」を選択します。

   ![](assets/ten.png)

1. 「**今すぐ実行**」を選択し、「**実行**」をクリックします。

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   やった！ これらのユーザーは、電子メールを受信しなくなります。

   >[!TIP]
   >
   >**Change Data Value** with **Block Listed is true**&#x200B;を使用して、トリガー可能な属性を持つ将来のすべての人に対して、[ブロックリストキャンペーンスマート](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)を作成します。
