---
title: Experience Manager ドキュメントを接続
description: AEM Assets を活用できるようにAdobe Experience Manager Cloud Services をAdobe Marketo Engageに接続する方法について説明します。
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 6%

---

# Adobe Experience Manager Cloud Services の接続 {#connect-adobe-experience-manager-cloud-services}

Marketo EngageのメールDesignerでAEM Assets Asset リポジトリーを活用できるように、Adobe Marketo Engage Cloud Services アカウントをAEM インスタンスに接続する方法について説明します。

>[!NOTE]
>
>**管理者権限が必要**

1. Marketo Engageで、「**管理者** エリアに移動し、左側のナビゲーションツリーで「**Adobe Experience Manager**」を選択します。

スクリーンショット

1. **2&rbrace;Adobe Experience Manager Cloud Services** の横にある「編集 _をクリックします。_

スクリーンショット

1. 1 つ以上のリポジトリーを選択します。

スクリーンショット

>[!NOTE]
>
>Marketo Engage サブスクリプションと同じ IMS 組織に関連付けられているリポジトリーのみが表示されます。

1. リポジトリを設定するには、[ サービス資格情報証明書 ](https://experienceleague.adobe.com/ja/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) を追加する必要があります。 「**+証明書を追加**」ボタンをクリックします。

スクリーンショット

1. 証明書（JSON ファイルのみ）をドラッグ&amp;ドロップするか、コンピューターから選択します。 終了したら「**追加**」をクリックします。

スクリーンショット

1. 設定済みのリポジトリが、ステータスと有効期限と共に以下に表示されます。 省略記号ボタン （**...**）をクリックして、証明書を表示します。 それ以外の場合は、完了です。

スクリーンショット

これで、そのリポジトリー内の Digital Asset Management ライブラリのすべての画像に、Marketo EngageのメールDesignerからアクセスできるようになりました。

>[!MORELIKETHIS]
>
>[Experience Manager アセットの操作 ](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
