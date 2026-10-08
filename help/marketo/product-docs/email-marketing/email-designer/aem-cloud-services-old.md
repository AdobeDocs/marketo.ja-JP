---
title: Connect Experience Manager doc
description: AEM Cloud ServicesをMarketo Engageに接続する方法について説明します。 デザイナーでメールを作成する際に、AEM アセットを使用します。
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: 'yes'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: f8f7d99a-f455-45bb-8028-428a55a7130b
    internal-label: Email Designer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 12%
---
# Adobe Experience Manager Cloud Servicesとの連携 {#connect-adobe-experience-manager-cloud-services}

AEM Assets Cloud Services アカウントをAdobe Marketo Engage インスタンスに接続して、Marketo Engage Email DesignerでAEM Asset リポジトリを活用できるようにする方法について説明します。

>[!NOTE]
>
>**管理者権限が必要**

1. Marketo Engageで、**管理者**&#x200B;領域に移動し、左側のナビゲーションツリーで「**Adobe Experience Manager**」を選択します。

スクリーンショット

1. _Adobe Experience Manager Cloud Services_&#x200B;の横にある&#x200B;**Edit**&#x200B;をクリックします。

スクリーンショット

1. 1つ以上のリポジトリを選択します。

スクリーンショット

>[!NOTE]
>
>Marketo Engage サブスクリプションと同じIMS組織に関連付けられているリポジトリのみが一覧表示されます。

1. リポジトリを設定するには、[ サービス資格情報の証明書](https://experienceleague.adobe.com/ja/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials)を追加する必要があります。 「**+証明書を追加**」ボタンをクリックします。

スクリーンショット

1. 証明書（JSON ファイルのみ）をドラッグ&amp;ドロップするか、コンピューターから選択します。 終了したら「**追加**」をクリックします。

スクリーンショット

1. 設定されたリポジトリが、ステータスと有効期限とともに以下に表示されます。 省略記号ボタン （**...**）をクリックします 証明書を表示します。 それ以外の場合は完了です。

スクリーンショット

これで、そのリポジトリ内のデジタルアセット管理ライブラリのすべての画像に、Marketo Engage電子メールDesignerからアクセスできるようになります。

>[!MORELIKETHIS]
>
>[Experience Manager Assetsの操作](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
