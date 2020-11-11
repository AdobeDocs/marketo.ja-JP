---
title: understanding-my-tokens
description: 自分のトークンについて
translation-type: tm+mt
source-git-commit: 642fd57105afff1031f18883c5809206f136b7c6
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---


# 自分のトークンについて

<br> 

マイトークンは、プログラムーやキャンペーンーフォルダーで作成および使用できるカスタム変数です。 次のようになります。 `{{_my.Name of Token_}}`

## 例

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

「マイトークン」にアクセスして作成するには、プログラムーまたはキャンペーンーフォルダーを選択し、「 [!UICONTROL マイトークン] 」タブに移動します。 任意のトークンを「 [!UICONTROL ローカルトークン] 」キャンバスにドラッグ&amp;ドロップします。

![イメージ1](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>マイトークンの名前は、保存後は変更できないので、慎重に選択してください。

>[!NOTE]
>
>Microsoft DynamicsまたはSalesforceのSales Insightから電子メールを送信すると、マイトークンが解決しません。標準のトークンのみが設定されます(リード、会社など)。 ただし、トークンのデフォルト値は有効です。

>[!NOTE]
>
>リンクトークンは、テキストのみの電子メールでは機能しません。

## トークンのネスト

新しいトークンを作成すると、ツリー内の他のオブジェクトから参照できます。 ツリー内の下位レベルでグローバル変数を上書きできます。 管理を容易にするためにトークンが作成された場所の命名構造があります。

* **ローカルトークン：** トークンは、そのプログラムーまたはフォルダーに直接作成されました。
* **[上書きされたトークン：](/help/sky/override-an-inherited-my-token.md)** トークンは継承されましたが、このプログラムーまたはフォルダーで例外が発生しました。
* **継承トークン：** トークンは、ツリーの上位レベルのプログラムーまたはフォルダーに作成されました。

これらの3つのタイプは、プログラムーまたはキャンペーンーフォルダーの [!UICONTROL **「マイトークン**] 」タブにあります。

![イメージ2](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

プログラムやフォルダーの移動は、トークンにも影響します。 移動中に参照が壊れていないことを必ず確認してください。

>[!NOTE]
>
>エンゲージメントプログラムから送信された電子メールが、デフォルトプログラムの子電子メール(エンゲージメントプログラムのローカル電子メールではなく)の場合、電子メールで使用されるマイトークンは、子電子メールが存在するデフォルトプログラムから解決されます。

## トークンの使用

任意のトークンを選択し、右上隅の使用状況アイコンをクリックして、そのトークンを含むアセットのリストを表示します。

![イメージ3](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![画像4](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**ディープダイブ**

各マイトークンの詳細：

* [CRMキャンペーン](/help/sky/my-token-crm-campaign.md)
* [日付](/help/sky/my-token-date.md)
* [カレンダーファイル](/help/sky/my-token-calendar-file.md)
* [画像](/help/sky/my-token-image.md)
* [リンク](/help/sky/my-token-link.md)
* [数値](/help/sky/my-token-number.md)
* [リッチテキスト](/help/sky/my-token-rich-text.md)
* [スコア](/help/sky/my-token-score.md)
* [電子メールスクリプト](/help/sky/my-token-email-script.md)
* [テキスト](/help/sky/my-token-text.md)
