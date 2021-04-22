---
unique-page-id: 12983619
description: LaunchPointサ追加ービスとしてのSlack-Marketoドキュメント — 製品ドキュメント
title: LaunchPointサービス追加としてのSlack
exl-id: 38c1501d-27ac-4c6c-967d-4decd10e0cb3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# LaunchPointサ追加ービス{#add-slack-as-a-launchpoint-service}としてのSlack

Slack統合には、次の2つの通知タイプが含まれます。

* **システム通知**:現在のキャンペーンのステータスや、直ちに注意を必要とする問題（CRMエラーおよびAPIの制限）に関するアラートなど、Marketoインスタンスの重要なイベントに関するSlack通知を取得します。
* **興味深い瞬間**:Marketoインサイトが営業アカウントから既知の個人によってトリガーされた場合、リードの所有者にはSlack経由で通知できます。通知には、リード情報と営業アカウントに関する詳細が含まれます。

>[!NOTE]
>
>**必要な管理者権限**

>[!PREREQUISITES]
>
>Slackシステム通知が既に有効になっていない場合は、[Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

1. **LaunchPoint**&#x200B;に移動し、**新しい**&#x200B;の下にある&#x200B;**新しいサービス**&#x200B;をクリックします。

   ![](assets/image2017-11-27-14-3a13-3a18.png)

1. Slack統合の表示名を入力します。 「**サービス**」ドロップダウンで、「**Slack**」を選択します。 「**作成**」をクリックします。

   ![](assets/image2017-11-27-15-3a54-3a11.png)

1. 「**許可**」をクリックします。 新しいタブにSlackが開き、認証を完了し、Slackから情報を取り込む権限をMarketoに付与します。

   ![](assets/image2017-11-27-14-3a16-3a6.png)

1. 新しいSlackタブで、ワークスペースのURLを入力し、「**続行**」をクリックします。

   ![](assets/image2017-11-27-15-3a1-3a29.png)

1. Slackの資格情報を入力し、「**サインイン**」をクリックします。

   ![](assets/image2017-11-27-15-3a1-3a3.png)

1. **投稿先**&#x200B;ドロップダウンで、Marketoからの通知を投稿するチャネルを選択します。 要求された権限を確認し、「**許可**」をクリックします。

   ![](assets/image2018-1-9-13-3a21-3a50.png)

1. 次の確認画面が表示されます。 タブが自動的に閉じます。

   ![](assets/image2017-11-27-15-3a51-3a57.png)

1. 「Marketo」タブを更新し、SlackがLaunchPointでアクティブなサービスとして表示されていることを確認します。

   ![](assets/image2017-11-27-15-3a55-3a37.png)

   通知は、手順6で選択したチャネルへの投稿を開始します。 次のようになります。

   ![](assets/samplenotification.png)
