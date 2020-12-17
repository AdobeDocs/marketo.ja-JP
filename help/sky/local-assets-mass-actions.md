---
title: local-assets-mass-actions
description: ローカル資産一括処理
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---


# ローカルアセット：一括処理

<br> 

複数のアセットに対してバルクアクションを直接実行するには、「**[!UICONTROL アセット]**」タブの「**[!UICONTROL アクション]**」セクションを使用します。 必要なアセットを見つけて、それらに一括アクションを適用する方法を次に示します。

## アセットタイプまたは条件でフィルター

アクションを実行する特定のアセットを検索するには、**[!UICONTROL アセットタイプ]**&#x200B;でフィルタリングします。そのためには、ドロップダウンから1つ以上のタイプを選択します。

![イメージ1](/help/sky/assets/programs/local-assets-mass-actions/local-assets-mass-actions-1.png)

また、ドロップダウンから1つ以上の条件を選択すると、**[!UICONTROL アセット条件]**&#x200B;でフィルタリングできます。 これは、個別に行うことも、アセットタイプのフィルタリングと組み合わせて行うこともできます。

![イメージ2](/help/sky/assets/programs/local-assets-mass-actions/local-assets-mass-actions-2.png)

>[!NOTE]
>
>[!DNL Marketo Sky] 現在、電子メール、バッチキャンペーン、ランディングページおよびトリガーキャンペーンのフィルタリングのみがサポートされています。

## 一括処理の適用

アセットのグループを選択し、**[!UICONTROL アクション]**&#x200B;を選択ドロップダウンからアクションを選択します。 選択したアセットの&#x200B;__&#x200B;に適用できないアクションは、自動的に灰色表示になります。

![イメージ3](/help/sky/assets/programs/local-assets-mass-actions/local-assets-mass-actions-3.png)

## 無視されたアセット

適用しようとしているステータスが既に存在するアセット、または適用する権限がないアセットは無視されます（例えば、アセットのグループを承認する場合、既に承認されているアセットは無視されます）。 選択したアクションに一致しない(トリガーキャンペーンを承認できないなど)アセットも無視されます。

一括処理を選択すると、確認ポップアップが表示され、無視されたアセットがリストされます。

![画像4](/help/sky/assets/programs/local-assets-mass-actions/local-assets-mass-actions-4.png)

## ステータス通知

一括処理の状態は、「**[!UICONTROL 最近の通知]**」トレイで確認できます。

![画像5](/help/sky/assets/programs/local-assets-mass-actions/local-assets-mass-actions-5.png)

## 一括操作の失敗

アセットの修正が必要なために選択したアクションを適用できない場合は、部分的なエラーの通知（黄色の注意記号）が表示されます。 アクションが選択したアセットの&#x200B;_すべての_&#x200B;に適用されなかった場合、通知には赤い注意記号が表示されます。 詳細については、**[!UICONTROL 表示エラー]**&#x200B;をクリックしてください。

![画像6](/help/sky/assets/programs/local-assets-mass-actions/local-assets-mass-actions-6.png)

![画像7](/help/sky/assets/programs/local-assets-mass-actions/local-assets-mass-actions-7.png)
